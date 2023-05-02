# Comparing `tmp/blond-2.0.11.tar.gz` & `tmp/blond-2.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/blond-2.0.11.tar", last modified: Mon Jul 15 15:39:40 2019, max compression
+gzip compressed data, was "blond-2.0.12.tar", last modified: Tue May  2 16:12:01 2023, max compression
```

## Comparing `blond-2.0.11.tar` & `blond-2.0.12.tar`

### file list

```diff
@@ -1,101 +1,313 @@
-drwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-15 15:39:40.000000 blond-2.0.11/
-drwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-15 15:39:40.000000 blond-2.0.11/blond/
-drwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-15 15:39:40.000000 blond-2.0.11/blond/beam/
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-12 14:23:09.000000 blond-2.0.11/blond/beam/__init__.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    11735 2019-07-12 14:23:09.000000 blond-2.0.11/blond/beam/beam.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     3685 2019-07-12 14:23:09.000000 blond-2.0.11/blond/beam/coasting_beam.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    40951 2019-07-15 15:39:24.000000 blond-2.0.11/blond/beam/distributions.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    37921 2019-07-12 14:23:09.000000 blond-2.0.11/blond/beam/distributions_multibunch.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    19660 2019-07-12 14:23:09.000000 blond-2.0.11/blond/beam/profile.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     2185 2019-07-12 14:23:09.000000 blond-2.0.11/blond/beam/sparse_histogram.cpp
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     5010 2019-07-12 14:23:09.000000 blond-2.0.11/blond/beam/sparse_slices.py
-drwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-15 15:39:40.000000 blond-2.0.11/blond/cpp_routines/
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     9863 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/blondmath.cpp
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     1310 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/convolution.cpp
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     1316 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/cos.h
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     2079 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/drift.cpp
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     4376 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/exp.h
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     2651 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/fast_resonator.cpp
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    15233 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/fft.cpp
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     2239 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/fft.h
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     5394 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/histogram.cpp
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     1955 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/kick.cpp
--rwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)    72552 2019-07-15 15:39:40.000000 blond-2.0.11/blond/cpp_routines/libblond.so
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     3517 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/linear_interp_kick.cpp
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     8052 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/music_track.cpp
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     1960 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/sin.h
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     5871 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/sincos.h
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     7480 2019-07-12 14:23:09.000000 blond-2.0.11/blond/cpp_routines/vdtcore_common.h
-drwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-15 15:39:40.000000 blond-2.0.11/blond/impedances/
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-12 14:23:09.000000 blond-2.0.11/blond/impedances/__init__.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    30079 2019-07-12 14:23:09.000000 blond-2.0.11/blond/impedances/impedance.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    22635 2019-07-12 14:23:09.000000 blond-2.0.11/blond/impedances/impedance_sources.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     3357 2019-07-12 14:23:09.000000 blond-2.0.11/blond/impedances/induced_voltage_analytical.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    13913 2019-07-12 14:23:09.000000 blond-2.0.11/blond/impedances/music.py
-drwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-15 15:39:40.000000 blond-2.0.11/blond/input_parameters/
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-12 14:23:09.000000 blond-2.0.11/blond/input_parameters/__init__.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    21284 2019-07-12 14:23:09.000000 blond-2.0.11/blond/input_parameters/rf_parameters.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    20249 2019-07-12 14:23:09.000000 blond-2.0.11/blond/input_parameters/rf_parameters_options.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    16349 2019-07-12 14:23:09.000000 blond-2.0.11/blond/input_parameters/ring.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    22443 2019-07-12 14:23:09.000000 blond-2.0.11/blond/input_parameters/ring_options.py
-drwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-15 15:39:40.000000 blond-2.0.11/blond/llrf/
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-12 14:23:09.000000 blond-2.0.11/blond/llrf/__init__.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    21943 2019-07-12 14:23:09.000000 blond-2.0.11/blond/llrf/beam_feedback.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    26674 2019-07-12 14:23:09.000000 blond-2.0.11/blond/llrf/cavity_feedback.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    13182 2019-07-12 14:23:09.000000 blond-2.0.11/blond/llrf/impulse_response.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     2337 2019-07-12 14:23:09.000000 blond-2.0.11/blond/llrf/notch_filter.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     7257 2019-07-12 14:23:09.000000 blond-2.0.11/blond/llrf/offset_frequency.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     4394 2019-07-12 14:23:09.000000 blond-2.0.11/blond/llrf/rf_modulation.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    15768 2019-07-12 14:23:09.000000 blond-2.0.11/blond/llrf/rf_noise.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     6995 2019-07-12 14:23:09.000000 blond-2.0.11/blond/llrf/signal_processing.py
-drwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-15 15:39:40.000000 blond-2.0.11/blond/monitors/
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-12 14:23:09.000000 blond-2.0.11/blond/monitors/__init__.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    14884 2019-07-12 14:23:09.000000 blond-2.0.11/blond/monitors/monitors.py
-drwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-15 15:39:40.000000 blond-2.0.11/blond/plots/
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-12 14:23:09.000000 blond-2.0.11/blond/plots/__init__.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    11025 2019-07-12 14:23:09.000000 blond-2.0.11/blond/plots/plot.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    10004 2019-07-12 14:23:09.000000 blond-2.0.11/blond/plots/plot_beams.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     4777 2019-07-12 14:23:09.000000 blond-2.0.11/blond/plots/plot_impedance.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    14165 2019-07-12 14:23:09.000000 blond-2.0.11/blond/plots/plot_llrf.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     1210 2019-07-12 14:23:09.000000 blond-2.0.11/blond/plots/plot_parameters.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     2725 2019-07-12 14:23:09.000000 blond-2.0.11/blond/plots/plot_slices.py
-drwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-15 15:39:40.000000 blond-2.0.11/blond/synchrotron_radiation/
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-12 14:23:09.000000 blond-2.0.11/blond/synchrotron_radiation/__init__.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     3125 2019-07-12 14:23:09.000000 blond-2.0.11/blond/synchrotron_radiation/synchrotron_radiation.cpp
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     8148 2019-07-12 14:23:09.000000 blond-2.0.11/blond/synchrotron_radiation/synchrotron_radiation.py
-drwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-15 15:39:40.000000 blond-2.0.11/blond/toolbox/
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-12 14:23:09.000000 blond-2.0.11/blond/toolbox/__init__.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     5221 2019-07-12 14:23:09.000000 blond-2.0.11/blond/toolbox/action.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     7570 2019-07-12 14:23:09.000000 blond-2.0.11/blond/toolbox/diffusion.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     7393 2019-07-12 14:23:09.000000 blond-2.0.11/blond/toolbox/filters_and_fitting.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     2070 2019-07-12 14:23:09.000000 blond-2.0.11/blond/toolbox/logger.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     3377 2019-07-12 14:23:09.000000 blond-2.0.11/blond/toolbox/next_regular.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    20816 2019-07-12 14:23:09.000000 blond-2.0.11/blond/toolbox/parameter_scaling.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     2128 2019-07-12 14:23:09.000000 blond-2.0.11/blond/toolbox/tomoscope.cpp
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     4877 2019-07-12 14:23:09.000000 blond-2.0.11/blond/toolbox/tomoscope.py
-drwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-15 15:39:40.000000 blond-2.0.11/blond/trackers/
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-12 14:23:09.000000 blond-2.0.11/blond/trackers/__init__.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    21917 2019-07-12 14:23:09.000000 blond-2.0.11/blond/trackers/tracker.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)    31291 2019-07-12 14:23:09.000000 blond-2.0.11/blond/trackers/utilities.py
-drwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-15 15:39:40.000000 blond-2.0.11/blond/utils/
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-12 14:23:09.000000 blond-2.0.11/blond/utils/__init__.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     3143 2019-07-12 14:23:09.000000 blond-2.0.11/blond/utils/bmath.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     5640 2019-07-12 14:23:09.000000 blond-2.0.11/blond/utils/bphysics_wrap.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     8160 2019-07-12 14:23:09.000000 blond-2.0.11/blond/utils/butils_wrap.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     3467 2019-07-12 14:23:09.000000 blond-2.0.11/blond/utils/data_check.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     1965 2019-07-12 14:23:09.000000 blond-2.0.11/blond/utils/exceptions.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     3914 2019-07-12 14:23:09.000000 blond-2.0.11/blond/utils/track_iteration.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)      710 2019-07-12 14:23:09.000000 blond-2.0.11/blond/__init__.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)       23 2019-07-15 15:39:24.000000 blond-2.0.11/blond/_version.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     6686 2019-07-12 14:23:09.000000 blond-2.0.11/blond/compile.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     6471 2019-07-12 14:23:09.000000 blond-2.0.11/blond/sanity_check.py
-drwxr-xr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2019-07-15 15:39:40.000000 blond-2.0.11/blond.egg-info/
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     8237 2019-07-15 15:39:40.000000 blond-2.0.11/blond.egg-info/PKG-INFO
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     2459 2019-07-15 15:39:40.000000 blond-2.0.11/blond.egg-info/SOURCES.txt
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)        1 2019-07-15 15:39:40.000000 blond-2.0.11/blond.egg-info/dependency_links.txt
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)        6 2019-07-15 15:39:40.000000 blond-2.0.11/blond.egg-info/top_level.txt
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)      377 2019-07-15 15:39:24.000000 blond-2.0.11/MANIFEST.in
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     6074 2019-07-12 14:23:09.000000 blond-2.0.11/README.rst
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     7172 2019-07-12 14:24:59.000000 blond-2.0.11/setup.py
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)     8237 2019-07-15 15:39:40.000000 blond-2.0.11/PKG-INFO
--rw-r--r--   0 kiliakis  (1000) kiliakis  (1000)       38 2019-07-15 15:39:40.000000 blond-2.0.11/setup.cfg
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.876531 blond-2.0.12/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      399 2023-05-02 07:47:33.000000 blond-2.0.12/.coveragerc
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     6226 2023-05-02 07:47:33.000000 blond-2.0.12/.gitignore
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3093 2023-05-02 07:47:33.000000 blond-2.0.12/.gitlab-ci.yml
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1665 2023-05-02 07:47:33.000000 blond-2.0.12/CHANGELOG
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    35797 2022-04-06 10:08:34.000000 blond-2.0.12/LICENSE.txt
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      339 2023-05-02 07:47:33.000000 blond-2.0.12/MANIFEST.in
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    14399 2023-05-02 16:12:01.876531 blond-2.0.12/PKG-INFO
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    13623 2023-05-02 07:47:33.000000 blond-2.0.12/README.rst
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      794 2022-04-06 10:08:34.000000 blond-2.0.12/WARNINGS.txt
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.840531 blond-2.0.12/__BENCHMARKS/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)       55 2022-04-06 10:08:34.000000 blond-2.0.12/__BENCHMARKS/.gitignore
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    16964 2022-08-23 13:41:21.000000 blond-2.0.12/__BENCHMARKS/BM1_OTFB_Vind_beam_1.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4291 2022-04-06 10:08:34.000000 blond-2.0.12/__BENCHMARKS/BM2_OTFB_no_beam.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1270 2022-04-06 10:08:34.000000 blond-2.0.12/__BENCHMARKS/BM3_OTFB_moving_average.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7415 2022-04-06 10:08:34.000000 blond-2.0.12/__BENCHMARKS/BM4_OTFB_with_beam.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     8956 2022-04-06 10:08:34.000000 blond-2.0.12/__BENCHMARKS/BM5_OTFB_feedforward.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.836531 blond-2.0.12/__EXAMPLES/
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.840531 blond-2.0.12/__EXAMPLES/gpu_main_files/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5807 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/gpu_main_files/EX_01_Acceleration.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     8578 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/gpu_main_files/EX_02_Main_long_ps_booster.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     6581 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/gpu_main_files/EX_03_RFnoise.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7056 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/gpu_main_files/EX_04_Stationary_multistation.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    14174 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/gpu_main_files/EX_05_Wake_impedance.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7328 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/gpu_main_files/EX_07_Ions.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5041 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/gpu_main_files/EX_08_Phase_Loop.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5582 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/gpu_main_files/EX_09_Radial_Loop.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5941 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/gpu_main_files/EX_10_Fixed_frequency.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5953 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/gpu_main_files/EX_16_impedance_test.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     9212 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/gpu_main_files/EX_17_multi_turn_wake.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     8115 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/gpu_main_files/EX_18_robinson_instability.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.840531 blond-2.0.12/__EXAMPLES/input_files/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    11866 2022-04-06 10:08:34.000000 blond-2.0.12/__EXAMPLES/input_files/EX_02_Ekicker_1.4GeV.txt
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    16868 2022-04-06 10:08:34.000000 blond-2.0.12/__EXAMPLES/input_files/EX_02_Finemet.txt
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1043 2022-04-06 10:08:34.000000 blond-2.0.12/__EXAMPLES/input_files/EX_05_new_HQ_table.dat
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    11976 2022-04-06 10:08:34.000000 blond-2.0.12/__EXAMPLES/input_files/EX_06_Source_TOF_P.csv
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      170 2022-04-06 10:08:34.000000 blond-2.0.12/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c02.txt
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      316 2022-04-06 10:08:34.000000 blond-2.0.12/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c04.txt
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      101 2022-04-06 10:08:34.000000 blond-2.0.12/__EXAMPLES/input_files/EX_06_voltage_program_LHC25_c16.txt
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.840531 blond-2.0.12/__EXAMPLES/main_files/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4668 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_01_Acceleration.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7353 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_02_Main_long_ps_booster.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5605 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_03_RFnoise.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5413 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_04_Stationary_multistation.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    11556 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_05_Wake_impedance.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3396 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_06_Preprocess.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     6400 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_07_Ions.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4348 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_08_Phase_Loop.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4864 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_09_Radial_Loop.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4938 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_10_Fixed_frequency.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4651 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_11_comparison_music_fourier_analytical.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    11630 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_12_synchrotron_frequency_distribution.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    10276 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_13_synchrotron_radiation.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4639 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_14_sparse_slicing.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4665 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_15_sparse_multi_bunch.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5447 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_16_impedance_test.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7736 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_17_multi_turn_wake.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7438 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_18_robinson_instability.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     6098 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_19_bunch_generation.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     6646 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_20_bunch_generation_multibunch.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3132 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_21_bunch_distribution.py
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)     4029 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/main_files/EX_22_Coherent_Radiation.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.840531 blond-2.0.12/__EXAMPLES/mpi_main_files/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5008 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/mpi_main_files/EX_01_Acceleration.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7618 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/mpi_main_files/EX_02_Main_long_ps_booster.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5932 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/mpi_main_files/EX_03_RFnoise.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5703 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/mpi_main_files/EX_04_Stationary_multistation.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    12098 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/mpi_main_files/EX_05_Wake_impedance.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     6688 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/mpi_main_files/EX_07_Ions.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4632 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/mpi_main_files/EX_08_Phase_Loop.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5181 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/mpi_main_files/EX_09_Radial_Loop.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5255 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/mpi_main_files/EX_10_Fixed_frequency.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5659 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/mpi_main_files/EX_16_impedance_test.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7914 2023-04-17 11:05:37.000000 blond-2.0.12/__EXAMPLES/mpi_main_files/EX_18_robinson_instability.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.844531 blond-2.0.12/__doc/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      603 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/Makefile
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5664 2022-08-23 13:41:21.000000 blond-2.0.12/__doc/conf.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1162 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/index.rst
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      809 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/make.bat
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.848531 blond-2.0.12/__doc/modules/
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)   135010 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/ACS_cavity_loop.png
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)   185223 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/ACS_cavity_loop.svg
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)     1144 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/RF_noise.gle
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)    81234 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/RF_noise.png
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)   176302 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/SPS_OTFB.png
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)   655573 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/SPS_OTFB.svg
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1002 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/beam.rst
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      177 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/compile.rst
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    51317 2022-08-23 13:41:21.000000 blond-2.0.12/__doc/modules/csr_impedance_real.png
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    19684 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/equations_of_motion.rst
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      737 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/impedances.rst
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      754 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/input_parameters.rst
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)     7100 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/lhc_cavity_loop.rst
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    20259 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/llrf.rst
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      191 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/monitors.rst
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      977 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/plots.rst
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)     1050 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/ring_and_RFstation.gle
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)    84423 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/ring_and_RFstation.png
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)       39 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/sample.dat
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)       77 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/sample2.dat
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)    14087 2022-08-23 13:41:21.000000 blond-2.0.12/__doc/modules/sps_cavity_loop.rst
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      269 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/synchrotron_radiation.rst
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1166 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/toolbox.rst
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      344 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/modules/trackers.rst
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      484 2022-09-12 09:41:29.000000 blond-2.0.12/__doc/modules/utils.rst
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.836531 blond-2.0.12/__doc/themes/
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.852531 blond-2.0.12/__doc/themes/sphinx_rtd_theme/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      324 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3740 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/breadcrumbs.html
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1978 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/footer.html
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7063 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/layout.html
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7526 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/layout_old.html
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1530 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/search.html
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      365 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/searchbox.html
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.836531 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.852531 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/css/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3381 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3153 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/css/badge_only.css.map
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)   114281 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/css/theme.css
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    67610 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/css/theme.css.map
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.856531 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/fonts/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)   124988 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/fonts/FontAwesome.otf
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)   109948 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Bold.ttf
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    96964 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/fonts/Inconsolata-Regular.ttf
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)   656544 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Bold.ttf
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)   656568 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/fonts/Lato-Regular.ttf
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)   170616 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Bold.ttf
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)   169064 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/fonts/RobotoSlab-Regular.ttf
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    76518 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)   391622 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)   152796 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    90412 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    71896 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/fonts/fontawesome-webfont.woff2
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.856531 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/js/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     2457 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/js/copybutton.js~
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    15414 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/js/modernizr.min.js
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     6477 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/static/js/theme.js
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      260 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/theme.conf
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1299 2022-04-06 10:08:34.000000 blond-2.0.12/__doc/themes/sphinx_rtd_theme/versions.html
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1380 2023-04-17 11:05:37.000000 blond-2.0.12/appveyor.yml
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.856531 blond-2.0.12/blond/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1199 2023-04-17 11:05:37.000000 blond-2.0.12/blond/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      162 2023-05-02 16:11:59.000000 blond-2.0.12/blond/_version.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.860531 blond-2.0.12/blond/beam/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2022-04-06 10:08:34.000000 blond-2.0.12/blond/beam/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    20461 2023-04-17 11:05:37.000000 blond-2.0.12/blond/beam/beam.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3685 2022-04-06 10:08:34.000000 blond-2.0.12/blond/beam/coasting_beam.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    41527 2023-04-17 11:05:37.000000 blond-2.0.12/blond/beam/distributions.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    39107 2023-04-17 11:05:37.000000 blond-2.0.12/blond/beam/distributions_multibunch.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    24385 2023-04-17 11:05:37.000000 blond-2.0.12/blond/beam/profile.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5740 2023-05-02 09:00:55.000000 blond-2.0.12/blond/beam/sparse_histogram.cpp
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4804 2022-08-23 13:41:21.000000 blond-2.0.12/blond/beam/sparse_slices.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    11638 2023-05-02 16:09:33.000000 blond-2.0.12/blond/compile.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.860531 blond-2.0.12/blond/cpp_routines/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    10999 2023-05-02 08:01:27.000000 blond-2.0.12/blond/cpp_routines/backup_linear_interp_kick.cpp
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3088 2023-04-17 11:05:37.000000 blond-2.0.12/blond/cpp_routines/beam_phase.cpp
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    29022 2023-05-02 09:00:55.000000 blond-2.0.12/blond/cpp_routines/blondmath.cpp
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    13334 2022-08-23 13:41:21.000000 blond-2.0.12/blond/cpp_routines/blondmath.h
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1316 2022-04-06 10:08:34.000000 blond-2.0.12/blond/cpp_routines/cos.h
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5747 2022-08-23 13:41:21.000000 blond-2.0.12/blond/cpp_routines/drift.cpp
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4376 2022-04-06 10:08:34.000000 blond-2.0.12/blond/cpp_routines/exp.h
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4661 2022-08-23 13:41:21.000000 blond-2.0.12/blond/cpp_routines/fast_resonator.cpp
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    29481 2022-08-23 13:41:21.000000 blond-2.0.12/blond/cpp_routines/fft.cpp
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4419 2022-08-23 13:41:21.000000 blond-2.0.12/blond/cpp_routines/fft.h
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    10013 2023-04-17 11:05:37.000000 blond-2.0.12/blond/cpp_routines/histogram.cpp
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3493 2022-08-23 13:41:21.000000 blond-2.0.12/blond/cpp_routines/kick.cpp
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)   126408 2023-05-02 16:12:01.000000 blond-2.0.12/blond/cpp_routines/libblond.so
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     6406 2023-05-02 09:00:55.000000 blond-2.0.12/blond/cpp_routines/linear_interp_kick.cpp
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    15181 2022-08-23 13:41:21.000000 blond-2.0.12/blond/cpp_routines/music_track.cpp
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      169 2022-04-06 10:08:34.000000 blond-2.0.12/blond/cpp_routines/openmp.cpp
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      245 2022-04-06 10:08:34.000000 blond-2.0.12/blond/cpp_routines/openmp.h
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1960 2022-04-06 10:08:34.000000 blond-2.0.12/blond/cpp_routines/sin.h
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5871 2022-04-06 10:08:34.000000 blond-2.0.12/blond/cpp_routines/sincos.h
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7480 2022-04-06 10:08:34.000000 blond-2.0.12/blond/cpp_routines/vdtcore_common.h
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.860531 blond-2.0.12/blond/gpu/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2023-04-17 11:05:37.000000 blond-2.0.12/blond/gpu/__init__.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.860531 blond-2.0.12/blond/gpu/cuda_kernels/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    14390 2023-04-17 11:05:37.000000 blond-2.0.12/blond/gpu/cuda_kernels/kernels_double.cu
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    14135 2023-04-17 11:05:37.000000 blond-2.0.12/blond/gpu/cuda_kernels/kernels_single.cu
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    10769 2023-04-17 11:05:37.000000 blond-2.0.12/blond/gpu/cupy_butils_wrap.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.860531 blond-2.0.12/blond/impedances/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2022-04-06 10:08:34.000000 blond-2.0.12/blond/impedances/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    39560 2023-04-17 11:05:37.000000 blond-2.0.12/blond/impedances/impedance.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    45892 2023-04-17 11:05:37.000000 blond-2.0.12/blond/impedances/impedance_sources.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3541 2022-08-23 13:41:21.000000 blond-2.0.12/blond/impedances/induced_voltage_analytical.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    12228 2022-04-06 10:08:34.000000 blond-2.0.12/blond/impedances/music.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.860531 blond-2.0.12/blond/input_parameters/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2022-04-06 10:08:34.000000 blond-2.0.12/blond/input_parameters/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    24903 2023-04-17 11:05:37.000000 blond-2.0.12/blond/input_parameters/rf_parameters.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    20249 2022-04-06 10:08:34.000000 blond-2.0.12/blond/input_parameters/rf_parameters_options.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    17272 2022-04-06 10:08:34.000000 blond-2.0.12/blond/input_parameters/ring.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    22443 2022-04-06 10:08:34.000000 blond-2.0.12/blond/input_parameters/ring_options.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.864531 blond-2.0.12/blond/llrf/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2022-04-06 10:08:34.000000 blond-2.0.12/blond/llrf/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    22090 2023-04-17 11:05:37.000000 blond-2.0.12/blond/llrf/beam_feedback.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    36313 2022-08-23 13:41:21.000000 blond-2.0.12/blond/llrf/cavity_feedback.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    14383 2022-08-23 13:41:21.000000 blond-2.0.12/blond/llrf/impulse_response.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     2337 2022-04-06 10:08:34.000000 blond-2.0.12/blond/llrf/notch_filter.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7257 2022-04-06 10:08:34.000000 blond-2.0.12/blond/llrf/offset_frequency.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4394 2022-04-06 10:08:34.000000 blond-2.0.12/blond/llrf/rf_modulation.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    15759 2023-04-17 11:05:37.000000 blond-2.0.12/blond/llrf/rf_noise.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    18814 2022-08-23 13:41:21.000000 blond-2.0.12/blond/llrf/signal_processing.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.864531 blond-2.0.12/blond/monitors/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2022-04-06 10:08:34.000000 blond-2.0.12/blond/monitors/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    20936 2023-04-17 11:05:37.000000 blond-2.0.12/blond/monitors/monitors.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.864531 blond-2.0.12/blond/plots/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2022-04-06 10:08:34.000000 blond-2.0.12/blond/plots/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    11025 2022-04-06 10:08:34.000000 blond-2.0.12/blond/plots/plot.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    10004 2022-04-06 10:08:34.000000 blond-2.0.12/blond/plots/plot_beams.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4777 2022-04-06 10:08:34.000000 blond-2.0.12/blond/plots/plot_impedance.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    14165 2022-04-06 10:08:34.000000 blond-2.0.12/blond/plots/plot_llrf.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1210 2022-04-06 10:08:34.000000 blond-2.0.12/blond/plots/plot_parameters.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     2725 2022-04-06 10:08:34.000000 blond-2.0.12/blond/plots/plot_slices.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     6671 2022-04-06 10:08:34.000000 blond-2.0.12/blond/sanity_check.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.864531 blond-2.0.12/blond/synchrotron_radiation/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2022-04-06 10:08:34.000000 blond-2.0.12/blond/synchrotron_radiation/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5364 2023-05-02 09:00:55.000000 blond-2.0.12/blond/synchrotron_radiation/synchrotron_radiation.cpp
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     8111 2023-04-17 11:05:37.000000 blond-2.0.12/blond/synchrotron_radiation/synchrotron_radiation.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.864531 blond-2.0.12/blond/toolbox/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2022-04-06 10:08:34.000000 blond-2.0.12/blond/toolbox/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5221 2022-04-06 10:08:34.000000 blond-2.0.12/blond/toolbox/action.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7570 2022-04-06 10:08:34.000000 blond-2.0.12/blond/toolbox/diffusion.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7715 2023-04-17 11:05:37.000000 blond-2.0.12/blond/toolbox/filters_and_fitting.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     2070 2022-04-06 10:08:34.000000 blond-2.0.12/blond/toolbox/logger.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3377 2022-04-06 10:08:34.000000 blond-2.0.12/blond/toolbox/next_regular.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    21008 2022-04-06 10:08:34.000000 blond-2.0.12/blond/toolbox/parameter_scaling.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     2358 2023-05-02 09:00:55.000000 blond-2.0.12/blond/toolbox/tomoscope.cpp
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4877 2022-04-06 10:08:34.000000 blond-2.0.12/blond/toolbox/tomoscope.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.864531 blond-2.0.12/blond/trackers/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2022-04-06 10:08:34.000000 blond-2.0.12/blond/trackers/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    26351 2023-04-17 11:05:37.000000 blond-2.0.12/blond/trackers/tracker.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    31233 2023-05-02 07:45:45.000000 blond-2.0.12/blond/trackers/utilities.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.864531 blond-2.0.12/blond/utils/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2022-04-06 10:08:34.000000 blond-2.0.12/blond/utils/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     8233 2023-04-17 11:05:37.000000 blond-2.0.12/blond/utils/bmath.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    48243 2023-04-17 11:05:37.000000 blond-2.0.12/blond/utils/butils_wrap.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3467 2022-04-06 10:08:34.000000 blond-2.0.12/blond/utils/data_check.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1965 2022-04-06 10:08:34.000000 blond-2.0.12/blond/utils/exceptions.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4145 2023-04-17 11:05:37.000000 blond-2.0.12/blond/utils/input_parser.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    14206 2023-04-17 11:05:37.000000 blond-2.0.12/blond/utils/mpi_config.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     1021 2023-04-17 11:05:37.000000 blond-2.0.12/blond/utils/profile_mock.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3914 2022-04-06 10:08:34.000000 blond-2.0.12/blond/utils/track_iteration.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.860531 blond-2.0.12/blond.egg-info/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    14399 2023-05-02 16:12:01.000000 blond-2.0.12/blond.egg-info/PKG-INFO
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     9932 2023-05-02 16:12:01.000000 blond-2.0.12/blond.egg-info/SOURCES.txt
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        1 2023-05-02 16:12:01.000000 blond-2.0.12/blond.egg-info/dependency_links.txt
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        1 2023-04-28 09:39:37.000000 blond-2.0.12/blond.egg-info/not-zip-safe
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      226 2023-05-02 16:12:01.000000 blond-2.0.12/blond.egg-info/requires.txt
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        6 2023-05-02 16:12:01.000000 blond-2.0.12/blond.egg-info/top_level.txt
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)      207 2023-05-02 07:47:33.000000 blond-2.0.12/pyproject.toml
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)       42 2023-05-02 07:47:33.000000 blond-2.0.12/requirements.txt
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)       38 2023-05-02 16:12:01.876531 blond-2.0.12/setup.cfg
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4450 2023-05-02 16:09:33.000000 blond-2.0.12/setup.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.836531 blond-2.0.12/unittests/
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.868531 blond-2.0.12/unittests/beam_profile/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/beam_profile/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)   800196 2022-04-06 10:08:34.000000 blond-2.0.12/unittests/beam_profile/dt_coordinates.npz
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    12422 2022-04-06 10:08:34.000000 blond-2.0.12/unittests/beam_profile/test_beam_profile_object.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7221 2022-08-23 13:41:21.000000 blond-2.0.12/unittests/beam_profile/test_sparse_profile.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.868531 blond-2.0.12/unittests/beams/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/beams/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    14105 2022-08-23 13:41:21.000000 blond-2.0.12/unittests/beams/test_beam_object.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5659 2022-04-06 10:08:34.000000 blond-2.0.12/unittests/beams/test_coasting_beam.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.868531 blond-2.0.12/unittests/general/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/general/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    16184 2022-04-06 10:08:34.000000 blond-2.0.12/unittests/general/test_separatrix_bigaussian.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.868531 blond-2.0.12/unittests/gpu/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/gpu/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5011 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/gpu/test_ffts.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    16996 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/gpu/test_impedance.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    22133 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/gpu/test_physics_kernels.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.868531 blond-2.0.12/unittests/impedances/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/impedances/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4475 2022-04-06 10:08:34.000000 blond-2.0.12/unittests/impedances/test_impedance.py
+-rwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)     4940 2022-08-23 13:41:21.000000 blond-2.0.12/unittests/impedances/test_impedance_sources.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.868531 blond-2.0.12/unittests/input_parameters/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/input_parameters/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     2695 2022-04-06 10:08:34.000000 blond-2.0.12/unittests/input_parameters/test_preprocess.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    10862 2022-08-23 13:41:21.000000 blond-2.0.12/unittests/input_parameters/test_rf_params_object.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     7576 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/input_parameters/test_ring.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.868531 blond-2.0.12/unittests/integration/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/integration/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4307 2023-05-02 07:47:33.000000 blond-2.0.12/unittests/integration/test_examples.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3047 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/integration/test_gpu_examples.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3043 2023-05-02 07:47:33.000000 blond-2.0.12/unittests/integration/test_mpi_examples.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4116 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/integration/test_validate_gpu.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     4005 2022-04-06 10:08:34.000000 blond-2.0.12/unittests/integration/test_validate_mpi.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.872531 blond-2.0.12/unittests/llrf/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/llrf/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    74048 2022-08-23 13:41:21.000000 blond-2.0.12/unittests/llrf/ref_DV_MOD_FR.npy
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    74048 2022-08-23 13:41:21.000000 blond-2.0.12/unittests/llrf/ref_DV_MOD_FRF.npy
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    74048 2022-08-23 13:41:21.000000 blond-2.0.12/unittests/llrf/ref_V_IND_COARSE_GEN.npy
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     8741 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/llrf/test_beam_feedback.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    31675 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/llrf/test_cavity_feedback.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    40554 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/llrf/test_impulse_response.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3649 2022-04-06 10:08:34.000000 blond-2.0.12/unittests/llrf/test_offset_frequency.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     8157 2022-04-06 10:08:34.000000 blond-2.0.12/unittests/llrf/test_rf_modulation.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    31838 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/llrf/test_signal_processing.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.872531 blond-2.0.12/unittests/synchrotron_radiation/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/synchrotron_radiation/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    32615 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/synchrotron_radiation/test_synch_rad.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.872531 blond-2.0.12/unittests/trackers/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/trackers/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    17866 2022-04-06 10:08:34.000000 blond-2.0.12/unittests/trackers/comparison_drift.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    19415 2022-04-06 10:08:34.000000 blond-2.0.12/unittests/trackers/test_drift.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    10188 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/trackers/test_tracker.py
+drwxrwxr-x   0 kiliakis  (1000) kiliakis  (1000)        0 2023-05-02 16:12:01.876531 blond-2.0.12/unittests/utils/
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)        0 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/utils/__init__.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)    21108 2023-04-17 11:05:37.000000 blond-2.0.12/unittests/utils/test_blondmath.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     3790 2022-04-06 10:08:34.000000 blond-2.0.12/unittests/utils/test_data_check.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     9952 2022-04-06 10:08:34.000000 blond-2.0.12/unittests/utils/test_ffts.py
+-rw-rw-r--   0 kiliakis  (1000) kiliakis  (1000)     5103 2022-04-06 10:08:34.000000 blond-2.0.12/unittests/utils/test_iteration.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `blond-2.0.11/blond/beam/coasting_beam.py` & `blond-2.0.12/blond/beam/coasting_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/beam/distributions.py` & `blond-2.0.12/blond/beam/distributions.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import copy
 import gc
 import matplotlib.pyplot as plt
 from scipy.integrate import cumtrapz
 from ..trackers.utilities import is_in_separatrix
 from ..beam.profile import Profile, CutOptions
 from ..trackers.utilities import potential_well_cut, minmax_location
+from ..utils import bmath as bm
 
 def matched_from_line_density(beam, full_ring_and_RF, line_density_input=None,
                               main_harmonic_option='lowest_freq',
                               TotalInducedVoltage=None, plot=False,
                               figdir='fig', half_option='first',
                               extraVoltageDict=None, n_iterations=100,
                               n_points_potential=1e4, n_points_grid=int(1e3),
@@ -41,19 +42,19 @@
     '''
     *Function to generate a beam by inputing the line density. The distribution
     function is then reconstructed with the Abel transform and the particles
     randomly generated.*
     '''    
         
     # Initialize variables depending on the accelerator parameters
-    slippage_factor = full_ring_and_RF.RingAndRFSection_list[0].eta_0[0]
+    slippage_factor = full_ring_and_RF.RingAndRFSection_list[0].rf_params.eta_0[0]
     
     eom_factor_dE = abs(slippage_factor) / (2*beam.beta**2. * beam.energy)
     eom_factor_potential = (np.sign(slippage_factor) * beam.Particle.charge /
-                          (full_ring_and_RF.RingAndRFSection_list[0].t_rev[0]))
+                          (full_ring_and_RF.RingAndRFSection_list[0].rf_params.t_rev[0]))
      
     #: *Number of points to be used in the potential well calculation*
     n_points_potential = int(n_points_potential)
     # Generate potential well
     full_ring_and_RF.potential_well_generation(n_points=n_points_potential, 
                                 dt_margin_percent=dt_margin_percent, 
                                 main_harmonic_option=main_harmonic_option)
@@ -68,30 +69,30 @@
         extra_potential_input = - (eom_factor_potential *
                                 cumtrapz(extra_voltage_input,
                                 dx=extra_voltage_time_input[1] -
                                 extra_voltage_time_input[0], initial=0))
         extra_potential = np.interp(time_potential, extra_voltage_time_input,
                                     extra_potential_input)
     
-    if line_density_type is not 'user_input':
+    if line_density_type != 'user_input':
         # Time coordinates for the line density
         n_points_line_den = int(1e4)
         time_line_den = np.linspace(float(time_potential[0]), float(time_potential[-1]),
                                     n_points_line_den)
         line_den_resolution = time_line_den[1] - time_line_den[0]
                         
         # Normalizing the line density
         line_density_ = line_density(time_line_den, line_density_type,
                  bunch_length, exponent=line_density_exponent,
                  bunch_position=(time_potential[0]+time_potential[-1])/2)
         
         line_density_ -= np.min(line_density_)
         line_density_ *= beam.n_macroparticles / np.sum(line_density_)
 
-    elif line_density_type is 'user_input':
+    elif line_density_type == 'user_input':
         # Time coordinates for the line density
         time_line_den = line_density_input['time_line_den']
         n_points_line_den = len(time_line_den)
         line_den_resolution = time_line_den[1] - time_line_den[0]
                         
         # Normalizing the line density
         line_density_ = line_density_input['line_density']
@@ -187,30 +188,30 @@
             profile.cut_options.set_cuts()
             profile.set_slices_parameters()
     
     # Taking the first/second half of line density and potential
     n_points_abel = int(n_points_abel)
     
     abel_both_step = 1
-    if half_option is 'both':
+    if half_option == 'both':
         abel_both_step = 2
         distribution_function_average = np.zeros((n_points_abel,2))
         hamiltonian_average = np.zeros((n_points_abel,2))
         
     for abel_index in range(0, abel_both_step):
-        if half_option is 'first':
+        if half_option == 'first':
             half_indexes = np.where((time_line_den >= time_line_den[0]) *
                                     (time_line_den <= max_profile_pos))
-        if half_option is 'second':
+        if half_option == 'second':
             half_indexes = np.where((time_line_den >= max_profile_pos) *
                                     (time_line_den <= time_line_den[-1]))
-        if half_option is 'both' and abel_index == 0:
+        if half_option == 'both' and abel_index == 0:
             half_indexes = np.where((time_line_den >= time_line_den[0]) *
                                     (time_line_den <= max_profile_pos))
-        if half_option is 'both' and abel_index == 1:
+        if half_option == 'both' and abel_index == 1:
             half_indexes = np.where((time_line_den >= max_profile_pos) *
                                     (time_line_den <= time_line_den[-1]))
         
         line_den_half = line_density_[half_indexes]
         time_half = time_line_den[half_indexes]
         potential_half = np.interp(time_half, time_potential_sep,
                                    potential_well_sep)
@@ -231,15 +232,15 @@
         
         distribution_function_ = np.zeros(n_points_abel)
         hamiltonian_coord = np.zeros(n_points_abel) 
         
         # Abel transform
         warnings.filterwarnings("ignore")
         
-        if (half_option is 'first') or (half_option is 'both' and
+        if (half_option == 'first') or (half_option == 'both' and
                                         abel_index == 0):
             for i in range(0, n_points_abel):
                 integrand = (line_den_diff_abel[:i+1] /
                              np.sqrt(potential_abel[:i+1] - potential_abel[i]))
                         
                 if len(integrand)>2:
                     integrand[-1] = integrand[-2] + (integrand[-2] -
@@ -250,15 +251,15 @@
                     integrand = np.array([0])
                     
                 distribution_function_[i] = (np.sqrt(eom_factor_dE) / np.pi *
                     np.trapz(integrand, dx=line_den_resolution))
         
                 hamiltonian_coord[i] = potential_abel[i]
                 
-        if (half_option is 'second') or (half_option is 'both' and
+        if (half_option == 'second') or (half_option == 'both' and
                                          abel_index == 1):
             for i in range(0, n_points_abel):
                 integrand = (line_den_diff_abel[i:] /
                              np.sqrt(potential_abel[i:] - potential_abel[i]))
     
                 if len(integrand)>2:
                     integrand[0] = integrand[1] + (integrand[2] - integrand[1])
@@ -273,21 +274,21 @@
         
         warnings.filterwarnings("default")
     
         # Cleaning the distribution function from unphysical results
         distribution_function_[np.isnan(distribution_function_)] = 0
         distribution_function_[distribution_function_<0] = 0
         
-        if half_option is 'both':
+        if half_option == 'both':
             hamiltonian_average[:,abel_index] = hamiltonian_coord
             distribution_function_average[:,abel_index] = \
                                                          distribution_function_
             
             
-    if half_option is 'both':
+    if half_option == 'both':
         hamiltonian_coord = hamiltonian_average[:,0]
         distribution_function_ = (distribution_function_average[:,0] +
                          np.interp(hamiltonian_coord, hamiltonian_average[:,1],
                                    distribution_function_average[:,1])) / 2
         
     # Compute deltaE frame corresponding to the separatrix
     max_potential = np.max(potential_half)
@@ -325,17 +326,17 @@
     # Ploting the result
     if plot:
         plt.figure('Generated bunch')
         plt.plot(time_line_den, line_density_)        
         plt.plot(time_for_grid, reconstructed_line_den / 
                         np.max(reconstructed_line_den) * np.max(line_density_))
         plt.title('Line densities')
-        if plot is 'show':
+        if plot == 'show':
             plt.show()
-        elif plot is 'savefig':
+        elif plot == 'savefig':
             fign = figdir + '/generated_bunch.png'
             plt.savefig(fign)
     
     # Populating the bunch
     populate_bunch(beam, time_grid, deltaE_grid, density_grid,
                    time_for_grid[1]-time_for_grid[0],
                    deltaE_for_grid[1]-deltaE_for_grid[0], seed)
@@ -406,21 +407,21 @@
     # Loading the distribution function if provided by the user
     if distribution_function_input is not None:
         distribution_function_ = distribution_function_input
     else:
         distribution_function_ = distribution_function
     
     # Initialize variables depending on the accelerator parameters
-    slippage_factor = full_ring_and_RF.RingAndRFSection_list[0].eta_0[turn_number]
+    slippage_factor = full_ring_and_RF.RingAndRFSection_list[0].rf_params.eta_0[turn_number]
     beta = full_ring_and_RF.RingAndRFSection_list[0].rf_params.beta[turn_number]
     energy = full_ring_and_RF.RingAndRFSection_list[0].rf_params.energy[turn_number]
     
     eom_factor_dE = abs(slippage_factor) / (2*beta**2. * energy)
     eom_factor_potential = (np.sign(slippage_factor) * beam.Particle.charge /
-                          (full_ring_and_RF.RingAndRFSection_list[0].t_rev[turn_number]))
+                          (full_ring_and_RF.RingAndRFSection_list[0].rf_params.t_rev[turn_number]))
 
     #: *Number of points to be used in the potential well calculation*
     n_points_potential = int(n_points_potential)
     # Generate potential well
     full_ring_and_RF.potential_well_generation(turn=turn_number,
                                     n_points=n_points_potential,
                                     dt_margin_percent=dt_margin_percent, 
@@ -536,18 +537,18 @@
         
         # Calculating the H and J grid
         H_grid = eom_factor_dE * deltaE_grid**2 + potential_well_grid
         J_grid = np.interp(H_grid, sorted_H_dE0, sorted_J_dE0, left=0,
                            right=np.inf)
         
         # Choice of either H or J as the variable used
-        if distribution_variable is 'Action':
+        if distribution_variable == 'Action':
             sorted_X_dE0 = sorted_J_dE0
             X_grid = J_grid
-        elif distribution_variable is 'Hamiltonian':
+        elif distribution_variable == 'Hamiltonian':
             sorted_X_dE0 = sorted_H_dE0
             X_grid = H_grid
         else:
             #DistributionError
             raise RuntimeError('The distribution_variable option was not ' +
                                'recognized')
         
@@ -557,17 +558,17 @@
             X0 = X0_from_bunch_length(bunch_length, bunch_length_fit, 
                                 X_grid, sorted_X_dE0, n_points_grid, 
                                 time_potential_low_res, distribution_function_, 
                                 distribution_type, distribution_exponent, beam,
                                 full_ring_and_RF)
        
         elif emittance is not None:
-            if distribution_variable is 'Action':
+            if distribution_variable == 'Action':
                 X0 = emittance / (2*np.pi)
-            elif distribution_variable is 'Hamiltonian':
+            elif distribution_variable == 'Hamiltonian':
                 X0 = np.interp(emittance / (2*np.pi), sorted_J_dE0,
                                sorted_H_dE0)
         
         # Computing the density grid
         if distribution_user_table is None:
             density_grid = distribution_function_(X_grid, distribution_type,
                                                   X0, distribution_exponent)
@@ -634,24 +635,24 @@
     tau = 0.0
     
     # Initial values for iteration
     X_low = sorted_X_dE0[0]
     X_hi = sorted_X_dE0[-1]
     X_min = sorted_X_dE0[0]
     X_max = sorted_X_dE0[-1]
-    X_accuracy = sorted_X_dE0[1] - sorted_X_dE0[0] / 2.0
+    X_accuracy = (sorted_X_dE0[1] - sorted_X_dE0[0]) / 2.0
     
     bin_size = (time_potential_low_res[1] - time_potential_low_res[0])
     
     # Iteration to find H0/J0 from the bunch length
     while np.abs(bunch_length-tau) > bin_size:
         # Takes middle point of the interval [X_low,X_hi]
         X0 = 0.5 * (X_low + X_hi)
         
-        if bunch_length_fit is 'full':
+        if bunch_length_fit == 'full':
             bunchIndices = np.where(np.sum(X_grid<=X0, axis=0))[0]
             tau = (time_potential_low_res[bunchIndices][-1] -
                    time_potential_low_res[bunchIndices][0])
         else:
             # Calculating the line density for the parameter X0
             density_grid = distribution_function_(X_grid,
                               distribution_type, X0, distribution_exponent)
@@ -675,21 +676,21 @@
 #                       full_ring_and_RF.RingAndRFSection_list[0].rf_params,
 #                       beam, n_points_grid, cut_left=time_potential_low_res[0] -
 #                       0.5*bin_size , cut_right=time_potential_low_res[-1] +
 #                       0.5*bin_size)
                         
                     profile.n_macroparticles = line_density_
                     
-                    if bunch_length_fit is 'gauss':
+                    if bunch_length_fit == 'gauss':
                         profile.bl_gauss = tau
                         profile.bp_gauss = np.sum(line_density_ *
                                 time_potential_low_res) / np.sum(line_density_)
                         profile.gaussian_fit()
                         tau = profile.bl_gauss
-                    elif bunch_length_fit is 'fwhm':
+                    elif bunch_length_fit == 'fwhm':
                         profile.fwhm()
                         tau = profile.bunchLength                        
         
         # Update of the interval for the next iteration
         if tau >= bunch_length:
             X_hi = X0
         else:
@@ -720,39 +721,39 @@
     # Generating particles randomly inside the grid cells according to the
     # provided density_grid
     indexes = np.random.choice(np.arange(0,np.size(density_grid)), 
                                beam.n_macroparticles, p=density_grid.flatten())
     
     # Randomize particles inside each grid cell (uniform distribution)
     beam.dt = (np.ascontiguousarray(time_grid.flatten()[indexes] +
-        (np.random.rand(beam.n_macroparticles) - 0.5) * time_step))
+                                    (np.random.rand(beam.n_macroparticles) - 0.5) * time_step)).astype(dtype=bm.precision.real_t, order='C', copy=False)
     beam.dE = (np.ascontiguousarray(deltaE_grid.flatten()[indexes] +
-        (np.random.rand(beam.n_macroparticles) - 0.5) * deltaE_step))
+                                    (np.random.rand(beam.n_macroparticles) - 0.5) * deltaE_step)).astype(dtype=bm.precision.real_t, order='C', copy=False)
 
 def distribution_function(action_array, dist_type, length, exponent=None):
     '''
     *Distribution function (formulas from Laclare).*
     '''
     
     if dist_type in ['binomial', 'waterbag', 'parabolic_amplitude',
                      'parabolic_line']:
-        if dist_type is 'waterbag':
+        if dist_type == 'waterbag':
             exponent = 0
-        elif dist_type is 'parabolic_amplitude':
+        elif dist_type == 'parabolic_amplitude':
             exponent = 1
-        elif dist_type is 'parabolic_line':
+        elif dist_type == 'parabolic_line':
             exponent = 0.5
 
         warnings.filterwarnings("ignore")
         distribution_function_ = (1 - action_array / length)**exponent
         warnings.filterwarnings("default")
         distribution_function_[action_array > length] = 0
         return distribution_function_
     
-    elif dist_type is 'gaussian':
+    elif dist_type == 'gaussian':
         distribution_function_ = np.exp(- 2 * action_array / length)
         return distribution_function_
 
     else:
         #DistributionError
         raise RuntimeError('The dist_type option was not recognized')
     
@@ -762,44 +763,44 @@
                  exponent=None):
     '''
     *Line density*
     '''
     
     if dist_type in ['binomial', 'waterbag', 'parabolic_amplitude',
                      'parabolic_line']:
-        if dist_type is 'waterbag':
+        if dist_type == 'waterbag':
             exponent = 0
-        elif dist_type is 'parabolic_amplitude':
+        elif dist_type == 'parabolic_amplitude':
             exponent = 1
-        elif dist_type is 'parabolic_line':
+        elif dist_type == 'parabolic_line':
             exponent = 0.5
         
         warnings.filterwarnings("ignore")
         line_density_ = ((1 - (2.0 * (coord_array - bunch_position) /
                          bunch_length)**2)**(exponent+0.5))
         warnings.filterwarnings("default")
         line_density_[np.abs(coord_array-bunch_position) > bunch_length/2] = 0
         return line_density_
     
-    elif dist_type is 'gaussian':
+    elif dist_type == 'gaussian':
         sigma = bunch_length/4
         line_density_ = np.exp(-(coord_array-bunch_position)**2 / (2*sigma**2))
         return line_density_
     
-    elif dist_type is 'cosine_squared':
+    elif dist_type == 'cosine_squared':
         warnings.filterwarnings("ignore")
         line_density_ = ( np.cos(np.pi * (coord_array - bunch_position) /
                                  bunch_length)**2 )
         warnings.filterwarnings("default")
         line_density_[np.abs(coord_array-bunch_position) > bunch_length/2] = 0
         return line_density_
 
 
 
-def bigaussian(Ring, RFStation, Beam, sigma_dt, sigma_dE = None, seed = None,
+def bigaussian(Ring, RFStation, Beam, sigma_dt, sigma_dE = None, seed = 1234,
                reinsertion = False):
     r"""Function generating a Gaussian beam both in time and energy 
     coordinates. Fills Beam.dt and Beam.dE arrays.
     
     Parameters
     ---------- 
     Ring : class
@@ -855,31 +856,30 @@
         sigma_dE = np.sqrt( voltage * energy * beta**2  
             * (np.cos(phi_b) - np.cos(phi_s) + (phi_b - phi_s) * np.sin(phi_s)) 
             / (np.pi * harmonic * np.fabs(eta0)) )
                 
     Beam.sigma_dt = sigma_dt
     Beam.sigma_dE = sigma_dE
     
-    # Generate coordinates
-    np.random.seed(seed)
-    
-    Beam.dt = sigma_dt*np.random.randn(Beam.n_macroparticles) + \
-              (phi_s - phi_rf)/omega_rf                  
-    Beam.dE = sigma_dE*np.random.randn(Beam.n_macroparticles)
+    # Generate coordinates. For reproducibility, a separate random number stream is used for dt and dE
+    rng_dt = np.random.default_rng(seed)
+    rng_dE = np.random.default_rng(seed+1)
+    
+    Beam.dt = sigma_dt * rng_dt.normal(size=Beam.n_macroparticles).astype(dtype=bm.precision.real_t, order='C', copy=False) + \
+        (phi_s - phi_rf)/omega_rf
+    Beam.dE = sigma_dE * rng_dE.normal(size=Beam.n_macroparticles).astype(dtype=bm.precision.real_t, order='C')
     
     # Re-insert if necessary
     if reinsertion == True:
         
         itemindex = np.where(is_in_separatrix(Ring, 
             RFStation, Beam, Beam.dt, Beam.dE) == False)[0]
          
         while itemindex.size != 0:
             
-            Beam.dt[itemindex] = sigma_dt*np.random.randn(itemindex.size) \
-                                 + (phi_s - phi_rf)/omega_rf
-                                     
-            Beam.dE[itemindex] = sigma_dE*np.random.randn(itemindex.size)
-            itemindex = np.where(is_in_separatrix(Ring, 
-                RFStation, Beam, Beam.dt, Beam.dE) == False)[0]
-
-
-
+            Beam.dt[itemindex] = sigma_dt * rng_dt.normal(size=itemindex.size).astype(dtype=bm.precision.real_t, order='C', copy=False) \
+                + (phi_s - phi_rf)/omega_rf
+            
+            Beam.dE[itemindex] = sigma_dE * rng_dE.normal(size=itemindex.size).astype(dtype=bm.precision.real_t, order='C')
+            
+            itemindex = np.where(is_in_separatrix(Ring,
+                                                  RFStation, Beam, Beam.dt, Beam.dE) == False)[0]
```

### Comparing `blond-2.0.11/blond/beam/distributions_multibunch.py` & `blond-2.0.12/blond/beam/distributions_multibunch.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,148 +6,150 @@
 
 from __future__ import division, print_function, absolute_import
 from builtins import range
 import numpy as np
 import copy
 import matplotlib.pyplot as plt
 from scipy.integrate import cumtrapz
+import gc
+from ..utils import bmath as bm
 
 from ..beam.beam import Beam
 from ..beam.distributions import matched_from_distribution_function,\
                            matched_from_line_density, populate_bunch,\
                            distribution_function, potential_well_cut,\
                            X0_from_bunch_length
 
 def matched_from_distribution_density_multibunch(beam, Ring, FullRingAndRF, distribution_options_list,
                                       n_bunches, bunch_spacing_buckets,
                                       intensity_list = None,
                                       minimum_n_macroparticles = None,
-                                      main_harmonic_option = 'lowest_freq', 
+                                      main_harmonic_option = 'lowest_freq',
                                       TotalInducedVoltage = None,
                                       n_iterations_input = 1,
                                       plot_option = False, seed=None):
     '''
     *Function to generate a multi-bunch beam using the matched_from_distribution_density
-    function for each bunch. The extra parameters to include are the number of 
+    function for each bunch. The extra parameters to include are the number of
     bunches and the spacing between two bunches (assumed constant presently).
     Moreover, the distribution_options_list corresponds to the distribution_options
     of the matched_from_distribution_density function. It can be inputed as
     a dictionary just like the matched_from_distribution_density function (assuming
     the same parameters for all bunches), or as a list of length n_bunches
     to have different parameters for each bunch.*
-    '''  
+    '''
+
 
-    
     if intensity_list is None:
         intensity_per_bunch = beam.intensity/n_bunches * np.ones(n_bunches)
         n_macroparticles_per_bunch = beam.n_macroparticles/n_bunches * np.ones(n_bunches)
     else:
         intensity_per_bunch = np.array(intensity_list)
         if minimum_n_macroparticles is None:
             n_macroparticles_per_bunch = np.round(beam.n_macroparticles/beam.intensity * intensity_per_bunch)
         else:
             n_macroparticles_per_bunch = np.round(minimum_n_macroparticles/np.min(intensity_per_bunch) * intensity_per_bunch)
-    
+
     if np.sum(intensity_per_bunch) != beam.intensity:
         print('WARNING !! The total intensity per bunch does not match the total intensity of the beam, the beam.intensity will be overwritten')
         beam.intensity = np.sum(intensity_per_bunch)
-    
-    
+
+
     if np.sum(n_macroparticles_per_bunch) != beam.n_macroparticles:
         print('WARNING !! The number of macroparticles per bunch does not match the total number of the beam, the beam.n_macroparticles will be overwritten')
         beam.n_macroparticles = int(np.sum(n_macroparticles_per_bunch))
 
     voltages = np.array([])
     harmonics = np.array([])
-        
+
     for RingAndRFSectionElement in FullRingAndRF.RingAndRFSection_list:
-            for rf_system in range(RingAndRFSectionElement.n_rf):
-                voltages = np.append(voltages, RingAndRFSectionElement.voltage[rf_system, 0])
-                harmonics = np.append(harmonics, RingAndRFSectionElement.harmonic[rf_system, 0])
-                
-    if main_harmonic_option is 'lowest_freq':
+            for rf_system in range(RingAndRFSectionElement.rf_params.n_rf):
+                voltages = np.append(voltages, RingAndRFSectionElement.rf_params.voltage[rf_system, 0])
+                harmonics = np.append(harmonics, RingAndRFSectionElement.rf_params.harmonic[rf_system, 0])
+
+    if main_harmonic_option == 'lowest_freq':
             main_harmonic = np.min(harmonics)
-    elif main_harmonic_option is 'highest_voltage':
+    elif main_harmonic_option == 'highest_voltage':
         main_harmonic = np.min(harmonics[voltages == np.max(voltages)])
     elif isinstance(main_harmonic_option, int) or isinstance(main_harmonic_option, float):
         if harmonics[harmonics == main_harmonic_option].size == 0:
             #GenerationError
             raise RuntimeError('The desired harmonic to compute the potential well does not match the RF parameters...')
         main_harmonic = np.min(harmonics[harmonics == main_harmonic_option])
-         
+
     bucket_size_tau = 2 * np.pi / (main_harmonic * Ring.omega_rev[0])
 
     beamIteration = Beam(Ring, 1, 0.)
-    
+
     extraVoltageDict = None
-    
+
     if TotalInducedVoltage is not None:
         bucket_tolerance = 0.40
         TotalInducedVoltageIteration = copy.deepcopy(TotalInducedVoltage)
         TotalInducedVoltageIteration.profile.Beam = beamIteration
-        
-    
+
+
     for indexBunch in range(0, n_bunches):
-        
+
         print('Generating bunch no %d' %(indexBunch+1))
-        
+
         bunch = Beam(Ring, int(n_macroparticles_per_bunch[indexBunch]), intensity_per_bunch[indexBunch])
-        
+
         if isinstance(distribution_options_list, list):
             distribution_options = distribution_options_list[indexBunch]
         elif isinstance(distribution_options_list, dict):
             distribution_options = distribution_options_list
         else:
             #DistributionError
             raise RuntimeError('The input distribution_options_list option of the matched_from_distribution_density_multibunch \
             function should either be a dictionary as requested by the matched_from_distribution_density \
             function, or a list of dictionaries containing n_bunches elements')
-        
+
         if 'type' in distribution_options:
             distribution_type = distribution_options['type']
         else:
             distribution_type = None
-        
+
         if 'exponent' in distribution_options:
             distribution_exponent = distribution_options['exponent']
         else:
             distribution_exponent = None
-        
+
         if 'emittance' in distribution_options:
             emittance = distribution_options['emittance']
         else:
             emittance = None
-        
+
         if 'bunch_length' in distribution_options:
             bunch_length = distribution_options['bunch_length']
         else:
             bunch_length = None
-        
+
         if 'bunch_length_fit' in distribution_options:
             bunch_length_fit = distribution_options['bunch_length_fit']
         else:
             bunch_length_fit = None
-        
+
         if 'density_variable' in distribution_options:
             distribution_variable = distribution_options['density_variable']
         else:
-            distribution_variable = None            
-        
-        if distribution_options['type'] is 'user_input':
+            distribution_variable = None
+
+        if distribution_options['type'] == 'user_input':
             distribution_function_input = distribution_options['function']
         else:
             distribution_function_input = None
-        
-        if distribution_options['type'] is 'user_input_table':
+
+        if distribution_options['type'] == 'user_input_table':
             distribution_user_table = {
               'user_table_action': distribution_options['user_table_action'],
               'user_table_density': distribution_options['user_table_density']}
         else:
             distribution_user_table = None
-            
+
         matched_from_distribution_function(bunch, FullRingAndRF,
                        distribution_function_input=distribution_function_input,
                        distribution_user_table=distribution_user_table,
                        main_harmonic_option=main_harmonic_option,
                        TotalInducedVoltage=TotalInducedVoltage,
                        n_iterations=n_iterations_input,
                        extraVoltageDict=extraVoltageDict,
@@ -157,172 +159,172 @@
                        bunch_length_fit=bunch_length_fit,
                        distribution_variable=distribution_variable, seed=seed)
 
         if indexBunch==0:
             beamIteration.dt = bunch.dt
             beamIteration.dE = bunch.dE
         else:
-            beamIteration.dt = np.append(beamIteration.dt, bunch.dt + 
+            beamIteration.dt = np.append(beamIteration.dt, bunch.dt +
                         (indexBunch * bunch_spacing_buckets * bucket_size_tau))
             beamIteration.dE = np.append(beamIteration.dE, bunch.dE)
-        
+
         beamIteration.n_macroparticles = int(np.sum(n_macroparticles_per_bunch[:indexBunch+1]))
         beamIteration.intensity = np.sum(intensity_per_bunch[:indexBunch+1])
         beamIteration.ratio = beamIteration.intensity / beamIteration.n_macroparticles
-        
-        
+
+
         if TotalInducedVoltage is not None:
             TotalInducedVoltageIteration.profile.track()
             TotalInducedVoltageIteration.induced_voltage_sum()
 
-            left_edge = ((indexBunch + 1) * bunch_spacing_buckets * 
+            left_edge = ((indexBunch + 1) * bunch_spacing_buckets *
                           bucket_size_tau - bucket_tolerance * bucket_size_tau)
-            right_edge = (((indexBunch + 1) * bunch_spacing_buckets + 1) * 
+            right_edge = (((indexBunch + 1) * bunch_spacing_buckets + 1) *
                           bucket_size_tau + bucket_tolerance * bucket_size_tau)
-            
+
             bin_centers = TotalInducedVoltageIteration.profile.bin_centers
-            
+
             tau_induced_voltage_next_bunch = bin_centers[
                         (bin_centers > left_edge) * (bin_centers < right_edge)]
             induced_voltage_next_bunch = \
                         TotalInducedVoltageIteration.induced_voltage[
                         (bin_centers > left_edge) * (bin_centers < right_edge)]
 
             time_induced_voltage_next_bunch = (tau_induced_voltage_next_bunch -
                       (indexBunch+1) * bunch_spacing_buckets * bucket_size_tau)
-            
+
             extraVoltageDict = {'time_array':time_induced_voltage_next_bunch,
                                 'voltage_array':induced_voltage_next_bunch}
 
-            
+
         if plot_option:
             plt.figure('Bunch train + induced voltage')
             plt.clf()
             plt.plot(TotalInducedVoltageIteration.profile.bin_centers,
-                     TotalInducedVoltageIteration.profile.n_macroparticles / 
+                     TotalInducedVoltageIteration.profile.n_macroparticles /
                      (1.*np.max(TotalInducedVoltageIteration.profile.n_macroparticles)) *
                      np.max(TotalInducedVoltageIteration.induced_voltage))
             plt.plot(TotalInducedVoltageIteration.profile.bin_centers,
                      TotalInducedVoltageIteration.induced_voltage)
             plt.show()
                 
-    beam.dt = beamIteration.dt
+    beam.dt = beamIteration.dt.astype(dtype=bm.precision.real_t, order='C', copy=False)
+    beam.dE = beamIteration.dE.astype(dtype=bm.precision.real_t, order='C', copy=False)
+    gc.collect()
+
 
-    beam.dE = beamIteration.dE
-    
-    
 def matched_from_line_density_multibunch(beam, Ring,
                         FullRingAndRF, line_density_options_list, n_bunches,
                         bunch_spacing_buckets, intensity_list=None,
                         minimum_n_macroparticles=None,
                         main_harmonic_option='lowest_freq',
                         TotalInducedVoltage=None, half_option='first',
                         plot_option=False, seed=None):
     '''
     *Function to generate a multi-bunch beam using the matched_from_distribution_density
-    function for each bunch. The extra parameters to include are the number of 
+    function for each bunch. The extra parameters to include are the number of
     bunches and the spacing between two bunches (assumed constant presently).
     Moreover, the line_density_options_list corresponds to the distribution_options
     of the matched_from_line_density function. It can be inputed as
     a dictionary just like the matched_from_line_density function (assuming
     the same parameters for all bunches), or as a list of length n_bunches
     to have different parameters for each bunch.*
     '''
-    
+
     if intensity_list is None:
         intensity_per_bunch = beam.intensity/n_bunches * np.ones(n_bunches)
         n_macroparticles_per_bunch = beam.n_macroparticles/n_bunches * np.ones(n_bunches)
     else:
         intensity_per_bunch = np.array(intensity_list)
         if minimum_n_macroparticles is None:
             n_macroparticles_per_bunch = np.round(beam.n_macroparticles/beam.intensity * intensity_per_bunch)
         else:
             n_macroparticles_per_bunch = np.round(minimum_n_macroparticles/np.min(intensity_per_bunch) * intensity_per_bunch)
-        
+
     if np.sum(intensity_per_bunch) != beam.intensity:
         print('WARNING !! The total intensity per bunch does not match the total intensity of the beam, the beam.intensity will be overwritten')
         beam.intensity = np.sum(intensity_per_bunch)
-    
+
     if np.sum(n_macroparticles_per_bunch) != beam.n_macroparticles:
         print('WARNING !! The number of macroparticles per bunch does not match the total number of the beam, the beam.n_macroparticles will be overwritten')
         beam.n_macroparticles = int(np.sum(n_macroparticles_per_bunch))
-    
+
     voltages = np.array([])
     harmonics = np.array([])
-        
+
     for RingAndRFSectionElement in FullRingAndRF.RingAndRFSection_list:
-            for rf_system in range(RingAndRFSectionElement.n_rf):
-                voltages = np.append(voltages, RingAndRFSectionElement.voltage[rf_system, 0])
-                harmonics = np.append(harmonics, RingAndRFSectionElement.harmonic[rf_system, 0])
-                
-    if main_harmonic_option is 'lowest_freq':
+            for rf_system in range(RingAndRFSectionElement.rf_params.n_rf):
+                voltages = np.append(voltages, RingAndRFSectionElement.rf_params.voltage[rf_system, 0])
+                harmonics = np.append(harmonics, RingAndRFSectionElement.rf_params.harmonic[rf_system, 0])
+
+    if main_harmonic_option == 'lowest_freq':
             main_harmonic = np.min(harmonics)
-    elif main_harmonic_option is 'highest_voltage':
+    elif main_harmonic_option == 'highest_voltage':
         main_harmonic = np.min(harmonics[voltages == np.max(voltages)])
     elif isinstance(main_harmonic_option, int) or isinstance(main_harmonic_option, float):
         if harmonics[harmonics == main_harmonic_option].size == 0:
             #GenerationError
             raise RuntimeError('The desired harmonic to compute the potential well does not match the RF parameters...')
         main_harmonic = np.min(harmonics[harmonics == main_harmonic_option])
-            
+
     bucket_size_tau = 2 * np.pi / (main_harmonic * Ring.omega_rev[0])
-    
+
     beamIteration = Beam(Ring, 1, 0.)
-    
+
     extraVoltageDict = None
-    
+
     if TotalInducedVoltage is not None:
         TotalInducedVoltageIteration = copy.deepcopy(TotalInducedVoltage)
         TotalInducedVoltageIteration.profile.Beam = beamIteration
-        
-    
+
+
     for indexBunch in range(0, n_bunches):
-        
+
         print('Generating bunch no %d' %(indexBunch+1))
-        
+
         bunch = Beam(Ring,
                      int(n_macroparticles_per_bunch[indexBunch]),
                      intensity_per_bunch[indexBunch])
-        
+
         if isinstance(line_density_options_list, list):
             line_density_options = line_density_options_list[indexBunch]
         elif isinstance(line_density_options_list, dict):
             line_density_options = line_density_options_list
         else:
             #GenerationError
             raise RuntimeError('The input line_density_options_list option ' +
                                'of the matched_from_line_density_multibunch ' +
                                'function should either be a dictionary as ' +
                                'requested by the matched_from_line_density ' +
                                'function, or a list of dictionaries ' +
                                'containing n_bunches elements')
-        
-        
+
+
         if 'bunch_length' in line_density_options:
             bunch_length = line_density_options['bunch_length']
         else:
             bunch_length = None
-                              
+
         if 'type' in line_density_options:
             line_density_type = line_density_options['type']
         else:
             line_density_type = None
-        
+
         if 'exponent' in line_density_options:
             line_density_exponent = line_density_options['exponent']
         else:
             line_density_exponent = None
-        
-        if line_density_options['type'] is 'user_input':
+
+        if line_density_options['type'] == 'user_input':
             line_density_input = {
                         'time_line_den': line_density_options['time_line_den'],
                         'line_density': line_density_options['line_density']}
         else:
             line_density_input = None
-        
+
         matched_from_line_density(bunch, FullRingAndRF,
                               line_density_input=line_density_input,
                               main_harmonic_option=main_harmonic_option,
                               TotalInducedVoltage=TotalInducedVoltage,
                               plot=plot_option, half_option=half_option,
                               extraVoltageDict=extraVoltageDict,
                               bunch_length=bunch_length,
@@ -333,70 +335,71 @@
         if indexBunch==0:
             beamIteration.dt = bunch.dt
             beamIteration.dE = bunch.dE
         else:
             beamIteration.dt = np.append(beamIteration.dt, bunch.dt +
                         (indexBunch * bunch_spacing_buckets * bucket_size_tau))
             beamIteration.dE = np.append(beamIteration.dE, bunch.dE)
-        
+
         beamIteration.n_macroparticles = int(np.sum(n_macroparticles_per_bunch[:indexBunch+1]))
         beamIteration.intensity = np.sum(intensity_per_bunch[:indexBunch+1])
         beamIteration.ratio = beamIteration.intensity/beamIteration.n_macroparticles
-        
+
         if TotalInducedVoltage is not None:
             TotalInducedVoltageIteration.profile.track()
-            TotalInducedVoltageIteration.induced_voltage_sum()        
-            
-            bucket_tolerance = 0.40  
-            
+            TotalInducedVoltageIteration.induced_voltage_sum()
+
+            bucket_tolerance = 0.40
+
             left_edge = (indexBunch+1) * bunch_spacing_buckets * bucket_size_tau - bucket_tolerance * bucket_size_tau
             right_edge = ((indexBunch+1) * bunch_spacing_buckets +1)* bucket_size_tau + bucket_tolerance * bucket_size_tau
-            
+
             tau_induced_voltage_next_bunch = TotalInducedVoltageIteration.profile.bin_centers[(TotalInducedVoltageIteration.profile.bin_centers > left_edge)*(TotalInducedVoltageIteration.profile.bin_centers < right_edge)]
             induced_voltage_next_bunch = TotalInducedVoltageIteration.induced_voltage[(TotalInducedVoltageIteration.profile.bin_centers > left_edge)*(TotalInducedVoltageIteration.profile.bin_centers < right_edge)]
-            
+
             time_induced_voltage_next_bunch = (tau_induced_voltage_next_bunch - (indexBunch+1) * bunch_spacing_buckets * bucket_size_tau)
-            
-            extraVoltageDict = {'time_array':time_induced_voltage_next_bunch, 'voltage_array':induced_voltage_next_bunch}         
-            
-            
+
+            extraVoltageDict = {'time_array':time_induced_voltage_next_bunch, 'voltage_array':induced_voltage_next_bunch}
+
+
     if plot_option:
         plt.figure('Bunch train + induced voltage')
         plt.clf()
         plt.plot(TotalInducedVoltageIteration.profile.bin_centers, TotalInducedVoltageIteration.profile.n_macroparticles / (1.*np.max(TotalInducedVoltageIteration.profile.n_macroparticles))*np.max(TotalInducedVoltageIteration.induced_voltage))
         plt.plot(TotalInducedVoltageIteration.profile.bin_centers, TotalInducedVoltageIteration.induced_voltage)
         plt.show()
                 
-    beam.dt = beamIteration.dt
-    beam.dE = beamIteration.dE
+    beam.dt = beamIteration.dt.astype(dtype=bm.precision.real_t, order='C', copy=False)
+    beam.dE = beamIteration.dE.astype(dtype=bm.precision.real_t, order='C', copy=False)
+    gc.collect()
 
 
 def match_beam_from_distribution(beam, FullRingAndRF, GeneralParameters,
                                   distribution_options, n_bunches,
                                   bunch_spacing_buckets,
                                   main_harmonic_option='lowest_freq',
                                   TotalInducedVoltage=None, n_iterations=1,
                                   n_points_potential=1e4,
                                   dt_margin_percent=0.40, seed=None,):
     '''
-    *This function generates n equaly spaced bunches for a stationary 
+    *This function generates n equaly spaced bunches for a stationary
     distribution and try to match them with intensity effects.*
-    
+
     *The corresponding distributions are specified by their exponent:*
-    
+
     .. math::
         g_0(J) \\sim (1-J/J_0)^{\\text{exponent}}}
-        
+
     *Knowing the distribution, to generate the phase space:
     - Compute the potential U
     - The value of H can be computed thanks to U
     - The action J can be integrated over the whole phase space
     - 2piJ = emittance, this restrict the value of J0 (or H0)
     - with g0(H) we can randomize the macroparticles*
-    '''           
+    '''
 #------------------------------------------------------------------------
 # USEFUL VARIABLES
 #------------------------------------------------------------------------
     # Slicing necessary only with intensity effects
     if TotalInducedVoltage is not None:
         profile = TotalInducedVoltage.profile
 
@@ -412,144 +415,182 @@
     # Minimum omega_rf is used to compute the size of the bucket
     omega_rf = []
     for i in range(n_rf):
         omega_rf += [rf_params.omega_rf[i][0]]
     omega_rf = np.array(omega_rf)
 
     eta_0 = rf_params.eta_0[0]
-    
+
     # Coefficient of Kin and Pot part of the hamiltonian
     normalization_DeltaE = np.abs(eta_0) / (2.*beta**2*E)
     normalization_potential = np.sign(eta_0)*charge/t_rev
-    
+
     intensity_per_bunch = beam.intensity/n_bunches
     n_macro_per_bunch = int(beam.n_macroparticles/n_bunches)
     bucket_size_tau = 2*np.pi/(np.min(omega_rf))
 
 #------------------------------------------------------------------------
 # GENERATES N BUNCHES WITHOUT INTENSITY EFFECTS
 #------------------------------------------------------------------------
 
-    FullRingAndRF.potential_well_generation(n_points=n_points_potential, 
-                                    dt_margin_percent=dt_margin_percent, 
+    FullRingAndRF.potential_well_generation(n_points=n_points_potential,
+                                    dt_margin_percent=dt_margin_percent,
                                     main_harmonic_option=main_harmonic_option)
 
     # Restrict the potential well inside the separatrix and put min on 0
     potential_well_coordinates, potential_well = potential_well_cut(\
         FullRingAndRF.potential_well_coordinates,\
         FullRingAndRF.potential_well)
     potential_well = potential_well - np.min(potential_well)
-    
+
     # Temporary beam, everything is done in the first bucket and then
     # shifted to plug into the real beam.
     temporary_beam = Beam(GeneralParameters, n_macro_per_bunch, intensity_per_bunch)
 
     # Bunches placed in all the buckets without intensity effects
     # Loop the match function to have "different" bunches in each bucket
+    matched_bunch_list = []
     for indexBunch in range(n_bunches):
-        match_a_bunch(normalization_DeltaE, temporary_beam,
-                      potential_well_coordinates,
-                      potential_well, seed, distribution_options,
-                      full_ring_and_RF=FullRingAndRF)
-        if indexBunch==0:
-            beam.dt = temporary_beam.dt
-            beam.dE = temporary_beam.dE
-        else:
-            beam.dt = np.append(beam.dt, temporary_beam.dt +(indexBunch *bunch_spacing_buckets *bucket_size_tau))
-            beam.dE = np.append(beam.dE, temporary_beam.dE)
-    
+        (time_grid, deltaE_grid, distribution, time_resolution,
+            energy_resolution, single_profile) = match_a_bunch(
+                normalization_DeltaE, temporary_beam,
+                potential_well_coordinates,
+                potential_well, seed, distribution_options,
+                full_ring_and_RF=FullRingAndRF)
+        matched_bunch_list.append(
+            (time_grid, deltaE_grid, distribution, time_resolution,
+             energy_resolution, single_profile))
+
     print(str(n_bunches)+' stationary bunches without intensity generated')
 #------------------------------------------------------------------------
 # REMATCH THE BUNCHES WITH INTENSITY EFFECTS
 #------------------------------------------------------------------------
     if TotalInducedVoltage is not None:
         print('Applying intensity effects ...')
+        previous_well = potential_well
         for it in range(n_iterations):
             conv = 0.
             # Compute the induced voltage/potential for all the beam
-            profile.track()
+            profile.n_macroparticles[:] = 0
+            for indexBunch in range(n_bunches):
+                profile.n_macroparticles += np.interp(
+                    profile.bin_centers,
+                    potential_well_coordinates +
+                    indexBunch*bunch_spacing_buckets*bucket_size_tau,
+                    matched_bunch_list[indexBunch][5],
+                    left=0, right=0)
+            profile.n_macroparticles[:] *= 1/(np.sum(profile.n_macroparticles)) * beam.n_macroparticles
+
             TotalInducedVoltage.induced_voltage_sum()
-            
+
             induced_voltage_coordinates = TotalInducedVoltage.time_array
             induced_voltage = TotalInducedVoltage.induced_voltage
-            induced_potential = - normalization_potential * cumtrapz(induced_voltage, dx=induced_voltage_coordinates[1] - induced_voltage_coordinates[0], initial=0)
+            induced_potential = - normalization_potential * cumtrapz(
+                induced_voltage,
+                dx=induced_voltage_coordinates[1] -
+                induced_voltage_coordinates[0],
+                initial=0)
 
             for indexBunch in range(n_bunches):
                 # Extract the induced potential for the specific bucket
                 induced_potential_bunch = np.interp(potential_well_coordinates\
                 + indexBunch*bunch_spacing_buckets*bucket_size_tau,\
                 induced_voltage_coordinates, induced_potential)
 
+                distorted_pot_well = potential_well+induced_potential_bunch
+                distorted_pot_well -= np.min(distorted_pot_well)
+
                 # Recompute the phase space distribution for the new
                 # perturbed potential (containing induced_potential_bunch)
-                match_a_bunch(normalization_DeltaE, temporary_beam,
-                              potential_well_coordinates,
-                              potential_well+induced_potential_bunch, seed,
-                              distribution_options,
-                              full_ring_and_RF=FullRingAndRF)
+                matched_bunch_list[indexBunch] = match_a_bunch(
+                    normalization_DeltaE, temporary_beam,
+                    potential_well_coordinates,
+                    distorted_pot_well, seed,
+                    distribution_options,
+                    full_ring_and_RF=FullRingAndRF)
 
-                dt = temporary_beam.dt
-                dE = temporary_beam.dE
-                
-                # Compute RMS emittance to observe convergence
-                conv += np.pi*np.std(dt)*np.std(dE)
-                
-                length_dt = len(dt)
-                length_dE = len(dE)
-                beam.dt[indexBunch*length_dt:(indexBunch+1)*length_dt] = dt+(indexBunch *bunch_spacing_buckets *bucket_size_tau)
-                beam.dE[indexBunch*length_dE:(indexBunch+1)*length_dE] = dE
+            conv = np.sqrt(np.sum((previous_well-distorted_pot_well)**2.)) / len(distorted_pot_well)
+            previous_well = distorted_pot_well
+
+            print('iteration ' + str(it+1) + ', convergence parameter = ' + str(conv))
+
+            profile.n_macroparticles[:] = 0
+            for indexBunch in range(n_bunches):
+                profile.n_macroparticles += np.interp(
+                    profile.bin_centers,
+                    potential_well_coordinates +
+                    indexBunch*bunch_spacing_buckets*bucket_size_tau,
+                    matched_bunch_list[indexBunch][5],
+                    left=0, right=0)
+            profile.n_macroparticles[:] *= 1/(np.sum(profile.n_macroparticles)) * beam.n_macroparticles
 
- 
-            print('iteration ' + str(it) + ', average RMS emittance (4sigma) = ' + str(4*conv/n_bunches))
-            profile.track()
             TotalInducedVoltage.induced_voltage_sum()
 
+    for indexBunch in range(n_bunches):
+
+        (time_grid, deltaE_grid, distribution, time_resolution,
+         energy_resolution, single_profile) = matched_bunch_list[indexBunch]
+        populate_bunch(temporary_beam, time_grid, deltaE_grid, distribution,
+                       time_resolution, energy_resolution, seed)
+                
+        length_dt = len(temporary_beam.dt)
+        length_dE = len(temporary_beam.dE)
+        
+        beam.dt[indexBunch*length_dt:(indexBunch+1)*length_dt] = np.array(
+            temporary_beam.dt)+(indexBunch *bunch_spacing_buckets *bucket_size_tau)
+        beam.dE[indexBunch*length_dE:(indexBunch+1)*length_dE] = np.array(
+            temporary_beam.dE)
+    
+    beam.dt = beam.dt.astype(dtype=bm.precision.real_t, order='C', copy=False)
+    beam.dE = beam.dE.astype(dtype=bm.precision.real_t, order='C', copy=False)
+    gc.collect()
+
 
 def match_beam_from_distribution_multibatch(beam, FullRingAndRF, GeneralParameters,
                                   distribution_options, n_bunches,
                                   bunch_spacing_buckets, n_batch,
                                   batch_spacing_buckets,
                                   main_harmonic_option='lowest_freq',
                                   TotalInducedVoltage=None, n_iterations=1,
                                   n_points_potential=1e4,
                                   dt_margin_percent=0.40, seed=None):
     '''
-    *This function generates n equaly spaced bunches for a stationary 
+    *This function generates n equaly spaced bunches for a stationary
     distribution and try to match them with intensity effects.*
-    
+
     *Then it copies the batch n_batch times with spacing batch_spacing_buckets*
-    
+
     *The corresponding distributions are specified by their exponent:*
-    
+
     .. math::
         g_0(J) \\sim (1-J/J_0)^{\\text{exponent}}}
-        
+
     *Knowing the distribution, to generate the phase space:
     - Compute the potential U
     - The value of H can be computed thanks to U
     - The action J can be integrated over the whole phase space
     - 2piJ = emittance, this restrict the value of J0 (or H0)
     - with g0(H) we can randomize the macroparticles*
-    '''           
+    '''
 #------------------------------------------------------------------------
 # USEFUL VARIABLES
 #------------------------------------------------------------------------
     # Ring informations, Trev, energy, RF parameters ...
     rf_params = FullRingAndRF.RingAndRFSection_list[0].rf_params
     n_rf = rf_params.n_rf
     # Slicing necessary only with intensity effects
     if TotalInducedVoltage is not None:
         profile = TotalInducedVoltage.profile
-        
+
         t_rev = rf_params.t_rev[0]
         beta = rf_params.beta[0]
         E = rf_params.energy[0]
         charge = rf_params.charge
         eta_0 = rf_params.eta_0[0]
-        
+
         normalization_DeltaE = np.abs(eta_0) / (2.*beta**2*E)
         normalization_potential = np.sign(eta_0)*charge/t_rev
 
     # Ring informations, Trev, energy, RF parameters ...
 #    beta = rf_params.beta[0]
 #    E = rf_params.energy[0]
 #    charge = rf_params.charge
@@ -558,31 +599,31 @@
     # Minimum omega_rf is used to compute the size of the bucket
     omega_rf = []
     for i in range(n_rf):
         omega_rf += [rf_params.omega_rf[i][0]]
     omega_rf = np.array(omega_rf)
 
 #    eta_0 = rf_params.eta_0[0]
-    
+
 #    # Coefficient of Kin and Pot part of the hamiltonian
 #    normalization_DeltaE = np.abs(eta_0) / (2.*beta**2*E)
 #    normalization_potential = np.sign(eta_0)*charge/t_rev
-    
+
     intensity_per_bunch = beam.intensity/n_bunches/n_batch
     n_macro_per_bunch = int(beam.n_macroparticles/n_bunches/n_batch)
     bucket_size_tau = 2*np.pi/(np.min(omega_rf))
 
     temporary_batch = Beam(GeneralParameters, int(n_macro_per_bunch*n_bunches), (intensity_per_bunch*n_bunches))
-    
+
 #    print(temporary_batch.dt)
     match_beam_from_distribution(temporary_batch, FullRingAndRF, GeneralParameters,
                                   distribution_options, n_bunches,bunch_spacing_buckets,
                                   TotalInducedVoltage=None, n_iterations=n_iterations,
                                   n_points_potential=n_points_potential)
-                                  
+
 #    matched_from_distribution_density_multibunch(temporary_batch, GeneralParameters, FullRingAndRF, distribution_options,
 #                                          n_bunches, bunch_spacing_buckets,
 #                                          TotalInducedVoltage = TotalInducedVoltage,
 #                                          n_iterations_input = n_iterations)
     length_dt = len(temporary_batch.dt)
     print(length_dt)
     for index_batch in range(n_batch):
@@ -593,115 +634,115 @@
     plt.plot(beam.dt[::100],beam.dE[::100],'b.')
     plt.figure('temporarybatch')
     plt.plot(temporary_batch.dt[::100],temporary_batch.dE[::100],'b.')
     plt.figure('profile before induced voltage')
     profile.track()
     plt.plot(profile.bin_centers,profile.n_macroparticles)
     plt.figure('beamInSlice')
-    plt.plot(profile.Beam.dt[::100],profile.Beam.dE[::100],'b.')   
+    plt.plot(profile.Beam.dt[::100],profile.Beam.dE[::100],'b.')
 #------------------------------------------------------------------------
 # REMATCH THE BUNCHES WITH INTENSITY EFFECTS
 #------------------------------------------------------------------------
     if TotalInducedVoltage is not None:
 #        TotalInducedVoltage.profile.Beam.dt[:len(beam.dt)] = beam.dt
 #        TotalInducedVoltage.profile.Beam.dE[:len(beam.dE)] = beam.dE
         print('Applying intensity effects ...')
         for it in range(n_iterations):
             conv = 0.
             # Compute the induced voltage/potential for all the beam
             profile.track()
             TotalInducedVoltage.induced_voltage_sum()
-            
+
             plt.figure('profile before induced voltage')
             profile.track()
             plt.plot(profile.bin_centers,profile.n_macroparticles)
-#            
+#
 #            plt.figure('inducedvoltage before induced voltage')
 #            profile.track()
 #            plt.plot(TotalInducedVoltage.time_array,TotalInducedVoltage.induced_voltage)
-#            
+#
             induced_voltage_coordinates = TotalInducedVoltage.time_array
             induced_voltage = TotalInducedVoltage.induced_voltage
             induced_potential = - normalization_potential * cumtrapz(induced_voltage, dx=induced_voltage_coordinates[1] - induced_voltage_coordinates[0], initial=0)
-            
+
             plt.figure('testInducedVolt')
             plt.plot(induced_voltage_coordinates,induced_voltage)
             plt.figure('testInducedPot')
             plt.plot(induced_voltage_coordinates,induced_potential)
 
-            FullRingAndRF.potential_well_generation(n_points=n_points_potential, 
-                                            dt_margin_percent=dt_margin_percent, 
+            FullRingAndRF.potential_well_generation(n_points=n_points_potential,
+                                            dt_margin_percent=dt_margin_percent,
                                             main_harmonic_option=main_harmonic_option)
-        
+
             # Restrict the potential well inside the separatrix and put min on 0
             potential_well_coordinates, potential_well = potential_well_cut(\
                 FullRingAndRF.potential_well_coordinates,\
                 FullRingAndRF.potential_well)
-            potential_well = potential_well - np.min(potential_well)   
-            
+            potential_well = potential_well - np.min(potential_well)
+
             temporary_beam = Beam(GeneralParameters, n_macro_per_bunch, intensity_per_bunch)
             for indexBatch in range(n_batch):
                 for indexBunch in range(n_bunches):
                     # Extract the induced potential for the specific bucket
                     induced_potential_bunch = np.interp(potential_well_coordinates\
                     + indexBunch*bunch_spacing_buckets*bucket_size_tau\
                     + indexBatch*(batch_spacing_buckets + (n_bunches-1)*bunch_spacing_buckets)*bucket_size_tau,\
                     induced_voltage_coordinates, induced_potential)
-    
+
                     # Recompute the phase space distribution for the new
                     # perturbed potential (containing induced_potential_bunch)
                     match_a_bunch(normalization_DeltaE, temporary_beam,
                                   potential_well_coordinates,
                                   potential_well+induced_potential_bunch, seed,
                                   distribution_options,
                                   full_ring_and_RF=FullRingAndRF)
-    
+
                     dt = temporary_beam.dt
                     dE = temporary_beam.dE
-                    
+
                     # Compute RMS emittance to observe convergence
                     conv += np.pi*np.std(dt)*np.std(dE)
-                    
+
                     length_dt = len(dt)
                     length_dE = len(dE)
                     beam.dt[(indexBunch+n_bunches*indexBatch)*length_dt:(indexBunch+n_bunches*indexBatch+1)*length_dt] = dt+(indexBunch *bunch_spacing_buckets *bucket_size_tau) + indexBatch*(batch_spacing_buckets + (n_bunches-1)*bunch_spacing_buckets)*bucket_size_tau
                     beam.dE[(indexBunch+n_bunches*indexBatch)*length_dE:(indexBunch+n_bunches*indexBatch+1)*length_dE] = dE
 
- 
+
             print('iteration ' + str(it) + ', average RMS emittance (4sigma) = ' + str(4*conv/n_bunches))
             profile.track()
             TotalInducedVoltage.induced_voltage_sum()
 
 
 def compute_X_grid(normalization_DeltaE, time_array, potential_well,
                    distribution_variable):
-    
+
     # Delta Energy array
     max_DeltaE = np.sqrt(np.max(potential_well)/normalization_DeltaE)
     coord_array_DeltaE = np.linspace(-float(max_DeltaE),float(max_DeltaE), len(time_array))
-    
+
     # Resolution in time and energy
     time_resolution = time_array[1]-time_array[0]
     energy_resolution = coord_array_DeltaE[1]-coord_array_DeltaE[0]
-    
+
     # Grid
     time_grid, deltaE_grid = np.meshgrid(time_array, coord_array_DeltaE)
     potential_well_grid = np.meshgrid(potential_well, potential_well)[0]
     H_grid = normalization_DeltaE * deltaE_grid**2 + potential_well_grid
-    
+
     # Compute the action J
     J_array = np.zeros(shape=potential_well.shape, dtype=float)
     for i in range(len(J_array)):
         DELTA = np.sqrt((potential_well[i]-potential_well)[potential_well <= potential_well[i]]/normalization_DeltaE)
         J_array[i] = 1./np.pi*np.trapz(DELTA, dx=time_array[1]-time_array[0])
-    
+
     # Compute J grid
     sorted_H = potential_well[potential_well.argsort()]
     sorted_J = J_array[potential_well.argsort()]
-    
+
     if distribution_variable == 'Action':
         J_grid = np.interp(H_grid, sorted_H, sorted_J,\
                            left=0, right=np.inf)
         return sorted_H, sorted_J, J_grid, time_grid, deltaE_grid,\
                time_resolution, energy_resolution
     else:
         return sorted_H, sorted_J, H_grid, time_grid, deltaE_grid,\
@@ -710,70 +751,71 @@
 def compute_H0(emittance, H, J):
     #  Estimation of H corresponding to the emittance
     return np.interp(emittance / (2.*np.pi), J, H)
 
 def match_a_bunch(normalization_DeltaE, beam, potential_well_coordinates,\
                   potential_well, seed, distribution_options,\
                   full_ring_and_RF=None):
-    
+
     if 'type' in distribution_options:
         distribution_type = distribution_options['type']
     else:
         distribution_type = None
-#    
+
     if 'exponent' in distribution_options:
         distribution_exponent = distribution_options['exponent']
     else:
         distribution_exponent = None
-#    
+
     if 'emittance' in distribution_options:
         emittance = distribution_options['emittance']
     else:
         emittance = None
-    
+
     if 'bunch_length' in distribution_options:
         bunch_length = distribution_options['bunch_length']
     else:
         bunch_length = None
-    
+
     if 'bunch_length_fit' in distribution_options:
         bunch_length_fit = distribution_options['bunch_length_fit']
     else:
         bunch_length_fit = None
-    
+
     if 'density_variable' in distribution_options:
         distribution_variable = distribution_options['density_variable']
     else:
         distribution_variable = 'Hamiltonian'
 
     H, J, X_grid, time_grid, deltaE_grid, time_resolution, energy_resolution =\
     compute_X_grid(normalization_DeltaE, potential_well_coordinates,
                    potential_well,distribution_variable)
-    
+
     # Choice of either H or J as the variable used
-    if distribution_variable is 'Action':
+    if distribution_variable == 'Action':
         sorted_X = J
-    elif distribution_variable is 'Hamiltonian':
+    elif distribution_variable == 'Hamiltonian':
         sorted_X = H
     else:
         #DistributionError
         raise SystemError('distribution_variable should be Action or Hamiltonian')
 
     if bunch_length is not None:
         n_points_grid = X_grid.shape[0]
         X0 = X0_from_bunch_length(bunch_length, bunch_length_fit, X_grid, sorted_X,
                          n_points_grid, potential_well_coordinates,
-                         distribution_function, distribution_type, 
+                         distribution_function, distribution_type,
                          distribution_exponent, beam, full_ring_and_RF)
     elif emittance is not None:
         X0 = compute_H0(emittance, H, J)
     else:
         #DistributionError
         raise SystemError('You should specify either bunch_length or emittance')
 
     distribution = distribution_function(X_grid, distribution_type, X0, exponent=distribution_exponent)
     distribution[X_grid>np.max(H)] = 0
     distribution = distribution / np.sum(distribution)
 
-    populate_bunch(beam, time_grid, deltaE_grid, distribution, time_resolution,
-                   energy_resolution, seed)
-
+    profile = np.sum(distribution, axis=0)
+    
+    return (time_grid, deltaE_grid, distribution, time_resolution,
+            energy_resolution, profile)
```

### Comparing `blond-2.0.11/blond/beam/profile.py` & `blond-2.0.12/blond/beam/profile.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 '''
 
 from __future__ import division, print_function
 from builtins import object
 import numpy as np
 # from numpy.fft import rfft, rfftfreq
 from scipy import ndimage
-import ctypes
 from ..toolbox import filters_and_fitting as ffroutines
 from ..utils import bmath as bm
 
+
 class CutOptions(object):
     r"""
     This class groups all the parameters necessary to slice the phase space
     distribution according to the time axis, apart from the array collecting
     the profile which is defined in the constructor of the class Profile below.
 
     Parameters
@@ -102,26 +102,26 @@
             self.n_sigma = n_sigma
 
         self.cuts_unit = str(cuts_unit)
 
         self.RFParams = RFSectionParameters
 
         if self.cuts_unit == 'rad' and self.RFParams is None:
-            #CutError
+            # CutError
             raise RuntimeError('You should pass an RFParams object to ' +
                                'convert from radians to seconds')
         if self.cuts_unit != 'rad' and self.cuts_unit != 's':
-            #CutError
+            # CutError
             raise RuntimeError('cuts_unit should be "s" or "rad"')
 
-        self.edges = np.zeros(n_slices + 1, dtype=float)
-        self.bin_centers = np.zeros(n_slices, dtype=float)
+        self.edges = np.zeros(n_slices + 1, dtype=bm.precision.real_t, order='C')
+        self.bin_centers = np.zeros(n_slices, dtype=bm.precision.real_t, order='C')
 
     def set_cuts(self, Beam=None):
-        """
+        r"""
         Method to set self.cut_left, self.cut_right, self.edges and
         self.bin_centers attributes.
         The frame is defined by :math:`n\sigma_{RMS}` or manually by the user.
         If not, a default frame consisting of taking the whole bunch +5% of the
         maximum distance between two particles in the bunch will be taken
         in each side of the frame.
         """
@@ -138,20 +138,20 @@
                 sigma_coords = np.std(Beam.dt)
                 self.cut_left = mean_coords - self.n_sigma*sigma_coords/2
                 self.cut_right = mean_coords + self.n_sigma*sigma_coords/2
 
         else:
 
             self.cut_left = float(self.convert_coordinates(self.cut_left,
-                                                     self.cuts_unit))
+                                                           self.cuts_unit))
             self.cut_right = float(self.convert_coordinates(self.cut_right,
-                                                      self.cuts_unit))
+                                                            self.cuts_unit))
 
         self.edges = np.linspace(self.cut_left, self.cut_right,
-                                 self.n_slices + 1)
+                                 self.n_slices + 1).astype(dtype=bm.precision.real_t, order='C', copy=False)
         self.bin_centers = (self.edges[:-1] + self.edges[1:])/2
         self.bin_size = (self.cut_right - self.cut_left) / self.n_slices
 
     def track_cuts(self, Beam):
         """
         Track the slice frame (limits and slice position) as the mean of the
         bunch moves.
@@ -167,28 +167,73 @@
         self.bin_centers += delta
 
     def convert_coordinates(self, value, input_unit_type):
         """
         Method to convert a value from 'rad' to 's'.
         """
 
-        if input_unit_type is 's':
+        if input_unit_type == 's':
             return value
 
-        elif input_unit_type is 'rad':
+        elif input_unit_type == 'rad':
             return value /\
                 self.RFParams.omega_rf[0, self.RFParams.counter[0]]
 
     def get_slices_parameters(self):
         """
         Reuturn all the computed parameters.
         """
         return self.n_slices, self.cut_left, self.cut_right, self.n_sigma, \
             self.edges, self.bin_centers, self.bin_size
 
+    def to_gpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays to the GPU
+        '''
+        # Check if to_gpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'GPU':
+            return
+
+        # transfer recursively objects
+        if recursive and self.RFParams:
+            self.RFParams.to_gpu()
+
+        assert bm.device == 'GPU'
+        import cupy as cp
+
+        self.edges = cp.array(self.edges)
+        self.bin_centers = cp.array(self.bin_centers)
+
+        # to make sure it will not be called again
+        self._device = 'GPU'
+        
+    def to_cpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays back to the CPU
+        '''
+        # Check if to_cpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'CPU':
+            return
+
+        # transfer recursively objects
+        if recursive and self.RFParams:
+            self.RFParams.to_cpu()
+
+        assert bm.device == 'CPU'
+        import cupy as cp
+
+        self.edges = cp.asnumpy(self.edges)
+        self.bin_centers = cp.asnumpy(self.bin_centers)
+
+        if hasattr(self, 'rf_voltage'):
+            self.rf_voltage = cp.asnumpy(self.rf_voltage)
+
+        # to make sure it will not be called again
+        self._device = 'CPU'
+
 
 class FitOptions(object):
     """
     This class defines the method to be used turn after turn to obtain the
     position and length of the bunch profile.
 
     Parameters
@@ -205,15 +250,14 @@
     ----------
 
     fit_method : string
     fitExtraOptions : unknown
     """
 
     def __init__(self, fit_option=None, fitExtraOptions=None):
-
         """
         Constructor
         """
 
         self.fit_option = str(fit_option)
         self.fitExtraOptions = fitExtraOptions
 
@@ -239,15 +283,14 @@
 
     filterMethod : string
     filterExtraOptions : dictionary
 
     """
 
     def __init__(self, filterMethod=None, filterExtraOptions=None):
-
         """
         Constructor
         """
 
         self.filterMethod = str(filterMethod)
         self.filterExtraOptions = filterExtraOptions
 
@@ -277,15 +320,14 @@
 
     smooth : boolean
     direct_slicing : boolean
 
     """
 
     def __init__(self, smooth=False, direct_slicing=False):
-
         """
         Constructor
         """
 
         self.smooth = smooth
         self.direct_slicing = direct_slicing
 
@@ -385,19 +427,19 @@
         # Import (reference) Beam
         self.Beam = Beam
 
         # Get all computed parameters from CutOptions
         self.set_slices_parameters()
 
         # Initialize profile array as zero array
-        self.n_macroparticles = np.zeros(self.n_slices, dtype=float)
+        self.n_macroparticles = np.zeros(self.n_slices, dtype=bm.precision.real_t, order='C')
 
         # Initialize beam_spectrum and beam_spectrum_freq as empty arrays
-        self.beam_spectrum = np.array([], dtype=float)
-        self.beam_spectrum_freq = np.array([], dtype=float)
+        self.beam_spectrum = np.array([], dtype=bm.precision.real_t, order='C')
+        self.beam_spectrum_freq = np.array([], dtype=bm.precision.real_t, order='C')
 
         if OtherSlicesOptions.smooth:
             self.operations = [self._slice_smooth]
         else:
             self.operations = [self._slice]
 
         if FitOptions.fit_option is not None:
@@ -414,63 +456,106 @@
         if FilterOptions.filterMethod == 'chebishev':
             self.filterExtraOptions = FilterOptions.filterExtraOptions
             self.operations.append(self.apply_filter)
 
         if OtherSlicesOptions.direct_slicing:
             self.track()
 
+
     def set_slices_parameters(self):
         self.n_slices, self.cut_left, self.cut_right, self.n_sigma, \
-                self.edges, self.bin_centers, self.bin_size = \
-                self.cut_options.get_slices_parameters()
+            self.edges, self.bin_centers, self.bin_size = \
+            self.cut_options.get_slices_parameters()
 
     def track(self):
         """
         Track method in order to update the slicing along with the tracker.
+        The kwargs are currently only needed to forward the reduce kw argument
+        needed for the MPI version.
         """
 
         for op in self.operations:
             op()
 
     def _slice(self):
         """
-        Constant space slicing with a constant frame. 
+        Constant space slicing with a constant frame.
         """
-        bm.slice(self)
-        # libblond.histogram(self.Beam.dt.ctypes.data_as(ctypes.c_void_p), 
-        #                  self.n_macroparticles.ctypes.data_as(ctypes.c_void_p), 
-        #                  ctypes.c_double(self.cut_left), 
-        #                  ctypes.c_double(self.cut_right), 
-        #                  ctypes.c_int(self.n_slices), 
-        #                  ctypes.c_int(self.Beam.n_macroparticles))
+        bm.slice(self.Beam.dt, self.n_macroparticles, self.cut_left,
+                 self.cut_right)
 
-    def _slice_smooth(self):
+        if bm.mpiMode():
+            self.reduce_histo()
+
+    def reduce_histo(self, dtype=np.uint32):
+        if not bm.mpiMode():
+            raise RuntimeError(
+                'ERROR: Cannot use this routine unless in MPI Mode')
+
+        from ..utils.mpi_config import worker
+
+        if worker.workers == 1:
+            return
+
+        if self.Beam.is_splitted:
+            
+            if bm.device == 'CPU':
+            # Convert to uint32t for better performance
+                self.n_macroparticles = self.n_macroparticles.astype(
+                    dtype, order='C')
+
+            if bm.device == 'GPU':
+                import cupy as cp
+                # tranfer to cpu
+                self.n_macroparticles = cp.asnumpy(self.n_macroparticles, dtype=dtype)
+
+            worker.allreduce(self.n_macroparticles)
+
+            if bm.device == 'GPU':
+                # transfer back to gpu
+                self.n_macroparticles = cp.array(self.n_macroparticles, dtype=bm.precision.real_t)
+
+            if bm.device == 'CPU':
+            # Convert back to float64
+                self.n_macroparticles = self.n_macroparticles.astype(
+                    dtype=bm.precision.real_t, order='C', copy=False)
+    
+    def scale_histo(self):
+        if not bm.mpiMode():
+            raise RuntimeError(
+                'ERROR: Cannot use this routine unless in MPI Mode')
+
+        from ..utils.mpi_config import worker
+        if self.Beam.is_splitted:
+            self.n_macroparticles *= worker.workers
+            # bm.mul(self.n_macroparticles, worker.workers, self.n_macroparticles)
+
+    def _slice_smooth(self, reduce=True):
         """
         At the moment 4x slower than _slice but smoother (filtered).
         """
-        bm.slice_smooth(self)
-        # libblond.smooth_histogram(self.Beam.dt.ctypes.data_as(ctypes.c_void_p), 
-        #                  self.n_macroparticles.ctypes.data_as(ctypes.c_void_p), 
-        #                  ctypes.c_double(self.cut_left), 
-        #                  ctypes.c_double(self.cut_right), 
-        #                  ctypes.c_uint(self.n_slices), 
-        #                  ctypes.c_uint(self.Beam.n_macroparticles))
+        bm.slice_smooth(self.Beam.dt, self.n_macroparticles, self.cut_left,
+                        self.cut_right)
+
+        if bm.mpiMode():
+            self.reduce_histo(dtype=np.float64)
 
-    
     def apply_fit(self):
         """
         It applies Gaussian fit to the profile.
         """
 
         if self.bunchLength == 0:
-            p0 = [max(self.n_macroparticles), np.mean(self.Beam.dt),
-                  np.std(self.Beam.dt)]
+            p0 = [float(self.n_macroparticles.max()), 
+                  float(self.Beam.dt.mean()),
+                  float(self.Beam.dt.std())]
         else:
-            p0 = [max(self.n_macroparticles), self.bunchPosition,
-                  self.bunchLength/4]
+            p0 = [float(self.n_macroparticles.max()),
+                  float(self.bunchPosition),
+                  float(self.bunchLength/4.)]
 
         self.fitExtraOptions = ffroutines.gaussian_fit(self.n_macroparticles,
                                                        self.bin_centers, p0)
         self.bunchPosition = self.fitExtraOptions[1]
         self.bunchLength = 4*self.fitExtraOptions[2]
 
     def apply_filter(self):
@@ -521,40 +606,98 @@
 
     def beam_spectrum_freq_generation(self, n_sampling_fft):
         """
         Frequency array of the beam spectrum
         """
 
         self.beam_spectrum_freq = bm.rfftfreq(n_sampling_fft, self.bin_size)
-
+    
     def beam_spectrum_generation(self, n_sampling_fft):
         """
         Beam spectrum calculation
         """
-
         self.beam_spectrum = bm.rfft(self.n_macroparticles, n_sampling_fft)
 
     def beam_profile_derivative(self, mode='gradient'):
         """
         The input is one of the three available methods for differentiating
         a function. The two outputs are the bin centres and the discrete
         derivative of the Beam profile respectively.*
         """
 
         x = self.bin_centers
         dist_centers = x[1] - x[0]
 
-        if mode is 'filter1d':
+        if mode == 'filter1d':
+            if bm.device == 'GPU':
+                raise RuntimeError('filter1d mode is not supported in GPU.')
+                
             derivative = ndimage.gaussian_filter1d(
                 self.n_macroparticles, sigma=1, order=1, mode='wrap') / \
                 dist_centers
-        elif mode is 'gradient':
-            derivative = np.gradient(self.n_macroparticles, dist_centers)
-        elif mode is 'diff':
-            derivative = np.diff(self.n_macroparticles) / dist_centers
+        elif mode == 'gradient':
+            derivative = bm.gradient(self.n_macroparticles, dist_centers)
+        elif mode == 'diff':
+            derivative = bm.diff(self.n_macroparticles) / dist_centers
             diffCenters = x[0:-1] + dist_centers/2
-            derivative = np.interp(x, diffCenters, derivative)
+            derivative = bm.interp(x, diffCenters, derivative)
         else:
-            #ProfileDerivativeError
+            # ProfileDerivativeError
             raise RuntimeError('Option for derivative is not recognized.')
 
         return x, derivative
+
+    def to_gpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays to the GPU
+        '''
+        # Check if to_gpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'GPU':
+            return
+
+        # transfer recursively objects to_gpu
+        if recursive and self.Beam:
+            self.Beam.to_gpu()
+
+        if recursive and self.cut_options:
+            self.cut_options.to_gpu()
+
+        assert bm.device == 'GPU'
+        import cupy as cp
+
+        self.bin_centers = self.cut_options.bin_centers
+        self.edges = self.cut_options.edges
+
+        self.n_macroparticles = cp.array(self.n_macroparticles)
+        self.beam_spectrum = cp.array(self.beam_spectrum)
+        self.beam_spectrum_freq = cp.array(self.beam_spectrum_freq)
+
+        # to make sure it will not be called again
+        self._device = 'GPU'
+
+    def to_cpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays back to the CPU
+        '''
+        # Check if to_cpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'CPU':
+            return
+
+        # transfer recursively objects
+        if recursive and self.Beam:
+            self.Beam.to_cpu()
+
+        if recursive and self.cut_options:
+            self.cut_options.to_cpu()
+
+        assert bm.device == 'CPU'
+        import cupy as cp
+
+        self.bin_centers = self.cut_options.bin_centers
+        self.edges = self.cut_options.edges
+
+        self.n_macroparticles = cp.asnumpy(self.n_macroparticles)
+        self.beam_spectrum = cp.asnumpy(self.beam_spectrum)
+        self.beam_spectrum_freq = cp.asnumpy(self.beam_spectrum_freq)
+
+        # to make sure it will not be called again
+        self._device = 'CPU'
```

### Comparing `blond-2.0.11/blond/beam/sparse_histogram.cpp` & `blond-2.0.12/blond/toolbox/tomoscope.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,82 @@
 /*
 Copyright 2016 CERN. This software is distributed under the
-terms of the GNU General Public Licence version 3 (GPL Version 3), 
+terms of the GNU General Public Licence version 3 (GPL Version 3),
 copied verbatim in the file LICENCE.md.
-In applying this licence, CERN does not waive the privileges and immunities 
-granted to it by virtue of its status as an Intergovernmental Organization or 
+In applying this licence, CERN does not waive the privileges and immunities
+granted to it by virtue of its status as an Intergovernmental Organization or
 submit itself to any jurisdiction.
 Project website: http://blond.web.cern.ch/
 */
 
-// Optimised C++ routine that calculates the histogram for a sparse beam
-// Author: Juan F. Esteban Mueller, Danilo Quartullo, Alexandre Lasheen
+// Generation of particle distribution from probability density
+// Author: Helga Timko
 
-#include <stdio.h>
+#include <stdlib.h>
+using uint = unsigned int;
 
-extern "C" void sparse_histogram(const double * __restrict__ input,
-		    double * __restrict__ output,
-               const double * __restrict__ cut_left_array,
-               const double * __restrict__ cut_right_array,
-               const double * __restrict__ bunch_indexes,
-               const int n_slices,
-               const int n_filled_buckets,
-               const int n_macroparticles){
-	
-    int i;
-    int j;
-    int i_bucket;
-    double a;
-    double fbin;
-    double fbunch;
-    int ffbin;
-    int ffbunch;
-    
-    // Only valid for cut_edges = edges
-    const double inv_bucket_length = 1.0 / (cut_right_array[0] - cut_left_array[0]);
-    const double inv_bin_width = inv_bucket_length * (double) n_slices;
-    
-    // Initialises all slicing arrays to zero
-    for (i = 0; i < n_filled_buckets*n_slices; i++){
-        output[i] = 0.0;
+double randd() {
+    return (double)rand() / (RAND_MAX + 1.0);
+}
+
+
+extern "C" void generate_distribution(double * __restrict__ dt,
+                                      double * __restrict__ dE, const double * probDistr, const uint seed,
+                                      const uint profLen, const double cutoff, const double x0, const double y0,
+                                      const double dtBin, const double dEBin, const uint nPart) {
+
+
+// Initialise random seed
+    srand(seed);
+
+// Initialise some variables
+    uint i, k, m;
+    double iPos, kPos;
+    double cutoff2 = cutoff * cutoff;
+    double dtMin = -1.*x0 * dtBin;
+    double dEMin = -1.*y0 * dEBin;
+
+
+// Calculate cumulative probability
+    double totProb = 0.;
+    uint profLen2 = uint(profLen * profLen);
+    double cumulDistr [profLen2];
+
+    for (m = 0; m < profLen2; m++) {
+        cumulDistr[m] = probDistr[m] + totProb;
+        totProb += probDistr[m];
     }
-    
-    // Histogram loop
-    for (i = 0; j < n_macroparticles; j++){
-        a = input[j];   // Particle dt
-        if ((a < cut_left_array[0])||(a > cut_right_array[n_filled_buckets-1]))
-            continue;
-        // Find bucket in which the particle is and its index
-        fbunch = (a - cut_left_array[0]) * inv_bucket_length;
-        ffbunch = (int) fbunch;
-        i_bucket = (int) bunch_indexes[ffbunch];
-        if (i_bucket == -1)
-            continue;
-        // Find the bin inside the corresponding bucket
-        fbin = (a - cut_left_array[i_bucket]) * inv_bin_width;
-        ffbin = i_bucket*n_slices + (int) fbin;
-        output[ffbin] = output[ffbin] + 1.0;
+
+
+// Normalise probability distribution
+    double invTotProb = 1. / totProb;
+
+    for (m = 0; m < profLen2; m++) {
+        cumulDistr[m] *= invTotProb;
     }
+
+
+// Generate particle coordinates
+    uint n = 0;
+    double randProb;
+
+    while ( n < nPart ) {
+        randProb = randd();
+        for (m = 0; m < profLen2; m++) {
+            if (randProb < cumulDistr[m])
+                break;
+        }
+        i = int(m / profLen);
+        k = m % profLen;
+
+        iPos = double(i) + randd() - 0.5;
+        kPos = double(k) + randd() - 0.5;
+
+        // Add particle if inside cutoff
+        if ( double ((iPos - x0) * (iPos - x0) + (kPos - y0) * (kPos - y0)) < cutoff2 ) {
+            dt[n] = dtMin + iPos * dtBin;
+            dE[n] = dEMin + kPos * dEBin;
+            n++;
+        }
+    }
+
 }
```

### Comparing `blond-2.0.11/blond/beam/sparse_slices.py` & `blond-2.0.12/blond/beam/sparse_slices.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,118 +13,111 @@
 
 :Authors: **Juan F. Esteban Mueller**
 '''
 
 from __future__ import division, print_function
 from builtins import range, object
 import numpy as np
-import ctypes
-# from ..setup_cpp import libblond
-from .. import libblond
-
+from ..utils import bmath as bm
 from ..beam.profile import Profile, CutOptions
 
 
-
 class SparseSlices(object):
     '''
-    *This class instantiates a Slice object for each filled bucket according
-    to the provided filling pattern. Each slice object will be of the size of 
+    *This class instantiates a Profile object for each filled bucket according
+    to the provided filling pattern. Each Profile object will be of the size of
     an RF bucket and will have the same number of slices.*
     '''
-    
-    def __init__(self, RFStation, Beam, n_slices, filling_pattern, tracker='C',
+
+    def __init__(self, RFStation, Beam, n_slices_bucket, filling_pattern, tracker='C',
                  direct_slicing=False):
-        
+
         #: *Import (reference) Beam*
         self.Beam = Beam
-        
+
         #: *Import (reference) RFStation*
         self.RFParams = RFStation
-        
+
         #: *Number of slices per bucket*
-        self.n_slices = n_slices
-        
+        self.n_slices_bucket = n_slices_bucket
+
         #: *Filling pattern as a boolean array where True (1) means filled
         # bucket*
         self.filling_pattern = filling_pattern
-        
+
         # Bunch index for each filled bucket (-1 if empty). Only for C++ track
         self.bunch_indexes = np.cumsum(filling_pattern) * filling_pattern - 1
-        
+
         #: *Number of buckets to be sliced*
         self.n_filled_buckets = int(np.sum(filling_pattern))
-        
+
         # Pre-processing the slicing edges
         self.set_cuts()
-        
+
         # Initialize individual slicing objects
-        self.slices_array = []
+        self.profiles_list = []
         # Group n_macroparticles from all objects in a single array
         # (for C++ track).
-        self.n_macroparticles_array = np.zeros((self.n_filled_buckets, 
-                                                n_slices))
+        self.n_macroparticles_array = np.zeros((self.n_filled_buckets,
+                                                n_slices_bucket))
         # Group bin_centers from all objects in a single array (for impedance)
-        self.bin_centers_array = np.zeros((self.n_filled_buckets, n_slices))
+        self.bin_centers_array = np.zeros((self.n_filled_buckets, n_slices_bucket))
+        self.edges_array = np.zeros((self.n_filled_buckets, n_slices_bucket+1))
         for i in range(self.n_filled_buckets):
             # Only valid for cut_edges='edges'
-                
-            self.slices_array.append(Profile(Beam, CutOptions(cut_left= self.cut_left_array[i], 
-                    cut_right=self.cut_right_array[i], n_slices=n_slices))   )
-                 
-            self.slices_array[i].n_macroparticles = \
-                                               self.n_macroparticles_array[i,:]
-            self.bin_centers_array[i,:] = self.slices_array[i].bin_centers
-            self.slices_array[i].bin_centers = self.bin_centers_array[i,:]
-        
+
+            self.profiles_list.append(Profile(Beam, CutOptions(cut_left=self.cut_left_array[i],
+                                                               cut_right=self.cut_right_array[i],
+                                                               n_slices=n_slices_bucket)))
+
+            self.profiles_list[i].n_macroparticles = self.n_macroparticles_array[i,:]
+            self.bin_centers_array[i,:] = self.profiles_list[i].bin_centers
+            self.edges_array[i,:] = self.profiles_list[i].edges
+            self.profiles_list[i].bin_centers = self.bin_centers_array[i,:]
+
         # Select the tracker
-        if tracker is 'C':
+        if tracker == 'C':
             self.track = self._histrogram_C
-        elif tracker is 'onebyone':
+        elif tracker == 'onebyone':
             self.track = self._histrogram_one_by_one
-            
+        else:
+            # WrongCalcError
+            raise RuntimeError(
+                'Tracking method not recognized!')
+
         # Track at initialisation
         if direct_slicing:
             self.track()
 
-
     def set_cuts(self):
         '''
-        *Method to set the self.cut_left_array and self.cut_right_array 
+        *Method to set the self.cut_left_array and self.cut_right_array
         properties, with the limits being an RF period.
         This is done as a pre-processing.*
         '''
         # RF period
-        Trf = 2.0 * np.pi / self.RFParams.omega_rf[0,self.RFParams.counter[0]]
-        
+        T_rf = self.RFParams.t_rf[0,self.RFParams.counter[0]]
+
         self.cut_left_array = np.zeros(self.n_filled_buckets)
         self.cut_right_array = np.zeros(self.n_filled_buckets)
         for i in range(self.n_filled_buckets):
             bucket_index = np.where(self.filling_pattern)[0][i]
-            self.cut_left_array[i] = bucket_index * Trf
-            self.cut_right_array[i] = (bucket_index + 1) * Trf
-
+            self.cut_left_array[i] = bucket_index * T_rf
+            self.cut_right_array[i] = (bucket_index + 1) * T_rf
 
     def _histrogram_C(self):
         '''
-        *Histrogram generated by calling an optimized C++ function that 
+        *Histrogram generated by calling an optimized C++ function that
         calculates all the profile at once.*
         '''
-               
-        libblond.sparse_histogram(self.Beam.dt.ctypes.data_as(ctypes.c_void_p), 
-                 self.n_macroparticles_array.ctypes.data_as(ctypes.c_void_p),
-                 self.cut_left_array.ctypes.data_as(ctypes.c_void_p), 
-                 self.cut_right_array.ctypes.data_as(ctypes.c_void_p),
-                 self.bunch_indexes.ctypes.data_as(ctypes.c_void_p),
-                 ctypes.c_int(self.n_slices), 
-                 ctypes.c_int(self.n_filled_buckets), 
-                 ctypes.c_int(self.Beam.n_macroparticles))
-                 
-                         
+        bm.sparse_histogram(self.Beam.dt, self.n_macroparticles_array,
+                            self.cut_left_array, self.cut_right_array,
+                            self.bunch_indexes, self.n_slices_bucket)
+
     def _histrogram_one_by_one(self):
         '''
-        *Histrogram generated by calling the tack() method of each Profile 
+        *Histrogram generated by calling the tack() method of each Profile
         object*
         '''
-        
+
         for i in range(self.n_filled_buckets):
-            self.slices_array[i].track()
+            self.profiles_list[i].track()
```

### Comparing `blond-2.0.11/blond/cpp_routines/blondmath.cpp` & `blond-2.0.12/blond/cpp_routines/histogram.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -1,316 +1,283 @@
-/**
-Copyright 2016 CERN. This software is distributed under the
-terms of the GNU General Public Licence version 3 (GPL Version 3),
-copied verbatim in the file LICENCE.md.
-In applying this licence, CERN does not waive the privileges and immunities
-granted to it by virtue of its status as an Intergovernmental Organization or
-submit itself to any jurisdiction.
-Project website: http://blond.web.cern.ch/
-
-
-C++ Math library
-@Author: Konstantinos Iliakis
-@Date: 20.10.2017
-*/
-
-
-#include "sin.h"
-#include "exp.h"
-#include "cos.h"
-#include <cmath>
-#include <algorithm>
-#include <functional>
-
-#ifdef PARALLEL
-#include <omp.h>
-#endif
-
-
-extern "C" {
-
-    void convolution(const double * __restrict__ signal,
-                     const int SignalLen,
-                     const double * __restrict__ kernel,
-                     const int KernelLen,
-                     double * __restrict__ res)
-    {
-        const int size = KernelLen + SignalLen - 1;
-
-        #pragma omp parallel for
-        for (int n = 0; n < size; ++n) {
-            res[n] = 0;
-            const int kmin = (n >= KernelLen - 1) ? n - (KernelLen - 1) : 0;
-            const int kmax = (n < SignalLen - 1) ? n : SignalLen - 1;
-            // uint j = n - kmin;
-            for (int k = kmin; k <= kmax; k++) {
-                res[n] += signal[k] * kernel[n - k];
-                //--j;
-            }
-        }
-    }
-
-    void where_more_than(const double *__restrict__ data, const int n,
-                         const double c1,
-                         bool *__restrict__ res)
-    {
-        #pragma omp parallel for
-        for (int i = 0; i < n; i++) {
-            res[i] = data[i] > c1;
-        }
-    }
-
-    void where_less_than(const double *__restrict__ data, const int n,
-                         const double c1,
-                         bool *__restrict__ res)
-    {
-        #pragma omp parallel for
-        for (int i = 0; i < n; i++) {
-            res[i] = data[i] < c1;
-        }
-    }
-
-    void where_more_less_than(const double *__restrict__ data, const int n,
-                         const double c1, const double c2,
-                         bool *__restrict__ res)
-    {
-        #pragma omp parallel for
-        for (int i = 0; i < n; i++) {
-            res[i] = (data[i] > c1) && (data[i] < c2);
-        }
-    }
-
-    double mean(const double * __restrict__ data, const int n)
-    {
-        double m = 0;
-        #pragma omp parallel for reduction(+:m)
-        for (int i = 0; i < n; ++i) {
-            m += data[i];
-        }
-        return m / n;
-    }
-
-    double stdev(const double * __restrict__ data,
-                 const int n)
-    {
-        const double m = mean(data, n);
-        double sum_deviation = 0.0;
-
-        #pragma omp parallel for reduction(+:sum_deviation)
-        for (int i = 0; i < n; ++i)
-            sum_deviation += (data[i] - m) * (data[i] - m);
-        return sqrt(sum_deviation / n);
-    }
-
-
-    double fast_sin(double x) {return vdt::fast_sin(x);}
-
-    double fast_cos(double x) {return vdt::fast_cos(x);}
-
-    double fast_exp(double x) {return vdt::fast_exp(x);}
-
-    // float fast_sinf(float x) {return vdt::fast_sinf(x);}
-    // float fast_cosf(float x) {return vdt::fast_cosf(x);}
-    // float fast_expf(float x) {return vdt::fast_expf(x);}
-
-    void fast_sinv(const double * __restrict__ in,
-                   const int size,
-                   double * __restrict__ out)
-    {
-        #pragma omp parallel for
-        for (int i = 0; i < size; ++i)
-            out[i] = fast_sin(in[i]);
-    }
-
-    void fast_cosv(const double * __restrict__ in,
-                   const int size,
-                   double * __restrict__ out)
-    {
-        #pragma omp parallel for
-        for (int i = 0; i < size; ++i)
-            out[i] = fast_cos(in[i]);
-    }
-
-    void fast_expv(const double * __restrict__ in,
-                   const int size,
-                   double * __restrict__ out)
-    {
-        #pragma omp parallel for
-        for (int i = 0; i < size; ++i)
-            out[i] = fast_exp(in[i]);
-    }
-
-    /**
-    Parameters are like python's np.interp
-
-    @x: x-coordinates of the interpolated values
-    @N: The x array size
-    @xp: The x-coords of the data points, !!must be sorted!!
-    @M: The xp array size
-    @yp: the y-coords of the data points
-    @left: value to return for x < xp[0]
-    @right: value to return for x > xp[last]
-    @y: the interpolated values, same shape as x
-    */
-    void interp(const double * __restrict__ x,
-                const int N,
-                const double * __restrict__ xp,
-                const int M,
-                const double * __restrict__ yp,
-                const double left,
-                const double right,
-                double * __restrict__ y)
-    {
-        #pragma omp parallel for
-        for (int i = 0; i < N; ++i) {
-            int pos = std::lower_bound(xp, xp + M, x[i]) - xp;
-            if (pos == M)
-                y[i] = right;
-            else if (xp[pos] == x[i])
-                y[i] = yp[pos];
-            else if (pos == 0)
-                y[i] = left;
-            else {
-                y[i] = yp[pos - 1] +
-                       (yp[pos] - yp[pos - 1]) * (x[i] - xp[pos - 1]) /
-                       (xp[pos] - xp[pos - 1]);
-            }
-        }
-    }
-
-
-    // Function to implement integration of f(x) over the interval
-    // [a,b] using the trapezoid rule with nsub subdivisions.
-    void cumtrapz_wo_initial(const double * __restrict__ f,
-                             const double deltaX,
-                             const int nsub,
-                             double * __restrict__ psum)
-    {
-        // initialize the partial sum to be f(a)+f(b) and
-        // deltaX to be the step size using nsub subdivisions
-        const double half_dx = deltaX / 2.0;
-        psum[0] = (f[1] + f[0]) * half_dx;
-
-        for (int i = 1; i < nsub - 1; ++i)
-            psum[i] = psum[i - 1] + (f[i + 1] + f[i]) * half_dx;
-    }
-
-    // Function to implement integration of f(x) over the interval
-    // [a,b] using the trapezoid rule with nsub subdivisions.
-    void cumtrapz_w_initial(const double * __restrict__ f,
-                            const double deltaX,
-                            const double initial,
-                            const int nsub,
-                            double * __restrict__ psum)
-    {
-        // initialize the partial sum to be f(a)+f(b) and
-        // deltaX to be the step size using nsub subdivisions
-        const double half_dx = deltaX / 2.0;
-
-        psum[0] = initial;
-        psum[1] = (f[1] + f[0]) * half_dx;
-        // increment the partial sum
-        for (int i = 2; i < nsub; ++i)
-            psum[i] = psum[i - 1] + (f[i] + f[i - 1]) * half_dx;
-    }
-
-
-    double trapz_var_delta(const double * __restrict__ f,
-                           const double * __restrict__ deltaX,
-                           const int nsub)
-    {
-        // initialize the partial sum to be f(a)+f(b) and
-        // deltaX to be the step size using nsub subdivisions
-
-        double psum = 0.0;
-        // increment the partial sum
-        #pragma omp parallel for reduction(+ : psum)
-        for (int i = 1; i < nsub; ++i)
-            psum += (f[i] + f[i - 1]) * (deltaX[i] - deltaX[i - 1]);
-
-        return psum / 2.;
-    }
-
-    double trapz_const_delta(const double * __restrict__ f,
-                             const double deltaX,
-                             const int nsub)
-    {
-        // initialize the partial sum to be f(a)+f(b) and
-        // deltaX to be the step size using nsub subdivisions
-        double psum = (f[0] + f[nsub - 1]) / 2.; // f(a)+f(b);
-
-        // increment the partial sum
-        #pragma omp parallel for reduction(+ : psum)
-        for (int i = 1; i < nsub - 1; ++i)
-            psum += f[i];
-
-        // multiply the sum by the constant deltaX/2.0
-        // return approximation
-        return deltaX * psum;;
-    }
-
-    int min_idx(const double * __restrict__ a, int size)
-    {
-        return (int) (std::min_element(a, a + size) - a);
-    }
-
-    int max_idx(const double * __restrict__ a, int size)
-    {
-        return (int) (std::max_element(a, a + size) - a);
-    }
-
-
-    void linspace(const double start, const double end, const int n,
-                  double *__restrict__ out)
-    {
-        const double step = (end - start) / (n - 1);
-        #pragma omp parallel for
-        for (int i = 0; i < n; ++i) out[i] = start + i * step;
-    }
-
-    void arange_double(const double start, const double stop,
-                       const double step,
-                       double * __restrict__ out)
-    {
-        const int size = (int) std::ceil((stop - start) / step);
-        #pragma omp parallel for
-        for (int i = 0; i < size; ++i) out[i] = start + i * step;
-    }
-
-    void arange_int(const int start, const int stop,
-                    const int step,
-                    int * __restrict__ out)
-    {
-        const int size = (int) std::ceil((stop - start) / step);
-        #pragma omp parallel for
-        for (int i = 0; i < size; ++i) out[i] = start + i * step;
-    }
-
-    double sum(const double * __restrict__ data, const int n)
-    {
-        double m = 0.0;
-        #pragma omp parallel for reduction(+ : m)
-        for (int i = 0; i < n; ++i) m += data[i];
-        return m;
-    }
-
-
-    void sort_double(double * __restrict__ in, const int n, bool reverse)
-    {
-        if (reverse) std::sort(in, in + n, std::greater<double>());
-        else std::sort(in, in + n);
-    }
-
-    void sort_int(int * __restrict__ in, const int n, bool reverse)
-    {
-        if (reverse) std::sort(in, in + n, std::greater<int>());
-        else std::sort(in, in + n);
-    }
-
-
-    void sort_longint(long int * __restrict__ in, const int n, bool reverse)
-    {
-        if (reverse) std::sort(in, in + n, std::greater<long int>());
-        else std::sort(in, in + n);
-    }
-
-}
+/*
+ Copyright 2016 CERN. This software is distributed under the
+ terms of the GNU General Public Licence version 3 (GPL Version 3),
+ copied verbatim in the file LICENCE.md.
+ In applying this licence, CERN does not waive the privileges and immunities
+ granted to it by virtue of its status as an Intergovernmental Organization or
+ submit itself to any jurisdiction.
+ Project website: http://blond.web.cern.ch/
+ */
+
+// Optimised C++ routine that calculates the histogram
+// Author: Danilo Quartullo, Alexandre Lasheen, Konstantinos Iliakis
+
+#include <string.h>     // memset()
+#include <stdlib.h>     // mmalloc()
+#include <math.h>
+#include "openmp.h"
+
+
+extern "C" void histogram(const double *__restrict__ input,
+                          double *__restrict__ output, const double cut_left,
+                          const double cut_right, const int n_slices,
+                          const int n_macroparticles)
+{
+    // Number of Iterations of the inner loop
+    const int STEP = 16;
+    const double inv_bin_width = n_slices / (cut_right - cut_left);
+
+    // allocate memory for the thread_private histogram
+    double **histo = (double **) malloc(omp_get_max_threads() * sizeof(double *));
+    histo[0] = (double *) malloc (omp_get_max_threads() * n_slices * sizeof(double));
+    for (int i = 0; i < omp_get_max_threads(); i++)
+        histo[i] = (*histo + n_slices * i);
+
+    #pragma omp parallel
+    {
+        const int id = omp_get_thread_num();
+        const int threads = omp_get_num_threads();
+        memset(histo[id], 0., n_slices * sizeof(double));
+        float fbin[STEP];
+        #pragma omp for
+        for (int i = 0; i < n_macroparticles; i += STEP) {
+
+            const int loop_count = n_macroparticles - i > STEP ?
+                                   STEP : n_macroparticles - i;
+
+            // First calculate the index to update
+            for (int j = 0; j < loop_count; j++) {
+                fbin[j] = floor((input[i + j] - cut_left) * inv_bin_width);
+            }
+            // Then update the corresponding bins
+            for (int j = 0; j < loop_count; j++) {
+                const int bin  = (int) fbin[j];
+                if (bin < 0 || bin >= n_slices) continue;
+                histo[id][bin] += 1.;
+            }
+        }
+
+        // Reduce to a single histogram
+        #pragma omp for
+        for (int i = 0; i < n_slices; i++) {
+            output[i] = 0.;
+            for (int t = 0; t < threads; t++)
+                output[i] += histo[t][i];
+        }
+    }
+
+    // free memory
+    free(histo[0]);
+    free(histo);
+}
+
+extern "C" void smooth_histogram(const double *__restrict__ input,
+                                 double *__restrict__ output, const double cut_left,
+                                 const double cut_right, const int n_slices,
+                                 const int n_macroparticles)
+{
+    // Constants init
+    const double inv_bin_width = n_slices / (cut_right - cut_left);
+    const double bin_width = (cut_right - cut_left) / n_slices;
+    const double const1 = (cut_left + bin_width * 0.5);
+    const double const2 = (cut_right - bin_width * 0.5);
+
+    // memory alloc for per thread histo
+    double **histo = (double **) malloc(omp_get_max_threads() * sizeof(double *));
+    histo[0] = (double *) malloc (omp_get_max_threads() * n_slices * sizeof(double));
+    for (int i = 0; i < omp_get_max_threads(); i++)
+        histo[i] = (*histo + n_slices * i);
+
+
+    #pragma omp parallel
+    {
+        const int id = omp_get_thread_num();
+        const int threads = omp_get_num_threads();
+        memset(histo[id], 0., n_slices * sizeof(double));
+
+        // main caclulation
+        #pragma omp for
+        for (int i = 0; i < n_macroparticles; i++) {
+            int fffbin = 0;
+            double a = input[i];
+            if ((a < const1) || (a > const2))
+                continue;
+            double fbin = (a - cut_left) * inv_bin_width;
+            int ffbin = (int)(fbin);
+            double distToCenter = fbin - (double)(ffbin);
+            if (distToCenter > 0.5)
+                fffbin = (int)(fbin + 1.0);
+            else
+                fffbin = (int)(fbin - 1.0);
+
+            histo[id][ffbin] = histo[id][ffbin] + 0.5 - distToCenter;
+            histo[id][fffbin] = histo[id][fffbin] + 0.5 + distToCenter;
+        }
+
+        // Reduce to a single histogram
+        #pragma omp for
+        for (int i = 0; i < n_slices; i++) {
+            output[i] = 0.;
+            for (int t = 0; t < threads; t++)
+                output[i] += histo[t][i];
+        }
+
+
+    }
+    // free memory
+    free(histo[0]);
+    free(histo);
+
+}
+
+
+extern "C" void histogramf(const float *__restrict__ input,
+                           float *__restrict__ output, const float cut_left,
+                           const float cut_right, const int n_slices,
+                           const int n_macroparticles)
+{
+    // Number of Iterations of the inner loop
+    const int STEP = 16;
+    const float inv_bin_width = n_slices / (cut_right - cut_left);
+
+    // allocate memory for the thread_private histogram
+    static float **histo = nullptr;
+
+    if (!histo) {
+        histo = (float **) malloc(omp_get_max_threads() * sizeof(float *));
+        histo[0] = (float *) malloc (omp_get_max_threads() * n_slices * sizeof(float));
+        for (int i = 0; i < omp_get_max_threads(); i++)
+            histo[i] = (*histo + n_slices * i);
+    }
+
+    #pragma omp parallel
+    {
+        const int id = omp_get_thread_num();
+        const int threads = omp_get_num_threads();
+        memset(histo[id], 0., n_slices * sizeof(float));
+        float fbin[STEP];
+        #pragma omp for
+        for (int i = 0; i < n_macroparticles; i += STEP) {
+
+            const int loop_count = n_macroparticles - i > STEP ?
+                                   STEP : n_macroparticles - i;
+
+            // First calculate the index to update
+            for (int j = 0; j < loop_count; j++) {
+                fbin[j] = floor((input[i + j] - cut_left) * inv_bin_width);
+            }
+            // Then update the corresponding bins
+            for (int j = 0; j < loop_count; j++) {
+                const int bin  = (int) fbin[j];
+                if (bin < 0 || bin >= n_slices) continue;
+                histo[id][bin] += 1.;
+            }
+        }
+
+        // Reduce to a single histogram
+        #pragma omp for
+        for (int i = 0; i < n_slices; i++) {
+            output[i] = 0.;
+            for (int t = 0; t < threads; t++)
+                output[i] += histo[t][i];
+        }
+    }
+
+    // free memory
+    // free(histo[0]);
+    // free(histo);
+}
+
+
+extern "C" void smooth_histogramf(const float *__restrict__ input,
+                                  float *__restrict__ output, const float cut_left,
+                                  const float cut_right, const int n_slices,
+                                  const int n_macroparticles)
+{
+    // Constants init
+    const float inv_bin_width = n_slices / (cut_right - cut_left);
+    const float bin_width = (cut_right - cut_left) / n_slices;
+    const float const1 = (cut_left + bin_width * 0.5);
+    const float const2 = (cut_right - bin_width * 0.5);
+
+    // memory alloc for per thread histo
+    float **histo = (float **) malloc(omp_get_max_threads() * sizeof(float *));
+    histo[0] = (float *) malloc (omp_get_max_threads() * n_slices * sizeof(float));
+    for (int i = 0; i < omp_get_max_threads(); i++)
+        histo[i] = (*histo + n_slices * i);
+
+
+    #pragma omp parallel
+    {
+        const int id = omp_get_thread_num();
+        const int threads = omp_get_num_threads();
+        memset(histo[id], 0., n_slices * sizeof(float));
+
+        // main caclulation
+        #pragma omp for
+        for (int i = 0; i < n_macroparticles; i++) {
+            int fffbin = 0;
+            float a = input[i];
+            if ((a < const1) || (a > const2))
+                continue;
+            float fbin = (a - cut_left) * inv_bin_width;
+            int ffbin = (int)(fbin);
+            float distToCenter = fbin - (float)(ffbin);
+            if (distToCenter > 0.5)
+                fffbin = (int)(fbin + 1.0);
+            else
+                fffbin = (int)(fbin - 1.0);
+
+            histo[id][ffbin] = histo[id][ffbin] + 0.5 - distToCenter;
+            histo[id][fffbin] = histo[id][fffbin] + 0.5 + distToCenter;
+        }
+
+        // Reduce to a single histogram
+        #pragma omp for
+        for (int i = 0; i < n_slices; i++) {
+            output[i] = 0.;
+            for (int t = 0; t < threads; t++)
+                output[i] += histo[t][i];
+        }
+
+
+    }
+    // free memory
+    free(histo[0]);
+    free(histo);
+
+}
+
+
+/***** serial histogram
+
+extern "C" void histogram(const double *__restrict__ input,
+                          double *__restrict__ output,
+                          const double cut_left, const double cut_right,
+                          const int n_slices, const int n_macroparticles)
+{
+    // Number of Iterations of the inner loop
+    const int STEP = 16;
+    const double inv_bin_width = n_slices / (cut_right - cut_left);
+    float fbin[STEP];
+
+    memset(output, 0., n_slices * sizeof(double));
+    for (int i = 0; i < n_macroparticles; i += STEP) {
+
+        const int loop_count = n_macroparticles - i > STEP ?
+                               STEP : n_macroparticles - i;
+
+        // First calculate the index to update
+        for (int j = 0; j < loop_count; j++) {
+            fbin[j] = floor((input[i + j] - cut_left) * inv_bin_width);
+        }
+        // Then update the corresponding bins
+        for (int j = 0; j < loop_count; j++) {
+            const int bin  = (int) fbin[j];
+            if (bin < 0 || bin >= n_slices) continue;
+            output[bin] += 1.;
+        }
+    }
+
+}
+
+*******/
```

### Comparing `blond-2.0.11/blond/cpp_routines/cos.h` & `blond-2.0.12/blond/cpp_routines/cos.h`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/cpp_routines/exp.h` & `blond-2.0.12/blond/cpp_routines/exp.h`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/cpp_routines/histogram.cpp` & `blond-2.0.12/blond/synchrotron_radiation/synchrotron_radiation.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -1,155 +1,154 @@
 /*
- Copyright 2016 CERN. This software is distributed under the
- terms of the GNU General Public Licence version 3 (GPL Version 3),
- copied verbatim in the file LICENCE.md.
- In applying this licence, CERN does not waive the privileges and immunities
- granted to it by virtue of its status as an Intergovernmental Organization or
- submit itself to any jurisdiction.
- Project website: http://blond.web.cern.ch/
- */
+Copyright 2016 CERN. This software is distributed under the
+terms of the GNU General Public Licence version 3 (GPL Version 3),
+copied verbatim in the file LICENCE.md.
+In applying this licence, CERN does not waive the privileges and immunities
+granted to it by virtue of its status as an Intergovernmental Organization or
+submit itself to any jurisdiction.
+Project website: http://blond.web.cern.ch/
+*/
+
+// Optimised C++ routine that calculates and applies synchrotron radiation (SR)
+// damping term
+// Author: Juan F. Esteban Mueller, Konstantinos Iliakis
 
-// Optimised C++ routine that calculates the histogram
-// Author: Danilo Quartullo, Alexandre Lasheen, Konstantinos Iliakis
-
-#include <string.h>     // memset()
-#include <stdlib.h>     // mmalloc()
 #include <math.h>
+#include <stdlib.h>
+#include <random>
+#include <thread>
+#include <chrono>
+#include "../cpp_routines/openmp.h"
+
+#ifdef BOOST
+#include <boost/random.hpp>
+#include <boost/random/normal_distribution.hpp>
+using namespace boost;
 
-#ifdef PARALLEL
-#include <omp.h>        // omp_get_thread_num(), omp_get_num_threads()
 #else
-int omp_get_max_threads() {return 1;}
-int omp_get_num_threads() {return 1;}
-int omp_get_thread_num() {return 0;}
+using namespace std;
+
 #endif
 
-extern "C" void histogram(const double *__restrict__ input,
-                          double *__restrict__ output, const double cut_left,
-                          const double cut_right, const int n_slices,
-                          const int n_macroparticles)
-{
-    // Number of Iterations of the inner loop
-    const int STEP = 16;
-    const double inv_bin_width = n_slices / (cut_right - cut_left);
-
-    // allocate memory for the thread_private histogram
-    double **histo = (double **) malloc(omp_get_max_threads() * sizeof(double *));
-    histo[0] = (double *) malloc (omp_get_max_threads() * n_slices * sizeof(double));
-    for (int i = 0; i < omp_get_max_threads(); i++)
-        histo[i] = (*histo + n_slices * i);
-
-    #pragma omp parallel
-    {
-        const int id = omp_get_thread_num();
-        const int threads = omp_get_num_threads();
-        memset(histo[id], 0., n_slices * sizeof(double));
-        float fbin[STEP];
-        #pragma omp for
-        for (int i = 0; i < n_macroparticles; i += STEP) {
-
-            const int loop_count = n_macroparticles - i > STEP ?
-                                   STEP : n_macroparticles - i;
-
-            // First calculate the index to update
-            for (int j = 0; j < loop_count; j++) {
-                fbin[j] = floor((input[i + j] - cut_left) * inv_bin_width);
-            }
-            // Then update the corresponding bins
-            for (int j = 0; j < loop_count; j++) {
-                const int bin  = (int) fbin[j];
-                if (bin < 0 || bin >= n_slices) continue;
-                histo[id][bin] += 1.;
-            }
-        }
+long unsigned int seed = 1234;
 
-        // Reduce to a single histogram
-        #pragma omp for
-        for (int i = 0; i < n_slices; i++) {
-            output[i] = 0.;
-            for (int t = 0; t < threads; t++)
-                output[i] += histo[t][i];
-        }
+// This function calculates and applies only the synchrotron radiation damping term
+extern "C" void synchrotron_radiation(double * __restrict__ beam_dE, const double U0,
+                                      const int n_macroparticles, const double tau_z,
+                                      const int n_kicks) {
+
+    // SR damping constant, adjusted for better performance
+    const double const_synch_rad = 1.0 - 2.0 / tau_z;
+
+    for (int j = 0; j < n_kicks; j++) {
+        // SR damping term due to energy spread and
+        // Average energy change due to SR
+        #pragma omp parallel for
+        for (int i = 0; i < n_macroparticles; i++)
+            beam_dE[i] = beam_dE[i] * const_synch_rad - U0;
+
+        // #pragma omp parallel for
+        // for (int i = 0; i < n_macroparticles; i++)
+        //     beam_dE[i] -= U0;
     }
-
-    // free memory
-    free(histo[0]);
-    free(histo);
 }
 
-extern "C" void smooth_histogram(const double *__restrict__ input,
-                                 double *__restrict__ output, const double cut_left,
-                                 const double cut_right, const int n_slices,
-                                 const int n_macroparticles)
+
+// This function calculates and applies synchrotron radiation damping and
+// quantum excitation terms
+extern "C" void synchrotron_radiation_full(double * __restrict__ beam_dE, const double U0,
+        const int n_macroparticles, const double sigma_dE,
+        const double tau_z, const double energy,
+        const int n_kicks)
 {
 
-    int i;
-    double a;
-    double fbin;
-    double ratioffbin;
-    double ratiofffbin;
-    double distToCenter;
-    int ffbin;
-    int fffbin;
-    const double inv_bin_width = n_slices / (cut_right - cut_left);
-    const double bin_width = (cut_right - cut_left) / n_slices;
+    // std::hash<std::thread::id> hash;
 
-    for (i = 0; i < n_slices; i++) {
-        output[i] = 0.0;
-    }
+    // Quantum excitation constant
+    const double const_quantum_exc = 2.0 * sigma_dE / sqrt(tau_z) * energy;
+
+    // Adjusted SR damping constant
+    const double const_synch_rad = 1.0 - 2.0 / tau_z;
 
-    for (i = 0; i < n_macroparticles; i++) {
-        a = input[i];
-        if ((a < (cut_left + bin_width * 0.5))
-                || (a > (cut_right - bin_width * 0.5)))
-            continue;
-        fbin = (a - cut_left) * inv_bin_width;
-        ffbin = (int)(fbin);
-        distToCenter = fbin - (double)(ffbin);
-        if (distToCenter > 0.5)
-            fffbin = (int)(fbin + 1.0);
-        ratioffbin = 1.5 - distToCenter;
-        ratiofffbin = 1 - ratioffbin;
-        if (distToCenter < 0.5)
-            fffbin = (int)(fbin - 1.0);
-        ratioffbin = 0.5 - distToCenter;
-        ratiofffbin = 1 - ratioffbin;
-        output[ffbin] = output[ffbin] + ratioffbin;
-        output[fffbin] = output[fffbin] + ratiofffbin;
+    // Random number generator for the quantum excitation term
+
+    for (int j = 0; j < n_kicks; j++) {
+        // Compute synchrotron radiation damping term and
+        // Applies the quantum excitation term
+        #pragma omp parallel
+        {
+            static __thread mt19937_64 *gen = nullptr;
+            if (!gen) gen = new mt19937_64(seed + omp_get_thread_num());
+            static thread_local normal_distribution<> dist(0.0, 1.0);
+            #pragma omp for
+            for (int i = 0; i < n_macroparticles; i++) {
+                beam_dE[i] = beam_dE[i] * const_synch_rad
+                             + const_quantum_exc * dist(*gen)
+                             - U0;
+            }
+        }
     }
 }
 
 
+// This function calculates and applies only the synchrotron radiation damping term
+extern "C" void synchrotron_radiationf(float * __restrict__ beam_dE, const float U0,
+                                      const int n_macroparticles, const float tau_z,
+                                      const int n_kicks) {
+
+    // SR damping constant, adjusted for better performance
+    const float const_synch_rad = 1.0 - 2.0 / tau_z;
+
+    for (int j = 0; j < n_kicks; j++) {
+        // SR damping term due to energy spread and
+        // Average energy change due to SR
+        #pragma omp parallel for
+        for (int i = 0; i < n_macroparticles; i++)
+            beam_dE[i] = beam_dE[i] * const_synch_rad - U0;
+
+        // #pragma omp parallel for
+        // for (int i = 0; i < n_macroparticles; i++)
+        //     beam_dE[i] -= U0;
+    }
+}
 
-/***** serial histogram
 
-extern "C" void histogram(const double *__restrict__ input,
-                          double *__restrict__ output,
-                          const double cut_left, const double cut_right,
-                          const int n_slices, const int n_macroparticles)
+// This function calculates and applies synchrotron radiation damping and
+// quantum excitation terms
+extern "C" void synchrotron_radiation_fullf(float * __restrict__ beam_dE, const float U0,
+        const int n_macroparticles, const float sigma_dE,
+        const float tau_z, const float energy,
+        const int n_kicks)
 {
-    // Number of Iterations of the inner loop
-    const int STEP = 16;
-    const double inv_bin_width = n_slices / (cut_right - cut_left);
-    float fbin[STEP];
-
-    memset(output, 0., n_slices * sizeof(double));
-    for (int i = 0; i < n_macroparticles; i += STEP) {
-
-        const int loop_count = n_macroparticles - i > STEP ?
-                               STEP : n_macroparticles - i;
-
-        // First calculate the index to update
-        for (int j = 0; j < loop_count; j++) {
-            fbin[j] = floor((input[i + j] - cut_left) * inv_bin_width);
-        }
-        // Then update the corresponding bins
-        for (int j = 0; j < loop_count; j++) {
-            const int bin  = (int) fbin[j];
-            if (bin < 0 || bin >= n_slices) continue;
-            output[bin] += 1.;
+
+    // std::hash<std::thread::id> hash;
+
+    // Quantum excitation constant
+    const float const_quantum_exc = 2.0 * sigma_dE / sqrt(tau_z) * energy;
+
+    // Adjusted SR damping constant
+    const float const_synch_rad = 1.0 - 2.0 / tau_z;
+
+    // Random number generator for the quantum excitation term
+
+    for (int j = 0; j < n_kicks; j++) {
+        // Compute synchrotron radiation damping term and
+        // Applies the quantum excitation term
+        #pragma omp parallel
+        {
+            static __thread mt19937_64 *gen = nullptr;
+            if (!gen) gen = new mt19937_64(seed + omp_get_thread_num());
+            static thread_local normal_distribution<> dist(0.0, 1.0);
+            #pragma omp for
+            for (int i = 0; i < n_macroparticles; i++) {
+                beam_dE[i] = beam_dE[i] * const_synch_rad
+                             + const_quantum_exc * dist(*gen)
+                             - U0;
+            }
         }
     }
-
 }
 
-*******/
+
+extern "C" void set_random_seed(const int _seed) {
+    seed = _seed;
+}
```

### Comparing `blond-2.0.11/blond/cpp_routines/kick.cpp` & `blond-2.0.12/blond/cpp_routines/kick.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -49,8 +49,50 @@
     for (int j = 0; j < n_rf; j++) {
         #pragma omp parallel for
         for (int i = 0; i < n_bins; i++) {
             rf_voltage[i] += voltage[j]
                              * fast_sin(omega_RF[j] * bin_centers[i] + phi_RF[j]);
         }
     }
-}
+}
+
+
+extern "C" void kickf(const float * __restrict__ beam_dt,
+                      float * __restrict__ beam_dE, const int n_rf,
+                      const float * __restrict__ voltage,
+                      const float * __restrict__ omega_RF,
+                      const float * __restrict__ phi_RF,
+                      const int n_macroparticles,
+                      const float acc_kick) {
+    int j;
+
+// KICK
+    for (j = 0; j < n_rf; j++)
+        #pragma omp parallel for
+        for (int i = 0; i < n_macroparticles; i++)
+            beam_dE[i] = beam_dE[i] + voltage[j]
+                         * fast_sinf(omega_RF[j] * beam_dt[i] + phi_RF[j]);
+
+// SYNCHRONOUS ENERGY CHANGE
+    #pragma omp parallel for
+    for (int i = 0; i < n_macroparticles; i++)
+        beam_dE[i] = beam_dE[i] + acc_kick;
+
+}
+
+extern "C" void rf_volt_compf(const float * __restrict__ voltage,
+                              const float * __restrict__ omega_RF,
+                              const float * __restrict__ phi_RF,
+                              const float * __restrict__ bin_centers,
+                              const int n_rf,
+                              const int n_bins,
+                              float *__restrict__ rf_voltage)
+{
+    for (int j = 0; j < n_rf; j++) {
+        #pragma omp parallel for
+        for (int i = 0; i < n_bins; i++) {
+            rf_voltage[i] += voltage[j]
+                             * fast_sinf(omega_RF[j] * bin_centers[i] + phi_RF[j]);
+        }
+    }
+}
+
```

### Comparing `blond-2.0.11/blond/cpp_routines/sin.h` & `blond-2.0.12/blond/cpp_routines/sin.h`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/cpp_routines/sincos.h` & `blond-2.0.12/blond/cpp_routines/sincos.h`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/cpp_routines/vdtcore_common.h` & `blond-2.0.12/blond/cpp_routines/vdtcore_common.h`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/impedances/induced_voltage_analytical.py` & `blond-2.0.12/blond/impedances/induced_voltage_analytical.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 from __future__ import division, print_function
 import numpy as np
 import scipy.special as scisp
 from scipy.constants import e
 
 
 def analytical_gaussian_resonator(sigma_t, Q, R_s, omega_r, tau_array, n_particles):
-    r"""It gives the analytical induced voltage for a gaussian bunch and a 
-    resonator.
+    r"""Calculate the analytical induced voltage for a gaussian bunch and a resonator.
     
     Parameters
     ----------
     sigma_t : float
-        Rms of the beam longitudinal coordinates [s].
+        RMS of the beam longitudinal coordinates [s].
     Q : float
         Quality factor of the resonator [1].
     R_s : float
         Shunt impedance of the resonator [:math:`\Omega`].
     omega_r : float
         Angular resonant frequency [rad/s].
     tau_array : float array
@@ -40,46 +39,50 @@
     induced_voltage : float array
         Induced voltage [V] (multiplied by -1 according to BLonD conventions).
 
     Notes
     -----
     The formula can be derived using the following lines of codes in 
     Mathematica:
-    
-    lambda = Exp[-(tau - t)^2 / (2 * sigma^2)] / ((2*Pi)^0.5 * sigma)
-    wake = 2 * alpha * Rs * Exp[-alpha * t] * (Cos[ombar * t] - alpha / ombar 
-            * Sin[ombar * t])
-    output = Integrate[wake * lambda, {t, 0, Infinity},
-        Assumptions -> {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in Reals}]
-    outputreal = Simplify[ComplexExpand[Re[output]],
-        {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in  Reals}]
-        
+
+    .. code-block:: mathematica
+
+        lambda = Exp[-(tau - t)^2 / (2 * sigma^2)] / ((2*Pi)^0.5 * sigma)
+        wake = 2 * alpha * Rs * Exp[-alpha * t] * (Cos[ombar * t] - alpha / ombar 
+                                                   * Sin[ombar * t])
+        output = Integrate[wake * lambda, {t, 0, Infinity},
+                           Assumptions -> {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in Reals}]
+        outputreal = Simplify[ComplexExpand[Re[output]],
+                              {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in  Reals}]
+
+
     The imaginary part of output is identically equal to zero even if 
     Mathematica cannot see that. To verify that the expression is correct 
     launch:
+
+    .. code-block:: mathematica
     
-    output2 = Integrate[wake * lambda, t]
-    outputreal2 = Simplify[ComplexExpand[Re[output2]],
-        {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in Reals, t > 0}]
-    d/dt output2;
-    Simplify[ComplexExpand[Re[%]],
-        {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in Reals, t > 0}]
+        output2 = Integrate[wake * lambda, t]
+        outputreal2 = Simplify[ComplexExpand[Re[output2]],
+                               {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in Reals, t > 0}]
+        d/dt output2;
+        Simplify[ComplexExpand[Re[%]],
+                 {sigma > 0, alpha > 0, Rs > 0, ombar > 0, tau in Reals, t > 0}]
     
+
     and check that applying the fundamental calculus theorem to outputreal2, 
     one obtains back outputreal; the formula [5] in 
     
     H. E. Salzer, "Formulas for Calculating the Error Function of a Complex 
     Variable", Mathematical Tables and Other Aids to Computation, Vol. 5, 
     No. 34 (Apr., 1951),pp. 67-70
     
-    can be useful.     
+    can be useful.
       
     """
-    
-    
     alpha = omega_r /(2*Q)
     ombar = np.sqrt(omega_r**2-alpha**2)
     
     A = (alpha*sigma_t**2-tau_array+1j*ombar*sigma_t**2)/(np.sqrt(2)*sigma_t)
     B = alpha*ombar*sigma_t**2-ombar*tau_array
     result = R_s*alpha/ombar*np.e**(0.5*(alpha**2-ombar**2)*sigma_t**2-alpha*tau_array)*\
                 (scisp.erfc(A).real*(ombar*np.cos(B)+alpha*np.sin(B))+scisp.erfc(A).imag*(alpha*np.cos(B)-ombar*np.sin(B)))
```

### Comparing `blond-2.0.11/blond/impedances/music.py` & `blond-2.0.12/blond/impedances/music.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 from __future__ import division
 from builtins import range, object
 import numpy as np
 from scipy.constants import e
 import ctypes
 from ..utils import bmath as bm
-
+
 
 class Music(object):
-    
+
     r"""
     Implementation of the MuSiC algorithm in C++ to calculate the exact induced 
     voltage generated by resonant modes in time domain without using slices, 
     cost = O(n). The corresponding methods in Python are kept for reference.
     The method track_classic, which calculates in time domain the
     exact voltage with the O(n^2) algorithm used in the usual voltage 
     definition, is kept just for reference. 
@@ -39,15 +39,15 @@
         quality factor [1]].
     n_macroparticles : int
         Number of macro-particles [1].
     n_particles : float
         Beam intensity [1].
     t_rev : float
         Revolution period [s]
-        
+
     Attributes
     ----------
     beam : object
         Beam object.
     R_S : float
         shunt impedance [:math:`\Omega`]
     omega_R : float
@@ -81,29 +81,29 @@
     t_rev : float
         Revolution period [s]
     last_dt: float
         Last longitudinal coordinate of the beam [s]
     array_parameters : float array
         Array gathering four attributes already defined to be used in the C++
         algorithm.
-    
+
     Notes
     -----
     The energies dE of the particles in the beam object are updated after the 
     induced voltage calculation.
-    
+
     See Also
     --------
     The MuSiC algorithm is described in:
     M. Migliorati, L. Palumbo, 'Multibunch and multiparticle simulation code 
     with an alternative approach to wakefield effects', Phys. Rev. ST Accel. 
     Beams 18, 2015.
- 
+
     """
-    
+
     def __init__(self, Beam, resonator, n_macroparticles, n_particles, t_rev):
 
         self.beam = Beam
         self.R_S = resonator[0]
         self.omega_R = resonator[1]
         self.Q = resonator[2]
         self.n_macroparticles = n_macroparticles
@@ -118,224 +118,188 @@
         self.coeff2 = -self.R_S*self.omega_R/(self.Q*self.omega_bar)
         self.coeff3 = self.omega_R*self.Q/(self.R_S*self.omega_bar)
         self.coeff4 = self.alpha/self.omega_bar
         self.input_first_component = 1
         self.input_second_component = 0
         self.t_rev = t_rev
         self.last_dt = self.beam.dt[-1]
-        self.array_parameters = np.array([self.input_first_component, 
-                        self.input_second_component, self.t_rev, self.last_dt])
-    
-    
+        self.array_parameters = np.array([self.input_first_component,
+                                          self.input_second_component, self.t_rev, self.last_dt])
+
     def track_cpp(self):
-        
         r"""
         Voltage in time domain (single-turn) using MuSiC (C++ code).
         Note: this method should also be called at turn number 1 when
         multi-turn voltage computations are needed.
-        
+
         Examples
         --------
         >>> import impedances.music as musClass
         >>> from setup_cpp import libblond
         >>>  
         >>> music_cpp = musClass.Music(my_beam, [R_S, 2*np.pi*frequency_R, Q], 
         >>>                               n_macroparticles, n_particles, t_rev)
         >>> music_cpp.track_cpp()
-        
+
         """
-        bm.music_track(self)
+        bm.music_track(self.beam.dt, self.beam.dE, self.induced_voltage,
+                       self.array_parameters, self.alpha, self.omega_bar,
+                       self.const, self.coeff1, self.coeff2, self.coeff3,
+                       self.coeff4)
 
-#          libblond.music_track(self.beam.dt.ctypes.data_as(ctypes.c_void_p),
-                        #       self.beam.dE.ctypes.data_as(ctypes.c_void_p),
-                        #  self.induced_voltage.ctypes.data_as(ctypes.c_void_p),
-                        #  self.array_parameters.ctypes.data_as(ctypes.c_void_p),
-                        #       ctypes.c_int(len(self.beam.dt)),
-                        #       ctypes.c_double(self.alpha),
-                        #       ctypes.c_double(self.omega_bar),
-                        #       ctypes.c_double(self.const),
-                        #       ctypes.c_double(self.coeff1),
-                        #       ctypes.c_double(self.coeff2),
-                        #       ctypes.c_double(self.coeff3),
-                        #       ctypes.c_double(self.coeff4))
-#      
-    
     def track_cpp_multi_turn(self):
-        
         r"""
         Voltage in time domain (multi-turn) using MuSiC (C++ code).
         Note: this method should be called from turn number 2 onwards when
         multi-turn voltage computations are needed..
-        
+
         Examples
         --------
         >>> import impedances.music as musClass
         >>> from setup_cpp import libblond
-        >>>  
-        >>> music_cpp = musClass.Music(my_beam, [R_S, 2*np.pi*frequency_R, Q], 
+        >>>
+        >>> music_cpp = musClass.Music(my_beam, [R_S, 2*np.pi*frequency_R, Q],
         >>>                               n_macroparticles, n_particles, t_rev)
         >>> music_cpp.track_cpp()
         >>> for i in range(2, n_turns):
         >>>     music_cpp.track_cpp_multi_turn()
-        
+
         """
-        bm.music_track_multiturn(self)
+        bm.music_track_multiturn(self.beam.dt, self.beam.dE, self.induced_voltage,
+                                 self.array_parameters, self.alpha, self.omega_bar,
+                                 self.const, self.coeff1, self.coeff2, self.coeff3,
+                                 self.coeff4)
 
-#          libblond.music_track_multiturn(
-                        #       self.beam.dt.ctypes.data_as(ctypes.c_void_p),
-                        #       self.beam.dE.ctypes.data_as(ctypes.c_void_p),
-                        #  self.induced_voltage.ctypes.data_as(ctypes.c_void_p),
-                        #  self.array_parameters.ctypes.data_as(ctypes.c_void_p),
-                        #       ctypes.c_int(len(self.beam.dt)),
-                        #       ctypes.c_double(self.alpha),
-                        #       ctypes.c_double(self.omega_bar),
-                        #       ctypes.c_double(self.const),
-                        #       ctypes.c_double(self.coeff1),
-                        #       ctypes.c_double(self.coeff2),
-                        #       ctypes.c_double(self.coeff3),
-                        #       ctypes.c_double(self.coeff4))
-#      
-    
     def track_py(self):
-        
         r"""
         Voltage in time domain (single-turn) using MuSiC (Python code).
         Note: this method should also be called at turn number 1 when
         multi-turn voltage computations are needed.
-        
+
         Examples
         --------
         >>> import impedances.music as musClass
         >>>  
         >>> music_cpp = musClass.Music(my_beam, [R_S, 2*np.pi*frequency_R, Q], 
         >>>                               n_macroparticles, n_particles, t_rev)
         >>> music_cpp.track_py()
-        
+
         """
-        
+
         indices_sorted = np.argsort(self.beam.dt)
         self.beam.dt = self.beam.dt[indices_sorted]
         self.beam.dE = self.beam.dE[indices_sorted]
         self.beam.dE[0] += self.induced_voltage[0]
         self.input_first_component = 1
         self.input_second_component = 0
-    
+
         for i in range(len(self.beam.dt)-1):
-    
+
             time_difference = self.beam.dt[i+1]-self.beam.dt[i]
-              
+
             exp_term = np.exp(-self.alpha * time_difference)
             cos_term = np.cos(self.omega_bar * time_difference)
             sin_term = np.sin(self.omega_bar * time_difference)
-            
+
             product_first_component = exp_term * \
-                ((cos_term+self.coeff1*sin_term)*self.input_first_component +
-                 self.coeff2*sin_term*self.input_second_component)
+                ((cos_term+self.coeff1*sin_term)*self.input_first_component
+                 + self.coeff2*sin_term*self.input_second_component)
             product_second_component = exp_term * \
-                (self.coeff3*sin_term*self.input_first_component +
-                 (cos_term+self.coeff4*sin_term)*self.input_second_component)
-                
+                (self.coeff3*sin_term*self.input_first_component
+                 + (cos_term+self.coeff4*sin_term)*self.input_second_component)
+
             self.induced_voltage[i+1] = self.const * \
                 (0.5+product_first_component)
             self.beam.dE[i+1] += self.induced_voltage[i+1]
-            
+
             self.input_first_component = product_first_component+1.0
             self.input_second_component = product_second_component
-            
+
         self.last_dt = self.beam.dt[-1]
-    
-    
+
     def track_py_multi_turn(self):
-        
         r"""
         Voltage in time domain (multi-turn) using MuSiC (Python code).
         Note: this method should be called from turn number 2 onwards when
         multi-turn voltage computations are needed..
-        
+
         Examples
         --------
         >>> import impedances.music as musClass
         >>>  
         >>> music_cpp = musClass.Music(my_beam, [R_S, 2*np.pi*frequency_R, Q], 
         >>>                               n_macroparticles, n_particles, t_rev)
         >>> music_cpp.track_py()
         >>> for i in range(2, n_turns):
         >>>     music_cpp.track_py_multi_turn()
-        
+
         """
-        
-        
+
         indices_sorted = np.argsort(self.beam.dt)
         self.beam.dt = self.beam.dt[indices_sorted]
         self.beam.dE = self.beam.dE[indices_sorted]
         time_difference_0 = self.beam.dt[0] + self.t_rev - self.last_dt
         exp_term = np.exp(-self.alpha * time_difference_0)
         cos_term = np.cos(self.omega_bar * time_difference_0)
         sin_term = np.sin(self.omega_bar * time_difference_0)
         product_first_component = exp_term * \
-            ((cos_term+self.coeff1*sin_term)*self.input_first_component +
-             self.coeff2*sin_term*self.input_second_component)
+            ((cos_term+self.coeff1*sin_term)*self.input_first_component
+             + self.coeff2*sin_term*self.input_second_component)
         product_second_component = exp_term * \
-            (self.coeff3*sin_term*self.input_first_component +
-             (cos_term+self.coeff4*sin_term)*self.input_second_component)
+            (self.coeff3*sin_term*self.input_first_component
+             + (cos_term+self.coeff4*sin_term)*self.input_second_component)
         self.induced_voltage[0] = self.const * \
             (0.5+product_first_component)
         self.beam.dE[0] += self.induced_voltage[0]
         self.input_first_component = product_first_component+1.0
         self.input_second_component = product_second_component
-    
+
         for i in range(len(self.beam.dt)-1):
-    
+
             time_difference = self.beam.dt[i+1]-self.beam.dt[i]
-              
+
             exp_term = np.exp(-self.alpha * time_difference)
             cos_term = np.cos(self.omega_bar * time_difference)
             sin_term = np.sin(self.omega_bar * time_difference)
-            
+
             product_first_component = exp_term * \
-                ((cos_term+self.coeff1*sin_term)*self.input_first_component +
-                 self.coeff2*sin_term*self.input_second_component)
+                ((cos_term+self.coeff1*sin_term)*self.input_first_component
+                 + self.coeff2*sin_term*self.input_second_component)
             product_second_component = exp_term * \
-                (self.coeff3*sin_term*self.input_first_component +
-                 (cos_term+self.coeff4*sin_term)*self.input_second_component)
-                
+                (self.coeff3*sin_term*self.input_first_component
+                 + (cos_term+self.coeff4*sin_term)*self.input_second_component)
+
             self.induced_voltage[i+1] = self.const * \
                 (0.5+product_first_component)
             self.beam.dE[i+1] += self.induced_voltage[i+1]
-            
+
             self.input_first_component = product_first_component+1.0
-            self.input_second_component = product_second_component 
-        
-        self.last_dt = self.beam.dt[-1]    
-        
-    
+            self.input_second_component = product_second_component
+
+        self.last_dt = self.beam.dt[-1]
+
     def track_classic(self):
-        
         r"""
         Voltage in time domain using the basic definition (Python code)
-        
+
         """
-        
+
         indices_sorted = np.argsort(self.beam.dt)
         self.beam.dt = self.beam.dt[indices_sorted]
         self.beam.dE = self.beam.dE[indices_sorted]
         self.beam.dE[0] += self.induced_voltage[0]
         self.induced_voltage[1:] = 0
-        
+
         for i in range(len(self.beam.dt)-1):
-            
+
             for j in range(i+1):
-                
+
                 time_difference = self.beam.dt[i+1]-self.beam.dt[j]
                 exp_term = np.exp(-self.alpha * time_difference)
                 cos_term = np.cos(self.omega_bar * time_difference)
                 sin_term = np.sin(self.omega_bar * time_difference)
                 self.induced_voltage[i+1] += \
                     exp_term*(cos_term+self.coeff1*sin_term)
-                
+
             self.induced_voltage[i+1] = \
-                self.const*(0.5+self.induced_voltage[i+1])    
+                self.const*(0.5+self.induced_voltage[i+1])
             self.beam.dE[i+1] += self.induced_voltage[i+1]
-            
-    
-        
-
```

### Comparing `blond-2.0.11/blond/input_parameters/rf_parameters.py` & `blond-2.0.12/blond/input_parameters/rf_parameters.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from __future__ import division, print_function
 from builtins import str, range, object
 import numpy as np
 from scipy.constants import c
 from scipy.integrate import cumtrapz
 from ..beam.beam import Proton
 from ..input_parameters.rf_parameters_options import RFStationOptions
+from ..utils import bmath as bm
 
 
 class RFStation(object):
     r""" Class containing all the RF parameters for all the RF systems in one
     ring segment or RF station.
 
     **How to use RF programs:**
@@ -129,14 +130,26 @@
         :py:attr:`input_parameters.ring.Ring.delta_E`
     alpha_order : int
         Inherited from
         :py:attr:`input_parameters.ring.Ring.alpha_order`
     charge : int
         Inherited from
         :py:attr:`beam.Particle.charge`
+    alpha_0 : float array [n_turns+1]
+        Zeroth order momentum compaction factor of the present section;
+        inherited from
+        :py:attr:`input_parameters.ring.Ring.alpha_0`
+    alpha_1 : float array [n_turns+1]
+        First order momentum compaction factor of the present section;
+        inherited from
+        :py:attr:`input_parameters.ring.Ring.alpha_1`
+    alpha_2 : float array [n_turns+1]
+        Second order momentum compaction factor of the present section;
+        inherited from
+        :py:attr:`input_parameters.ring.Ring.alpha_2`
     eta_0 : float array [n_turns+1]
         Zeroth order slippage factor of the present section; inherited from
         :py:attr:`input_parameters.ring.Ring.eta_0`
     eta_1 : float array [n_turns+1]
         First order slippage factor of the present section; inherited from
         :py:attr:`input_parameters.ring.Ring.eta_1`
     eta_2 : float array [n_turns+1]
@@ -171,18 +184,18 @@
         Programmed cavity phase modulation for each RF harmonic.
     dphi_rf : float matrix [n_rf]
         Accumulated RF phase error of each harmonic system
         :math:`\Delta \phi_{rf,l,n}` [rad]
     t_rf : float matrix [n_rf, n_turns+1]
         RF period :math:`\frac{2 \pi}{\omega_{rf,l,n}}` [s]
     phi_s : float array [n_turns+1]
-        Synchronous phase for this section, calculated in
+        Synchronous phase for this section (if not empty), calculated in
         :py:func:`input_parameters.rf_parameters.calculate_phi_s`
     Q_s : float array [n_turns+1]
-        Synchrotron tune for this section, calculated in
+        Synchrotron tune for this section (if not empty), calculated in
         :py:func:`input_parameters.rf_parameters.calculate_Q_s`
     omega_s0 : float array [n_turns+1]
         Central synchronous angular frequency corresponding to Q_s (single
         harmonic, no intensity effects)
         :math:`\omega_{s,0} = Q_s \omega_{\text{rev}}` [1/s], where
         :math:`\omega_{\text{rev}}` is defined in
         :py:class:`input_parameters.ring.Ring`)
@@ -204,14 +217,16 @@
 
     """
 
     def __init__(self, Ring, harmonic, voltage, phi_rf_d, n_rf=1,
                  section_index=1, omega_rf=None, phi_noise=None,
                  phi_modulation=None, RFStationOptions=RFStationOptions()):
 
+
+
         # Different indices
         self.counter = [int(0)]
         self.section_index = int(section_index - 1)
         if self.section_index < 0 \
                 or self.section_index > Ring.n_sections - 1:
             raise RuntimeError("ERROR in RFStation: section_index out of" +
                                " allowed range!")
@@ -228,37 +243,43 @@
         self.beta = Ring.beta[self.section_index]
         self.gamma = Ring.gamma[self.section_index]
         self.energy = Ring.energy[self.section_index]
         self.delta_E = Ring.delta_E[self.section_index]
         self.alpha_order = Ring.alpha_order
         self.charge = self.Particle.charge
 
+
+
         # The order alpha_order used here can be replaced by Ring.alpha_order
-        # when the assembler can differentiate the cases 'simple' and 'full'
+        # when the assembler can differentiate the cases 'simple' and 'exact'
         # for the drift
         alpha_order = 2
         for i in range(alpha_order+1):
             dummy = getattr(Ring, 'eta_' + str(i))
             setattr(self, "eta_%s" % i, dummy[self.section_index])
+            dummy = getattr(Ring, 'alpha_' + str(i))
+            setattr(self, "alpha_%s" % i, dummy[self.section_index])
         self.sign_eta_0 = np.sign(self.eta_0)
 
         # Reshape input rf programs
         # Reshape design harmonic
         self.harmonic = RFStationOptions.reshape_data(harmonic,
                                                       self.n_turns,
                                                       self.n_rf,
                                                       Ring.cycle_time,
                                                       Ring.RingOptions.t_start)
+        self.harmonic = self.harmonic.astype(bm.precision.real_t, order='C', copy=False)
+
         # Reshape design voltage
         self.voltage = RFStationOptions.reshape_data(voltage,
                                                      self.n_turns,
                                                      self.n_rf,
                                                      Ring.cycle_time,
                                                      Ring.RingOptions.t_start)
-
+        self.voltage = self.voltage.astype(bm.precision.real_t, order='C', copy=False)
         # Checking if the RFStation is empty
         if np.sum(self.voltage) == 0:
             self.empty = True
         else:
             self.empty = False
 
         # Reshape design phase
@@ -275,35 +296,39 @@
         else:
             self.omega_rf_d = RFStationOptions.reshape_data(
                 omega_rf,
                 self.n_turns,
                 self.n_rf,
                 Ring.cycle_time,
                 Ring.RingOptions.t_start)
+        self.omega_rf_d = self.omega_rf_d.astype(bm.precision.real_t, order='C', copy=False)
 
         # Reshape phase noise
         if phi_noise is not None:
             self.phi_noise = RFStationOptions.reshape_data(
                 phi_noise,
                 self.n_turns,
                 self.n_rf,
                 Ring.cycle_time,
                 Ring.RingOptions.t_start)
+            self.phi_noise = self.phi_noise.astype(bm.precision.real_t, order='C', copy=False)
+
+            
         else:
             self.phi_noise = None
             
         if phi_modulation is not None:
             
             try:
                 iter(phi_modulation)
             except TypeError:
                 phi_modulation = [phi_modulation]
             
-            dPhi = np.zeros([self.n_rf, self.n_turns+1])
-            dOmega = np.zeros([self.n_rf, self.n_turns+1])
+            dPhi = np.zeros([self.n_rf, self.n_turns+1], dtype=bm.precision.real_t)
+            dOmega = np.zeros([self.n_rf, self.n_turns+1], dtype=bm.precision.real_t)
             for pMod in phi_modulation:
                 system = np.where(self.harmonic[:,0] == pMod.harmonic)[0]
                 if len(system) == 0:
                     raise ValueError("No matching harmonic in phi_modulation")
                 elif len(system) > 1:
                     raise RuntimeError("""Phase modulation not yet 
                                        implemented with multiple systems 
@@ -328,25 +353,28 @@
                 
             
             self.phi_modulation = (dPhi, dOmega)
         else:
             
             self.phi_modulation = None
 
+
         # Copy of the desing rf programs in the one used for tracking
         # and that can be changed by feedbacks
-        self.phi_rf = np.array(self.phi_rf_d)
-        self.dphi_rf = np.zeros(self.n_rf)
-        self.omega_rf = np.array(self.omega_rf_d)
+        self.phi_rf = np.array(self.phi_rf_d).astype(bm.precision.real_t)
+        self.dphi_rf = np.zeros(self.n_rf).astype(bm.precision.real_t)
+        self.omega_rf = np.array(self.omega_rf_d).astype(bm.precision.real_t)
         self.t_rf = 2*np.pi / self.omega_rf
 
         # From helper functions
-        self.phi_s = calculate_phi_s(self, self.Particle)
-        self.Q_s = calculate_Q_s(self, self.Particle)
-        self.omega_s0 = self.Q_s*Ring.omega_rev
+        if not self.empty:
+            self.phi_s = calculate_phi_s(self, self.Particle)
+            self.Q_s = calculate_Q_s(self, self.Particle)
+            self.omega_s0 = self.Q_s*Ring.omega_rev
+
 
     def eta_tracking(self, beam, counter, dE):
         r"""Function to calculate the slippage factor as a function of the
         energy offset :math:`\Delta E` of the particle. The slippage factor
         of the :math:`i` th order is :math:`\eta(\delta) = \sum_{i}(\eta_i \,
         \delta^i) = \sum_{i} \left(\eta_i \, \left[ \frac{\Delta E}
         {\beta_s^2 E_s} \right]^i \right)`
@@ -359,14 +387,66 @@
             eta = 0
             delta = dE/(beam.beta**2 * beam.energy)
             for i in range(self.alpha_order+1):
                 eta_i = getattr(self, 'eta_' + str(i))[counter]
                 eta += eta_i * (delta**i)
             return eta
 
+    def to_gpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays to the GPU
+        '''
+        # Check if to_gpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'GPU':
+            return
+        assert bm.device == 'GPU'
+        import cupy as cp
+        if self.phi_modulation is not None:
+            self.phi_modulation = (cp.array(self.phi_modulation[0]),
+                                   cp.array(self.phi_modulation[1]))
+        if self.phi_noise is not None:
+            self.phi_noise = cp.array(self.phi_noise)
+
+        self.voltage = cp.array(self.voltage)
+        self.omega_rf = cp.array(self.omega_rf)
+        self.phi_rf = cp.array(self.phi_rf)
+        self.omega_rf_d = cp.array(self.omega_rf_d)
+        self.harmonic = cp.array(self.harmonic)
+        self.dphi_rf = cp.array(self.dphi_rf)
+        self.t_rf = cp.array(self.t_rf)
+        self.t_rev = cp.array(self.t_rev)
+
+        # to make sure it will not be called again
+        self._device = 'GPU'
+
+    def to_cpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays back to the CPU
+        '''
+        # Check if to_cpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'CPU':
+            return
+        assert bm.device == 'CPU'
+        import cupy as cp
+        if self.phi_modulation is not None:
+            self.phi_modulation = (cp.asnumpy(self.phi_modulation[0]),
+                                   cp.asnumpy(self.phi_modulation[1]))
+        if self.phi_noise is not None:
+            self.phi_noise = cp.asnumpy(self.phi_noise)
+
+        self.voltage = cp.asnumpy(self.voltage)
+        self.omega_rf = cp.asnumpy(self.omega_rf)
+        self.phi_rf = cp.asnumpy(self.phi_rf)
+        self.omega_rf_d = cp.asnumpy(self.omega_rf_d)
+        self.harmonic = cp.asnumpy(self.harmonic)
+        self.dphi_rf = cp.asnumpy(self.dphi_rf)
+        self.t_rf = cp.asnumpy(self.t_rf)
+        self.t_rev = cp.asnumpy(self.t_rev)
+        # to make sure it will not be called again
+        self._device = 'CPU'
 
 def calculate_Q_s(RFStation, Particle=Proton()):
     r""" Function calculating the turn-by-turn synchrotron tune for
     single-harmonic RF, without intensity effects.
 
     Parameters
     ----------
@@ -446,16 +526,19 @@
         # Identify where eta swaps sign
         eta0_middle_points = (eta0[1:] + eta0[:-1])/2
         eta0_middle_points = np.append(eta0_middle_points, eta0[-1])
         index = np.where(eta0_middle_points > 0)[0]
         index_below = np.where(eta0_middle_points < 0)[0]
 
         # Project phi_s in correct range
-        phi_s[index] = (np.pi - phi_s[index]) % (2*np.pi)
-        phi_s[index_below] = (np.pi + phi_s[index_below]) % (2*np.pi)
+        phi_s[index] = (np.heaviside(np.sign(Particle.charge),0) * np.pi - phi_s[index]) % (2*np.pi)
+        phi_s[index_below] = (np.heaviside(np.sign(Particle.charge),0) * np.pi + phi_s[index_below])\
+            % (2*np.pi)
+        # phi_s[index] = (np.pi - phi_s[index]) % (2*np.pi)
+        # phi_s[index_below] = (np.pi + phi_s[index_below]) % (2*np.pi)
 
         return phi_s
 
     elif accelerating_systems == 'all':
 
         phi_s = np.zeros(len(RFStation.voltage[0, 1:]))
 
@@ -497,7 +580,8 @@
 
         print("WARNING in calculate_phi_s(): accelerating_systems 'first'" +
               " not yet implemented")
         pass
     else:
         raise RuntimeError("ERROR in calculate_phi_s(): unrecognised" +
                            " accelerating_systems option")
+
```

### Comparing `blond-2.0.11/blond/input_parameters/rf_parameters_options.py` & `blond-2.0.12/blond/input_parameters/rf_parameters_options.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/input_parameters/ring.py` & `blond-2.0.12/blond/input_parameters/ring.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,25 @@
         Circumference of the synchrotron. Sum of ring segment lengths,
         :math:`C = \sum_k L_k` [m]
     ring_radius : float
         Radius of the synchrotron, :math:`R = C/(2 \pi)` [m]
     bending_radius : float
         Bending radius in dipole magnets, :math:`\rho` [m]
     alpha_order : int
-        Number of orders of the momentum compaction factor (from 0 to 2)
+        Highest order of momentum compaction (as defined by the input). Can
+        be 0,1,2.
+    alpha_0 : float matrix [n_sections, n_turns+1]
+        Zeroth order momentum compaction factor
+        :math:`\alpha_{0,k,n}`
+    alpha_1 : float matrix [n_sections, n_turns+1]
+        First order momentum compaction factor
+        :math:`\alpha_{1,k,n}`
+    alpha_2 : float matrix [n_sections, n_turns+1]
+        Second order momentum compaction factor
+        :math:`\alpha_{2,k,n}`
     eta_0 : float matrix [n_sections, n_turns+1]
         Zeroth order slippage factor :math:`\eta_{0,k,n} = \alpha_{0,k,n} -
         \frac{1}{\gamma_{s,k,n}^2}` [1]
     eta_1 : float matrix [n_sections, n_turns+1]
         First order slippage factor :math:`\eta_{1,k,n} =
         \frac{3\beta_{s,k,n}^2}{2\gamma_{s,k,n}^2} + \alpha_{1,k,n} -
         \alpha_{0,k,n}\eta_{0,k,n}` [1]
@@ -134,17 +144,14 @@
         Revolution frequency :math:`f_{0,n} = \frac{1}{T_{0,n}}` [Hz]
     omega_rev : float array [n_turns+1]
         Revolution angular frequency :math:`\omega_{0,n} = 2\pi f_{0,n}` [1/s]
     cycle_time : float array [n_turns+1]
         Cumulative cycle time, turn by turn, :math:`t_n = \sum_n T_{0,n}` [s].
         Possibility to extract cycle parameters at these moments using
         'parameters_at_time'.
-    alpha_order : int
-        Highest order of momentum compaction (as defined by the input). Can
-        be 0,1,2.
     RingOptions : RingOptions()
         The RingOptions is kept as an attribute of the Ring object for further
         usage.
 
     Examples
     --------
     >>> # To declare a single-section synchrotron at constant energy:
@@ -235,34 +242,47 @@
         self.delta_E = np.diff(self.energy, axis=1)
         self.t_rev = np.dot(self.ring_length, 1/(self.beta*c))
         self.cycle_time = np.cumsum(self.t_rev)  # Always starts with zero
         self.f_rev = 1/self.t_rev
         self.omega_rev = 2*np.pi*self.f_rev
 
         # Momentum compaction, checks, and derived slippage factors
+        if RingOptions.t_start is None:
+            interp_time = self.cycle_time
+        else:
+            interp_time = self.cycle_time+RingOptions.t_start
+
         self.alpha_0 = RingOptions.reshape_data(
             alpha_0, self.n_turns, self.n_sections,
-            interp_time=self.cycle_time)
+            interp_time=interp_time)
         self.alpha_order = 0
 
         if alpha_1 is not None:
             self.alpha_1 = RingOptions.reshape_data(
                 alpha_1, self.n_turns, self.n_sections,
-                interp_time=self.cycle_time)
+                interp_time=interp_time)
             self.alpha_order = 1
+        else:
+            # Filling alpha_1 with zeros
+            # This can be removed when the BLonD assembler is in place
+            # to avoid high order momentum compaction programs filled
+            # with zeros (should be propagated in RFStation.__init__())
+            self.alpha_1 = np.zeros(self.alpha_0.shape)
 
         if alpha_2 is not None:
             self.alpha_2 = RingOptions.reshape_data(
                 alpha_2, self.n_turns, self.n_sections,
-                interp_time=self.cycle_time)
+                interp_time=interp_time)
             self.alpha_order = 2
-
-            # Filling alpha_1 with zeros if only alpha_2 program was set
-            if alpha_1 is None:
-                self.alpha_1 = np.zeros(self.alpha_2.shape)
+        else:
+            # Filling alpha_2 with zeros
+            # This can be removed when the BLonD assembler is in place
+            # to avoid high order momentum compaction programs filled
+            # with zeros (should be propagated in RFStation.__init__())
+            self.alpha_2 = np.zeros(self.alpha_0.shape)
 
         # Slippage factor derived from alpha, beta, gamma
         self.eta_generation()
 
     def eta_generation(self):
         """ Function to generate the slippage factors (zeroth, first, and
         second orders, see [1]_) from the momentum compaction and the
```

### Comparing `blond-2.0.11/blond/input_parameters/ring_options.py` & `blond-2.0.12/blond/input_parameters/ring_options.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/llrf/beam_feedback.py` & `blond-2.0.12/blond/llrf/beam_feedback.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,562 +1,587 @@
 # coding: utf8
 # Copyright 2014-2017 CERN. This software is distributed under the
-# terms of the GNU General Public Licence version 3 (GPL Version 3), 
+# terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
-# In applying this licence, CERN does not waive the privileges and immunities 
+# In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 **Various beam phase loops with optional synchronisation/frequency/radial loops
 for the CERN machines**
 
 :Authors: **Helga Timko**, **Alexandre Lasheen**
 '''
 
 from __future__ import division
 from builtins import object
 import numpy as np
+from ..utils import bmath as bm
 
 
-class BeamFeedback(object): 
+class BeamFeedback(object):
     '''
     One-turn beam phase loop for different machines with different hardware. 
     Use 'period' for a phase loop that is active only in certain turns. 
     The phase loop acts directly on the RF frequency of all harmonics and
     affects the RF phase as well.
-    '''    
-    def __init__(self, Ring, RFStation, Profile, 
+    '''
+
+    def __init__(self, Ring, RFStation, Profile,
                  configuration,
-                 PhaseNoise = None, 
-                 LHCNoiseFB = None, delay = 0):
+                 PhaseNoise=None,
+                 LHCNoiseFB=None, delay=0):
 
         #: | *Import Ring*
         self.ring = Ring
 
         #: | *Import RFStation*
         self.rf_station = RFStation
-        
+
         #: | *Import Profile*
         self.profile = Profile
 
         #: | *Machine-dependent configuration of LLRF system.*
         self.config = configuration
-        
+
         self.delay = delay
-        
+
         #: | *Machine name; see description of each machine.*
-        if 'machine' not in self.config:  
+        if 'machine' not in self.config:
             self.machine = 'LHC'
-        else: 
-            self.machine = self.config['machine'] 
+        else:
+            self.machine = self.config['machine']
 
         #: | *Band-pass filter window coefficient for beam phase calculation.*
-        if 'window_coefficient' not in self.config:  
+        if 'window_coefficient' not in self.config:
             self.alpha = 0.
-        else: 
+        else:
             self.alpha = self.config['window_coefficient']
-        
+
         # determines from which RF-buckets the band-pass filter starts to acts
         if 'time_offset' not in self.config:
             self.time_offset = None
         else:
             self.time_offset = self.config['time_offset']
 
-        #: | *Phase loop gain. Implementation depends on machine.*        
+        #: | *Phase loop gain. Implementation depends on machine.*
         try:
-            self.gain = self.config['PL_gain'] 
+            self.gain = self.config['PL_gain']
         except:
-            #PhaseLoopError
-            raise RuntimeError("You need to specify the Phase Loop gain! Aborting")
-        
+            # PhaseLoopError
+            raise RuntimeError(
+                "You need to specify the Phase Loop gain! Aborting")
+
         # LHC CONFIGURATION
         if self.machine == 'LHC':
 
-            #: | *Synchronisation loop gain.*            
-            if 'SL_gain' not in self.config:  
+            #: | *Synchronisation loop gain.*
+            if 'SL_gain' not in self.config:
                 self.gain2 = 0.
-            else: 
-                self.gain2 = self.config['SL_gain'] 
+            else:
+                self.gain2 = self.config['SL_gain']
 
             #: | *LHC Synchroronisation loop recursion variable*
-            self.lhc_y = 0 
-            
+            self.lhc_y = 0
+
             if self.gain2 != 0:
-                
+
                 #: | *LHC Synchronisation loop coefficient [1]*
-                self.lhc_a = 5.25 - self.rf_station.omega_s0/(np.pi*40.) 
+                self.lhc_a = 5.25 - self.rf_station.omega_s0/(np.pi*40.)
                 #: | *LHC Synchronisation loop time constant [turns]*
-                self.lhc_t = ( 2*np.pi*self.rf_station.Q_s*np.sqrt(self.lhc_a) )/ \
-                               np.sqrt(1 + self.gain/self.gain2* \
-                               np.sqrt((1 + 1/self.lhc_a)/(1 + self.lhc_a)))
-                               
+                self.lhc_t = (2*np.pi*self.rf_station.Q_s*np.sqrt(self.lhc_a)) / \
+                    np.sqrt(1 + self.gain/self.gain2 *
+                            np.sqrt((1 + 1/self.lhc_a)/(1 + self.lhc_a)))
+
             else:
-                
+
                 self.lhc_a = np.zeros(self.rf_station.n_turns + 1)
                 self.lhc_t = np.zeros(self.rf_station.n_turns + 1)
 
-                
         # LHC_F CONFIGURATION
         elif self.machine == 'LHC_F':
 
-            #: | *Frequency loop gain.*            
-            if 'FL_gain' not in self.config:  
+            #: | *Frequency loop gain.*
+            if 'FL_gain' not in self.config:
                 self.gain2 = 0.
-            else: 
-                self.gain2 = self.config['FL_gain'] 
-                
-                
+            else:
+                self.gain2 = self.config['FL_gain']
+
         # SPS_RL CONFIGURATION
         elif self.machine == 'SPS_RL':
 
-            #: | *Frequency loop gain.*            
-            if 'RL_gain' not in self.config:  
+            #: | *Frequency loop gain.*
+            if 'RL_gain' not in self.config:
                 self.gain2 = 0.
-            else: 
+            else:
                 self.gain2 = self.config['RL_gain']
-                
+
+            #: | *Number of particles to sample from dE for orbit calculation*
+            if 'sample_dE' not in self.config:
+                self.sample_dE = 1
+            else:
+                self.sample_dE = self.config['sample_dE']
+
         elif self.machine == 'SPS_F':
-            #: | *Frequency loop gain.*            
-            if 'FL_gain' not in self.config:  
+            #: | *Frequency loop gain.*
+            if 'FL_gain' not in self.config:
                 self.gain2 = 0.
-            else: 
+            else:
                 self.gain2 = self.config['FL_gain']
-                
-        # PSB CONFIGURATION        
+
+        # PSB CONFIGURATION
         elif self.machine == 'PSB':
-            
+
             self.gain = self.gain * np.ones(Ring.n_turns+1)
-            
+
             #: | *Radial loop gain, proportional [1] and integral [1/s].*
-            if 'RL_gain' not in self.config:  
+            if 'RL_gain' not in self.config:
                 self.gain2 = [0., 0.]
-            else: 
-                self.gain2 = self.config['RL_gain'] 
-            
+            else:
+                self.gain2 = self.config['RL_gain']
+
             self.gain2[0] = self.gain2[0] * np.ones(Ring.n_turns+1)
             self.gain2[1] = self.gain2[1] * np.ones(Ring.n_turns+1)
-                        
+
             #: | *Optional: PL & RL acting only in certain time intervals/turns.*
             self.dt = 0
-            #| *Phase Loop sampling period [s]*
-            if 'period' not in self.config:  
-                self.dt = 10.e-6 # [s]
-            else: 
-                self.dt = self.config['period'] 
-            
+            # | *Phase Loop sampling period [s]*
+            if 'period' not in self.config:
+                self.dt = 10.e-6  # [s]
+            else:
+                self.dt = self.config['period']
+
             # Counter of turns passed since last time the PL was active
             self.PL_counter = 0
             self.on_time = np.array([])
-            
+
             self.precalculate_time(Ring)
-        
+
             #: | *Array of transfer function coefficients.*
-            if 'coefficients' not in self.config:  
-                self.coefficients = [0.999019,-0.999019,0.,1.,-0.998038,0.]  
+            if 'coefficients' not in self.config:
+                self.coefficients = [0.999019, -0.999019, 0., 1., -0.998038, 0.]
             else:
                 self.coefficients = self.config['coefficients']
-                
-            #: | *Memory of previous phase correction, for phase loop.*        
+
+            #: | *Memory of previous phase correction, for phase loop.*
             self.dphi_sum = 0.
             self.dphi_av = 0.
             self.dphi_av_prev = 0.
 
-            #: | *Memory of previous relative radial correction, for rad loop.*        
+            #: | *Memory of previous relative radial correction, for rad loop.*
             self.dR_over_R_prev = 0.
-            
+
             #: | *Phase loop frequency correction [1/s]*
             self.domega_PL = 0.
 
             #: | *Radial loop frequency correction [1/s]*
             self.domega_RL = 0.
-            
+
             self.dR_over_R = 0
 
-        #: | *Relative radial displacement [1], for radial loop.*        
+        #: | *Relative radial displacement [1], for radial loop.*
         self.drho = 0.
-        
+
         #: | *Phase loop frequency correction of the main RF system.*
         self.domega_rf = 0.
-        
-        #: | *Beam phase measured at the main RF frequency.*        
+
+        #: | *Beam phase measured at the main RF frequency.*
         self.phi_beam = 0.
-        
-        #: | *Phase difference between beam and RF.*        
+
+        #: | *Phase difference between beam and RF.*
         self.dphi = 0.
-                    
-        #: | *Reference signal for secondary loop to test step response.*        
+
+        #: | *Reference signal for secondary loop to test step response.*
         self.reference = 0.
-                    
-        #: | *Optional import of RF PhaseNoise object*       
+
+        #: | *Optional import of RF PhaseNoise object*
         self.RFnoise = PhaseNoise
-        if (self.RFnoise != None and 
-            (len(self.RFnoise.dphi) != Ring.n_turns + 1)):
-            #PhaseNoiseError
-            raise RuntimeError('Phase noise has to have a length of n_turns + 1')
-        
-        #: | *Optional import of amplitude-scaling feedback object LHCNoiseFB*       
+        if (self.RFnoise is not None
+                and (len(self.RFnoise.dphi) != Ring.n_turns + 1)):
+            # PhaseNoiseError
+            raise RuntimeError(
+                'Phase noise has to have a length of n_turns + 1')
+
+        #: | *Optional import of amplitude-scaling feedback object LHCNoiseFB*
         self.noiseFB = LHCNoiseFB
-        
-        
-    
+
     def track(self):
         '''
-        Calculate PL correction on main RF frequency depending on machine.
-        Update the RF phase and frequency of the next turn for all systems.
-        '''    
-        
-        # Calculate PL correction on RF frequency    
+        Calculate PL correction on main RF frequency depending on machine and
+        propagate it to other RF systems.
+        The update of the RF phase and frequency for the next turn,
+        for all systems is done in the tracker.
+        '''
+
+        # Calculate PL correction on RF frequency
         getattr(self, self.machine)()
 
         # Update the RF frequency of all systems for the next turn
         counter = self.rf_station.counter[0] + 1
-        self.rf_station.omega_rf[:,counter] += self.domega_rf* \
-            self.rf_station.harmonic[:,counter]/self.rf_station.harmonic[0,counter]  
-
-        # Update the RF phase of all systems for the next turn
-        # Accumulated phase offset due to PL in each RF system
-        self.rf_station.dphi_rf += 2.*np.pi*self.rf_station.harmonic[:,counter]* \
-            (self.rf_station.omega_rf[:,counter] - 
-             self.rf_station.omega_rf_d[:,counter])/ \
-             self.rf_station.omega_rf_d[:,counter] 
-        
-        # Total phase offset
-        self.rf_station.phi_rf[:,counter] += self.rf_station.dphi_rf
-        
+        self.rf_station.omega_rf[:, counter] += self.domega_rf * \
+            self.rf_station.harmonic[:, counter] / \
+            self.rf_station.harmonic[0, counter]
 
     def precalculate_time(self, Ring):
         '''
         *For machines like the PSB, where the PL acts only in certain time
         intervals, pre-calculate on which turns to act.*
-        '''    
-        
+        '''
+
         if self.dt > 0:
             n = self.delay + 1
-            while n < Ring.t_rev.size: 
+            while n < Ring.t_rev.size:
                 summa = 0
                 while summa < self.dt:
                     try:
                         summa += Ring.t_rev[n]
                         n += 1
                     except:
                         self.on_time = np.append(self.on_time, 0)
-                        return 
+                        return
                 self.on_time = np.append(self.on_time, n-1)
         else:
             self.on_time = np.arange(Ring.t_rev.size)
-        
-        
 
     def beam_phase(self):
         '''
         *Beam phase measured at the main RF frequency and phase. The beam is 
         convolved with the window function of the band-pass filter of the 
         machine. The coefficients of sine and cosine components determine the 
         beam phase, projected to the range -Pi/2 to 3/2 Pi. Note that this beam
         phase is already w.r.t. the instantaneous RF phase.*
-        '''    
-        
+        '''
+
         # Main RF frequency at the present turn
-        omega_rf = self.rf_station.omega_rf[0,self.rf_station.counter[0]]
-        phi_rf = self.rf_station.phi_rf[0,self.rf_station.counter[0]]
-        
+        omega_rf = self.rf_station.omega_rf[0, self.rf_station.counter[0]]
+        phi_rf = self.rf_station.phi_rf[0, self.rf_station.counter[0]]
+
         if self.time_offset is None:
-            indexes = np.ones(self.profile.n_slices, dtype=bool)
-            time_offset = 0.0
+            # indexes = np.ones(self.profile.n_slices, dtype=bool)
+            # time_offset = 0.0
+            coeff = bm.beam_phase(self.profile.bin_centers,
+                                  self.profile.n_macroparticles,
+                                  self.alpha, omega_rf, phi_rf,
+                                  self.profile.bin_size)
         else:
             indexes = self.profile.bin_centers >= self.time_offset
             time_offset = self.time_offset
-        
-        # Convolve with window function
-        scoeff = np.trapz( np.exp(self.alpha*(self.profile.bin_centers[indexes]
-                                                - time_offset)) \
-                           *np.sin(omega_rf*self.profile.bin_centers[indexes]\
-                                   + phi_rf) \
-                           *self.profile.n_macroparticles[indexes],
-                           dx=self.profile.bin_size )
-        ccoeff = np.trapz( np.exp(self.alpha*(self.profile.bin_centers[indexes]
-                                                - time_offset)) \
-                           *np.cos(omega_rf*self.profile.bin_centers[indexes]\
-                                   + phi_rf) \
-                           *self.profile.n_macroparticles[indexes],
-                           dx=self.profile.bin_size )
+            coeff = bm.beam_phase(self.profile.bin_centers[indexes],
+                              self.profile.n_macroparticles[indexes],
+                                  self.alpha, omega_rf, phi_rf,
+                                  self.profile.bin_size)
+            # exp = bm.exp(self.alpha*(self.profile.bin_centers[indexes] -
+            #                          time_offset))
+            # # Convolve with window function
+            # scoeff = bm.trapz(exp *
+            #                   bm.sin(omega_rf*self.profile.bin_centers[indexes] +
+            #                          phi_rf) *
+            #                   self.profile.n_macroparticles[indexes],
+            #                   dx=self.profile.bin_size)
+            # ccoeff = bm.trapz(exp *
+            #                   bm.cos(omega_rf*self.profile.bin_centers[indexes] +
+            #                          phi_rf) *
+            #                   self.profile.n_macroparticles[indexes],
+            #                   dx=self.profile.bin_size)
+            # # needed to make sure the result is scalar and not 0-dim array
+            # coeff = float(scoeff/ccoeff)
 
         # Project beam phase to (pi/2,3pi/2) range
-        self.phi_beam = np.arctan(scoeff/ccoeff) + np.pi
-        
+        self.phi_beam = np.arctan(coeff) + np.pi
+
     def beam_phase_sharpWindow(self):
         '''
-        *Beam phase measured at the main RF frequency and phase. The beam is 
+        *Beam phase measured at the main RF frequency and phase. The beam is
         averaged over a window. The coefficients of sine and cosine components
-        determine the 
-        beam phase, projected to the range -Pi/2 to 3/2 Pi. Note that this beam
-        phase is already w.r.t. the instantaneous RF phase.*
-        '''    
-        
+        determine the beam phase, projected to the range -Pi/2 to 3/2 Pi.
+        Note that this beam phase is already w.r.t. the instantaneous RF phase.*
+        '''
+
         # Main RF frequency at the present turn
-        omega_rf = self.rf_station.omega_rf[0,self.rf_station.counter[0]]
-        phi_rf = self.rf_station.phi_rf[0,self.rf_station.counter[0]]
-        
+        turn = self.rf_station.counter[0]
+        omega_rf = self.rf_station.omega_rf[0, turn]
+        phi_rf = self.rf_station.phi_rf[0, turn]
+
         if self.alpha != 0.0:
-            left_boundary = self.profile.bin_centers \
-                >= self.time_offset - np.pi/omega_rf
-            right_boundary = self.profile.bin_centers \
-                <= -1/self.alpha + self.time_offset - 2*np.pi/omega_rf
-            indexes = left_boundary * right_boundary
+            indexes = bm.logical_and((self.time_offset - np.pi / omega_rf)
+                                     <= self.profile.bin_centers,
+                                     self.profile.bin_centers
+                                     <= (-1/self.alpha + self.time_offset -
+                                         2 * np.pi / omega_rf))
         else:
-            indexes = np.ones(self.profile.n_slices, dtype=bool)
-        
+            indexes = bm.ones(self.profile.n_slices, dtype=bool)
+
         # Convolve with window function
-        scoeff = np.trapz( np.sin(omega_rf*self.profile.bin_centers[indexes]\
-                                   + phi_rf) \
-                           *self.profile.n_macroparticles[indexes],
-                           dx=self.profile.bin_size )
-        ccoeff = np.trapz( np.cos(omega_rf*self.profile.bin_centers[indexes]\
-                                   + phi_rf) \
-                           *self.profile.n_macroparticles[indexes],
-                           dx=self.profile.bin_size )
+        scoeff = bm.trapz(bm.sin(omega_rf*self.profile.bin_centers[indexes]
+                                 + phi_rf)
+                          * self.profile.n_macroparticles[indexes],
+                          dx=self.profile.bin_size)
+        ccoeff = bm.trapz(bm.cos(omega_rf*self.profile.bin_centers[indexes]
+                                 + phi_rf) *
+                          self.profile.n_macroparticles[indexes],
+                          dx=self.profile.bin_size)
 
         # Project beam phase to (pi/2,3pi/2) range
         self.phi_beam = np.arctan(scoeff/ccoeff) + np.pi
 
-
-    def phase_difference(self):               
+    def phase_difference(self):
         '''
         *Phase difference between beam and RF phase of the main RF system.
         Optional: add RF phase noise through dphi directly.*
-        '''    
-        
+        '''
+
         # Correct for design stable phase
         counter = self.rf_station.counter[0]
         self.dphi = self.phi_beam - self.rf_station.phi_s[counter]
-        
+
         # Possibility to add RF phase noise through the PL
-        if self.RFnoise != None:
-            if self.noiseFB != None:
+        if self.RFnoise is not None:
+            if self.noiseFB is not None:
                 self.dphi += self.noiseFB.x*self.RFnoise.dphi[counter]
             else:
                 if self.machine == 'PSB':
                     self.dphi = self.dphi
                 else:
                     self.dphi += self.RFnoise.dphi[counter]
-                
-                
-    def radial_difference(self):               
+
+    def radial_difference(self):
         '''
         *Radial difference between beam and design orbit.*
-        '''    
-        
+        '''
+
         counter = self.rf_station.counter[0]
-        
+
         # Correct for design orbit
 #        self.average_dE = np.mean(self.profile.Beam.dE[(self.profile.Beam.dt >
 #            self.profile.bin_centers[0])*(self.profile.Beam.dt <
 #                                         self.profile.bin_centers[-1])])
-        self.average_dE = np.mean(self.profile.Beam.dE)
-        
-        self.drho = self.ring.alpha_0[0,counter]* \
-            self.ring.ring_radius*self.average_dE/ \
-            (self.ring.beta[0,counter]**2.* \
-             self.ring.energy[0,counter])
-    
-    
-    def radial_steering_from_freq(self):               
+        self.average_dE = bm.mean(self.profile.Beam.dE[::self.sample_dE])
+
+        self.drho = self.ring.alpha_0[0, counter] * \
+            self.ring.ring_radius*self.average_dE / \
+            (self.ring.beta[0, counter]**2.
+             * self.ring.energy[0, counter])
+
+    def radial_steering_from_freq(self):
         '''
         *Frequency and phase change for the current turn due to the radial steering program.*
-        '''    
-        
+        '''
+
         counter = self.rf_station.counter[0]
-        
-        self.radial_steering_domega_rf = - self.rf_station.omega_rf_d[0,counter]* \
-            self.rf_station.eta_0[counter]/self.ring.alpha_0[0,counter]* \
+
+        self.radial_steering_domega_rf = - self.rf_station.omega_rf_d[0, counter] * \
+            self.rf_station.eta_0[counter]/self.ring.alpha_0[0, counter] * \
             self.reference/self.ring.ring_radius
-        
-        self.rf_station.omega_rf[:,counter] += self.radial_steering_domega_rf* \
-                                self.rf_station.harmonic[:,counter]/ \
-                                self.rf_station.harmonic[0,counter]  
+
+        self.rf_station.omega_rf[:, counter] += self.radial_steering_domega_rf * \
+            self.rf_station.harmonic[:, counter] / \
+            self.rf_station.harmonic[0, counter]
 
         # Update the RF phase of all systems for the next turn
         # Accumulated phase offset due to PL in each RF system
-        self.rf_station.dphi_rf_steering += 2.*np.pi*self.rf_station.harmonic[:,counter]* \
-            (self.rf_station.omega_rf[:,counter] - 
-             self.rf_station.omega_rf_d[:,counter])/ \
-             self.rf_station.omega_rf_d[:,counter] 
-               
+        self.rf_station.dphi_rf_steering += 2.*np.pi*self.rf_station.harmonic[:, counter] * \
+            (self.rf_station.omega_rf[:, counter] -
+             self.rf_station.omega_rf_d[:, counter]) / \
+            self.rf_station.omega_rf_d[:, counter]
+
         # Total phase offset
-        self.rf_station.phi_rf[:,counter] += self.rf_station.dphi_rf_steering
-                
+        self.rf_station.phi_rf[:, counter] += self.rf_station.dphi_rf_steering
 
     def LHC_F(self):
         '''
         Calculation of the LHC RF frequency correction from the phase difference
         between beam and RF (actual synchronous phase). The transfer function is
-        
+
         .. math::
             \\Delta \\omega_{rf}^{PL} = - g_{PL} (\\Delta\\varphi_{PL} + \\phi_{N}) 
-            
+
         where the phase noise for the controlled blow-up can be optionally 
         activated.  
         Using 'gain2', a frequency loop can be activated in addition to remove
         long-term frequency drifts:
-        
+
         .. math::
             \\Delta \\omega_{rf}^{FL} = - g_{FL} (\\omega_{rf} - h \\omega_{0})    
         '''
-        
+
         counter = self.rf_station.counter[0]
-        
+
         self.beam_phase()
         self.phase_difference()
-        
+
         # Frequency correction from phase loop and frequency loop
         self.domega_rf = - self.gain*self.dphi \
-            - self.gain2*(self.rf_station.omega_rf[0,counter] 
-               - self.rf_station.omega_rf_d[0,counter]
-               + self.reference) 
-            
-    
+            - self.gain2*(self.rf_station.omega_rf[0, counter] -
+               self.rf_station.omega_rf_d[0, counter] +
+                          self.reference)
+
     def SPS_F(self):
         '''
         Calculation of the SPS RF frequency correction from the phase
         difference between beam and RF (actual synchronous phase). Same as 
         LHC_F, except the calculation of the beam phase.
         '''
-        
+
         counter = self.rf_station.counter[0]
-                    
+
         self.beam_phase_sharpWindow()
         self.phase_difference()
-        
+
         # Frequency correction from phase loop and frequency loop
         self.domega_dphi = - self.gain * self.dphi
-        self.domega_df = - self.gain2*(self.rf_station.omega_rf[0,counter] 
-               - self.rf_station.omega_rf_d[0,counter])
-        
+        self.domega_df = - self.gain2*(self.rf_station.omega_rf[0, counter] -
+                                       self.rf_station.omega_rf_d[0, counter])
+
         self.domega_rf = self.domega_dphi + self.domega_df
-        
+
     def SPS_RL(self):
         '''
         Calculation of the SPS RF frequency correction from the phase difference
         between beam and RF (actual synchronous phase). The transfer function is
-        
+
         .. math::
             \\Delta \\omega_{rf}^{PL} = - g_{PL} (\\Delta\\varphi_{PL} + \\phi_{N}) 
-            
+
         where the phase noise for the controlled blow-up can be optionally 
         activated.  
         Using 'gain2', a radial loop can be activated in addition to remove
         long-term frequency drifts
         '''
-        
+
         counter = self.rf_station.counter[0]
-        
+
         if self.reference != 0:
             self.radial_steering_from_freq()
-            
+
         self.beam_phase()
         self.phase_difference()
         self.radial_difference()
-        
+
         # Frequency correction from phase loop and radial loop
         self.domega_dphi = - self.gain * self.dphi
-        self.domega_dR = - np.sign(self.rf_station.eta_0[counter])*self.gain2* \
+        self.domega_dR = - bm.sign(self.rf_station.eta_0[counter])*self.gain2 * \
             (self.reference - self.drho) / self.ring.ring_radius
-        
-        self.domega_rf = self.domega_dphi + self.domega_dR
-
 
+        self.domega_rf = self.domega_dphi + self.domega_dR
 
     def LHC(self):
         '''
         Calculation of the LHC RF frequency correction from the phase difference
         between beam and RF (actual synchronous phase). The transfer function is
-        
+
         .. math::
             \\Delta \\omega_{rf}^{PL} = - g_{PL} (\\Delta\\varphi_{PL} + \\phi_{N}) 
-            
+
         where the phase noise for the controlled blow-up can be optionally 
         activated.  
         Using 'gain2', a synchro loop can be activated in addition to remove
         long-term frequency drifts:     
-        
+
         .. math::
             \\Delta \\omega_{rf}^{SL} = - g_{SL} (y + a \\Delta\\varphi_{rf}) ,
-            
+
         where we use the recursion
-        
+
         .. math::
             y_{n+1} = (1 - \\tau) y_n + (1 - a) \\tau \\Delta\\varphi_{rf} ,
-            
+
         with a and \tau being defined through the synchrotron frequency f_s and
         the synchrotron tune Q_s as
-        
+
         .. math::
             a (f_s) \\equiv 5.25 - \\frac{f_s}{\\pi 40~\\text{Hz}} ,
-            
+
         .. math::
             \\tau(f_s) \\equiv 2 \\pi Q_s \\sqrt{ \\frac{a}{1 + \\frac{g_{PL}}{g_{SL}} \\sqrt{\\frac{1 + 1/a}{1 + a}} }}
         '''
-        
+
         counter = self.rf_station.counter[0]
         dphi_rf = self.rf_station.dphi_rf[0]
-        
+
         self.beam_phase()
         self.phase_difference()
-        
+
         # Frequency correction from phase loop and synchro loop
         self.domega_rf = - self.gain*self.dphi \
-                         - self.gain2*(self.lhc_y + self.lhc_a[counter]*
-                                       (dphi_rf + self.reference)) 
+                         - self.gain2*(self.lhc_y + self.lhc_a[counter]
+                                       * (dphi_rf + self.reference))
 
         # Update recursion variable
         self.lhc_y = (1 - self.lhc_t[counter])*self.lhc_y + \
-                     (1 - self.lhc_a[counter])*self.lhc_t[counter]* \
+                     (1 - self.lhc_a[counter])*self.lhc_t[counter] * \
                      (dphi_rf + self.reference)
 
-
     def PSB(self):
         '''
         Phase and radial loops for PSB. See documentation on-line for details.
         '''
 
         # Average phase error while frequency is updated
         counter = self.rf_station.counter[0]
         self.beam_phase()
         self.phase_difference()
-        
-        
+
         self.dphi_sum += self.dphi
 
         # Phase and radial loop active on certain turns
-        if counter == self.on_time[self.PL_counter] and counter>=self.delay:
-            #Phase loop
-            self.dphi_av = self.dphi_sum / (self.on_time[self.PL_counter] 
-                             - self.on_time[self.PL_counter-1])
-            
+        if counter == self.on_time[self.PL_counter] and counter >= self.delay:
+            # Phase loop
+            self.dphi_av = self.dphi_sum / (self.on_time[self.PL_counter]
+                                            - self.on_time[self.PL_counter-1])
+
             if self.RFnoise != None:
                 self.dphi_av += self.RFnoise.dphi[counter]
-                
+
             self.domega_PL = 0.99803799*self.domega_PL \
-                + self.gain[counter]*(0.99901903*self.dphi_av - 0.99901003*self.dphi_av_prev)
-                    
+                + self.gain[counter]*(0.99901903*self.dphi_av -
+                                      0.99901003*self.dphi_av_prev)
+
             self.dphi_av_prev = self.dphi_av
             self.dphi_sum = 0.
-            
-            #Radial loop    
-            self.dR_over_R = (self.rf_station.omega_rf[0,counter] - 
-                         self.rf_station.omega_rf_d[0,counter])/(
-                         self.rf_station.omega_rf_d[0,counter] * 
-                         (1./(self.ring.alpha_0[0,counter]*
+
+            # Radial loop
+            self.dR_over_R = (self.rf_station.omega_rf[0, counter] -
+                              self.rf_station.omega_rf_d[0, counter])/(
+                self.rf_station.omega_rf_d[0, counter] *
+                         (1./(self.ring.alpha_0[0, counter] *
                               self.rf_station.gamma[counter]**2) - 1.))
-            
-            self.domega_RL = self.domega_RL + self.gain2[0][counter]*(self.dR_over_R - 
-                self.dR_over_R_prev) + self.gain2[1][counter]*self.dR_over_R
-            
+
+            self.domega_RL = self.domega_RL + self.gain2[0][counter]*(self.dR_over_R
+                                                                      - self.dR_over_R_prev) + self.gain2[1][counter]*self.dR_over_R
+
             self.dR_over_R_prev = self.dR_over_R
-                
+
             # Counter to pick the next time step when the PL & RL will be active
-            self.PL_counter += 1 
-            
+            self.PL_counter += 1
+
         # Apply frequency correction
         self.domega_rf = - self.domega_PL - self.domega_RL
+
+    def to_gpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays to the GPU
+        '''
+        # Check if to_gpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'GPU':
+            return
+
+        assert bm.device == 'GPU'
+        # No arrays need to be transfered
+
+        # to make sure it will not be called again
+        self._device = 'GPU'
+
+    def to_cpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays back to the CPU
+        '''
+        # Check if to_cpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'CPU':
+            return
+
+        assert bm.device == 'CPU'
+        # No arrays need to be transfered
+
+        # to make sure it will not be called again
+        self._device = 'CPU'
```

### Comparing `blond-2.0.11/blond/llrf/cavity_feedback.py` & `blond-2.0.12/blond/trackers/tracker.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,680 +3,588 @@
 # terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
 # In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
-'''
-**Various cavity loops for the CERN machines**
+"""
+**Module containing all the elements to track the RF frequency, voltage, phase,
+and the beam coordinates in phase space.**
 
-:Authors: **Helga Timko**
-'''
+:Authors:  **Helga Timko**, **Alexandre Lasheen**, **Danilo Quartullo**
+"""
 
 from __future__ import division
-import logging
+from builtins import range, object
 import numpy as np
-import scipy
-from matplotlib import pyplot as plt
-from scipy.constants import e
-
-from ..llrf.signal_processing import comb_filter, cartesian_to_polar, \
-    polar_to_cartesian, modulator, moving_average, rf_beam_current
-from ..llrf.impulse_response import SPS4Section200MHzTWC, SPS5Section200MHzTWC
+from scipy.integrate import cumtrapz
+import ctypes
+# import logging
+import warnings
 from ..utils import bmath as bm
-from ..beam.profile import Profile, CutOptions
-
-class CavityFeedbackCommissioning(object):
-
-    def __init__(self, debug=False, open_loop=False, open_FB=False,
-                 open_drive=False):
-
-        self.debug = bool(debug)
-        # Multiply with zeros if open == True
-        self.open_loop = int(np.invert(bool(open_loop)))
-        self.open_FB = int(np.invert(bool(open_FB)))
-        self.open_drive = int(np.invert(bool(open_drive)))
-
-
-class SPSCavityFeedback(object):
-    """Class determining the turn-by-turn total RF voltage and phase correction
-    originating from the individual cavity feedbacks. Assumes two 4-section and
-    two 5-section travelling wave cavities and a voltage partition proportional
-    to the number of sections.
-
-    Parameters
-    ----------
-    RFStation : class
-        An RFStation type class
-    Beam : class
-        A Beam type class
-    Profile : class
-        A Profile type class
-    G_llrf : float or list
-        LLRF Gain [1]; if passed as a float, both 4- and 5-section cavities
-        have the same G_llrf; if passed as a list, the first and second
-        elements correspond to the G_llrf of the 4- and 5-section cavity
-        feedback; default is 10
-    G_tx : float or list
-        Transmitter gain [1] of the cavity feedback; convention same as G_llrf;
-        default is 0.5
-    open_loop : int(bool)
-        Open (0) or closed (1) feedback loop; default is 1
-
-    Attributes
-    ----------
-    OTFB_4 : class
-        An SPSOneTurnFeedback type class
-    OTFB_5 : class
-        An SPSOneTurnFeedback type class
-    V_sum : complex array
-        Vector sum of RF voltage from all the cavities
-    V_corr : float array
-        RF voltage correction array to be applied in the tracker
-    phi_corr : float array
-        RF phase correction array to be applied in the tracker
-    logger : logger
-        Logger of the present class
 
+class FullRingAndRF(object):
+    """
+    *Definition of the full ring and RF parameters in order to be able to have
+    a full turn information (used in the hamiltonian for example).*
     """
 
-    def __init__(self, RFStation, Beam, Profile, G_llrf=10, G_tx=0.5,
-                 a_comb=15/16, turns=1000,
-                 Commissioning=CavityFeedbackCommissioning()):
-
-        # Options for commissioning the feedback
-        self.Commissioning = Commissioning
-
-        self.rf = RFStation
-
-        # Parse input for G_llrf
-        if type(G_llrf) is list:
-            G_llrf_4 = G_llrf[0]
-            G_llrf_5 = G_llrf[1]
-        else:
-            G_llrf_4 = G_llrf
-            G_llrf_5 = G_llrf
-
-        if type(G_tx) is list:
-            G_tx_4 = G_tx[0]
-            G_tx_5 = G_tx[1]
-        else:
-            G_tx_4 = G_tx
-            G_tx_5 = G_tx
+    def __init__(self, RingAndRFSection_list):
 
-        # Voltage partition proportional to the number of sections
-        self.OTFB_4 = SPSOneTurnFeedback(RFStation, Beam, Profile, 4,
-                                         n_cavities=2, V_part=4/9,
-                                         G_llrf=float(G_llrf_4),
-                                         G_tx=float(G_tx_4),
-                                         a_comb=float(a_comb),
-                                         Commissioning=self.Commissioning)
-        self.OTFB_5 = SPSOneTurnFeedback(RFStation, Beam, Profile, 5,
-                                         n_cavities=2, V_part=5/9,
-                                         G_llrf=float(G_llrf_5),
-                                         G_tx=float(G_tx_5),
-                                         a_comb=float(a_comb),
-                                         Commissioning=self.Commissioning)
+        #: *List of the total RingAndRFSection objects*
+        self.RingAndRFSection_list = RingAndRFSection_list
 
-        # Set up logging
-        self.logger = logging.getLogger(__class__.__name__)
-        self.logger.info("Class initialized")
+        #: *Total potential well in [V]*
+        self.potential_well = 0
 
-        # Initialise OTFB without beam
-        self.turns = int(turns)
-        if turns < 1:
-            #FeedbackError
-            raise RuntimeError("ERROR in SPSCavityFeedback: 'turns' has to" +
-                               " be a positive integer!")
-        self.track_init(debug=Commissioning.debug)
+        #: *Total potential well theta coordinates in [rad]*
+        self.potential_well_coordinates = 0
+
+        #: *Ring circumference in [m]*
+        self.ring_circumference = 0
+        for RingAndRFSectionElement in self.RingAndRFSection_list:
+            self.ring_circumference += RingAndRFSectionElement.section_length
+
+        #: *Ring radius in [m]*
+        self.ring_radius = self.ring_circumference / (2*np.pi)
+
+    def potential_well_generation(self, turn=0, n_points=int(1e5),
+                                  main_harmonic_option='lowest_freq',
+                                  dt_margin_percent=0., time_array=None):
+        """Method to generate the potential well out of the RF systems. The
+        assumption made is that all the RF voltages are averaged over one turn.
+        The potential well is then approximated over one turn, which is not the
+        exact potential. This approximation should be fine enough to generate a
+        bunch (the mismatch should be small and damped fast enough). The
+        default main harmonic is defined to be the lowest one in frequency. The
+        user can change this option if it is not the case for his simulations
+        (other options are: 'highest_voltage', or inputing directly the value
+        of the desired main harmonic). A margin on the time array can be
+        applied in order to be able to see the min/max that might be exactly on
+        the edges of the frame (by adding a % to the length of the frame, this
+        is set to 0 by default. It assumes also that the slippage factor is the
+        same in the whole ring.
+        """
 
-    def track(self):
+        voltages = np.array([])
+        omega_rf = np.array([])
+        phi_offsets = np.array([])
+
+        for RingAndRFSectionElement in self.RingAndRFSection_list:
+            RF_params = RingAndRFSectionElement.rf_params
+            charge = RF_params.Particle.charge
+            for rf_system in range(RF_params.n_rf):
+                voltages = np.append(voltages,
+                                     RF_params.voltage[rf_system, turn])
+                omega_rf = np.append(omega_rf,
+                                     RF_params.omega_rf[rf_system, turn])
+                phi_offsets = np.append(phi_offsets,
+                                        RF_params.phi_rf[rf_system, turn])
+
+        voltages = np.array(voltages, ndmin=2)
+        omega_rf = np.array(omega_rf, ndmin=2)
+        phi_offsets = np.array(phi_offsets, ndmin=2)
+
+        if main_harmonic_option == 'lowest_freq':
+            main_omega_rf = np.min(omega_rf)
+        elif main_harmonic_option == 'highest_voltage':
+            main_omega_rf = np.min(omega_rf[voltages == np.max(voltages)])
+        elif isinstance(main_harmonic_option, int) or \
+                isinstance(main_harmonic_option, float):
+            if omega_rf[omega_rf == main_harmonic_option].size == 0:
+                # PotentialWellError
+                raise RuntimeError("ERROR in FullRingAndRF: The desired" +
+                                   " harmonic to compute the potential well does not match" +
+                                   " the RF parameters...")
+            main_omega_rf = np.min(omega_rf[omega_rf == main_harmonic_option])
+
+        slippage_factor = self.RingAndRFSection_list[0].rf_params.eta_0[turn]
+
+        if time_array is None:
+            time_array_margin = dt_margin_percent*2*np.pi/main_omega_rf
+
+            first_dt = - time_array_margin/2
+            last_dt = 2*np.pi/main_omega_rf + time_array_margin/2
+
+            time_array = np.linspace(float(first_dt), float(last_dt), int(n_points))
+
+        self.total_voltage = np.sum(voltages.T *
+                                    np.sin(omega_rf.T*time_array + phi_offsets.T), axis=0)
+
+        eom_factor_potential = np.sign(slippage_factor)*charge / \
+            (RingAndRFSectionElement.rf_params.t_rev[turn])
+
+        potential_well = - cumtrapz(eom_factor_potential*(self.total_voltage -
+                                                          (- RingAndRFSectionElement.acceleration_kick[turn])/abs(charge)),
+                                    dx=time_array[1] - time_array[0], initial=0)
+        potential_well = potential_well - np.min(potential_well)
 
-        self.OTFB_4.track()
-        self.OTFB_5.track()
+        self.potential_well_coordinates = time_array
+        self.potential_well = potential_well
 
-        self.V_sum = self.OTFB_4.V_fine_tot + self.OTFB_5.V_fine_tot
+    def track(self):
+        """Function to loop over all the RingAndRFSection.track methods
+        """
 
-        self.V_corr, alpha_sum = cartesian_to_polar(self.V_sum)
+        for RingAndRFSectionElement in self.RingAndRFSection_list:
+            RingAndRFSectionElement.track()
 
-        # Calculate OTFB correction w.r.t. RF voltage and phase in RFStation
-        self.V_corr /= self.rf.voltage[0, self.rf.counter[0]]
-        self.phi_corr = 0.5*np.pi - alpha_sum \
-            - self.rf.phi_rf[0, self.rf.counter[0]]
 
-    def track_init(self, debug=False):
-        r''' Tracking of the SPSCavityFeedback without beam.
-        '''
-        
-        if debug:
-            cmap = plt.get_cmap('jet')
-            colors = cmap(np.linspace(0,1, self.turns))
-            plt.figure('voltage')
-            plt.clf()
-            plt.grid()
-
-        for i in range(self.turns):
-            #            print('OTFB pre-tracking iteration ', i)
-            self.logger.debug("Pre-tracking w/o beam, iteration %d", i)
-            self.OTFB_4.track_no_beam()
-            if debug:
-                plt.plot(self.OTFB_4.profile.bin_centers*1e6,
-                         np.abs(self.OTFB_4.V_fine_tot), color=colors[i])
-                plt.plot(self.OTFB_4.rf_centers*1e6,
-                         np.abs(self.OTFB_4.V_coarse_tot), color=colors[i],
-                         linestyle='', marker='.')
-            self.OTFB_5.track_no_beam()
-
-        # Interpolate from the coarse mesh to the fine mesh of the beam
-        self.V_sum = np.interp(
-            self.OTFB_4.profile.bin_centers, self.OTFB_4.rf_centers,
-            self.OTFB_4.V_coarse_ind_gen + self.OTFB_5.V_coarse_ind_gen)
-
-        self.V_corr, alpha_sum = cartesian_to_polar(self.V_sum)
-
-        # Calculate OTFB correction w.r.t. RF voltage and phase in RFStation
-        self.V_corr /= self.rf.voltage[0, self.rf.counter[0]]
-        self.phi_corr = 0.5*np.pi - alpha_sum \
-            - self.rf.phi_rf[0, self.rf.counter[0]]
-
-
-class SPSOneTurnFeedback(object):
-
-    r'''Voltage feedback around a travelling wave cavity with given amount of
-    sections. The quantities of the LLRF system cover one turn with a coarse
-    resolution.
+class RingAndRFTracker(object):
+    r""" Class taking care of basic particle coordinate tracking for a given
+    RF station and the part of the ring until the next station, see figure.
+
+    .. image:: ring_and_RFstation.png
+        :align: center
+        :width: 600
+        :height: 600
+
+    The time step is fixed to be one turn, but the tracking can consist of
+    multiple RingAndRFTracker objects. In this case, the user should make sure
+    that the lengths of the stations sum up exactly to the circumference or use
+    the FullRingAndRF object in order to let the code pre-process the
+    parameters. Each RF station may contain several RF harmonic systems which
+    are considered to be in the same location. First, the energy kick of the RF
+    station is applied, and then the particle arrival time to the next station
+    is updated. The change in RF phase, voltage, and frequency due to control
+    loops is tracked as well.
 
     Parameters
     ----------
     RFStation : class
-        An RFStation type class
+        A RFStation type class
+    counter : [int]
+        Inherited from
+        :py:attr:`input_parameters.rf_parameters.RFStation.counter`
+    length_ratio : float
+        Inherited from
+        :py:attr:`input_parameters.ring.Ring.length_ratio`
+    section_length : float
+        Inherited from
+        :py:attr:`input_parameters.ring.Ring.section_length`
+    t_rev : float
+        Inherited from
+        :py:attr:`input_parameters.ring.Ring.t_rev`
+    n_rf : float
+        Inherited from
+        :py:attr:`input_parameters.rf_parameters.RFStation.n_rf`
+    beta : float
+        Inherited from
+        :py:attr:`input_parameters.ring.Ring.beta`
+    charge : float
+        Inherited from
+        :py:attr:`input_parameters.ring.Ring.Particle.charge`
+    harmonic : float array
+        Inherited from
+        :py:attr:`input_parameters.rf_parameters.RFStation.harmonic`
+    voltage : float array
+        Inherited from
+        :py:attr:`input_parameters.rf_parameters.RFStation.voltage`
+    phi_noise : float array
+        Inherited from
+        :py:attr:`input_parameters.rf_parameters.RFStation.phi_noise`
+    phi_modulation : 2-tuple of float array
+        Inherited from
+        :py:attr:`input_parameters.rf_parameters.RFStation.phi_modulation`
+    phi_rf : float array
+        Inherited from
+        :py:attr:`input_parameters.rf_parameters.RFStation.phi_rf`
+    phi_s : float array
+        Inherited from
+        :py:attr:`input_parameters.rf_parameters.RFStation.phi_s`
+    alpha_0 : float array
+        Inherited from
+        :py:attr:`input_parameters.ring.Ring.alpha_0`
+    alpha_1 : float array
+        Inherited from
+        :py:attr:`input_parameters.ring.Ring.alpha_1`
+    alpha_2 : float array
+        Inherited from
+        :py:attr:`input_parameters.ring.Ring.alpha_2`
+    eta_0 : float array
+        Inherited from
+        :py:attr:`input_parameters.ring.Ring.eta_0`
+    eta_1 : float array
+        Inherited from
+        :py:attr:`input_parameters.ring.Ring.eta_1`
+    eta_2 : float array
+        Inherited from
+        :py:attr:`input_parameters.ring.Ring.eta_2`
+    alpha_order : float array
+        Inherited from
+        :py:attr:`input_parameters.ring.Ring.alpha_order`
+    acceleration_kick : float array
+        Inherited from
+        :py:attr:`input_parameters.ring.Ring.delta_E`
+        and multiplied by -1
     Beam : class
         A Beam type class
-    Profile : class
-        Beam profile object
-    n_sections : int
-        Number of sections in the cavities
-    n_cavities : int
-        Number of cavities of the same type
-    V_part : float
-        Voltage partition for the given n_cavities; in range (0,1)
-    G_tx : float
-        Transmitter gain [A/V]; default is :math:`(50 \Omega)^{-1}`
-    open_loop : int(bool)
-        Open (0) or closed (1) feedback loop; default is 1
+    solver : str
+        Type of solver used for the drift equation; use 'simple' for 1st order
+        approximation and 'exact' for exact solver
+    BeamFeedback : class (optional)
+        A BeamFeedback type class, beam-based feedback on RF frequency;
+        default is None
+    NoiseFeedback : class (optional)
+        A NoiseFeedback type class, bunch-length feedback on RF noise;
+        default is None
+    periodicity : bool (optional)
+        Option to switch periodic solver on/off; default is False (off)
+    interpolation : bool (optional)
+        Option to use sliced and interpolated voltage for the kicker; default
+        is False
 
-    Attributes
-    ----------
-    TWC : class
-        A TravellingWaveCavity type class
-    counter : int
-        Counter of the current time step
-    omega_c : float
-        Carrier revolution frequency [1/s] at the current time step
-    omega_r : const float
-        Resonant revolution frequency [1/s] of the travelling wave cavities
-    n_coarse : int
-        Number of bins for the coarse grid (equals harmonic number)
-    V_gen : complex array
-        Generator voltage [V] of the present turn in (I,Q) coordinates
-    V_gen_prev : complex array
-        Generator voltage [V] of the previous turn in (I,Q) coordinates
-    V_fine_ind_beam : complex array
-        Beam-induced voltage [V] in (I,Q) coordinates on the fine grid
-        used for tracking the beam
-    V_coarse_ind_beam : complex array
-        Beam-induced voltage [V] in (I,Q) coordinates on the coarse grid used
-        tracking the LLRF
-    V_coarse_ind_gen : complex array
-        Generator-induced voltage [V] in (I,Q) coordinates on the coarse grid
-        used tracking the LLRF
-    V_coarse_tot : complex array
-        Cavity voltage [V] at present turn in (I,Q) coordinates which is used
-        for tracking the LLRF
-    V_fine_tot : complex array
-        Cavity voltage [V] at present turn in (I,Q) coordinates which is used
-        for tracking the beam
-    a_comb : float
-        Recursion constant of the comb filter; :math:`a_{\mathsf{comb}}=15/16`
-    n_mov_av : const int
-        Number of points for moving average modelling cavity response;
-        :math:`n_{\mathsf{mov.av.}} = \frac{f_r}{f_{\mathsf{bw,cav}}}`, where
-        :math:`f_r` is the cavity resonant frequency of TWC_4 and TWC_5
-    logger : logger
-        Logger of the present class
-
-    '''
-
-    def __init__(self, RFStation, Beam, Profile_, n_sections, n_cavities=2,
-                 V_part=4/9, G_llrf=10, G_tx=0.5, a_comb=15/16,
-                 Commissioning=CavityFeedbackCommissioning()):
+    """
+
+    def __init__(self, RFStation, Beam, solver='simple', BeamFeedback=None,
+                 NoiseFeedback=None, CavityFeedback=None, periodicity=False,
+                 interpolation=False, Profile=None, TotalInducedVoltage=None):
 
         # Set up logging
-        self.logger = logging.getLogger(__class__.__name__)
+        # self.logger = logging.getLogger(__class__.__name__)
+        # self.logger.info("Class initialized")
 
-        # Commissioning options
-        self.open_loop = Commissioning.open_loop
-        self.logger.debug("Opening overall OTFB loop")
-        self.open_FB = Commissioning.open_FB
-        self.logger.debug("Opening feedback of drive correction")
-        self.open_drive = Commissioning.open_drive
-        self.logger.debug("Opening drive to generator")
+        # Imports from RF parameters
+        self.rf_params = RFStation
+        self.counter = RFStation.counter
+        self.length_ratio = RFStation.length_ratio
+        self.section_length = RFStation.section_length
+        # self.t_rev = RFStation.t_rev
+        # self.n_rf = RFStation.n_rf
+        # self.beta = RFStation.beta
+        # self.charge = RFStation.Particle.charge
+        # self.harmonic = RFStation.harmonic
+        # self.voltage = RFStation.voltage
+        # self.phi_noise = RFStation.phi_noise
+        # self.phi_modulation = RFStation.phi_modulation
+        # self.phi_rf = RFStation.phi_rf
+        # if not self.rf_params.empty:
+        #     self.phi_s = RFStation.phi_s
+        # self.omega_rf = RFStation.omega_rf
+        # self.alpha_0 = RFStation.alpha_0
+        # self.alpha_1 = RFStation.alpha_1
+        # self.alpha_2 = RFStation.alpha_2
+        # self.eta_0 = RFStation.eta_0
+        # self.eta_1 = RFStation.eta_1
+        # self.eta_2 = RFStation.eta_2
+        # self.alpha_order = RFStation.alpha_order
+        self.acceleration_kick = - RFStation.delta_E
 
-        # Read input
-        self.rf = RFStation
+        # Other imports
         self.beam = Beam
-        self.profile = Profile_
-        self.n_cavities = int(n_cavities)
-        if self.n_cavities < 1:
-            #FeedbackError
-            raise RuntimeError("ERROR in SPSOneTurnFeedback: argument" +
-                               " n_cavities has invalid value!")
-        self.V_part = float(V_part)
-        if self.V_part*(1 - self.V_part) < 0:
-            #FeedbackError
-            raise RuntimeError("ERROR in SPSOneTurnFeedback: V_part" +
-                               " should be in range (0,1)!")
-
-        # Gain settings
-        self.G_llrf = float(G_llrf)
-        self.G_tx = float(G_tx)
-
-        # 200 MHz travelling wave cavity (TWC) model
-        if n_sections in [4, 5]:
-            self.TWC = eval("SPS" + str(n_sections) + "Section200MHzTWC()")
-        else:
-            #FeedbackError
-            raise RuntimeError("ERROR in SPSOneTurnFeedback: argument" +
-                               " n_sections has invalid value!")
-        self.logger.debug("SPS OTFB cavities: %d, sections: %d, voltage" +
-                          " partition %.2f, gain: %.2e", self.n_cavities,
-                          n_sections, self.V_part, self.G_tx)
-
-        # TWC resonant frequency
-        self.omega_r = self.TWC.omega_r
-
-        # Initialise bunch-by-bunch voltage array with LENGTH OF PROFILE
-        self.V_fine_tot = np.zeros(self.profile.n_slices, dtype=complex)
-
-        # Length of arrays in LLRF
-        self.n_coarse = int(self.rf.harmonic[0, 0])
-
-        # Array to hold the bucket-by-bucket voltage with LENGTH OF LLRF
-        self.V_coarse_tot = np.zeros(self.n_coarse, dtype=complex)
-
-        # Centers of the RF-buckets
-        self.rf_centers = (np.arange(self.n_coarse) + 0.5) * self.rf.t_rf[0, 0]
-
-        # TODO: Bin size can change! Update affected variables!!
-        self.logger.debug("Length of arrays in generator path %d",
-                          self.n_coarse)
-
-        # Initialise comb filter
-        self.dV_gen_prev = np.zeros(self.n_coarse, dtype=complex)
-        self.a_comb = float(a_comb)
-
-        # Initialise cavity filter (moving average)
-        self.n_mov_av = int(self.TWC.tau/self.rf.t_rf[0, 0])
-        self.logger.debug("Moving average over %d points", self.n_mov_av)
-        # TODO: update condition for new n_mov_av
-        if self.n_mov_av < 2:
-            #FeedbackError
-            raise RuntimeError("ERROR in SPSOneTurnFeedback: profile has to" +
-                               " have at least 12.5 ns resolution!")
-        self.dV_mov_av_prev = np.zeros(self.n_coarse, dtype=complex)
-
-        # Initialise generator-induced voltage
-        self.I_gen_prev = np.zeros(self.n_mov_av, dtype=complex)
-
-        # Pre-compute factor for semi-analytic method
-        self.pre_compute_semi_analytic_factor(self.rf_centers)
+        self.solver = str(solver)
+        if self.solver not in ['simple', 'exact', 'legacy']:
+            # SolverError
+            raise RuntimeError("ERROR in RingAndRFTracker: Choice of" +
+                               " longitudinal solver not recognised!")
+        if self.rf_params.alpha_order > 1:  # Force exact solver for higher orders of eta
+            self.solver = 'exact'
+        self.solver = self.solver.encode(encoding='utf_8')
+
+        # Options
+        self.beamFB = BeamFeedback
+        self.noiseFB = NoiseFeedback
+        self.cavityFB = CavityFeedback
+        try:
+            self.periodicity = bool(periodicity)
+        except:
+            # PeriodicityError
+            raise RuntimeError("ERROR in RingAndRFTracker: Choice of" +
+                               " periodicity not recognised!")
+        try:
+            self.interpolation = bool(interpolation)
+        except:
+            # InterpolationError
+            raise RuntimeError("ERROR in RingAndRFTracker: Choice of" +
+                               " interpolation not recognised!")
+        self.profile = Profile
+        self.totalInducedVoltage = TotalInducedVoltage
+        if (self.interpolation is True) and (self.profile is None):
+            # ProfileError
+            raise RuntimeError("ERROR in RingAndRFTracker: Please specify a" +
+                               " Profile object to use the interpolation option")
+
+        if (self.cavityFB is not None) and (self.profile is None):
+            # ProfileError
+            raise RuntimeError("ERROR in RingAndRFTracker: Please specify a" +
+                               " Profile object to use the CavityFeedback class")
+        if (self.rf_params.empty is True) and (self.periodicity is True):
+            # PeriodicityError
+            raise RuntimeError("ERROR in RingAndRFTracker: Empty RFStation" +
+                               " with periodicity not yet implemented!")
+        if (self.cavityFB is not None) and (self.interpolation is False):
+            self.interpolation = True
+            warnings.warn('Setting interpolation to TRUE')
+            # self.logger.warning("Setting interpolation to TRUE")
+
+
+    def kick(self, beam_dt, beam_dE, index):
+        r"""Function updating the particle energy due to the RF kick in a given
+        RF station. The kicks are summed over the different harmonic RF systems
+        in the station. The cavity phase can be shifted by the user via
+        phi_offset. The main RF (harmonic[0]) has by definition phase = 0 at
+        time = 0 below transition. The phases of all other RF systems are
+        defined w.r.t.\ to the main RF. The increment in energy is given by the
+        discrete equation of motion:
 
-        self.logger.info("Class initialized")
-
-    def track(self):
-        """Turn-by-turn tracking method."""
+        .. math::
+            \Delta E^{n+1} = \Delta E^n + \sum_{k=0}^{n_{\mathsf{rf}}-1}{e V_k^n \\sin{\\left(\omega_{\mathsf{rf,k}}^n \\Delta t^n + \phi_{\mathsf{rf,k}}^n \\right)}} - (E_s^{n+1} - E_s^n)
 
-        # Present time step
-        self.counter = self.rf.counter[0]
-        # Present carrier frequency: main RF frequency
-        self.omega_c = self.rf.omega_rf[0, self.counter]
-        # Present delay time
-        self.n_delay = int((self.rf.t_rev[self.counter] - self.TWC.tau)
-                           / self.rf.t_rf[0, self.counter])
-
-        # Update the impulse response at present carrier frequency
-        self.TWC.impulse_response_gen(self.omega_c, self.rf_centers)
-        self.TWC.impulse_response_beam(self.omega_c, self.profile.bin_centers)
-
-        # On current measured (I,Q) voltage, apply LLRF model
-        self.llrf_model()
-
-        # Generator-induced voltage from generator current
-        self.generator_induced_voltage()
-
-        # Beam-induced voltage from beam profile
-        self.beam_induced_voltage(lpf=False)
-
-        # Sum and generator- and beam-induced voltages for coarse grid
-        self.V_coarse_tot = self.V_coarse_ind_gen + self.V_coarse_ind_beam
-        # Obtain generator-induced voltage on the fine grid by interpolation
-        self.V_fine_tot = self.V_fine_ind_beam \
-            + np.interp(self.profile.bin_centers,
-                        self.rf_centers, self.V_coarse_ind_gen)
-
-    def track_no_beam(self):
-        """Initial tracking method, before injecting beam."""
-
-        # Present time step
-        self.counter = int(0)
-        # Present carrier frequency: main RF frequency
-        self.omega_c = self.rf.omega_rf[0, self.counter]
-        # Present delay time
-        self.n_delay = int((self.rf.t_rev[self.counter] - self.TWC.tau)
-                           / self.rf.t_rf[0, self.counter])
-
-        # Update the impulse response at present carrier frequency
-        self.TWC.impulse_response_gen(self.omega_c, self.rf_centers)
-
-        # On current measured (I,Q) voltage, apply LLRF model
-        self.llrf_model()
-
-        # Generator-induced voltage from generator current
-        self.generator_induced_voltage()
-        self.logger.debug("Total voltage to generator %.3e V",
-                          np.mean(np.absolute(self.V_gen)))
-        self.logger.debug("Total current from generator %.3e A",
-                          np.mean(np.absolute(self.I_gen))
-                          / self.profile.bin_size)
-
-        # Without beam, total voltage equals generator-induced voltage
-        self.V_coarse_tot = self.V_coarse_ind_gen
-
-        self.logger.debug(
-            "Average generator voltage, last half of array %.3e V",
-            np.mean(np.absolute(self.V_coarse_ind_gen[int(0.5*self.n_coarse):])))
-
-    def llrf_model(self):
-        """Models the LLRF part of the OTFB.
-
-        Attributes
-        ----------
-        V_set : complex array
-            Voltage set point [V] in (I,Q); :math:`V_{\mathsf{set}}`, amplitude
-            proportional to voltage partition
-        dV_gen : complex array
-            Generator voltage [V] in (I,Q);
-            :math:`dV_{\mathsf{gen}} = V_{\mathsf{set}} - V_{\mathsf{tot}}`
         """
 
-        # Voltage set point of current turn (I,Q); depends on voltage partition
-        # Sinusoidal voltage completely in Q
-
-        self.V_set = polar_to_cartesian(
-            self.V_part*self.rf.voltage[0, self.counter],
-            0.5*np.pi - self.rf.phi_rf[0, self.counter])
-
-        # Convert to array
-        self.V_set *= np.ones(self.n_coarse)
-
-        # Difference of set point and actual voltage
-        self.dV_gen = self.V_set - self.open_loop*self.V_coarse_tot
-
-        # Closed-loop gain
-        self.dV_gen *= self.G_llrf
-        self.logger.debug("Set voltage %.6f MV",
-                          1e-6*np.mean(np.absolute(self.V_set)))
-        self.logger.debug("Antenna voltage %.6f MV",
-                          1e-6*np.mean(np.absolute(self.V_coarse_tot)))
-        self.logger.debug("Voltage error %.6f MV",
-                          1e-6*np.mean(np.absolute(self.dV_gen)))
-
-        # One-turn delay comb filter; memorise the value of the previous turn
-        self.dV_gen = comb_filter(self.dV_gen_prev, self.dV_gen, self.a_comb)
-        self.dV_gen_prev = np.copy(self.dV_gen)
-
-        # Modulate from omega_rf to omega_r
-        self.dV_gen = modulator(self.dV_gen, self.omega_c, self.omega_r,
-                                self.rf.t_rf[0, self.counter])
-
-        # Shift signals with the delay time
-        dV_gen_in = np.copy(self.dV_gen)
-        self.dV_gen = np.concatenate((self.dV_mov_av_prev[-self.n_delay:],
-                                      self.dV_gen[:self.n_coarse-self.n_delay]))
-
-        # Cavity filter: CIRCULAR moving average over filling time
-        # Memorize last points of previous turn for beginning of next turn
-        self.dV_gen = moving_average(
-            self.dV_gen, self.n_mov_av,
-            x_prev=self.dV_mov_av_prev[-self.n_delay-self.n_mov_av+1:
-                                       -self.n_delay])
-
-        self.dV_mov_av_prev = np.copy(dV_gen_in)
-
-    def generator_induced_voltage(self):
-        r"""Calculates the generator-induced voltage. The transmitter model is
-        a simple linear gain [C/V] converting voltage to charge.
-
-        .. math:: I = G_{\mathsf{tx}}\,\frac{V}{R_{\mathsf{gen}}} \, ,
-
-        where :math:`R_{\mathsf{gen}}` is the generator resistance,
-        :py:attr:`llrf.impulse_response.TravellingWaveCavity.R_gen`
-
-        Attributes
-        ----------
-        I_gen : complex array
-            RF component of the generator charge [C] at the present time step
-        V_coarse_ind_gen : complex array
-            Induced voltage [V] from generator-cavity interaction
+        # voltage_kick = bm.ascontiguousarray(self.rf_params.charge*self.rf_params.voltage[:, index])
+        # omegarf_kick = bm.ascontiguousarray(self.rf_params.omega_rf[:, index])
+        # phirf_kick = bm.ascontiguousarray(self.rf_params.phi_rf[:, index])
+        bm.kick(beam_dt, beam_dE, self.rf_params.voltage[:, index],
+                self.rf_params.omega_rf[:, index], self.rf_params.phi_rf[:, index],
+                self.rf_params.charge, self.rf_params.n_rf, self.acceleration_kick[index])
+
+    def drift(self, beam_dt, beam_dE, index):
+        r"""Function updating the particle arrival time to the RF station
+        (drift). If only the zeroth order slippage factor is given, 'simple'
+        and 'exact' solvers are available. The 'simple' solver is somewhat
+        faster. Otherwise, the solver is automatically 'exact' and calculates
+        the frequency slippage up to second order. The corresponding equations
+        are (nb: the n indices correspond to the turn number):
 
-        """
-
-        # Add correction to the drive already existing
-        self.V_gen = self.open_FB * modulator(self.dV_gen, self.omega_r,
-                                              self.omega_c,
-                                              self.rf.t_rf[0, self.counter]) \
-            + self.open_drive*self.V_set
-
-        # Generator charge from voltage, transmitter model
-        self.I_gen = self.G_tx*self.V_gen\
-            / self.TWC.R_gen*self.rf.t_rf[0, self.counter]
-
-        # Circular convolution: attach last points of previous turn
-        self.I_gen = np.concatenate((self.I_gen_prev, self.I_gen))
-
-        # Generator-induced voltage
-        self.induced_voltage('gen')
-        # Update memory of previous turn
-        self.I_gen_prev = self.I_gen[-self.n_mov_av:]
-
-    def induced_voltage(self, name):
-        r"""Generation of beam- or generator-induced voltage from the beam or
-        generator current, at a given carrier frequency and turn. The induced
-        voltage :math:`V(t)` is calculated from the impulse response matrix
-        :math:`h(t)` as follows:
+        .. math::
+            \\Delta t^{n+1} = \\Delta t^{n} + \\frac{L}{C} T_0^{n+1} \\left[ \\left(1+\\sum_{i=0}^{2}{\\alpha_i\\left(\\delta^{n+1}\\right)^{i+1}}\\right)   \\frac{1+\\left(\\Delta E/E_s\\right)^{n+1}}{1+\\delta^{n+1}}    - 1\\right] \quad \\text{(exact)}
 
         .. math::
-            \left( \begin{matrix} V_I(t) \\
-            V_Q(t) \end{matrix} \right)
-            = \left( \begin{matrix} h_s(t) & - h_c(t) \\
-            h_c(t) & h_s(t) \end{matrix} \right)
-            * \left( \begin{matrix} I_I(t) \\
-            I_Q(t) \end{matrix} \right) \, ,
-
-        where :math:`*` denotes convolution,
-        :math:`h(t)*x(t) = \int d\tau h(\tau)x(t-\tau)`. If the carrier
-        frequency is close to the cavity resonant frequency, :math:`h_c = 0`.
+            \\Delta t^{n+1} = \\Delta t^{n} + \\frac{L}{C} T_0^{n+1} \\left(\\frac{1}{1 - \\eta(\\delta^{n+1})\\delta^{n+1}} - 1\\right) \quad \\text{(legacy)}
 
-        :see also: :py:class:`llrf.impulse_response.TravellingWaveCavity`
+        .. math::
+            \\Delta t^{n+1} = \\Delta t^{n} + \\frac{L}{C} T_0^{n+1}\\eta_0\\delta^{n+1} \quad \\text{(simple)}
 
-        The impulse response is made to be the same length as the beam profile.
+        The relative momentum needs to be calculated from the relative energy
+        and is obtained as follow:
 
-        """
+        .. math::
+            \\delta = \\sqrt{1+\\beta_s^{-2}\\left[\\left(\\frac{\\Delta E}{E_s}\\right)^2 + 2\\frac{\\Delta E}{E_s}\\right]} - 1 \quad \\text{(exact)}
 
-        self.logger.debug("Matrix convolution for V_ind")
+        .. math::
+            \\delta = \\frac{\\Delta E}{\\beta_s^2 E_s} \quad \\text{(simple, legacy)}
 
-        if name == "beam":
-            # Compute the beam-induced voltage on the fine grid by convolution
-            self.__setattr__("V_fine_ind_"+name,
-                             self.matr_conv(self.__getattribute__("I_"+name),
-                                            self.TWC.__getattribute__("h_"+name)))
-
-            self.V_fine_ind_beam = -self.n_cavities \
-                * self.V_fine_ind_beam[:self.profile.n_slices]
-
-            # Beam-induced voltage on the coarse grid from semi-analytic method
-            self.V_coarse_ind_beam = -self.n_cavities \
-                * self.beam_induced_voltage_semi_analytic()
-
-        elif name == "gen":
-            self.__setattr__("V_coarse_ind_"+name,
-                             self.matr_conv(self.__getattribute__("I_"+name),
-                                            self.TWC.__getattribute__("h_"+name)))
-
-            # Circular convolution
-            self.V_coarse_ind_gen = +self.n_cavities \
-                * self.V_coarse_ind_gen[self.n_mov_av:
-                                        self.n_coarse+self.n_mov_av]
-
-    def beam_induced_voltage(self, lpf=False):
-        """Calculates the beam-induced voltage
-
-        Parameters
-        ----------
-        lpf : bool
-            Apply low-pass filter for beam current calculation;
-            default is False
-
-        Attributes
-        ----------
-        I_beam : complex array
-            RF component of the beam charge [C] at the present time step
-        V_coarse_ind_beam : complex array
-            Induced voltage [V] from beam-cavity interaction on the coarse grid
-        V_fine_ind_beam : complex array
-            Induced voltage [V] from beam-cavity interaction on the fine grid
         """
+        bm.drift(beam_dt, beam_dE, self.solver, self.rf_params.t_rev[index],
+                 self.rf_params.length_ratio, self.rf_params.alpha_order, self.rf_params.eta_0[index],
+                 self.rf_params.eta_1[index], self.rf_params.eta_2[index], self.rf_params.alpha_0[index],
+                 self.rf_params.alpha_1[index], self.rf_params.alpha_2[index],
+                 self.rf_params.beta[index], self.rf_params.energy[index])
+
+    def rf_voltage_calculation(self):
+        """Function calculating the total, discretised RF voltage seen by the
+        beam at a given turn. Requires a Profile object.
 
-        # Beam current from profile
-        self.I_beam = rf_beam_current(self.profile, self.omega_c,
-                                      self.rf.t_rev[self.counter], lpf=lpf)
-
-        # Beam-induced voltage
-        self.induced_voltage('beam')
-
-    def pre_compute_semi_analytic_factor(self, time):
-        r""" Pre-computes factor for semi-analytic method, which is used to
-        compute the beam-induced voltage on the coarse grid.
-
-        Parameters
-        ----------
-        time : float array [s]
-            Time array at which to compute the beam-induced voltage
-
-        Attributes
-        ----------
-        profile_coarse : class
-            Beam profile with 20 bins per RF-bucket
-        semi_analytic_factor : complex array [:math:`\Omega\,s`]
-            Factor that is used to compute the beam-induced voltage
         """
+        voltages = bm.ascontiguousarray(self.rf_params.voltage[:, self.counter[0]])
+        omega_rf = bm.ascontiguousarray(self.rf_params.omega_rf[:, self.counter[0]])
+        phi_rf = bm.ascontiguousarray(self.rf_params.phi_rf[:, self.counter[0]])
+        # TODO: test with multiple harmonics, think about 800 MHz OTFB
+        if self.cavityFB:
+            self.rf_voltage = voltages[0] * self.cavityFB.V_corr * \
+                bm.sin(omega_rf[0]*self.profile.bin_centers +
+                       phi_rf[0] + self.cavityFB.phi_corr) + \
+                bm.rf_volt_comp(voltages[1:], omega_rf[1:], phi_rf[1:],
+                                self.profile.bin_centers)
+        else:
+            self.rf_voltage = bm.rf_volt_comp(voltages, omega_rf, phi_rf,
+                                              self.profile.bin_centers)
 
-        self.logger.info("Pre-computing semi-analytic factor")
-
-        n_slices_per_bucket = 20
-
-        n_buckets = int(np.round(
-            (self.profile.cut_right - self.profile.cut_left)
-            / self.rf.t_rf[0, 0]))
-
-        self.profile_coarse = Profile(self.beam, CutOptions=CutOptions(
-            cut_left=self.profile.cut_left,
-            cut_right=self.profile.cut_right,
-            n_slices=n_buckets*n_slices_per_bucket))
-
-        # pre-factor [Ohm s]
-
-        pre_factor = 2*self.TWC.R_beam / self.TWC.tau**2 / self.omega_r**3
-
-        # Matrix of time differences [1]
-        dt1 = np.zeros(shape=(len(time), self.profile_coarse.n_slices))
-
-        for i in range(len(time)):
-            dt1[i] = (time[i] - self.profile_coarse.bin_centers) * self.omega_r
-
-#        dt2 = dt1 - self.TWC.tau * self.omega_r
-
-#        phase1 = np.exp(-1j * dt1)
-        phase = np.exp(-1j * self.TWC.tau * self.TWC.omega_r)
-
-#        diff1 = 2j - dt1 + self.TWC.tau * self.omega_r
-
-#        diff2 = (2j - dt1 + self.TWC.tau * self.omega_r) * np.exp(-1j * dt1)
-
-        tmp = (-2j - dt1 + self.TWC.tau*self.omega_r
-               + (2j - dt1 + self.TWC.tau*self.omega_r) * np.exp(-1j * dt1))\
-            * np.sign(dt1) \
-            - ((2j - dt1 + self.TWC.tau * self.omega_r) * np.exp(-1j * dt1)
-               + (-2j - dt1 + self.TWC.tau * self.omega_r) * phase) \
-            * np.sign(dt1 - self.TWC.tau * self.omega_r) \
-            - (2 - 1j*dt1) * self.TWC.tau * self.TWC.omega_r * np.sign(dt1)
-
-#        tmp = (-2j - dt1 + self.TWC.tau*self.omega_r + diff2) * np.sign(dt1) \
-#            - (diff2 + (-2j - dt1 + self.TWC.tau * self.omega_r) * phase) \
-#                * np.sign(dt1 - self.TWC.tau * self.omega_r) \
-#            - (2 - 1j*dt1) * self.TWC.tau * self.TWC.omega_r * np.sign(dt1)
-
-#        tmp = (diff1.conjugate() + diff2) * np.sign(dt1) \
-#            - (diff2 + diff1.conjugate() * phase) \
-#                * np.sign(dt1 - self.TWC.tau * self.omega_r) \
-#            - (2 - 1j*dt1) * self.TWC.tau * self.TWC.omega_r * np.sign(dt1)
-
-        tmp *= pre_factor
-
-        self.semi_analytic_factor = np.diff(tmp)
-
-    def beam_induced_voltage_semi_analytic(self):
-        r"""Computes the beam-induced voltage in (I,Q) at the present carrier
-        frequency :math:`\omega_c` using the semi-analytic method. It requires
-        that pre_compute_semi_analytic_factor() was called previously.
+    def track(self):
+        """Tracking method for the section. Applies first the kick, then the
+        drift. Calls also RF/beam feedbacks if applicable. Updates the counter
+        of the corresponding RFStation class and the energy-related variables
+        of the Beam class.
 
-        Returns
-        -------
-        complex array [V]
-            Beam-induced voltage in (I,Q) at :math:`\omega_c`
         """
+        turn = self.counter[0]
 
-        # Update the coarse profile
-        self.profile_coarse.track()
-
-        # Slope of line segments [A/s]
-        kappa = self.beam.ratio*self.beam.Particle.charge*e \
-            * np.diff(self.profile_coarse.n_macroparticles) \
-            / self.profile_coarse.bin_size**2
+        # Add phase noise directly to the cavity RF phase
+        if self.rf_params.phi_noise is not None:
+            if self.noiseFB is not None:
+                self.rf_params.phi_rf[:, turn] += \
+                    self.noiseFB.x * self.rf_params.phi_noise[:, turn]
+            else:
+                self.rf_params.phi_rf[:, turn] += \
+                    self.rf_params.phi_noise[:, turn]
+
+        # Add phase modulation directly to the cavity RF phase
+        if self.rf_params.phi_modulation is not None:
+            self.rf_params.phi_rf[:, turn] += \
+                self.rf_params.phi_modulation[0][:, turn]
+            self.rf_params.omega_rf[:, turn] += \
+                self.rf_params.phi_modulation[1][:, turn]
+
+        # Determine phase loop correction on RF phase and frequency
+        if self.beamFB is not None and turn >= self.beamFB.delay:
+            self.beamFB.track()
+
+        # Update the RF phase of all systems for the next turn
+        # Accumulated phase offset due to beam phase loop or frequency offset
+        self.rf_params.dphi_rf += 2.*np.pi*self.rf_params.harmonic[:,turn+1]* \
+                                  (self.rf_params.omega_rf[:,turn+1] -
+                                   self.rf_params.omega_rf_d[:,turn+1]) / \
+                                  self.rf_params.omega_rf_d[:,turn+1]
+
+        # Total phase offset
+        self.rf_params.phi_rf[:,turn+1] += self.rf_params.dphi_rf
+
+        if self.periodicity:
+
+            # Distinguish the particles inside the frame from the particles on
+            # the right-hand side of the frame.
+            self.indices_right_outside = \
+                bm.where(self.beam.dt > self.rf_params.t_rev[turn + 1])[0]
+            self.indices_inside_frame = \
+                bm.where(self.beam.dt < self.rf_params.t_rev[turn + 1])[0]
+
+            if len(self.indices_right_outside) > 0:
+                # Change reference of all the particles on the right of the
+                # current frame; these particles skip one kick and drift
+                self.beam.dt[self.indices_right_outside] -= \
+                    self.rf_params.t_rev[turn + 1]
+                # Synchronize the bunch with the particles that are on the
+                # RHS of the current frame applying kick and drift to the
+                # bunch
+                # After that all the particles are in the new updated frame
+                self.insiders_dt = bm.ascontiguousarray(
+                    self.beam.dt[self.indices_inside_frame])
+                self.insiders_dE = bm.ascontiguousarray(
+                    self.beam.dE[self.indices_inside_frame])
+                self.kick(self.insiders_dt, self.insiders_dE, turn)
+                self.drift(self.insiders_dt, self.insiders_dE, turn+1)
+                self.beam.dt[self.indices_inside_frame] = self.insiders_dt
+                self.beam.dE[self.indices_inside_frame] = self.insiders_dE
+                # Check all the particles on the left of the just updated
+                # frame and apply a second kick and drift to them with the
+                # previous wave after having changed reference.
+                self.indices_left_outside = bm.where(self.beam.dt < 0)[0]
+
+            else:
+                self.kick(self.beam.dt, self.beam.dE, turn)
+                self.drift(self.beam.dt, self.beam.dE, turn + 1)
+                # Check all the particles on the left of the just updated
+                # frame and apply a second kick and drift to them with the
+                # previous wave after having changed reference.
+                self.indices_left_outside = bm.where(self.beam.dt < 0)[0]
+
+            if len(self.indices_left_outside) > 0:
+                left_outsiders_dt = bm.ascontiguousarray(
+                    self.beam.dt[self.indices_left_outside])
+                left_outsiders_dE = bm.ascontiguousarray(
+                    self.beam.dE[self.indices_left_outside])
+                left_outsiders_dt += self.rf_params.t_rev[turn+1]
+                self.kick(left_outsiders_dt, left_outsiders_dE, turn)
+                self.drift(left_outsiders_dt, left_outsiders_dE, turn+1)
+                self.beam.dt[self.indices_left_outside] = left_outsiders_dt
+                self.beam.dE[self.indices_left_outside] = left_outsiders_dE
 
-        return np.exp(1j*self.rf_centers*self.omega_c)\
-            * np.sum(self.semi_analytic_factor * kappa, axis=1)
+        else:
 
-    def matr_conv(self, I, h):
-        """Convolution of beam current with impulse response; uses a complete
-        matrix with off-diagonal elements."""
+            if self.rf_params.empty is False:
+                if self.interpolation:
+                    self.rf_voltage_calculation()
+                    if self.totalInducedVoltage is not None:
+                        self.total_voltage = self.rf_voltage \
+                            + self.totalInducedVoltage.induced_voltage
+                    else:
+                        self.total_voltage = self.rf_voltage
+
+                    bm.linear_interp_kick(dt=self.beam.dt, dE=self.beam.dE,
+                                          voltage=self.total_voltage,
+                                          bin_centers=self.profile.bin_centers,
+                                          charge=self.beam.Particle.charge,
+                                          acceleration_kick=self.acceleration_kick[turn])
+
+                else:
+                    self.kick(self.beam.dt, self.beam.dE, turn)
+
+            self.drift(self.beam.dt, self.beam.dE, turn + 1)
+
+        # Updating the beam synchronous momentum etc.
+        self.beam.beta = self.rf_params.beta[turn+1]
+        self.beam.gamma = self.rf_params.gamma[turn+1]
+        self.beam.energy = self.rf_params.energy[turn+1]
+        self.beam.momentum = self.rf_params.momentum[turn+1]
 
-        return scipy.signal.fftconvolve(I, h, mode='full')
+        # Increment by one the turn counter
+        self.counter[0] += 1
 
-    def call_conv(self, signal, kernel):
-        """Routine to call optimised C++ convolution"""
+    def to_gpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays to the GPU
+        '''
+        # Check if to_gpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'GPU':
+            return
+
+        # transfer recursively objects
+        if recursive and self.profile:
+            self.profile.to_gpu()
+        if recursive and self.totalInducedVoltage:
+            self.totalInducedVoltage.to_gpu()
+        if recursive and self.beam:
+            self.beam.to_gpu()
+        if recursive and self.beamFB:
+            self.beamFB.to_gpu()
+        if recursive and self.rf_params:
+            self.rf_params.to_gpu()
+
+        assert bm.device == 'GPU'
+        import cupy as cp
+
+        # import from rf_params
+        # self.t_rev = self.rf_params.t_rev
+        # self.harmonic = self.rf_params.harmonic
+        # self.voltage = self.rf_params.voltage
+        # self.phi_noise = self.rf_params.phi_noise
+        # self.phi_modulation = self.rf_params.phi_modulation
+        # self.phi_rf = self.rf_params.phi_rf
+        # self.phi_s = self.rf_params.phi_s
+        # self.omega_rf = self.rf_params.omega_rf
 
-        # Make sure that the buffers are stored contiguously
-        signal = np.ascontiguousarray(signal)
-        kernel = np.ascontiguousarray(kernel)
+        if hasattr(self, 'rf_voltage'):
+            self.rf_voltage = self.rf_params.rf_voltage
 
-        result = np.zeros(len(kernel) + len(signal) - 1)
-        bm.convolve(signal, kernel, result)
+        # to make sure it will not be called again
+        self._device = 'GPU'
+        
+    def to_cpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays back to the CPU
+        '''
+        # Check if to_cpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'CPU':
+            return
+
+        # transfer recursively objects
+        if recursive and self.profile:
+            self.profile.to_cpu()
+        if recursive and self.totalInducedVoltage:
+            self.totalInducedVoltage.to_cpu()
+        if recursive and self.beam:
+            self.beam.to_cpu()
+        if recursive and self.beamFB:
+            self.beamFB.to_cpu()
+        if recursive and self.rf_params:
+            self.rf_params.to_cpu()
+
+        assert bm.device == 'CPU'
+        import cupy as cp
+
+        # import from rf_params
+        # self.t_rev = self.rf_params.t_rev
+        # self.harmonic = self.rf_params.harmonic
+        # self.voltage = self.rf_params.voltage
+        # self.phi_noise = self.rf_params.phi_noise
+        # self.phi_modulation = self.rf_params.phi_modulation
+        # self.phi_rf = self.rf_params.phi_rf
+        # self.phi_s = self.rf_params.phi_s
+        # self.omega_rf = self.rf_params.omega_rf
 
-        #  libblond.convolution(signal.ctypes.data_as(ctypes.c_void_p),
-        #                       ctypes.c_int(len(signal)),
-        #                       kernel.ctypes.data_as(ctypes.c_void_p),
-        #                       ctypes.c_int(len(kernel)),
-        #                       result.ctypes.data_as(ctypes.c_void_p))
+        if hasattr(self, 'rf_voltage'):
+            self.rf_voltage = cp.asnumpy(self.rf_voltage)
 
-        return result
+        # to make sure it will not be called again
+        self._device = 'CPU'
```

### Comparing `blond-2.0.11/blond/llrf/impulse_response.py` & `blond-2.0.12/blond/llrf/impulse_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # coding: utf8
-# Copyright 2014-2017 CERN. This software is distributed under the
+# Copyright 2014-2020 CERN. This software is distributed under the
 # terms of the GNU General Public Licence version 3 (GPL Version 3),
 # copied verbatim in the file LICENCE.md.
 # In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
 '''
 **Filters and methods for control loops**
 
 :Authors: **Helga Timko**
 '''
 
 from __future__ import division
+
+import matplotlib.pyplot as plt
 import numpy as np
 from scipy.constants import c
 
 # Set up logging
 import logging
 logger = logging.getLogger(__name__)
 
@@ -204,26 +206,26 @@
     l_cav : float
         Length [m] of the interaction region
     tau : float
         Cavity filling time [s]
 
     """
 
-    def __init__(self, l_cell, N_cells, rho, v_g, omega_r):
+    def __init__(self, l_cell, N_cells, rho, v_g, omega_r, df = 0):
 
         self.l_cell = float(l_cell)
         self.N_cells = int(N_cells)
         self.rho = float(rho)
         if v_g > 0 and v_g < 1:
             self.v_g = float(v_g)
         else:
             #ImpulseError
             raise RuntimeError("ERROR in TravellingWaveCavity: group" +
                                " velocity out of limits (0,1)!")
-        self.omega_r = float(omega_r)
+        self.omega_r = float(omega_r) + 2 * np.pi * float(df)
 
         # Calculated
         self.l_cav = float(self.l_cell*self.N_cells)
         # v_g opposite to wave!
         self.tau = self.l_cav/(self.v_g*c)*(1 + self.v_g)
 
         # Assumed impedance for measurement of generator current
@@ -255,92 +257,101 @@
         Attributes
         ----------
         d_omega : float
             :math:`\omega_c - \omega_r` [1/s]
         t_gen : float array
             time array for generator wake and impulse response; starts from
             :math:`- \tau/2`
-        hs_gen : float array
-            :math:`h_{s,g}(t)` [\Omega/s] as defined above
-        hc_gen : float array
-            :math:`h_{c,g}(t)` [\Omega/s] as defined above
-
+        h_gen : complex array
+            :math:`h_{s,b}(t) + i*h_{c,b}(t)` [\Omega/s] as defined above
         """
 
         self.omega_c = float(omega_c)
         self.d_omega = self.omega_c - self.omega_r
         if np.fabs((self.d_omega)/self.omega_r) > 0.1:
             #ImpulseError
             raise RuntimeError("ERROR in TravellingWaveCavity" +
                                " impulse_response(): carrier frequency" +
                                " should be close to central frequency of the" +
                                " cavity!")
 
         # Move starting point of impulse response to correct value
-        t_gen = time_coarse - time_coarse[0] - 0.5*self.tau
+        t_gen = time_coarse - time_coarse[0]
 
         # Impulse response if on carrier frequency
         self.h_gen = (self.R_gen / self.tau *
-                      rectangle(t_gen, self.tau)).astype(np.complex128)
+                      rectangle(t_gen - 0.5*self.tau, self.tau)).astype(np.complex128)
 
         # Impulse response if not on carrier frequency
         if np.fabs((self.d_omega)/self.omega_r) > 1e-12:
+            self.h_gen = self.h_gen.real*(np.cos(self.d_omega*t_gen) -          # TODO: Introduced a plus here
+                                          1j*np.sin(self.d_omega*t_gen))
 
-            self.h_gen.imag = self.h_gen.real*np.sin(self.d_omega * t_gen)
-            self.h_gen.real *= np.cos(self.d_omega * t_gen)
-
-    def impulse_response_beam(self, omega_c, time_fine):
+    def impulse_response_beam(self, omega_c, time_fine, time_coarse=None):
         r"""Impulse response from the cavity towards the beam. For a signal
         that is I,Q demodulated at a given carrier
         frequency :math:`\omega_c`. The formulae assume that the carrier
         frequency is be close to the central frequency
         :math:`\omega_c/\omega_r \ll 1` and that the signal is low-pass
         filtered (i.e.\ high-frequency components can be neglected).
 
         Parameters
         ----------
         omega_c : float
             Carrier revolution frequency [1/s]
         time_fine : float
             Time array of the beam profile to act on
+        time_coarse : float
+            Time array of the LLRF to act on; default is None
 
         Attributes
         ----------
         d_omega : float
             :math:`\omega_c - \omega_r` [1/s]
         t_beam : float array
             time array for beam wake and impulse response; starts from zero
-        hs_beam : float array
-            :math:`h_{s,b}(t)` [\Omega/s] as defined above
-        hc_beam : float array
-            :math:`h_{c,b}(t)` [\Omega/s] as defined above
-
+        h_beam : complex array
+            :math:`h_{s,b}(t) + i*h_{c,b}(t)` [\Omega/s] as defined above
+        h_beam_coarse : complex array
+            Impulse response evaluated on the coarse grid
         """
 
         self.omega_c = float(omega_c)
         self.d_omega = self.omega_c - self.omega_r
         if np.fabs((self.d_omega)/self.omega_r) > 0.1:
-            #ImpulseError
             raise RuntimeError("ERROR in TravellingWaveCavity" +
                                " impulse_response(): carrier frequency" +
                                " should be close to central frequency of the" +
                                " cavity!")
 
         # Move starting point of impulse response to correct value
         t_beam = time_fine - time_fine[0]
 
         # Impulse response if on carrier frequency
-        self.h_beam = (2*self.R_beam / self.tau *
+        self.h_beam = (-2*self.R_beam/self.tau*
                        triangle(t_beam, self.tau)).astype(np.complex128)
 
         # Impulse response if not on carrier frequency
         if np.fabs((self.d_omega)/self.omega_r) > 1e-12:
+            self.h_beam = self.h_beam.real*(np.cos(self.d_omega*t_beam) -           # TODO: Introduced a plus here
+                                            1j*np.sin(self.d_omega*t_beam))
 
-            self.h_beam.imag = self.h_beam.real*np.sin(self.d_omega*t_beam)
-            self.h_beam.real *= np.cos(self.d_omega * t_beam)
+        if time_coarse is not None:
+            # Move starting point of impulse response to correct value
+            t_beam = time_coarse - time_coarse[0]
+
+            # Impulse response if on carrier frequency
+            self.h_beam_coarse = (-2*self.R_beam/self.tau*
+                                  triangle(t_beam, self.tau)).astype(np.complex128)
+
+            # Impulse response if not on carrier frequency
+            if np.fabs((self.d_omega)/self.omega_r) > 1e-12:
+                self.h_beam_coarse = self.h_beam_coarse.real* \
+                                     (np.cos(self.d_omega*t_beam) -                 # TODO: Introduced a plus here
+                                      1j*np.sin(self.d_omega*t_beam))
 
     def compute_wakes(self, time):
         r"""Computes the wake fields towards the beam and generator on the
         central cavity frequency.
 
         Parameters
         ----------
@@ -362,21 +373,29 @@
         t_gen = time - time[0] - 0.5*self.tau
 
         # Wake fields towards beam and generator
         self.W_beam = 2*self.h_beam.real*np.cos(self.omega_r*t_beam)
         self.W_gen = 2*self.h_gen.real*np.cos(self.omega_r*t_gen)
 
 
+class SPS3Section200MHzTWC(TravellingWaveCavity):
+
+    def __init__(self, df = 0):
+
+        TravellingWaveCavity.__init__(self, 0.374, 32, 2.71e4, 0.0946,
+                                      2*np.pi*200.03766667e6, df = df)
+
+
 class SPS4Section200MHzTWC(TravellingWaveCavity):
 
-    def __init__(self):
+    def __init__(self, df = 0):
 
         TravellingWaveCavity.__init__(self, 0.374, 43, 2.71e4, 0.0946,
-                                      2*np.pi*200.222e6)
+                                      2*np.pi*199.9945e6, df = df)
 
 
 class SPS5Section200MHzTWC(TravellingWaveCavity):
 
-    def __init__(self):
+    def __init__(self, df = 0):
 
         TravellingWaveCavity.__init__(self, 0.374, 54, 2.71e4, 0.0946,
-                                      2*np.pi*200.222e6)
+                                      2*np.pi*200.1e6, df = df)
```

### Comparing `blond-2.0.11/blond/llrf/notch_filter.py` & `blond-2.0.12/blond/llrf/notch_filter.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/llrf/offset_frequency.py` & `blond-2.0.12/blond/llrf/offset_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/llrf/rf_modulation.py` & `blond-2.0.12/blond/llrf/rf_modulation.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/llrf/rf_noise.py` & `blond-2.0.12/blond/llrf/rf_noise.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         # Use only real part for the phase shift and normalize
         self.t = np.linspace(0, float(nt*dt), nt) 
         self.dphi_output = dPt.real
  
     
     def generate(self):
        
-        for i in range(0, np.int(np.ceil(self.n_turns/self.corr))):
+        for i in range(0, int(np.ceil(self.n_turns/self.corr))):
         
             # Scale amplitude to keep area (phase noise amplitude) constant
             k = i*self.corr       # current time step
             ampl = self.A_i*self.fs[0]/self.fs[k]
             
             # Calculate the frequency step
             f_max = self.f0[k]/2
@@ -141,16 +141,16 @@
                 #NoiseError
                 raise RuntimeError('Error in noise generation!')
             n_points_pos_f_incl_zero = int(nt_regular/2 + 1)  
             freq = np.linspace(0, float(f_max), n_points_pos_f_incl_zero)
             delta_f = f_max/(n_points_pos_f_incl_zero-1) 
 
             # Construct spectrum   
-            nmin = np.int(np.floor(self.fmin_s0*self.fs[k]/delta_f))  
-            nmax = np.int(np.ceil(self.fmax_s0*self.fs[k]/delta_f))    
+            nmin = int(np.floor(self.fmin_s0*self.fs[k]/delta_f))  
+            nmax = int(np.ceil(self.fmax_s0*self.fs[k]/delta_f))    
             
             # To compensate the notch due to PL at central frequency
             if self.predistortion == 'exponential':
                 
                 spectrum = np.concatenate((np.zeros(nmin), ampl*np.exp(
                     np.log(100.)*np.arange(0,nmax-nmin+1)/(nmax-nmin) ), 
                                            np.zeros(n_points_pos_f_incl_zero-nmax-1) ))
```

### Comparing `blond-2.0.11/blond/llrf/signal_processing.py` & `blond-2.0.12/__EXAMPLES/main_files/EX_18_robinson_instability.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,438 +1,465 @@
-00000000: 2320 636f 6469 6e67 3a20 7574 6638 0d0a  # coding: utf8..
-00000010: 2320 436f 7079 7269 6768 7420 3230 3134  # Copyright 2014
-00000020: 2d32 3031 3720 4345 524e 2e20 5468 6973  -2017 CERN. This
-00000030: 2073 6f66 7477 6172 6520 6973 2064 6973   software is dis
-00000040: 7472 6962 7574 6564 2075 6e64 6572 2074  tributed under t
-00000050: 6865 0d0a 2320 7465 726d 7320 6f66 2074  he..# terms of t
-00000060: 6865 2047 4e55 2047 656e 6572 616c 2050  he GNU General P
-00000070: 7562 6c69 6320 4c69 6365 6e63 6520 7665  ublic Licence ve
-00000080: 7273 696f 6e20 3320 2847 504c 2056 6572  rsion 3 (GPL Ver
-00000090: 7369 6f6e 2033 292c 0d0a 2320 636f 7069  sion 3),..# copi
-000000a0: 6564 2076 6572 6261 7469 6d20 696e 2074  ed verbatim in t
-000000b0: 6865 2066 696c 6520 4c49 4345 4e43 452e  he file LICENCE.
-000000c0: 6d64 2e0d 0a23 2049 6e20 6170 706c 7969  md...# In applyi
-000000d0: 6e67 2074 6869 7320 6c69 6365 6e63 652c  ng this licence,
-000000e0: 2043 4552 4e20 646f 6573 206e 6f74 2077   CERN does not w
-000000f0: 6169 7665 2074 6865 2070 7269 7669 6c65  aive the privile
-00000100: 6765 7320 616e 6420 696d 6d75 6e69 7469  ges and immuniti
-00000110: 6573 0d0a 2320 6772 616e 7465 6420 746f  es..# granted to
-00000120: 2069 7420 6279 2076 6972 7475 6520 6f66   it by virtue of
-00000130: 2069 7473 2073 7461 7475 7320 6173 2061   its status as a
-00000140: 6e20 496e 7465 7267 6f76 6572 6e6d 656e  n Intergovernmen
-00000150: 7461 6c20 4f72 6761 6e69 7a61 7469 6f6e  tal Organization
-00000160: 206f 720d 0a23 2073 7562 6d69 7420 6974   or..# submit it
-00000170: 7365 6c66 2074 6f20 616e 7920 6a75 7269  self to any juri
-00000180: 7364 6963 7469 6f6e 2e0d 0a23 2050 726f  sdiction...# Pro
-00000190: 6a65 6374 2077 6562 7369 7465 3a20 6874  ject website: ht
-000001a0: 7470 3a2f 2f62 6c6f 6e64 2e77 6562 2e63  tp://blond.web.c
-000001b0: 6572 6e2e 6368 2f0d 0a0d 0a27 2727 0d0a  ern.ch/....'''..
-000001c0: 2a2a 4669 6c74 6572 7320 616e 6420 6d65  **Filters and me
-000001d0: 7468 6f64 7320 666f 7220 636f 6e74 726f  thods for contro
-000001e0: 6c20 6c6f 6f70 732a 2a0d 0a0d 0a3a 4175  l loops**....:Au
-000001f0: 7468 6f72 733a 202a 2a48 656c 6761 2054  thors: **Helga T
-00000200: 696d 6b6f 2a2a 0d0a 2727 270d 0a0d 0a66  imko**..'''....f
-00000210: 726f 6d20 5f5f 6675 7475 7265 5f5f 2069  rom __future__ i
-00000220: 6d70 6f72 7420 6469 7669 7369 6f6e 0d0a  mport division..
-00000230: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
-00000240: 6e70 0d0a 6672 6f6d 2073 6369 7079 2e63  np..from scipy.c
-00000250: 6f6e 7374 616e 7473 2069 6d70 6f72 7420  onstants import 
-00000260: 650d 0a66 726f 6d20 7363 6970 7920 696d  e..from scipy im
-00000270: 706f 7274 2073 6967 6e61 6c20 6173 2073  port signal as s
-00000280: 676e 0d0a 0d0a 0d0a 2320 5365 7420 7570  gn......# Set up
-00000290: 206c 6f67 6769 6e67 0d0a 696d 706f 7274   logging..import
-000002a0: 206c 6f67 6769 6e67 0d0a 6c6f 6767 6572   logging..logger
-000002b0: 203d 206c 6f67 6769 6e67 2e67 6574 4c6f   = logging.getLo
-000002c0: 6767 6572 285f 5f6e 616d 655f 5f29 0d0a  gger(__name__)..
-000002d0: 0d0a 0d0a 6465 6620 706f 6c61 725f 746f  ....def polar_to
-000002e0: 5f63 6172 7465 7369 616e 2861 6d70 6c69  _cartesian(ampli
-000002f0: 7475 6465 2c20 7068 6173 6529 3a0d 0a20  tude, phase):.. 
-00000300: 2020 2022 2222 436f 6e76 6572 7420 6461     """Convert da
-00000310: 7461 2066 726f 6d20 706f 6c61 7220 746f  ta from polar to
-00000320: 2063 6172 7465 7369 616e 2028 492c 5129   cartesian (I,Q)
-00000330: 2063 6f6f 7264 696e 6174 6573 2e0d 0a0d   coordinates....
-00000340: 0a20 2020 2050 6172 616d 6574 6572 730d  .    Parameters.
-00000350: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d  .    ----------.
-00000360: 0a20 2020 2061 6d70 6c69 7475 6465 203a  .    amplitude :
-00000370: 2066 6c6f 6174 2061 7272 6179 0d0a 2020   float array..  
-00000380: 2020 2020 2020 416d 706c 6974 7564 6520        Amplitude 
-00000390: 6f66 2073 6967 6e61 6c0d 0a20 2020 2070  of signal..    p
-000003a0: 6861 7365 203a 2066 6c6f 6174 2061 7272  hase : float arr
-000003b0: 6179 0d0a 2020 2020 2020 2020 5068 6173  ay..        Phas
-000003c0: 6520 6f66 2073 6967 6e61 6c0d 0a0d 0a20  e of signal.... 
-000003d0: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
-000003e0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2063 6f6d  -------..    com
-000003f0: 706c 6578 2061 7272 6179 0d0a 2020 2020  plex array..    
-00000400: 2020 2020 5369 676e 616c 2077 6974 6820      Signal with 
-00000410: 696e 2d70 6861 7365 2061 6e64 2071 7561  in-phase and qua
-00000420: 6472 6174 7572 6520 2849 2c51 2920 636f  drature (I,Q) co
-00000430: 6d70 6f6e 656e 7473 0d0a 2020 2020 2222  mponents..    ""
-00000440: 220d 0a0d 0a20 2020 206c 6f67 6765 722e  "....    logger.
-00000450: 6465 6275 6728 2243 6f6e 7665 7274 696e  debug("Convertin
-00000460: 6720 6672 6f6d 2070 6f6c 6172 2074 6f20  g from polar to 
-00000470: 4361 7274 6573 6961 6e22 290d 0a0d 0a20  Cartesian").... 
-00000480: 2020 2072 6574 7572 6e20 616d 706c 6974     return amplit
-00000490: 7564 652a 286e 702e 636f 7328 7068 6173  ude*(np.cos(phas
-000004a0: 6529 202b 2031 6a2a 6e70 2e73 696e 2870  e) + 1j*np.sin(p
-000004b0: 6861 7365 2929 0d0a 0d0a 0d0a 6465 6620  hase))......def 
-000004c0: 6361 7274 6573 6961 6e5f 746f 5f70 6f6c  cartesian_to_pol
-000004d0: 6172 2849 515f 7665 6374 6f72 293a 0d0a  ar(IQ_vector):..
-000004e0: 2020 2020 2222 2243 6f6e 7665 7274 2064      """Convert d
-000004f0: 6174 6120 6672 6f6d 2043 6172 7465 7369  ata from Cartesi
-00000500: 616e 2028 492c 5129 2074 6f20 706f 6c61  an (I,Q) to pola
-00000510: 7220 636f 6f72 6469 6e61 7465 732e 0d0a  r coordinates...
-00000520: 0d0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-00000530: 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  ..    ----------
-00000540: 0d0a 2020 2020 4951 5f76 6563 746f 7220  ..    IQ_vector 
-00000550: 3a20 636f 6d70 6c65 7820 6172 7261 790d  : complex array.
-00000560: 0a20 2020 2020 2020 2053 6967 6e61 6c20  .        Signal 
-00000570: 7769 7468 2069 6e2d 7068 6173 6520 616e  with in-phase an
-00000580: 6420 7175 6164 7261 7475 7265 2028 492c  d quadrature (I,
-00000590: 5129 2063 6f6d 706f 6e65 6e74 730d 0a0d  Q) components...
-000005a0: 0a20 2020 2052 6574 7572 6e73 0d0a 2020  .    Returns..  
-000005b0: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 2066    -------..    f
-000005c0: 6c6f 6174 2061 7272 6179 0d0a 2020 2020  loat array..    
-000005d0: 2020 2020 416d 706c 6974 7564 6520 6f66      Amplitude of
-000005e0: 2073 6967 6e61 6c0d 0a20 2020 2066 6c6f   signal..    flo
-000005f0: 6174 2061 7272 6179 0d0a 2020 2020 2020  at array..      
-00000600: 2020 5068 6173 6520 6f66 2073 6967 6e61    Phase of signa
-00000610: 6c0d 0a0d 0a20 2020 2022 2222 0d0a 0d0a  l....    """....
-00000620: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00000630: 2822 436f 6e76 6572 7469 6e67 2066 726f  ("Converting fro
-00000640: 6d20 4361 7274 6573 6961 6e20 746f 2070  m Cartesian to p
-00000650: 6f6c 6172 2229 0d0a 0d0a 2020 2020 7265  olar")....    re
-00000660: 7475 726e 206e 702e 6162 736f 6c75 7465  turn np.absolute
-00000670: 2849 515f 7665 6374 6f72 292c 206e 702e  (IQ_vector), np.
-00000680: 616e 676c 6528 4951 5f76 6563 746f 7229  angle(IQ_vector)
-00000690: 0d0a 0d0a 0d0a 6465 6620 6d6f 6475 6c61  ......def modula
-000006a0: 746f 7228 7369 676e 616c 2c20 6f6d 6567  tor(signal, omeg
-000006b0: 615f 692c 206f 6d65 6761 5f66 2c20 545f  a_i, omega_f, T_
-000006c0: 7361 6d70 6c69 6e67 293a 0d0a 2020 2020  sampling):..    
-000006d0: 2222 2244 656d 6f64 756c 6174 6520 6120  """Demodulate a 
-000006e0: 7369 676e 616c 2066 726f 6d20 696e 6974  signal from init
-000006f0: 6961 6c20 6672 6571 7565 6e63 7920 746f  ial frequency to
-00000700: 2066 696e 616c 2066 7265 7175 656e 6379   final frequency
-00000710: 2e20 5468 6520 7477 6f0d 0a20 2020 2066  . The two..    f
-00000720: 7265 7175 656e 6369 6573 2073 686f 756c  requencies shoul
-00000730: 6420 6265 2063 6c6f 7365 2e0d 0a0d 0a20  d be close..... 
-00000740: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
-00000750: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-00000760: 2020 2073 6967 6e61 6c20 3a20 666c 6f61     signal : floa
-00000770: 7420 6172 7261 790d 0a20 2020 2020 2020  t array..       
-00000780: 2053 6967 6e61 6c20 746f 2062 6520 6465   Signal to be de
-00000790: 6d6f 6475 6c61 7465 640d 0a20 2020 206f  modulated..    o
-000007a0: 6d65 6761 5f69 203a 2066 6c6f 6174 0d0a  mega_i : float..
-000007b0: 2020 2020 2020 2020 496e 6974 6961 6c20          Initial 
-000007c0: 7265 766f 6c75 7469 6f6e 2066 7265 7175  revolution frequ
-000007d0: 656e 6379 205b 312f 735d 206f 6620 7369  ency [1/s] of si
-000007e0: 676e 616c 2028 6265 666f 7265 2064 656d  gnal (before dem
-000007f0: 6f64 756c 6174 696f 6e29 0d0a 2020 2020  odulation)..    
-00000800: 6f6d 6567 615f 6620 3a20 666c 6f61 740d  omega_f : float.
-00000810: 0a20 2020 2020 2020 2046 696e 616c 2072  .        Final r
-00000820: 6576 6f6c 7574 696f 6e20 6672 6571 7565  evolution freque
-00000830: 6e63 7920 5b31 2f73 5d20 6f66 2073 6967  ncy [1/s] of sig
-00000840: 6e61 6c20 2861 6674 6572 2064 656d 6f64  nal (after demod
-00000850: 756c 6174 696f 6e29 0d0a 2020 2020 545f  ulation)..    T_
-00000860: 7361 6d70 6c69 6e67 203a 2066 6c6f 6174  sampling : float
-00000870: 0d0a 2020 2020 2020 2020 5361 6d70 6c69  ..        Sampli
-00000880: 6e67 2070 6572 696f 6420 2874 656d 706f  ng period (tempo
-00000890: 7261 6c20 6269 6e20 7369 7a65 2920 5b73  ral bin size) [s
-000008a0: 5d20 6f66 2074 6865 2073 6967 6e61 6c0d  ] of the signal.
-000008b0: 0a0d 0a20 2020 2052 6574 7572 6e73 0d0a  ...    Returns..
-000008c0: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
-000008d0: 2066 6c6f 6174 2061 7272 6179 0d0a 2020   float array..  
-000008e0: 2020 2020 2020 4465 6d6f 6475 6c61 7465        Demodulate
-000008f0: 6420 7369 676e 616c 2061 7420 665f 6669  d signal at f_fi
-00000900: 6e61 6c0d 0a0d 0a20 2020 2022 2222 0d0a  nal....    """..
-00000910: 0d0a 2020 2020 6966 206c 656e 2873 6967  ..    if len(sig
-00000920: 6e61 6c29 203c 2032 3a0d 0a20 2020 2020  nal) < 2:..     
-00000930: 2020 2023 5479 7065 4572 726f 720d 0a20     #TypeError.. 
-00000940: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
-00000950: 7469 6d65 4572 726f 7228 2245 5252 4f52  timeError("ERROR
-00000960: 2069 6e20 6669 6c74 6572 732e 7079 2f64   in filters.py/d
-00000970: 656d 6f64 756c 6174 6f72 3a20 7369 676e  emodulator: sign
-00000980: 616c 2073 686f 756c 6422 202b 0d0a 2020  al should" +..  
-00000990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009a0: 2020 2020 2020 2020 2022 2062 6520 616e           " be an
-000009b0: 2061 7272 6179 2122 290d 0a20 2020 2064   array!")..    d
-000009c0: 656c 7461 5f70 6869 203d 2028 6f6d 6567  elta_phi = (omeg
-000009d0: 615f 6920 2d20 6f6d 6567 615f 6629 2a54  a_i - omega_f)*T
-000009e0: 5f73 616d 706c 696e 6720 2a20 6e70 2e61  _sampling * np.a
-000009f0: 7261 6e67 6528 6c65 6e28 7369 676e 616c  range(len(signal
-00000a00: 2929 0d0a 2020 2020 2320 5072 6520 636f  ))..    # Pre co
-00000a10: 6d70 7574 6520 7369 6e65 2061 6e64 2063  mpute sine and c
-00000a20: 6f73 696e 6520 666f 7220 7370 6565 6420  osine for speed 
-00000a30: 7570 0d0a 2020 2020 6373 203d 206e 702e  up..    cs = np.
-00000a40: 636f 7328 6465 6c74 615f 7068 6929 0d0a  cos(delta_phi)..
-00000a50: 2020 2020 736e 203d 206e 702e 7369 6e28      sn = np.sin(
-00000a60: 6465 6c74 615f 7068 6929 0d0a 2020 2020  delta_phi)..    
-00000a70: 495f 6e65 7720 3d20 6373 2a73 6967 6e61  I_new = cs*signa
-00000a80: 6c2e 7265 616c 202d 2073 6e2a 7369 676e  l.real - sn*sign
-00000a90: 616c 2e69 6d61 670d 0a20 2020 2051 5f6e  al.imag..    Q_n
-00000aa0: 6577 203d 2073 6e2a 7369 676e 616c 2e72  ew = sn*signal.r
-00000ab0: 6561 6c20 2b20 6373 2a73 6967 6e61 6c2e  eal + cs*signal.
-00000ac0: 696d 6167 0d0a 0d0a 2020 2020 7265 7475  imag....    retu
-00000ad0: 726e 2049 5f6e 6577 202b 2031 6a2a 515f  rn I_new + 1j*Q_
-00000ae0: 6e65 770d 0a0d 0a0d 0a64 6566 2072 665f  new......def rf_
-00000af0: 6265 616d 5f63 7572 7265 6e74 2850 726f  beam_current(Pro
-00000b00: 6669 6c65 2c20 6f6d 6567 615f 632c 2054  file, omega_c, T
-00000b10: 5f72 6576 2c20 6c70 663d 5472 7565 293a  _rev, lpf=True):
-00000b20: 0d0a 2020 2020 7222 2222 4675 6e63 7469  ..    r"""Functi
-00000b30: 6f6e 2063 616c 6375 6c61 7469 6e67 2074  on calculating t
-00000b40: 6865 2062 6561 6d20 6368 6172 6765 2061  he beam charge a
-00000b50: 7420 7468 6520 2852 4629 2066 7265 7175  t the (RF) frequ
-00000b60: 656e 6379 2c20 736c 6963 6520 6279 0d0a  ency, slice by..
-00000b70: 2020 2020 736c 6963 652e 2054 6865 2063      slice. The c
-00000b80: 6861 7267 6520 6469 7374 7269 6275 7469  harge distributi
-00000b90: 6f6e 205b 435d 206f 6620 7468 6520 6265  on [C] of the be
-00000ba0: 616d 2069 7320 6465 7465 726d 696e 6564  am is determined
-00000bb0: 2066 726f 6d20 7468 6520 6265 616d 0d0a   from the beam..
-00000bc0: 2020 2020 7072 6f66 696c 6520 3a6d 6174      profile :mat
-00000bd0: 683a 605c 6c61 6d62 6461 5f69 602c 2074  h:`\lambda_i`, t
-00000be0: 6865 2070 6172 7469 636c 6520 6368 6172  he particle char
-00000bf0: 6765 203a 6d61 7468 3a60 715f 7060 2061  ge :math:`q_p` a
-00000c00: 6e64 2074 6865 2072 6561 6c20 7673 2e0d  nd the real vs..
-00000c10: 0a20 2020 206d 6163 726f 2d70 6172 7469  .    macro-parti
-00000c20: 636c 6520 7261 7469 6f20 3a6d 6174 683a  cle ratio :math:
-00000c30: 604e 5f7b 5c6d 6174 6873 667b 7265 616c  `N_{\mathsf{real
-00000c40: 7d7d 2f4e 5f7b 5c6d 6174 6873 667b 6d61  }}/N_{\mathsf{ma
-00000c50: 6372 6f7d 7d60 0d0a 0d0a 2020 2020 2e2e  cro}}`....    ..
-00000c60: 206d 6174 683a 3a0d 0a20 2020 2020 2020   math::..       
-00000c70: 2051 5f69 203d 205c 6672 6163 7b4e 5f7b   Q_i = \frac{N_{
-00000c80: 5c6d 6174 6873 667b 7265 616c 7d7d 7d7b  \mathsf{real}}}{
-00000c90: 4e5f 7b5c 6d61 7468 7366 7b6d 6163 726f  N_{\mathsf{macro
-00000ca0: 7d7d 7d20 715f 7020 5c6c 616d 6264 615f  }}} q_p \lambda_
-00000cb0: 690d 0a0d 0a20 2020 2054 6865 2074 6f74  i....    The tot
-00000cc0: 616c 2063 6861 7267 6520 5b43 5d20 696e  al charge [C] in
-00000cd0: 2074 6865 2062 6561 6d20 6973 2074 6865   the beam is the
-00000ce0: 6e0d 0a0d 0a20 2020 202e 2e20 6d61 7468  n....    .. math
-00000cf0: 3a3a 0d0a 2020 2020 2020 2020 515f 7b5c  ::..        Q_{\
-00000d00: 6d61 7468 7366 7b74 6f74 7d7d 203d 205c  mathsf{tot}} = \
-00000d10: 7375 6d5f 697b 515f 697d 0d0a 0d0a 2020  sum_i{Q_i}....  
-00000d20: 2020 5468 6520 4443 2062 6561 6d20 6375    The DC beam cu
-00000d30: 7272 656e 7420 5b41 5d20 6973 2074 6865  rrent [A] is the
-00000d40: 2074 6f74 616c 206e 756d 6265 7220 6f66   total number of
-00000d50: 2063 6861 7267 6573 2070 6572 2074 7572   charges per tur
-00000d60: 6e20 3a6d 6174 683a 6054 5f30 600d 0a0d  n :math:`T_0`...
-00000d70: 0a20 2020 202e 2e20 6d61 7468 3a3a 2049  .    .. math:: I
-00000d80: 5f7b 5c6d 6174 6873 667b 4443 7d7d 203d  _{\mathsf{DC}} =
-00000d90: 205c 6672 6163 7b51 5f7b 5c6d 6174 6873   \frac{Q_{\maths
-00000da0: 667b 746f 747d 7d7d 7b54 5f30 7d0d 0a0d  f{tot}}}{T_0}...
-00000db0: 0a20 2020 2054 6865 2052 4620 6265 616d  .    The RF beam
-00000dc0: 2063 6861 7267 6520 6469 7374 7269 6275   charge distribu
-00000dd0: 7469 6f6e 205b 435d 2061 7420 6120 7265  tion [C] at a re
-00000de0: 766f 6c75 7469 6f6e 2066 7265 7175 656e  volution frequen
-00000df0: 6379 0d0a 2020 2020 3a6d 6174 683a 605c  cy..    :math:`\
-00000e00: 6f6d 6567 615f 6360 2069 7320 7468 6520  omega_c` is the 
-00000e10: 636f 6d70 6c65 7820 7175 616e 7469 7479  complex quantity
-00000e20: 0d0a 0d0a 2020 2020 2e2e 206d 6174 683a  ....    .. math:
-00000e30: 3a0d 0a20 2020 2020 2020 205c 6c65 6674  :..        \left
-00000e40: 2820 5c62 6567 696e 7b6d 6174 7269 787d  ( \begin{matrix}
-00000e50: 2049 5f7b 7266 2c69 7d20 5c5c 0d0a 2020   I_{rf,i} \\..  
-00000e60: 2020 2020 2020 515f 7b72 662c 697d 205c        Q_{rf,i} \
-00000e70: 656e 647b 6d61 7472 6978 7d20 5c72 6967  end{matrix} \rig
-00000e80: 6874 290d 0a20 2020 2020 2020 203d 2032  ht)..        = 2
-00000e90: 2051 5f69 205c 6c65 6674 2820 5c62 6567   Q_i \left( \beg
-00000ea0: 696e 7b6d 6174 7269 787d 205c 636f 7328  in{matrix} \cos(
-00000eb0: 5c6f 6d65 6761 5f63 2074 5f69 2920 5c5c  \omega_c t_i) \\
-00000ec0: 0d0a 2020 2020 2020 2020 5c73 696e 285c  ..        \sin(\
-00000ed0: 6f6d 6567 615f 6320 745f 6929 5c65 6e64  omega_c t_i)\end
-00000ee0: 7b6d 6174 7269 787d 205c 7269 6768 7429  {matrix} \right)
-00000ef0: 205c 2c20 2c0d 0a0d 0a20 2020 2077 6865   \, ,....    whe
-00000f00: 7265 203a 6d61 7468 3a60 745f 6960 2061  re :math:`t_i` a
-00000f10: 7265 2074 6865 2074 696d 6520 636f 6f72  re the time coor
-00000f20: 6469 6e61 7465 7320 6f66 2074 6865 2062  dinates of the b
-00000f30: 6561 6d20 7072 6f66 696c 652e 2041 6674  eam profile. Aft
-00000f40: 6572 2064 652d 0d0a 2020 2020 6d6f 6475  er de-..    modu
-00000f50: 6c61 7469 6f6e 2c20 6120 6c6f 772d 7061  lation, a low-pa
-00000f60: 7373 2066 696c 7465 7220 6174 2032 3020  ss filter at 20 
-00000f70: 4d48 7a20 6973 2061 7070 6c69 6564 2e0d  MHz is applied..
-00000f80: 0a0d 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-00000f90: 730d 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  s..    ---------
-00000fa0: 2d0d 0a20 2020 2050 726f 6669 6c65 203a  -..    Profile :
-00000fb0: 2063 6c61 7373 0d0a 2020 2020 2020 2020   class..        
-00000fc0: 4120 5072 6f66 696c 6520 7479 7065 2063  A Profile type c
-00000fd0: 6c61 7373 0d0a 2020 2020 6f6d 6567 615f  lass..    omega_
-00000fe0: 6320 3a20 666c 6f61 740d 0a20 2020 2020  c : float..     
-00000ff0: 2020 2052 6576 6f6c 7574 696f 6e20 6672     Revolution fr
-00001000: 6571 7565 6e63 7920 5b31 2f73 5d20 6174  equency [1/s] at
-00001010: 2077 6869 6368 2074 6865 2063 7572 7265   which the curre
-00001020: 6e74 2073 686f 756c 6420 6265 2063 616c  nt should be cal
-00001030: 6375 6c61 7465 640d 0a20 2020 2054 5f72  culated..    T_r
-00001040: 6576 203a 2066 6c6f 6174 0d0a 2020 2020  ev : float..    
-00001050: 2020 2020 5265 766f 6c75 7469 6f6e 2070      Revolution p
-00001060: 6572 696f 6420 5b73 5d20 6f66 2074 6865  eriod [s] of the
-00001070: 206d 6163 6869 6e65 0d0a 2020 2020 6c70   machine..    lp
-00001080: 6620 3a20 626f 6f6c 0d0a 2020 2020 2020  f : bool..      
-00001090: 2020 4170 706c 7920 6c6f 772d 7061 7373    Apply low-pass
-000010a0: 2066 696c 7465 723b 2064 6566 6175 6c74   filter; default
-000010b0: 2069 7320 5472 7565 0d0a 0d0a 2020 2020   is True....    
-000010c0: 5265 7475 726e 730d 0a20 2020 202d 2d2d  Returns..    ---
-000010d0: 2d2d 2d2d 0d0a 2020 2020 636f 6d70 6c65  ----..    comple
-000010e0: 7820 6172 7261 790d 0a20 2020 2020 2020  x array..       
-000010f0: 2052 4620 6265 616d 2063 6861 7267 6520   RF beam charge 
-00001100: 6172 7261 7920 5b43 5d20 6174 2027 6672  array [C] at 'fr
-00001110: 6571 7565 6e63 7927 206f 6d65 6761 5f63  equency' omega_c
-00001120: 2e20 546f 206f 6274 6169 6e20 6375 7272  . To obtain curr
-00001130: 656e 742c 0d0a 2020 2020 2020 2020 6469  ent,..        di
-00001140: 7669 6465 2062 7920 7468 6520 7361 6d70  vide by the samp
-00001150: 6c69 6e67 2074 696d 650d 0a0d 0a20 2020  ling time....   
-00001160: 2022 2222 0d0a 0d0a 2020 2020 2320 436f   """....    # Co
-00001170: 6e76 6572 7420 6672 6f6d 2064 696d 656e  nvert from dimen
-00001180: 7369 6f6e 6c65 7373 2074 6f20 436f 756c  sionless to Coul
-00001190: 6f6d 622f 416d 70c3 a872 6573 0d0a 2020  omb/Amp..res..  
-000011a0: 2020 2320 5461 6b65 2069 6e74 6f20 6163    # Take into ac
-000011b0: 636f 756e 7420 6d61 6372 6f2d 7061 7274  count macro-part
-000011c0: 6963 6c65 2063 6861 7267 6520 7769 7468  icle charge with
-000011d0: 2072 6561 6c2d 746f 2d6d 6163 726f 2d70   real-to-macro-p
-000011e0: 6172 7469 636c 6520 7261 7469 6f0d 0a20  article ratio.. 
-000011f0: 2020 2063 6861 7267 6573 203d 2050 726f     charges = Pro
-00001200: 6669 6c65 2e42 6561 6d2e 7261 7469 6f2a  file.Beam.ratio*
-00001210: 5072 6f66 696c 652e 4265 616d 2e50 6172  Profile.Beam.Par
-00001220: 7469 636c 652e 6368 6172 6765 2a65 5c0d  ticle.charge*e\.
-00001230: 0a20 2020 2020 2020 202a 206e 702e 636f  .        * np.co
-00001240: 7079 2850 726f 6669 6c65 2e6e 5f6d 6163  py(Profile.n_mac
-00001250: 726f 7061 7274 6963 6c65 7329 0d0a 2020  roparticles)..  
-00001260: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-00001270: 5375 6d20 6f66 2070 6172 7469 636c 6573  Sum of particles
-00001280: 3a20 2564 2c20 746f 7461 6c20 6368 6172  : %d, total char
-00001290: 6765 3a20 252e 3465 2043 222c 0d0a 2020  ge: %.4e C",..  
-000012a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000012b0: 702e 7375 6d28 5072 6f66 696c 652e 6e5f  p.sum(Profile.n_
-000012c0: 6d61 6372 6f70 6172 7469 636c 6573 292c  macroparticles),
-000012d0: 206e 702e 7375 6d28 6368 6172 6765 7329   np.sum(charges)
-000012e0: 290d 0a20 2020 206c 6f67 6765 722e 6465  )..    logger.de
-000012f0: 6275 6728 2244 4320 6375 7272 656e 7420  bug("DC current 
-00001300: 6973 2025 2e34 6520 4122 2c20 6e70 2e73  is %.4e A", np.s
-00001310: 756d 2863 6861 7267 6573 292f 545f 7265  um(charges)/T_re
-00001320: 7629 0d0a 0d0a 2020 2020 2320 4d69 7820  v)....    # Mix 
-00001330: 7769 7468 2066 7265 7175 656e 6379 206f  with frequency o
-00001340: 6620 696e 7465 7265 7374 3b20 7265 6d65  f interest; reme
-00001350: 6d62 6572 2066 6163 746f 7220 3220 6465  mber factor 2 de
-00001360: 6d6f 6475 6c61 7469 6f6e 0d0a 2020 2020  modulation..    
-00001370: 495f 6620 3d20 322e 2a63 6861 7267 6573  I_f = 2.*charges
-00001380: 2a6e 702e 636f 7328 6f6d 6567 615f 632a  *np.cos(omega_c*
-00001390: 5072 6f66 696c 652e 6269 6e5f 6365 6e74  Profile.bin_cent
-000013a0: 6572 7329 0d0a 2020 2020 515f 6620 3d20  ers)..    Q_f = 
-000013b0: 322e 2a63 6861 7267 6573 2a6e 702e 7369  2.*charges*np.si
-000013c0: 6e28 6f6d 6567 615f 632a 5072 6f66 696c  n(omega_c*Profil
-000013d0: 652e 6269 6e5f 6365 6e74 6572 7329 0d0a  e.bin_centers)..
-000013e0: 0d0a 2020 2020 2320 5061 7373 2074 6872  ..    # Pass thr
-000013f0: 6f75 6768 2061 206c 6f77 2d70 6173 7320  ough a low-pass 
-00001400: 6669 6c74 6572 0d0a 2020 2020 6966 206c  filter..    if l
-00001410: 7066 2069 7320 5472 7565 3a0d 0a20 2020  pf is True:..   
-00001420: 2020 2020 2023 204e 7971 7569 7374 2066       # Nyquist f
-00001430: 7265 7175 656e 6379 2030 2e35 2a66 5f73  requency 0.5*f_s
-00001440: 6c69 6365 733b 2063 7574 6f66 6620 6174  lices; cutoff at
-00001450: 2032 3020 4d48 7a0d 0a20 2020 2020 2020   20 MHz..       
-00001460: 2063 7574 6f66 6620 3d20 3230 2e65 362a   cutoff = 20.e6*
-00001470: 322e 2a50 726f 6669 6c65 2e62 696e 5f73  2.*Profile.bin_s
-00001480: 697a 650d 0a20 2020 2020 2020 2049 5f66  ize..        I_f
-00001490: 203d 206c 6f77 5f70 6173 735f 6669 6c74   = low_pass_filt
-000014a0: 6572 2849 5f66 2c20 6375 746f 6666 5f66  er(I_f, cutoff_f
-000014b0: 7265 7175 656e 6379 3d63 7574 6f66 6629  requency=cutoff)
-000014c0: 0d0a 2020 2020 2020 2020 515f 6620 3d20  ..        Q_f = 
-000014d0: 6c6f 775f 7061 7373 5f66 696c 7465 7228  low_pass_filter(
-000014e0: 515f 662c 2063 7574 6f66 665f 6672 6571  Q_f, cutoff_freq
-000014f0: 7565 6e63 793d 6375 746f 6666 290d 0a20  uency=cutoff).. 
-00001500: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00001510: 2252 4620 746f 7461 6c20 6375 7272 656e  "RF total curren
-00001520: 7420 6973 2025 2e34 6520 4122 2c20 6e70  t is %.4e A", np
-00001530: 2e66 6162 7328 6e70 2e73 756d 2849 5f66  .fabs(np.sum(I_f
-00001540: 2929 2f54 5f72 6576 290d 0a0d 0a20 2020  ))/T_rev)....   
-00001550: 2072 6574 7572 6e20 495f 6620 2b20 316a   return I_f + 1j
-00001560: 2a51 5f66 0d0a 0d0a 0d0a 6465 6620 636f  *Q_f......def co
-00001570: 6d62 5f66 696c 7465 7228 792c 2078 2c20  mb_filter(y, x, 
-00001580: 6129 3a0d 0a20 2020 2022 2222 4665 6564  a):..    """Feed
-00001590: 6261 636b 2063 6f6d 6220 6669 6c74 6572  back comb filter
-000015a0: 2e0d 0a20 2020 2022 2222 0d0a 0d0a 2020  ...    """....  
-000015b0: 2020 7265 7475 726e 2061 2a79 202b 2028    return a*y + (
-000015c0: 3120 2d20 6129 2a78 0d0a 0d0a 0d0a 6465  1 - a)*x......de
-000015d0: 6620 6c6f 775f 7061 7373 5f66 696c 7465  f low_pass_filte
-000015e0: 7228 7369 676e 616c 2c20 6375 746f 6666  r(signal, cutoff
-000015f0: 5f66 7265 7175 656e 6379 3d30 2e35 293a  _frequency=0.5):
-00001600: 0d0a 2020 2020 2222 224c 6f77 2d70 6173  ..    """Low-pas
-00001610: 7320 6669 6c74 6572 2062 6173 6564 206f  s filter based o
-00001620: 6e20 4275 7474 6572 776f 7274 6820 3574  n Butterworth 5t
-00001630: 6820 6f72 6465 7220 6469 6769 7461 6c20  h order digital 
-00001640: 6669 6c74 6572 2066 726f 6d0d 0a20 2020  filter from..   
-00001650: 2073 6369 7079 2c0d 0a20 2020 2068 7474   scipy,..    htt
-00001660: 703a 2f2f 646f 6373 2e73 6369 7079 2e6f  p://docs.scipy.o
-00001670: 7267 0d0a 0d0a 2020 2020 5061 7261 6d65  rg....    Parame
-00001680: 7465 7273 0d0a 2020 2020 2d2d 2d2d 2d2d  ters..    ------
-00001690: 2d2d 2d2d 0d0a 2020 2020 7369 676e 616c  ----..    signal
-000016a0: 203a 2066 6c6f 6174 2061 7272 6179 0d0a   : float array..
-000016b0: 2020 2020 2020 2020 5369 676e 616c 2074          Signal t
-000016c0: 6f20 6265 2066 696c 7465 7265 640d 0a20  o be filtered.. 
-000016d0: 2020 2063 7574 6f66 665f 6672 6571 7565     cutoff_freque
-000016e0: 6e63 7920 3a20 666c 6f61 740d 0a20 2020  ncy : float..   
-000016f0: 2020 2020 2043 7574 6f66 6620 6672 6571       Cutoff freq
-00001700: 7565 6e63 7920 5b31 5d20 636f 7272 6573  uency [1] corres
-00001710: 706f 6e64 696e 6720 746f 2061 2033 2064  ponding to a 3 d
-00001720: 4220 6761 696e 2064 726f 702c 2072 656c  B gain drop, rel
-00001730: 6174 6976 6520 746f 2074 6865 0d0a 2020  ative to the..  
-00001740: 2020 2020 2020 4e79 7175 6973 7420 6672        Nyquist fr
-00001750: 6571 7565 6e63 7920 6f66 2031 3b20 6465  equency of 1; de
-00001760: 6661 756c 7420 6973 2030 2e35 0d0a 0d0a  fault is 0.5....
-00001770: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
-00001780: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 666c   -------..    fl
-00001790: 6f61 7420 6172 7261 790d 0a20 2020 2020  oat array..     
-000017a0: 2020 204c 6f77 2d70 6173 7320 6669 6c74     Low-pass filt
-000017b0: 6572 6564 2073 6967 6e61 6c0d 0a0d 0a20  ered signal.... 
-000017c0: 2020 2022 2222 0d0a 0d0a 2020 2020 622c     """....    b,
-000017d0: 2061 203d 2073 676e 2e62 7574 7465 7228   a = sgn.butter(
-000017e0: 352c 2063 7574 6f66 665f 6672 6571 7565  5, cutoff_freque
-000017f0: 6e63 792c 2027 6c6f 7727 2c20 616e 616c  ncy, 'low', anal
-00001800: 6f67 3d46 616c 7365 290d 0a0d 0a20 2020  og=False)....   
-00001810: 2072 6574 7572 6e20 7367 6e2e 6669 6c74   return sgn.filt
-00001820: 6669 6c74 2862 2c20 612c 2073 6967 6e61  filt(b, a, signa
-00001830: 6c29 0d0a 0d0a 0d0a 6465 6620 6d6f 7669  l)......def movi
-00001840: 6e67 5f61 7665 7261 6765 2878 2c20 4e2c  ng_average(x, N,
-00001850: 2078 5f70 7265 763d 4e6f 6e65 293a 0d0a   x_prev=None):..
-00001860: 2020 2020 2222 2246 756e 6374 696f 6e20      """Function 
-00001870: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
-00001880: 206d 6f76 696e 6720 6176 6572 6167 6520   moving average 
-00001890: 286f 7220 7275 6e6e 696e 6720 6d65 616e  (or running mean
-000018a0: 2920 6f66 2074 6865 2069 6e70 7574 0d0a  ) of the input..
-000018b0: 2020 2020 6461 7461 2e0d 0a0d 0a20 2020      data.....   
-000018c0: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
-000018d0: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
-000018e0: 2078 203a 2066 6c6f 6174 2061 7272 6179   x : float array
-000018f0: 0d0a 2020 2020 2020 2020 4461 7461 2074  ..        Data t
-00001900: 6f20 6265 2073 6d6f 6f74 6865 640d 0a20  o be smoothed.. 
-00001910: 2020 204e 203a 2069 6e74 0d0a 2020 2020     N : int..    
-00001920: 2020 2020 5769 6e64 6f77 2073 697a 6520      Window size 
-00001930: 696e 2070 6f69 6e74 730d 0a20 2020 2078  in points..    x
-00001940: 5f70 7265 7620 3a20 666c 6f61 7420 6172  _prev : float ar
-00001950: 7261 790d 0a20 2020 2020 2020 2044 6174  ray..        Dat
-00001960: 6120 746f 2070 6164 2077 6974 6820 696e  a to pad with in
-00001970: 2066 726f 6e74 0d0a 0d0a 2020 2020 5265   front....    Re
-00001980: 7475 726e 730d 0a20 2020 202d 2d2d 2d2d  turns..    -----
-00001990: 2d2d 0d0a 2020 2020 666c 6f61 7420 6172  --..    float ar
-000019a0: 7261 790d 0a20 2020 2020 2020 2053 6d6f  ray..        Smo
-000019b0: 6f74 6865 6420 6461 7461 2061 7272 6179  othed data array
-000019c0: 206f 6620 7369 7a65 0d0a 2020 2020 2020   of size..      
-000019d0: 2020 2020 2020 2a20 6c65 6e28 7829 202d        * len(x) -
-000019e0: 204e 202b 2031 2c20 6966 2078 5f70 7265   N + 1, if x_pre
-000019f0: 7620 3d20 4e6f 6e65 0d0a 2020 2020 2020  v = None..      
-00001a00: 2020 2020 2020 2a20 6c65 6e28 7829 202b        * len(x) +
-00001a10: 206c 656e 2878 5f70 7265 7629 202d 204e   len(x_prev) - N
-00001a20: 202b 2031 2c20 6966 2078 5f70 7265 7620   + 1, if x_prev 
-00001a30: 6769 7665 6e0d 0a0d 0a20 2020 2022 2222  given....    """
-00001a40: 0d0a 0d0a 2020 2020 6966 2078 5f70 7265  ....    if x_pre
-00001a50: 7620 6973 206e 6f74 204e 6f6e 653a 0d0a  v is not None:..
-00001a60: 2020 2020 2020 2020 2320 5061 6420 696e          # Pad in
-00001a70: 2066 726f 6e74 2077 6974 6820 785f 7072   front with x_pr
-00001a80: 6576 2073 6967 6e61 6c0d 0a20 2020 2020  ev signal..     
-00001a90: 2020 2078 203d 206e 702e 636f 6e63 6174     x = np.concat
-00001aa0: 656e 6174 6528 2878 5f70 7265 762c 2078  enate((x_prev, x
-00001ab0: 2929 0d0a 0d0a 2020 2020 2320 6261 7365  ))....    # base
-00001ac0: 6420 6f6e 2068 7474 7073 3a2f 2f73 7461  d on https://sta
-00001ad0: 636b 6f76 6572 666c 6f77 2e63 6f6d 2f61  ckoverflow.com/a
-00001ae0: 2f31 3433 3134 3035 340d 0a20 2020 206d  /14314054..    m
-00001af0: 6f76 5f61 7667 203d 206e 702e 6375 6d73  ov_avg = np.cums
-00001b00: 756d 2878 290d 0a20 2020 206d 6f76 5f61  um(x)..    mov_a
-00001b10: 7667 5b4e 3a5d 203d 206d 6f76 5f61 7667  vg[N:] = mov_avg
-00001b20: 5b4e 3a5d 202d 206d 6f76 5f61 7667 5b3a  [N:] - mov_avg[:
-00001b30: 2d4e 5d0d 0a20 2020 2072 6574 7572 6e20  -N]..    return 
-00001b40: 6d6f 765f 6176 675b 4e2d 313a 5d20 2f20  mov_avg[N-1:] / 
-00001b50: 4e0d 0a                                  N..
+00000000: 0d0a 2320 436f 7079 7269 6768 7420 3230  ..# Copyright 20
+00000010: 3134 2d32 3031 3720 4345 524e 2e20 5468  14-2017 CERN. Th
+00000020: 6973 2073 6f66 7477 6172 6520 6973 2064  is software is d
+00000030: 6973 7472 6962 7574 6564 2075 6e64 6572  istributed under
+00000040: 2074 6865 0d0a 2320 7465 726d 7320 6f66   the..# terms of
+00000050: 2074 6865 2047 4e55 2047 656e 6572 616c   the GNU General
+00000060: 2050 7562 6c69 6320 4c69 6365 6e63 6520   Public Licence 
+00000070: 7665 7273 696f 6e20 3320 2847 504c 2056  version 3 (GPL V
+00000080: 6572 7369 6f6e 2033 292c 200d 0a23 2063  ersion 3), ..# c
+00000090: 6f70 6965 6420 7665 7262 6174 696d 2069  opied verbatim i
+000000a0: 6e20 7468 6520 6669 6c65 204c 4943 454e  n the file LICEN
+000000b0: 4345 2e6d 642e 0d0a 2320 496e 2061 7070  CE.md...# In app
+000000c0: 6c79 696e 6720 7468 6973 206c 6963 656e  lying this licen
+000000d0: 6365 2c20 4345 524e 2064 6f65 7320 6e6f  ce, CERN does no
+000000e0: 7420 7761 6976 6520 7468 6520 7072 6976  t waive the priv
+000000f0: 696c 6567 6573 2061 6e64 2069 6d6d 756e  ileges and immun
+00000100: 6974 6965 7320 0d0a 2320 6772 616e 7465  ities ..# grante
+00000110: 6420 746f 2069 7420 6279 2076 6972 7475  d to it by virtu
+00000120: 6520 6f66 2069 7473 2073 7461 7475 7320  e of its status 
+00000130: 6173 2061 6e20 496e 7465 7267 6f76 6572  as an Intergover
+00000140: 6e6d 656e 7461 6c20 4f72 6761 6e69 7a61  nmental Organiza
+00000150: 7469 6f6e 206f 720d 0a23 2073 7562 6d69  tion or..# submi
+00000160: 7420 6974 7365 6c66 2074 6f20 616e 7920  t itself to any 
+00000170: 6a75 7269 7364 6963 7469 6f6e 2e0d 0a23  jurisdiction...#
+00000180: 2050 726f 6a65 6374 2077 6562 7369 7465   Project website
+00000190: 3a20 6874 7470 3a2f 2f62 6c6f 6e64 2e77  : http://blond.w
+000001a0: 6562 2e63 6572 6e2e 6368 2f0d 0a0d 0a27  eb.cern.ch/....'
+000001b0: 2727 0d0a 4578 616d 706c 6520 7363 7269  ''..Example scri
+000001c0: 7074 2074 6f20 7461 6b65 2069 6e74 6f20  pt to take into 
+000001d0: 6163 636f 756e 7420 696e 7465 6e73 6974  account intensit
+000001e0: 7920 6566 6665 6374 7320 7769 7468 206d  y effects with m
+000001f0: 756c 7469 2d74 7572 6e20 7761 6b65 730d  ulti-turn wakes.
+00000200: 0a45 7861 6d70 6c65 2066 6f72 2074 6865  .Example for the
+00000210: 2050 5342 2077 6974 6820 6120 6e61 7272   PSB with a narr
+00000220: 6f77 2d62 616e 6420 7265 736f 6e61 746f  ow-band resonato
+00000230: 722c 2074 6f20 6368 6563 6b20 526f 6269  r, to check Robi
+00000240: 6e73 6f6e 2069 6e73 7461 6269 6c69 7479  nson instability
+00000250: 0d0a 0d0a 3a41 7574 686f 7273 3a20 2a2a  ....:Authors: **
+00000260: 4a75 616e 2046 2e20 4573 7465 6261 6e20  Juan F. Esteban 
+00000270: 4d75 656c 6c65 722a 2a0d 0a27 2727 0d0a  Mueller**..'''..
+00000280: 0d0a 6672 6f6d 205f 5f66 7574 7572 655f  ..from __future_
+00000290: 5f20 696d 706f 7274 2064 6976 6973 696f  _ import divisio
+000002a0: 6e0d 0a66 726f 6d20 5f5f 6675 7475 7265  n..from __future
+000002b0: 5f5f 2069 6d70 6f72 7420 7072 696e 745f  __ import print_
+000002c0: 6675 6e63 7469 6f6e 0d0a 6672 6f6d 2062  function..from b
+000002d0: 7569 6c74 696e 7320 696d 706f 7274 2072  uiltins import r
+000002e0: 616e 6765 0d0a 696d 706f 7274 206f 730d  ange..import os.
+000002f0: 0a69 6d70 6f72 7420 6e75 6d70 7920 6173  .import numpy as
+00000300: 206e 700d 0a69 6d70 6f72 7420 7079 6c61   np..import pyla
+00000310: 6220 6173 2070 6c74 0d0a 6672 6f6d 2062  b as plt..from b
+00000320: 6c6f 6e64 2e69 6e70 7574 5f70 6172 616d  lond.input_param
+00000330: 6574 6572 732e 7269 6e67 2069 6d70 6f72  eters.ring impor
+00000340: 7420 5269 6e67 0d0a 6672 6f6d 2062 6c6f  t Ring..from blo
+00000350: 6e64 2e69 6e70 7574 5f70 6172 616d 6574  nd.input_paramet
+00000360: 6572 732e 7266 5f70 6172 616d 6574 6572  ers.rf_parameter
+00000370: 7320 696d 706f 7274 2052 4653 7461 7469  s import RFStati
+00000380: 6f6e 0d0a 6672 6f6d 2062 6c6f 6e64 2e74  on..from blond.t
+00000390: 7261 636b 6572 732e 7472 6163 6b65 7220  rackers.tracker 
+000003a0: 696d 706f 7274 2052 696e 6741 6e64 5246  import RingAndRF
+000003b0: 5472 6163 6b65 722c 2046 756c 6c52 696e  Tracker, FullRin
+000003c0: 6741 6e64 5246 0d0a 6672 6f6d 2062 6c6f  gAndRF..from blo
+000003d0: 6e64 2e62 6561 6d2e 6265 616d 2069 6d70  nd.beam.beam imp
+000003e0: 6f72 7420 4265 616d 2c20 5072 6f74 6f6e  ort Beam, Proton
+000003f0: 0d0a 6672 6f6d 2062 6c6f 6e64 2e62 6561  ..from blond.bea
+00000400: 6d2e 6469 7374 7269 6275 7469 6f6e 7320  m.distributions 
+00000410: 696d 706f 7274 206d 6174 6368 6564 5f66  import matched_f
+00000420: 726f 6d5f 6469 7374 7269 6275 7469 6f6e  rom_distribution
+00000430: 5f66 756e 6374 696f 6e0d 0a66 726f 6d20  _function..from 
+00000440: 626c 6f6e 642e 6265 616d 2e70 726f 6669  blond.beam.profi
+00000450: 6c65 2069 6d70 6f72 7420 5072 6f66 696c  le import Profil
+00000460: 652c 2043 7574 4f70 7469 6f6e 730d 0a66  e, CutOptions..f
+00000470: 726f 6d20 626c 6f6e 642e 696d 7065 6461  rom blond.impeda
+00000480: 6e63 6573 2e69 6d70 6564 616e 6365 2069  nces.impedance i
+00000490: 6d70 6f72 7420 496e 6475 6365 6456 6f6c  mport InducedVol
+000004a0: 7461 6765 4672 6571 2c20 546f 7461 6c49  tageFreq, TotalI
+000004b0: 6e64 7563 6564 566f 6c74 6167 650d 0a66  nducedVoltage..f
+000004c0: 726f 6d20 626c 6f6e 642e 696d 7065 6461  rom blond.impeda
+000004d0: 6e63 6573 2e69 6d70 6564 616e 6365 5f73  nces.impedance_s
+000004e0: 6f75 7263 6573 2069 6d70 6f72 7420 5265  ources import Re
+000004f0: 736f 6e61 746f 7273 0d0a 6672 6f6d 2073  sonators..from s
+00000500: 6369 7079 2e63 6f6e 7374 616e 7473 2069  cipy.constants i
+00000510: 6d70 6f72 7420 632c 2065 2c20 6d5f 700d  mport c, e, m_p.
+00000520: 0a69 6d70 6f72 7420 6d61 7470 6c6f 746c  .import matplotl
+00000530: 6962 2061 7320 6d70 6c0d 0a6d 706c 2e75  ib as mpl..mpl.u
+00000540: 7365 2827 4167 6727 290d 0a0d 0a74 6869  se('Agg')....thi
+00000550: 735f 6469 7265 6374 6f72 7920 3d20 6f73  s_directory = os
+00000560: 2e70 6174 682e 6469 726e 616d 6528 6f73  .path.dirname(os
+00000570: 2e70 6174 682e 7265 616c 7061 7468 285f  .path.realpath(_
+00000580: 5f66 696c 655f 5f29 2920 2b20 272f 270d  _file__)) + '/'.
+00000590: 0a0d 0a6f 732e 6d61 6b65 6469 7273 2874  ...os.makedirs(t
+000005a0: 6869 735f 6469 7265 6374 6f72 7920 2b20  his_directory + 
+000005b0: 272e 2e2f 6f75 7470 7574 5f66 696c 6573  '../output_files
+000005c0: 2f45 585f 3138 5f66 6967 2f27 2c20 6578  /EX_18_fig/', ex
+000005d0: 6973 745f 6f6b 3d54 7275 6529 0d0a 0d0a  ist_ok=True)....
+000005e0: 0d0a 2320 5349 4d55 4c41 5449 4f4e 2050  ..# SIMULATION P
+000005f0: 4152 414d 4554 4552 5320 2d2d 2d2d 2d2d  ARAMETERS ------
+00000600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000630: 2d0d 0a0d 0a23 2042 6561 6d20 7061 7261  -....# Beam para
+00000640: 6d65 7465 7273 0d0a 6e5f 7061 7274 6963  meters..n_partic
+00000650: 6c65 7320 3d20 3165 3131 0d0a 6e5f 6d61  les = 1e11..n_ma
+00000660: 6372 6f70 6172 7469 636c 6573 203d 2031  croparticles = 1
+00000670: 6535 0d0a 6b69 6e5f 6265 616d 5f65 6e65  e5..kin_beam_ene
+00000680: 7267 7920 3d20 312e 3465 3920 2020 2020  rgy = 1.4e9     
+00000690: 2320 5b65 565d 0d0a 0d0a 0d0a 6469 7374  # [eV]......dist
+000006a0: 7269 6275 7469 6f6e 5f74 7970 6520 3d20  ribution_type = 
+000006b0: 2770 6172 6162 6f6c 6963 5f6c 696e 6527  'parabolic_line'
+000006c0: 0d0a 6275 6e63 685f 6c65 6e67 7468 203d  ..bunch_length =
+000006d0: 2031 3030 652d 3920 2020 2020 2020 2023   100e-9        #
+000006e0: 205b 735d 0d0a 0d0a 0d0a 2320 4d61 6368   [s]......# Mach
+000006f0: 696e 6520 616e 6420 5246 2070 6172 616d  ine and RF param
+00000700: 6574 6572 730d 0a72 6164 6975 7320 3d20  eters..radius = 
+00000710: 3235 2e30 0d0a 6761 6d6d 615f 7472 616e  25.0..gamma_tran
+00000720: 7369 7469 6f6e 203d 2034 2e34 0d0a 4320  sition = 4.4..C 
+00000730: 3d20 3220 2a20 6e70 2e70 6920 2a20 7261  = 2 * np.pi * ra
+00000740: 6469 7573 2020 2020 2020 2320 5b6d 5d0d  dius      # [m].
+00000750: 0a0d 0a23 2054 7261 636b 696e 6720 6465  ...# Tracking de
+00000760: 7461 696c 730d 0a6e 5f74 7572 6e73 203d  tails..n_turns =
+00000770: 2069 6e74 2831 3030 3030 290d 0a6e 5f74   int(10000)..n_t
+00000780: 7572 6e73 5f62 6574 7765 656e 5f74 776f  urns_between_two
+00000790: 5f70 6c6f 7473 203d 2035 3030 0d0a 0d0a  _plots = 500....
+000007a0: 2320 4465 7269 7665 6420 7061 7261 6d65  # Derived parame
+000007b0: 7465 7273 0d0a 455f 3020 3d20 6d5f 702a  ters..E_0 = m_p*
+000007c0: 632a 2a32 2f65 2020 2020 2020 2020 2020  c**2/e          
+000007d0: 2020 2320 5b65 565d 0d0a 746f 745f 6265    # [eV]..tot_be
+000007e0: 616d 5f65 6e65 7267 7920 3d20 2045 5f30  am_energy =  E_0
+000007f0: 202b 206b 696e 5f62 6561 6d5f 656e 6572   + kin_beam_ener
+00000800: 6779 2020 2020 2020 2020 2020 2020 2020  gy              
+00000810: 2020 2320 5b65 565d 0d0a 7379 6e63 5f6d    # [eV]..sync_m
+00000820: 6f6d 656e 7475 6d20 3d20 6e70 2e73 7172  omentum = np.sqr
+00000830: 7428 746f 745f 6265 616d 5f65 6e65 7267  t(tot_beam_energ
+00000840: 792a 2a32 202d 2045 5f30 2a2a 3229 2020  y**2 - E_0**2)  
+00000850: 2020 2320 5b65 562f 635d 0d0a 0d0a 6761    # [eV/c]....ga
+00000860: 6d6d 6120 3d20 746f 745f 6265 616d 5f65  mma = tot_beam_e
+00000870: 6e65 7267 7920 2f20 455f 300d 0a62 6574  nergy / E_0..bet
+00000880: 6120 3d20 6e70 2e73 7172 7428 312e 302d  a = np.sqrt(1.0-
+00000890: 312e 302f 6761 6d6d 612a 2a32 2e30 290d  1.0/gamma**2.0).
+000008a0: 0a0d 0a6d 6f6d 656e 7475 6d5f 636f 6d70  ...momentum_comp
+000008b0: 6163 7469 6f6e 203d 2031 202f 2067 616d  action = 1 / gam
+000008c0: 6d61 5f74 7261 6e73 6974 696f 6e2a 2a32  ma_transition**2
+000008d0: 0d0a 0d0a 2320 4361 7669 7469 6573 2070  ....# Cavities p
+000008e0: 6172 616d 6574 6572 730d 0a6e 5f72 665f  arameters..n_rf_
+000008f0: 7379 7374 656d 7320 3d20 310d 0a68 6172  systems = 1..har
+00000900: 6d6f 6e69 635f 6e75 6d62 6572 7320 3d20  monic_numbers = 
+00000910: 310d 0a76 6f6c 7461 6765 5f70 726f 6772  1..voltage_progr
+00000920: 616d 203d 2038 6533 2020 2023 5b56 5d0d  am = 8e3   #[V].
+00000930: 0a70 6869 5f6f 6666 7365 7420 3d20 2d6e  .phi_offset = -n
+00000940: 702e 7069 0d0a 0d0a 0d0a 2320 4445 4649  p.pi......# DEFI
+00000950: 4e45 2052 494e 472d 2d2d 2d2d 2d2d 2d2d  NE RING---------
+00000960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000990: 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a67 656e  ---------....gen
+000009a0: 6572 616c 5f70 6172 616d 7320 3d20 5269  eral_params = Ri
+000009b0: 6e67 2843 2c20 6d6f 6d65 6e74 756d 5f63  ng(C, momentum_c
+000009c0: 6f6d 7061 6374 696f 6e2c 0d0a 2020 2020  ompaction,..    
+000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000009f0: 796e 635f 6d6f 6d65 6e74 756d 2c20 5072  ync_momentum, Pr
+00000a00: 6f74 6f6e 2829 2c20 6e5f 7475 726e 7329  oton(), n_turns)
+00000a10: 0d0a 0d0a 5246 5f73 6374 5f70 6172 203d  ....RF_sct_par =
+00000a20: 2052 4653 7461 7469 6f6e 2867 656e 6572   RFStation(gener
+00000a30: 616c 5f70 6172 616d 732c 205b 6861 726d  al_params, [harm
+00000a40: 6f6e 6963 5f6e 756d 6265 7273 5d2c 205b  onic_numbers], [
+00000a50: 766f 6c74 6167 655f 7072 6f67 7261 6d5d  voltage_program]
+00000a60: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000a70: 2020 2020 2020 2020 2020 5b70 6869 5f6f            [phi_o
+00000a80: 6666 7365 745d 2c20 6e5f 7266 5f73 7973  ffset], n_rf_sys
+00000a90: 7465 6d73 290d 0a0d 0a62 6561 6d20 3d20  tems)....beam = 
+00000aa0: 4265 616d 2867 656e 6572 616c 5f70 6172  Beam(general_par
+00000ab0: 616d 732c 206e 5f6d 6163 726f 7061 7274  ams, n_macropart
+00000ac0: 6963 6c65 732c 206e 5f70 6172 7469 636c  icles, n_particl
+00000ad0: 6573 290d 0a72 696e 675f 5246 5f73 6563  es)..ring_RF_sec
+00000ae0: 7469 6f6e 203d 2052 696e 6741 6e64 5246  tion = RingAndRF
+00000af0: 5472 6163 6b65 7228 5246 5f73 6374 5f70  Tracker(RF_sct_p
+00000b00: 6172 2c20 6265 616d 290d 0a0d 0a66 756c  ar, beam)....ful
+00000b10: 6c5f 7472 6163 6b65 7220 3d20 4675 6c6c  l_tracker = Full
+00000b20: 5269 6e67 416e 6452 4628 5b72 696e 675f  RingAndRF([ring_
+00000b30: 5246 5f73 6563 7469 6f6e 5d29 0d0a 0d0a  RF_section])....
+00000b40: 6673 203d 2052 465f 7363 745f 7061 722e  fs = RF_sct_par.
+00000b50: 6f6d 6567 615f 7330 5b30 5d2f 322f 6e70  omega_s0[0]/2/np
+00000b60: 2e70 690d 0a0d 0a62 7563 6b65 745f 6c65  .pi....bucket_le
+00000b70: 6e67 7468 203d 2032 2e30 202a 206e 702e  ngth = 2.0 * np.
+00000b80: 7069 202f 2052 465f 7363 745f 7061 722e  pi / RF_sct_par.
+00000b90: 6f6d 6567 615f 7266 5b30 2c30 5d0d 0a0d  omega_rf[0,0]...
+00000ba0: 0a23 2044 4546 494e 4520 534c 4943 4553  .# DEFINE SLICES
+00000bb0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00000bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000bf0: 0d0a 0d0a 6e75 6d62 6572 5f73 6c69 6365  ....number_slice
+00000c00: 7320 3d20 3130 300d 0a73 6c69 6365 5f62  s = 100..slice_b
+00000c10: 6561 6d20 3d20 5072 6f66 696c 6528 6265  eam = Profile(be
+00000c20: 616d 2c20 4375 744f 7074 696f 6e73 2863  am, CutOptions(c
+00000c30: 7574 5f6c 6566 743d 302c 200d 0a20 2020  ut_left=0, ..   
+00000c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c50: 2063 7574 5f72 6967 6874 3d62 7563 6b65   cut_right=bucke
+00000c60: 745f 6c65 6e67 7468 2c20 6e5f 736c 6963  t_length, n_slic
+00000c70: 6573 3d6e 756d 6265 725f 736c 6963 6573  es=number_slices
+00000c80: 2929 200d 0a20 2020 2020 2020 2020 2020  )) ..           
+00000c90: 2020 2020 200d 0a23 204c 4f41 4420 494d       ..# LOAD IM
+00000ca0: 5045 4441 4e43 4520 5441 424c 4553 202d  PEDANCE TABLES -
+00000cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ce0: 2d2d 2d2d 2d2d 0d0a 0d0a 525f 5320 3d20  ------....R_S = 
+00000cf0: 3165 350d 0a23 202d 2075 6e73 7461 626c  1e5..# - unstabl
+00000d00: 652c 202b 2073 7461 626c 650d 0a66 7265  e, + stable..fre
+00000d10: 7175 656e 6379 5f52 203d 2052 465f 7363  quency_R = RF_sc
+00000d20: 745f 7061 722e 6f6d 6567 615f 7266 5b30  t_par.omega_rf[0
+00000d30: 2c30 5d20 2f20 322e 3020 2f20 6e70 2e70  ,0] / 2.0 / np.p
+00000d40: 6920 2d20 6673 0d0a 5120 3d20 3130 3030  i - fs..Q = 1000
+00000d50: 0d0a 0d0a 7265 736f 6e61 746f 7220 3d20  ....resonator = 
+00000d60: 5265 736f 6e61 746f 7273 2852 5f53 2c20  Resonators(R_S, 
+00000d70: 6672 6571 7565 6e63 795f 522c 2051 290d  frequency_R, Q).
+00000d80: 0a0d 0a23 2052 6f62 696e 736f 6e20 696e  ...# Robinson in
+00000d90: 7374 6162 696c 6974 7920 6772 6f77 7468  stability growth
+00000da0: 2072 6174 650d 0a52 7020 3d20 525f 5320   rate..Rp = R_S 
+00000db0: 2f20 2831 202b 2031 6a20 2a20 5120 2a20  / (1 + 1j * Q * 
+00000dc0: 2828 5246 5f73 6374 5f70 6172 2e6f 6d65  ((RF_sct_par.ome
+00000dd0: 6761 5f72 665b 302c 305d 202f 2032 2e30  ga_rf[0,0] / 2.0
+00000de0: 202f 206e 702e 7069 2b66 7329 202f 205c   / np.pi+fs) / \
+00000df0: 0d0a 2020 2020 2066 7265 7175 656e 6379  ..     frequency
+00000e00: 5f52 202d 2066 7265 7175 656e 6379 5f52  _R - frequency_R
+00000e10: 202f 2028 5246 5f73 6374 5f70 6172 2e6f   / (RF_sct_par.o
+00000e20: 6d65 6761 5f72 665b 302c 305d 202f 2032  mega_rf[0,0] / 2
+00000e30: 2e30 202f 206e 702e 7069 2b66 7329 2929  .0 / np.pi+fs)))
+00000e40: 0d0a 526d 203d 2052 5f53 202f 2028 3120  ..Rm = R_S / (1 
+00000e50: 2b20 316a 202a 2051 202a 2028 2852 465f  + 1j * Q * ((RF_
+00000e60: 7363 745f 7061 722e 6f6d 6567 615f 7266  sct_par.omega_rf
+00000e70: 5b30 2c30 5d20 2f20 322e 3020 2f20 6e70  [0,0] / 2.0 / np
+00000e80: 2e70 692d 6673 2920 2f20 5c0d 0a20 2020  .pi-fs) / \..   
+00000e90: 2020 6672 6571 7565 6e63 795f 5220 2d20    frequency_R - 
+00000ea0: 6672 6571 7565 6e63 795f 5220 2f20 2852  frequency_R / (R
+00000eb0: 465f 7363 745f 7061 722e 6f6d 6567 615f  F_sct_par.omega_
+00000ec0: 7266 5b30 2c30 5d20 2f20 322e 3020 2f20  rf[0,0] / 2.0 / 
+00000ed0: 6e70 2e70 692d 6673 2929 290d 0a0d 0a65  np.pi-fs)))....e
+00000ee0: 7474 6120 3d20 312e 302f 6761 6d6d 615f  tta = 1.0/gamma_
+00000ef0: 7472 616e 7369 7469 6f6e 2a2a 3220 2d20  transition**2 - 
+00000f00: 312e 302f 6761 6d6d 612a 2a32 0d0a 0d0a  1.0/gamma**2....
+00000f10: 7461 755f 5253 203d 206d 5f70 202a 2063  tau_RS = m_p * c
+00000f20: 2a2a 322e 3020 2a20 322e 3020 2a20 6761  **2.0 * 2.0 * ga
+00000f30: 6d6d 6120 2a20 5c0d 0a20 2020 2020 2020  mma * \..       
+00000f40: 2020 5246 5f73 6374 5f70 6172 2e74 5f72    RF_sct_par.t_r
+00000f50: 6576 5b30 5d2a 2a32 2e30 202a 2052 465f  ev[0]**2.0 * RF_
+00000f60: 7363 745f 7061 722e 6f6d 6567 615f 7330  sct_par.omega_s0
+00000f70: 5b30 5d20 2f20 5c0d 0a20 2020 2020 2020  [0] / \..       
+00000f80: 2020 2865 2a2a 322e 3020 2a20 6e5f 7061    (e**2.0 * n_pa
+00000f90: 7274 6963 6c65 7320 2a20 6574 7461 202a  rticles * etta *
+00000fa0: 2052 465f 7363 745f 7061 722e 6f6d 6567   RF_sct_par.omeg
+00000fb0: 615f 7266 5b30 2c30 5d20 2a20 5c0d 0a20  a_rf[0,0] * \.. 
+00000fc0: 2020 2020 2020 2020 6e70 2e72 6561 6c28          np.real(
+00000fd0: 5270 202d 2052 6d29 290d 0a0d 0a70 7269  Rp - Rm))....pri
+00000fe0: 6e74 2827 526f 6269 6e73 6f6e 2069 6e73  nt('Robinson ins
+00000ff0: 7461 6269 6c69 7479 2067 726f 7774 6820  tability growth 
+00001000: 7261 7465 203d 207b 303a 312e 3366 7d20  rate = {0:1.3f} 
+00001010: 7475 726e 7327 2e66 6f72 6d61 7428 7461  turns'.format(ta
+00001020: 755f 5253 202f 205c 0d0a 2020 2020 2020  u_RS / \..      
+00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001060: 2020 2020 5246 5f73 6374 5f70 6172 2e74      RF_sct_par.t
+00001070: 5f72 6576 5b30 5d29 290d 0a0d 0a0d 0a23  _rev[0]))......#
+00001080: 2049 4e44 5543 4544 2056 4f4c 5441 4745   INDUCED VOLTAGE
+00001090: 2046 524f 4d20 494d 5045 4441 4e43 4520   FROM IMPEDANCE 
+000010a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000010b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000010c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  --------------..
+000010d0: 0d0a 696d 705f 6c69 7374 203d 205b 7265  ..imp_list = [re
+000010e0: 736f 6e61 746f 725d 0d0a 0d0a 696e 645f  sonator]....ind_
+000010f0: 766f 6c74 5f66 7265 7120 3d20 496e 6475  volt_freq = Indu
+00001100: 6365 6456 6f6c 7461 6765 4672 6571 2862  cedVoltageFreq(b
+00001110: 6561 6d2c 2073 6c69 6365 5f62 6561 6d2c  eam, slice_beam,
+00001120: 2069 6d70 5f6c 6973 742c 0d0a 2020 2020   imp_list,..    
+00001130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001140: 5246 5061 7261 6d73 3d52 465f 7363 745f  RFParams=RF_sct_
+00001150: 7061 722c 2066 7265 7175 656e 6379 5f72  par, frequency_r
+00001160: 6573 6f6c 7574 696f 6e3d 3565 322c 0d0a  esolution=5e2,..
+00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001180: 2020 2020 6d75 6c74 695f 7475 726e 5f77      multi_turn_w
+00001190: 616b 653d 5472 7565 2c20 6d74 775f 6d6f  ake=True, mtw_mo
+000011a0: 6465 3d27 7469 6d65 2729 0d0a 0d0a 746f  de='time')....to
+000011b0: 7461 6c5f 696e 645f 766f 6c74 203d 2054  tal_ind_volt = T
+000011c0: 6f74 616c 496e 6475 6365 6456 6f6c 7461  otalInducedVolta
+000011d0: 6765 2862 6561 6d2c 2073 6c69 6365 5f62  ge(beam, slice_b
+000011e0: 6561 6d2c 205b 696e 645f 766f 6c74 5f66  eam, [ind_volt_f
+000011f0: 7265 715d 290d 0a0d 0a66 5f72 6620 3d20  req])....f_rf = 
+00001200: 5246 5f73 6374 5f70 6172 2e6f 6d65 6761  RF_sct_par.omega
+00001210: 5f72 665b 302c 305d 202f 2032 2e30 202f  _rf[0,0] / 2.0 /
+00001220: 206e 702e 7069 0d0a 706c 742e 6669 6775   np.pi..plt.figu
+00001230: 7265 2829 0d0a 706c 742e 706c 6f74 2869  re()..plt.plot(i
+00001240: 6e64 5f76 6f6c 745f 6672 6571 2e66 7265  nd_volt_freq.fre
+00001250: 712a 3165 2d36 2c20 6e70 2e61 6273 2869  q*1e-6, np.abs(i
+00001260: 6e64 5f76 6f6c 745f 6672 6571 2e74 6f74  nd_volt_freq.tot
+00001270: 616c 5f69 6d70 6564 616e 6365 202a 205c  al_impedance * \
+00001280: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012a0: 2020 2020 2020 2020 2020 2073 6c69 6365             slice
+000012b0: 5f62 6561 6d2e 6269 6e5f 7369 7a65 292c  _beam.bin_size),
+000012c0: 206c 773d 3229 0d0a 706c 742e 706c 6f74   lw=2)..plt.plot
+000012d0: 285b 665f 7266 2a31 652d 365d 2a32 2c20  ([f_rf*1e-6]*2, 
+000012e0: 706c 742e 796c 696d 2829 2c20 276b 272c  plt.ylim(), 'k',
+000012f0: 206c 773d 3229 0d0a 706c 742e 706c 6f74   lw=2)..plt.plot
+00001300: 285b 665f 7266 2a31 652d 3620 2b20 6673  ([f_rf*1e-6 + fs
+00001310: 2a31 652d 365d 2a32 2c20 706c 742e 796c  *1e-6]*2, plt.yl
+00001320: 696d 2829 2c20 276b 2d2d 272c 206c 773d  im(), 'k--', lw=
+00001330: 3229 0d0a 706c 742e 706c 6f74 285b 665f  2)..plt.plot([f_
+00001340: 7266 2a31 652d 3620 2d20 6673 2a31 652d  rf*1e-6 - fs*1e-
+00001350: 365d 2a32 2c20 706c 742e 796c 696d 2829  6]*2, plt.ylim()
+00001360: 2c20 276b 2d2d 272c 206c 773d 3229 0d0a  , 'k--', lw=2)..
+00001370: 706c 742e 786c 696d 2831 2e37 342c 312e  plt.xlim(1.74,1.
+00001380: 3736 290d 0a70 6c74 2e6c 6567 656e 6428  76)..plt.legend(
+00001390: 2827 496d 7065 6461 6e63 6527 2c27 5246  ('Impedance','RF
+000013a0: 2066 7265 7175 656e 6379 272c 2753 796e   frequency','Syn
+000013b0: 6368 726f 7472 6f6e 2073 6964 6562 616e  chrotron sideban
+000013c0: 6473 2729 2c20 6c6f 633d 302c 200d 0a20  ds'), loc=0, .. 
+000013d0: 2020 2020 2020 2020 2020 666f 6e74 7369            fontsi
+000013e0: 7a65 3d27 6d65 6469 756d 2729 0d0a 706c  ze='medium')..pl
+000013f0: 742e 786c 6162 656c 2827 4672 6571 7565  t.xlabel('Freque
+00001400: 6e63 7920 5b4d 487a 5d27 290d 0a70 6c74  ncy [MHz]')..plt
+00001410: 2e79 6c61 6265 6c28 7227 496d 7065 6461  .ylabel(r'Impeda
+00001420: 6e63 6520 5b24 5c4f 6d65 6761 245d 2729  nce [$\Omega$]')
+00001430: 0d0a 706c 742e 7361 7665 6669 6728 7468  ..plt.savefig(th
+00001440: 6973 5f64 6972 6563 746f 7279 202b 2027  is_directory + '
+00001450: 2e2e 2f6f 7574 7075 745f 6669 6c65 732f  ../output_files/
+00001460: 4558 5f31 385f 6669 672f 696d 7065 6461  EX_18_fig/impeda
+00001470: 6e63 652e 706e 6727 290d 0a70 6c74 2e63  nce.png')..plt.c
+00001480: 6c6f 7365 2829 0d0a 0d0a 0d0a 2320 4245  lose()......# BE
+00001490: 414d 2047 454e 4552 4154 494f 4e20 2d2d  AM GENERATION --
+000014a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000014b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000014c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000014d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a6d  -----------....m
+000014e0: 6174 6368 6564 5f66 726f 6d5f 6469 7374  atched_from_dist
+000014f0: 7269 6275 7469 6f6e 5f66 756e 6374 696f  ribution_functio
+00001500: 6e28 6265 616d 2c20 6675 6c6c 5f74 7261  n(beam, full_tra
+00001510: 636b 6572 2c0d 0a20 2020 2020 2020 2020  cker,..         
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 2020 2020 2020 2020 2064 6973 7472 6962           distrib
+00001540: 7574 696f 6e5f 7479 7065 3d64 6973 7472  ution_type=distr
+00001550: 6962 7574 696f 6e5f 7479 7065 2c0d 0a20  ibution_type,.. 
+00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001580: 2062 756e 6368 5f6c 656e 6774 683d 6275   bunch_length=bu
+00001590: 6e63 685f 6c65 6e67 7468 2c20 6e5f 6974  nch_length, n_it
+000015a0: 6572 6174 696f 6e73 3d32 302c 0d0a 2020  erations=20,..  
+000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015d0: 546f 7461 6c49 6e64 7563 6564 566f 6c74  TotalInducedVolt
+000015e0: 6167 653d 746f 7461 6c5f 696e 645f 766f  age=total_ind_vo
+000015f0: 6c74 2c20 7365 6564 3d31 3029 0d0a 0d0a  lt, seed=10)....
+00001600: 2320 466f 7220 7465 7374 696e 6720 7075  # For testing pu
+00001610: 7270 6f73 6573 0d0a 7465 7374 5f73 7472  rposes..test_str
+00001620: 696e 6720 3d20 2727 0d0a 7465 7374 5f73  ing = ''..test_s
+00001630: 7472 696e 6720 2b3d 2027 7b3a 3c31 377d  tring += '{:<17}
+00001640: 5c74 7b3a 3c31 377d 5c74 7b3a 3c31 377d  \t{:<17}\t{:<17}
+00001650: 5c74 7b3a 3c31 377d 5c6e 272e 666f 726d  \t{:<17}\n'.form
+00001660: 6174 280d 0a20 2020 2027 6d65 616e 5f64  at(..    'mean_d
+00001670: 4527 2c20 2773 7464 5f64 4527 2c20 276d  E', 'std_dE', 'm
+00001680: 6561 6e5f 6474 272c 2027 7374 645f 6474  ean_dt', 'std_dt
+00001690: 2729 0d0a 7465 7374 5f73 7472 696e 6720  ')..test_string 
+000016a0: 2b3d 2027 7b3a 2b31 302e 3130 657d 5c74  += '{:+10.10e}\t
+000016b0: 7b3a 2b31 302e 3130 657d 5c74 7b3a 2b31  {:+10.10e}\t{:+1
+000016c0: 302e 3130 657d 5c74 7b3a 2b31 302e 3130  0.10e}\t{:+10.10
+000016d0: 657d 5c6e 272e 666f 726d 6174 280d 0a20  e}\n'.format(.. 
+000016e0: 2020 206e 702e 6d65 616e 2862 6561 6d2e     np.mean(beam.
+000016f0: 6445 292c 206e 702e 7374 6428 6265 616d  dE), np.std(beam
+00001700: 2e64 4529 2c20 6e70 2e6d 6561 6e28 6265  .dE), np.mean(be
+00001710: 616d 2e64 7429 2c20 6e70 2e73 7464 2862  am.dt), np.std(b
+00001720: 6561 6d2e 6474 2929 0d0a 0d0a 0d0a 2320  eam.dt))......# 
+00001730: 4143 4345 4c45 5241 5449 4f4e 204d 4150  ACCELERATION MAP
+00001740: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00001750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d  -------------...
+00001780: 0a6d 6170 5f20 3d20 5b73 6c69 6365 5f62  .map_ = [slice_b
+00001790: 6561 6d5d 202b 205b 746f 7461 6c5f 696e  eam] + [total_in
+000017a0: 645f 766f 6c74 5d20 2b20 5b72 696e 675f  d_volt] + [ring_
+000017b0: 5246 5f73 6563 7469 6f6e 5d0d 0a0d 0a69  RF_section]....i
+000017c0: 6d70 6f72 7420 7469 6d65 0d0a 7430 203d  mport time..t0 =
+000017d0: 2074 696d 652e 7469 6d65 2829 0d0a 0d0a   time.time()....
+000017e0: 6275 6e63 685f 6365 6e74 6572 203d 206e  bunch_center = n
+000017f0: 702e 7a65 726f 7328 6e5f 7475 726e 7329  p.zeros(n_turns)
+00001800: 0d0a 6275 6e63 685f 7374 6420 3d20 6e70  ..bunch_std = np
+00001810: 2e7a 6572 6f73 286e 5f74 7572 6e73 290d  .zeros(n_turns).
+00001820: 0a0d 0a0d 0a23 2054 5241 434b 494e 4720  .....# TRACKING 
+00001830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001870: 2d2d 2d2d 0d0a 666f 7220 6920 696e 2072  ----..for i in r
+00001880: 616e 6765 286e 5f74 7572 6e73 293a 0d0a  ange(n_turns):..
+00001890: 2020 2020 0d0a 2020 2020 7072 696e 7428      ..    print(
+000018a0: 6929 0d0a 2020 2020 666f 7220 6d20 696e  i)..    for m in
+000018b0: 206d 6170 5f3a 0d0a 2020 2020 2020 2020   map_:..        
+000018c0: 6d2e 7472 6163 6b28 290d 0a20 2020 200d  m.track()..    .
+000018d0: 0a20 2020 2062 756e 6368 5f63 656e 7465  .    bunch_cente
+000018e0: 725b 695d 203d 2062 6561 6d2e 6474 2e6d  r[i] = beam.dt.m
+000018f0: 6561 6e28 290d 0a20 2020 2062 756e 6368  ean()..    bunch
+00001900: 5f73 7464 5b69 5d20 3d20 6265 616d 2e64  _std[i] = beam.d
+00001910: 742e 7374 6428 290d 0a20 2020 200d 0a20  t.std()..    .. 
+00001920: 2020 2069 6620 6920 2520 6e5f 7475 726e     if i % n_turn
+00001930: 735f 6265 7477 6565 6e5f 7477 6f5f 706c  s_between_two_pl
+00001940: 6f74 7320 3d3d 2030 3a0d 0a20 2020 2020  ots == 0:..     
+00001950: 2020 2070 6c74 2e66 6967 7572 6528 290d     plt.figure().
+00001960: 0a20 2020 2020 2020 2070 6c74 2e70 6c6f  .        plt.plo
+00001970: 7428 6265 616d 2e64 742a 3165 392c 6265  t(beam.dt*1e9,be
+00001980: 616d 2e64 452a 3165 2d36 2c27 2e27 290d  am.dE*1e-6,'.').
+00001990: 0a20 2020 2020 2020 2070 6c74 2e78 6c61  .        plt.xla
+000019a0: 6265 6c28 2754 696d 6520 5b6e 735d 2729  bel('Time [ns]')
+000019b0: 0d0a 2020 2020 2020 2020 706c 742e 796c  ..        plt.yl
+000019c0: 6162 656c 2827 456e 6572 6779 205b 4d65  abel('Energy [Me
+000019d0: 565d 2729 0d0a 2020 2020 2020 2020 706c  V]')..        pl
+000019e0: 742e 7361 7665 6669 6728 7468 6973 5f64  t.savefig(this_d
+000019f0: 6972 6563 746f 7279 202b 2027 2e2e 2f6f  irectory + '../o
+00001a00: 7574 7075 745f 6669 6c65 732f 4558 5f31  utput_files/EX_1
+00001a10: 385f 6669 672f 7068 6173 655f 7370 6163  8_fig/phase_spac
+00001a20: 655f 7b30 3a64 7d2e 706e 6727 2e66 6f72  e_{0:d}.png'.for
+00001a30: 6d61 7428 6929 290d 0a20 2020 2020 2020  mat(i))..       
+00001a40: 2070 6c74 2e63 6c6f 7365 2829 0d0a 0d0a   plt.close()....
+00001a50: 7072 696e 7428 7469 6d65 2e74 696d 6528  print(time.time(
+00001a60: 2920 2d20 7430 290d 0a0d 0a70 6c74 2e66  ) - t0)....plt.f
+00001a70: 6967 7572 6528 290d 0a70 6c74 2e70 6c6f  igure()..plt.plo
+00001a80: 7428 6275 6e63 685f 6365 6e74 6572 2a31  t(bunch_center*1
+00001a90: 6539 290d 0a70 6c74 2e78 6c61 6265 6c28  e9)..plt.xlabel(
+00001aa0: 2754 7572 6e73 2729 0d0a 706c 742e 796c  'Turns')..plt.yl
+00001ab0: 6162 656c 2827 4275 6e63 6820 6365 6e74  abel('Bunch cent
+00001ac0: 6572 205b 6e73 5d27 290d 0a70 6c74 2e73  er [ns]')..plt.s
+00001ad0: 6176 6566 6967 2874 6869 735f 6469 7265  avefig(this_dire
+00001ae0: 6374 6f72 7920 2b20 272e 2e2f 6f75 7470  ctory + '../outp
+00001af0: 7574 5f66 696c 6573 2f45 585f 3138 5f66  ut_files/EX_18_f
+00001b00: 6967 2f62 756e 6368 5f63 656e 7465 722e  ig/bunch_center.
+00001b10: 706e 6727 290d 0a70 6c74 2e63 6c6f 7365  png')..plt.close
+00001b20: 2829 0d0a 706c 742e 6669 6775 7265 2829  ()..plt.figure()
+00001b30: 0d0a 706c 742e 706c 6f74 2862 756e 6368  ..plt.plot(bunch
+00001b40: 5f73 7464 2a31 6539 290d 0a70 6c74 2e78  _std*1e9)..plt.x
+00001b50: 6c61 6265 6c28 2754 7572 6e73 2729 0d0a  label('Turns')..
+00001b60: 706c 742e 796c 6162 656c 2827 4275 6e63  plt.ylabel('Bunc
+00001b70: 6820 6c65 6e67 7468 205b 6e73 5d27 290d  h length [ns]').
+00001b80: 0a70 6c74 2e73 6176 6566 6967 2874 6869  .plt.savefig(thi
+00001b90: 735f 6469 7265 6374 6f72 7920 2b20 272e  s_directory + '.
+00001ba0: 2e2f 6f75 7470 7574 5f66 696c 6573 2f45  ./output_files/E
+00001bb0: 585f 3138 5f66 6967 2f62 756e 6368 5f6c  X_18_fig/bunch_l
+00001bc0: 656e 6774 682e 706e 6727 290d 0a70 6c74  ength.png')..plt
+00001bd0: 2e63 6c6f 7365 2829 0d0a 0d0a 2320 466f  .close()....# Fo
+00001be0: 7220 7465 7374 696e 6720 7075 7270 6f73  r testing purpos
+00001bf0: 6573 0d0a 7465 7374 5f73 7472 696e 6720  es..test_string 
+00001c00: 2b3d 2027 7b3a 2b31 302e 3130 657d 5c74  += '{:+10.10e}\t
+00001c10: 7b3a 2b31 302e 3130 657d 5c74 7b3a 2b31  {:+10.10e}\t{:+1
+00001c20: 302e 3130 657d 5c74 7b3a 2b31 302e 3130  0.10e}\t{:+10.10
+00001c30: 657d 5c6e 272e 666f 726d 6174 280d 0a20  e}\n'.format(.. 
+00001c40: 2020 206e 702e 6d65 616e 2862 6561 6d2e     np.mean(beam.
+00001c50: 6445 292c 206e 702e 7374 6428 6265 616d  dE), np.std(beam
+00001c60: 2e64 4529 2c20 6e70 2e6d 6561 6e28 6265  .dE), np.mean(be
+00001c70: 616d 2e64 7429 2c20 6e70 2e73 7464 2862  am.dt), np.std(b
+00001c80: 6561 6d2e 6474 2929 0d0a 7769 7468 206f  eam.dt))..with o
+00001c90: 7065 6e28 7468 6973 5f64 6972 6563 746f  pen(this_directo
+00001ca0: 7279 202b 2027 2e2e 2f6f 7574 7075 745f  ry + '../output_
+00001cb0: 6669 6c65 732f 4558 5f31 385f 7465 7374  files/EX_18_test
+00001cc0: 5f64 6174 612e 7478 7427 2c20 2777 2729  _data.txt', 'w')
+00001cd0: 2061 7320 663a 0d0a 2020 2020 662e 7772   as f:..    f.wr
+00001ce0: 6974 6528 7465 7374 5f73 7472 696e 6729  ite(test_string)
+00001cf0: 0d0a 0d0a 2020 2020 0d0a 0d0a 0d0a 7072  ....    ......pr
+00001d00: 696e 7428 2244 6f6e 6521 2229 0d0a       int("Done!")..
```

### Comparing `blond-2.0.11/blond/plots/plot.py` & `blond-2.0.12/blond/plots/plot.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/plots/plot_beams.py` & `blond-2.0.12/blond/plots/plot_beams.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/plots/plot_impedance.py` & `blond-2.0.12/blond/plots/plot_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/plots/plot_llrf.py` & `blond-2.0.12/blond/plots/plot_llrf.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/plots/plot_parameters.py` & `blond-2.0.12/blond/plots/plot_parameters.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/plots/plot_slices.py` & `blond-2.0.12/blond/plots/plot_slices.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/synchrotron_radiation/synchrotron_radiation.py` & `blond-2.0.12/blond/synchrotron_radiation/synchrotron_radiation.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,174 +12,188 @@
 
 :Authors: **Juan F. Esteban Mueller**
 '''
 
 from __future__ import division, print_function
 from builtins import range, object
 import numpy as np
-import ctypes
-from scipy.constants import e, c, epsilon_0, hbar
 from ..utils import bmath as bm
 
 
 class SynchrotronRadiation(object):
-    
+
     ''' Class to compute synchrotron radiation effects, including radiation
         damping and quantum excitation.
         For multiple RF section, instanciate one object per RF section an call
         the track() method after tracking each section.
     '''
-    
+
     def __init__(self, Ring, RFParameters, Beam, bending_radius,
-                 n_kicks=1, quantum_excitation=True, python=False, seed=None):
-        
-        self.general_params = Ring
+                 n_kicks=1, quantum_excitation=True, python=False, seed=None,
+                 shift_beam=True):
+
+        self.ring = Ring
         self.rf_params = RFParameters
         self.beam = Beam
         self.rho = bending_radius
         self.n_kicks = n_kicks  # To apply SR in several kicks
         np.random.seed(seed=seed)
-        
+
         # Calculate static parameters
-        self.Cgamma = 1.0 / (e**2.0 * 3.0 * epsilon_0 *
-                             self.general_params.Particle.mass**4.0)
-        self.Cq = (55.0 / (32.0 * np.sqrt(3.0)) * hbar * c /
-                   (self.general_params.Particle.mass * e))
-        
+        self.C_gamma = self.ring.Particle.C_gamma
+        self.C_q = self.ring.Particle.C_q
+
         self.I2 = 2.0 * np.pi / self.rho     # Assuming isomagnetic machine
         self.I3 = 2.0 * np.pi / self.rho**2.0
-        self.I4 = (self.general_params.ring_circumference *
-                   self.general_params.alpha_0[0,0] / self.rho**2.0)
+        self.I4 = self.ring.ring_circumference * self.ring.alpha_0[0, 0] / self.rho**2.0
         self.jz = 2.0 + self.I4 / self.I2
-        
+
         # Calculate synchrotron radiation parameters
         self.calculate_SR_params()
-        
+
         # Initialize the random number array if quantum excitation is included
         if quantum_excitation:
             self.random_array = np.zeros(self.beam.n_macroparticles)
-        
-        # Displace the beam in phase to account for the energy loss due to 
+
+        # Displace the beam in phase to account for the energy loss due to
         # synchrotron radiation (temporary until bunch generation is updated)
-        if self.rf_params.section_index == 0:
-            self.beam.dt -= (np.arcsin(self.U0/self.rf_params.voltage[0][0]) *
-                             self.rf_params.t_rf[0, 0]/ (2.0*np.pi))
-        
+        if (shift_beam) and (self.rf_params.section_index == 0):
+            self.beam_phase_to_compensate_SR = np.abs(np.arcsin(
+                self.U0 / (self.ring.Particle.charge * self.rf_params.voltage[0][0]) ))
+            self.beam_position_to_compensate_SR = self.beam_phase_to_compensate_SR \
+                * self.rf_params.t_rf[0, 0] / (2.0*np.pi)
+
+            self.beam.dt -= self.beam_position_to_compensate_SR
+
         # Select the right method for the tracker according to the selected
         # settings
         if python:
             if quantum_excitation:
                 self.track = self.track_full_python
             else:
                 self.track = self.track_SR_python
         else:
             if quantum_excitation:
+                if seed is not None:
+                    bm.set_random_seed(seed)
                 self.track = self.track_full_C
             else:
                 self.track = self.track_SR_C
 
     # Method to compute the SR parameters
     def calculate_SR_params(self):
         i_turn = self.rf_params.counter[0]
-        
-        # Energy loss per turn/RF section [eV]        
-        self.U0 = (self.Cgamma * self.general_params.energy[0,i_turn]**4.0 *
-                  self.I2 / (2.0 * np. pi) * e**3.0 *
-                  self.rf_params.section_length /
-                  self.general_params.ring_circumference)   
 
-        # Damping time [turns]        
-        self.tau_z = (2.0 / self.jz * self.general_params.energy[0,i_turn] /
+        # Energy loss per turn/RF section [eV]
+        self.U0 = (self.C_gamma * self.ring.energy[0, i_turn]**4.0
+                   * self.I2 / (2.0 * np. pi)
+                   * self.rf_params.section_length
+                   / self.ring.ring_circumference)
+
+        # Damping time [turns]
+        self.tau_z = (2.0 / self.jz * self.ring.energy[0, i_turn] /
                       self.U0)
 
-        # Equilibrium energy spread     
-        self.sigma_dE = np.sqrt(self.Cq *
-                                self.general_params.gamma[0,i_turn]**2.0 *
+        # Equilibrium energy spread
+        self.sigma_dE = np.sqrt(self.C_q *
+                                self.ring.gamma[0, i_turn]**2.0 *
                                 self.I3 / (self.jz * self.I2))
 
     # Print SR parameters
     def print_SR_params(self):
         i_turn = self.rf_params.counter[0]
-        
-        print( '------- Synchrotron radiation parameters -------' )
-        print( 'jz = {0:1.8f} '.format( self.jz ) )
-        if (self.rf_params.section_length ==
-                self.general_params.ring_circumference):
-            print( 'Energy loss per turn = {0:1.4f} GeV/turn'.format(
-                    self.U0*1e-9) )
-            print( 'Damping time = {0:1.4f} turns'.format(self.tau_z) )
+
+        print('------- Synchrotron radiation parameters -------')
+        print(f'jz = {self.jz:1.8f}')
+        if (self.rf_params.section_length
+                == self.ring.ring_circumference):
+            print(f'Energy loss per turn = {self.U0/1e9:1.4f} GeV/turn')
+            print(f'Damping time = {self.tau_z:1.4f} turns')
         else:
-            print( 'Energy loss per RF section = {0:1.4f} GeV/section'.format(
-                    self.U0*1e-9) )
-            print( 'Energy loss per turn = {0:1.4f} GeV/turn'.format(
-                    self.U0*1e-9 * self.general_params.ring_circumference /
-                    self.rf_params.section_length) )
-            print( 'Damping time = {0:1.4f} turns'.format(self.tau_z *
-                    self.rf_params.section_length /
-                    self.general_params.ring_circumference ) )
-        print( 'Equilibrium energy spread = {0:1.4f}% ({1:1.4f} MeV)'.format(
-                self.sigma_dE * 100,self.sigma_dE *
-                self.general_params.energy[0,i_turn]*1e-6)  )
-        print( '------------------------------------------------' )
+            print('Energy loss per RF section = {0:1.4f} GeV/section'.format(
+                self.U0*1e-9))
+            print('Energy loss per turn = {0:1.4f} GeV/turn'.format(
+                self.U0*1e-9 * self.ring.ring_circumference
+                / self.rf_params.section_length))
+            print('Damping time = {0:1.4f} turns'.format(self.tau_z
+                                                         * self.rf_params.section_length
+                                                         / self.ring.ring_circumference))
+        print(f'Equilibrium energy spread = {self.sigma_dE * 100:1.4f}%'
+              + f' ({self.sigma_dE * self.ring.energy[0, i_turn]*1e-6:1.4f}) MeV')
+        print('------------------------------------------------')
 
     # Track particles with SR only (without quantum excitation)
     def track_SR_python(self):
         i_turn = self.rf_params.counter[0]
         # Recalculate SR parameters if energy changes
-        if (i_turn != 0 and self.general_params.energy[0,i_turn] !=
-                self.general_params.energy[0,i_turn-1]):
+        if (i_turn != 0 and self.ring.energy[0, i_turn] !=
+                self.ring.energy[0, i_turn-1]):
             self.calculate_SR_params()
         for i in range(self.n_kicks):
-            self.beam.dE += -(2.0 / self.tau_z / self.n_kicks * self.beam.dE +
-                              self.U0 / self.n_kicks)
-    
+            self.beam.dE += -(2.0 / self.tau_z / self.n_kicks * self.beam.dE
+                              + self.U0 / self.n_kicks)
+
     # Track particles with SR and quantum excitation
     def track_full_python(self):
         i_turn = self.rf_params.counter[0]
         # Recalculate SR parameters if energy changes
-        if (i_turn != 0 and self.general_params.energy[0,i_turn] !=
-                self.general_params.energy[0,i_turn-1]):
+        if (i_turn != 0 and self.ring.energy[0, i_turn] !=
+                self.ring.energy[0, i_turn-1]):
             self.calculate_SR_params()
         for i in range(self.n_kicks):
             self.beam.dE += -(2.0 / self.tau_z / self.n_kicks * self.beam.dE +
                               self.U0 / self.n_kicks - 2.0 * self.sigma_dE /
                               np.sqrt(self.tau_z * self.n_kicks) *
-                              self.general_params.energy[0,i_turn] *
+                              self.ring.energy[0, i_turn] *
                               np.random.randn(self.beam.n_macroparticles))
 
     # Track particles with SR only (without quantum excitation)
     # C implementation
     def track_SR_C(self):
         i_turn = self.rf_params.counter[0]
         # Recalculate SR parameters if energy changes
-        if (i_turn != 0 and self.general_params.energy[0,i_turn] !=
-                self.general_params.energy[0,i_turn-1]):
+        if (i_turn != 0 and self.ring.energy[0, i_turn] !=
+                self.ring.energy[0, i_turn-1]):
             self.calculate_SR_params()
-        
-        bm.synchrotron_radiation(self, i_turn)
 
-#          libsrqe.synchrotron_radiation(
-            #  self.beam.dE.ctypes.data_as(ctypes.c_void_p), 
-            #  ctypes.c_double(self.U0 / self.n_kicks),
-            #  ctypes.c_int(self.beam.n_macroparticles), 
-            #  ctypes.c_double(self.tau_z * self.n_kicks),
-            #  ctypes.c_int(self.n_kicks))
-#      
+        bm.synchrotron_radiation(self.beam.dE, self.U0,
+                                 self.n_kicks, self.tau_z)
+
     # Track particles with SR and quantum excitation. C implementation
     def track_full_C(self):
         i_turn = self.rf_params.counter[0]
         # Recalculate SR parameters if energy changes
-        if (i_turn != 0 and self.general_params.energy[0,i_turn] !=
-                self.general_params.energy[0,i_turn-1]):
+        if (i_turn != 0 and self.ring.energy[0, i_turn] !=
+                self.ring.energy[0, i_turn-1]):
             self.calculate_SR_params()
 
-        bm.synchrotron_radiation_full(self, i_turn)
+        bm.synchrotron_radiation_full(self.beam.dE, self.U0, self.n_kicks,
+                                      self.tau_z, self.sigma_dE,
+                                      self.ring.energy[0, i_turn])
+
+    def to_gpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays to the GPU
+        '''
+        # Check if to_gpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'GPU':
+            return
+
+        assert bm.device == 'GPU'
+        # No arrays need to be transfered
+
+        # to make sure it will not be called again
+        self._device = 'GPU'
+
+    def to_cpu(self, recursive=True):
+        '''
+        Transfer all necessary arrays back to the CPU
+        '''
+        # Check if to_cpu has been invoked already
+        if hasattr(self, '_device') and self._device == 'CPU':
+            return
+
+        assert bm.device == 'CPU'
+        # No arrays need to be transfered
 
-#          libsrqe.synchrotron_radiation_full(
-            #  self.beam.dE.ctypes.data_as(ctypes.c_void_p), 
-            #  ctypes.c_double(self.U0 / self.n_kicks),
-            #  ctypes.c_int(self.beam.n_macroparticles), 
-            #  ctypes.c_double(self.sigma_dE), 
-            #  ctypes.c_double(self.tau_z * self.n_kicks), 
-            #  ctypes.c_double(self.general_params.energy[0,i_turn]),
-            #  self.random_array.ctypes.data_as(ctypes.c_void_p),
-#              ctypes.c_int(self.n_kicks))
+        # to make sure it will not be called again
+        self._device = 'CPU'
```

### Comparing `blond-2.0.11/blond/toolbox/action.py` & `blond-2.0.12/blond/toolbox/action.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/toolbox/diffusion.py` & `blond-2.0.12/blond/toolbox/diffusion.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/toolbox/filters_and_fitting.py` & `blond-2.0.12/blond/toolbox/filters_and_fitting.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
           **Juan F. Esteban Mueller**
 '''
 
 import numpy as np
 from scipy.signal import cheb2ord, cheby2, filtfilt, freqz
 import matplotlib.pyplot as plt
 from scipy.optimize import curve_fit
-
+from ..utils import bmath as bm
 
 def beam_profile_filter_chebyshev(Y_array, X_array, filter_option):
     """
     This routine is filtering the beam profile with a type II Chebyshev
     filter. The input is a library having the following structure and
     informations:
 
@@ -99,20 +99,23 @@
 
 
 def gaussian_fit(Y_array, X_array, p0):
     """
     Gaussian fit of the profile, in order to get the bunch length and
     position. Returns fit values in units of s.
     """
-
+    if bm.device == 'GPU':
+        X_array = X_array.get()
+        Y_array = Y_array.get()
+        
     return curve_fit(gauss, X_array, Y_array, p0)[0]
 
 
 def gauss(x, *p):
-    """
+    r"""
     Defined as:
 
     .. math:: A \, e^{\\frac{\\left(x-x_0\\right)^2}{2\\sigma_x^2}}
 
     """
 
     A, x0, sx = p
@@ -175,14 +178,17 @@
     Computation of the bunch length and position from the FWHM
     assuming Gaussian line density for multibunch case.
     """
 
     bl_fwhm = np.zeros(n_bunches)
     bp_fwhm = np.zeros(n_bunches)
 
+    if bm.device == 'GPU':
+        X_array = X_array.get()
+        Y_array = Y_array.get()
     for indexBunch in range(0, n_bunches):
 
         left_edge = indexBunch * bunch_spacing_buckets * bucket_size_tau -\
             bucket_tolerance * bucket_size_tau
         right_edge = indexBunch * bunch_spacing_buckets * bucket_size_tau +\
             bucket_size_tau + bucket_tolerance * bucket_size_tau
         indexes_bucket = np.where((X_array > left_edge) *
@@ -200,16 +206,19 @@
     """
     Computation of the rms bunch length (4sigma) and position.
     """
 
     bl_rms = np.zeros(n_bunches)
     bp_rms = np.zeros(n_bunches)
 
-    for indexBunch in range(0, n_bunches):
+    if bm.device == 'GPU':
+        X_array = X_array.get()
+        Y_array = Y_array.get()
 
+    for indexBunch in range(0, n_bunches):
         left_edge = indexBunch * bunch_spacing_buckets * bucket_size_tau -\
             bucket_tolerance * bucket_size_tau
         right_edge = indexBunch * bunch_spacing_buckets * bucket_size_tau +\
             bucket_size_tau + bucket_tolerance * bucket_size_tau
 
         indexes_bucket = np.where((X_array > left_edge) *
                                   (X_array < right_edge))[0]
```

### Comparing `blond-2.0.11/blond/toolbox/logger.py` & `blond-2.0.12/blond/toolbox/logger.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/toolbox/next_regular.py` & `blond-2.0.12/blond/toolbox/next_regular.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/toolbox/parameter_scaling.py` & `blond-2.0.12/blond/toolbox/parameter_scaling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding: utf8
-# Copyright 2014-2017 CERN. This software is distributed under the
+# Copyright 2014-2020 CERN. This software is distributed under the
 # terms of the GNU General Public Licence version 3 (GPL Version 3), 
 # copied verbatim in the file LICENCE.md.
 # In applying this licence, CERN does not waive the privileges and immunities 
 # granted to it by virtue of its status as an Intergovernmental Organization or
 # submit itself to any jurisdiction.
 # Project website: http://blond.web.cern.ch/
 
@@ -16,450 +16,482 @@
 from PyQt5 import QtCore, QtGui, QtWidgets
 from PyQt5.Qt import QButtonGroup, QHBoxLayout, QGroupBox
 from scipy import integrate
 from scipy.constants import m_p, e, c
 
 import numpy as np
 
+# Machine-dependent parameters [SI-units] -------------------------------------
+set_ups = {'PSB': '0',
+           'CPS': '1',
+           'SPS, Q20': '2', 'SPS, Q22': '3', 'SPS, Q26': '4',
+           'LHC, -2016': '5', 'LHC, 2017-': '6'}
+gamma_ts = {'0': 4.0767,
+            '1': np.sqrt(37.2),
+            '2': 18., '3': 20., '4': 22.83,
+            '5': 55.759505, '6': 53.8}
+harmonics = {'0': 1,
+             '1': 21,
+             '2': 4620, '3': 4620, '4': 4620,
+             '5': 35640, '6': 35640}
+circumferences = {'0': 2*np.pi*25,
+                  '1': 2*np.pi*100.,
+                  '2': 2*np.pi*1100.009, '3': 2*np.pi*1100.009, '4': 2*np.pi*1100.009,
+                  '5': 26658.883, '6': 26658.883}
+energies_fb = {'0': (160.e6 + m_p*c**2/e),
+               '1': (2.0e9 + m_p*c**2/e),
+               '2': 25.92e9, '3': 25.92e9, '4': 25.92e9,
+               '5': 450.e9, '6': 450.e9}
+energies_ft = {'0': (2.0e9 + m_p*c**2/e),
+               '1': 25.92e9,
+               '2': 450.e9, '3': 450.e9, '4': 450.e9,
+               '5': 6.5e12, '6': 6.5e12}
+# Machine-dependent parameters [SI-units] -------------------------------------
+
+
 
 class ParameterScaling(object):
-    
+
     @property
     def phi_b(self):
-        
-        return self.omega_rf * self.tau / 2.
+        return self.omega_rf*self.tau/2.
 
-        
     @property
     def delta_b(self):
-        
-        return self.dE_b / (self.beta_sq * self.energy)
-    
-    
+        return self.dE_b/(self.beta_sq*self.energy)
+
     @property
     def dE_b(self):
-        
-        return np.sqrt(self.beta_sq * self.energy * self.voltage * (1 - 
-                       np.cos(self.phi_b)) / (np.pi * self.harmonic * self.eta_0))
-
+        return np.sqrt(self.beta_sq*self.energy*self.voltage*(1 -
+                       np.cos(self.phi_b)) / (np.pi*self.harmonic*self.eta_0))
 
     @property
     def integral(self):
-        
         return integrate.quad(lambda x: np.sqrt(2.*(np.cos(x) - 
                               np.cos(self.phi_b))), 0, self.phi_b)[0]
 
-                              
     @property
     def emittance(self):
-                          
-        return 4.*self.energy * self.omega_s0 * self.beta_sq * \
-                         self.integral / (self.omega_rf ** 2 * self.eta_0)
+        return 4.*self.energy*self.omega_s0*self.beta_sq*self.integral / \
+               (self.omega_rf**2*self.eta_0)
 
 
     def relativistic_quantities(self):
 
-        self.momentum = np.sqrt(self.energy ** 2 - self.mass ** 2)
-        self.tb1.append("    Synchronous momentum: " 
-                               + np.str(self.momentum) + " eV")
+        self.momentum = np.sqrt(self.energy**2 - self.mass**2)
+        self.tb1.append("    Synchronous momentum: "+
+                        np.str(self.momentum)+" eV")
 
         self.kinetic_energy = self.energy - self.mass
-        self.tb1.append("    Synchronous kinetic energy: " 
-                               + np.str(self.kinetic_energy) + " eV")
+        self.tb1.append("    Synchronous kinetic energy: "+
+                        np.str(self.kinetic_energy)+" eV")
 
-        self.gamma = self.energy / self.mass
-        self.tb1.append("    Synchronous relativistic gamma: " 
-                               + np.str(self.gamma) + "")
-
-        self.beta = np.sqrt(1. - 1. / self.gamma ** 2)
-        self.tb1.append("    Synchronous relativistic beta: " 
-                               + np.str(self.beta) + "")
+        self.gamma = self.energy/self.mass
+        self.tb1.append("    Synchronous relativistic gamma: "+
+                        np.str(self.gamma)+"")
+
+        self.beta = np.sqrt(1. - 1./self.gamma**2)
+        self.tb1.append("    Synchronous relativistic beta: "+
+                        np.str(self.beta)+"")
 
         self.beta_sq = self.beta ** 2
-        self.tb1.append("    Synchronous relativistic beta squared: " 
-                               + np.str(self.beta_sq) + "\n")
+        self.tb1.append("    Synchronous relativistic beta squared: "+
+                        np.str(self.beta_sq)+"\n")
            
     
     def frequencies(self):
         
-        self.t_rev = self.circumference / (self.beta * c)
-        self.tb1.append("    Revolution period: " 
-                               + np.str(self.t_rev * 1.e6) + " us")
-
-        self.f_rev = 1. / self.t_rev
-        self.tb1.append("    Revolution frequency: " 
-                               + np.str(self.f_rev) + " Hz")
-
-        self.omega_rev = 2.*np.pi * self.f_rev
-        self.tb1.append("        Angular revolution frequency: " 
-                               + np.str(self.omega_rev) + " 1/s")
-        
-        self.f_RF = self.harmonic * self.f_rev           
-        self.tb1.append("    RF frequency: " 
-                               + np.str(self.f_RF * 1.e-6) + " MHz")
-
-        self.omega_rf = 2.*np.pi * self.f_RF           
-        self.tb1.append("        Angular RF frequency: " 
-                               + np.str(self.omega_rf) + " 1/s\n")
+        self.t_rev = self.circumference/(self.beta*c)
+        self.tb1.append("    Revolution period: "+
+                        np.str(self.t_rev * 1.e6)+" us")
+
+        self.f_rev = 1./self.t_rev
+        self.tb1.append("    Revolution frequency: "+
+                        np.str(self.f_rev)+" Hz")
+
+        self.omega_rev = 2.*np.pi*self.f_rev
+        self.tb1.append("        Angular revolution frequency: "+
+                        np.str(self.omega_rev)+" 1/s")
+        
+        self.f_RF = self.harmonic*self.f_rev
+        self.tb1.append("    RF frequency: "+np.str(self.f_RF*1.e-6)+" MHz")
+
+        self.omega_rf = 2.*np.pi*self.f_RF
+        self.tb1.append("        Angular RF frequency: "+
+                        np.str(self.omega_rf)+" 1/s\n")
     
     
     def tune(self):
     
-        self.eta_0 = np.fabs(1. / self.gamma_t ** 2 - 1. / self.gamma ** 2)
-        self.tb1.append("    Slippage factor (zeroth order): " 
-                               + np.str(self.eta_0) + "")
-
-        self.Q_s0 = np.sqrt(self.harmonic * self.voltage * self.eta_0 / 
-                           (2.*np.pi * self.beta_sq * self.energy))
-        self.tb1.append("    Central synchrotron tune: " 
-                               + np.str(self.Q_s0) + "")
-
-        self.f_s0 = self.Q_s0 * self.f_rev
-        self.tb1.append("    Central synchrotron frequency: " 
-                               + np.str(self.f_s0) + "")
-
-        self.omega_s0 = 2.*np.pi * self.f_s0           
-        self.tb1.append("        Angular synchrotron frequency: " 
-                               + np.str(self.omega_s0) + " 1/s\n")
+        self.eta_0 = np.fabs(1./self.gamma_t**2 - 1./self.gamma**2)
+        self.tb1.append("    Slippage factor (zeroth order): "+
+                        np.str(self.eta_0)+"")
+
+        self.Q_s0 = np.sqrt(self.harmonic*self.voltage*self.eta_0 /
+                            (2.*np.pi*self.beta_sq*self.energy))
+        self.tb1.append("    Central synchrotron tune: "+np.str(self.Q_s0)+"")
+
+        self.f_s0 = self.Q_s0*self.f_rev
+        self.tb1.append("    Central synchrotron frequency: "+
+                        np.str(self.f_s0)+"")
+
+        self.omega_s0 = 2.*np.pi*self.f_s0
+        self.tb1.append("        Angular synchrotron frequency: "+
+                        np.str(self.omega_s0)+" 1/s\n")
 
 
     def bucket_parameters(self):
         
-        self.tb1.append("Bucket parameters assuming single RF, stationary case, and no intensity effects.\n")
+        self.tb1.append("Bucket parameters assume: single RF, stationary case, and no intensity effects.\n")
 
-        self.bucket_area = 8.*np.sqrt(2.*self.beta_sq * self.energy * self.voltage / 
-                           (np.pi * self.harmonic * self.eta_0)) / self.omega_rf
-        self.tb1.append("    Bucket area: " 
-                               + np.str(self.bucket_area) + " eVs")
-
-        self.dt_max = 0.5 * self.t_rev / self.harmonic
-        self.tb1.append("    Half of bucket length: " 
-                               + np.str(self.dt_max * 1.e9) + " ns")
-        
-        self.dE_max = np.sqrt(2.*self.beta ** 2 * self.energy * self.voltage / 
-                              (np.pi * self.eta_0 * self.harmonic))
-        self.tb1.append("    Half of bucket height: " 
-                               + np.str(self.dE_max * 1.e-6) + " MeV")
+        self.bucket_area = 8.*np.sqrt(2.*self.beta_sq*self.energy*self.voltage /
+                           (np.pi*self.harmonic*self.eta_0)) / self.omega_rf
+        self.tb1.append("    Bucket area: "+np.str(self.bucket_area)+" eVs")
+
+        self.dt_max = 0.5*self.t_rev/self.harmonic
+        self.tb1.append("    Half of bucket length: "+
+                        np.str(self.dt_max*1.e9)+" ns")
+        
+        self.dE_max = np.sqrt(2.*self.beta**2*self.energy*self.voltage /
+                              (np.pi*self.eta_0*self.harmonic))
+        self.tb1.append("    Half of bucket height: "+
+                        np.str(self.dE_max*1.e-6)+" MeV")
        
-        self.delta_max = self.dE_max / (self.beta_sq * self.energy)
-        self.tb1.append("        In relative momentum offset: " 
-                               + np.str(self.delta_max) + "\n")
+        self.delta_max = self.dE_max/(self.beta_sq*self.energy)
+        self.tb1.append("        In relative momentum offset: "+
+                        np.str(self.delta_max)+"\n")
         
         
     def emittance_from_bunch_length(self, four_sigma_bunch_length):
         
         self.tau = four_sigma_bunch_length
         if self.tau >= 2.*self.dt_max:
             self.tb1.append("Chosen bunch length too large for this bucket. Aborting!")
-            #PhaseSpaceError
             raise RuntimeError("Chosen bunch length too large for this bucket. Aborting!")
-        self.tb1.append("Calculating emittance of 4-sigma bunch length: " 
-                               + np.str(self.tau * 1.e9) + " ns")
-
-        self.tb1.append("    Emittance contour in phase: " 
-                               + np.str(self.phi_b) + " rad")
-        self.tb1.append("    Emittance contour in relative momentum: " 
-                               + np.str(self.delta_b) + "")
-        self.tb1.append("    Emittance contour in energy offset: " 
-                               + np.str(self.dE_b * 1.e-6) + " MeV")
-        self.tb1.append("    Longitudinal emittance is: " 
-                               + np.str(self.emittance) + " eVs\n")
+        self.tb1.append("Calculating emittance of 4-sigma bunch length: "+
+                        np.str(self.tau*1.e9)+" ns")
+        self.tb1.append("    Emittance contour in phase: "+
+                        np.str(self.phi_b)+" rad")
+        self.tb1.append("    Emittance contour in relative momentum: "+
+                        np.str(self.delta_b)+"")
+        self.tb1.append("    Emittance contour in energy offset: "+
+                        np.str(self.dE_b*1.e-6)+" MeV")
+        self.tb1.append("    R.m.s. bunch length is: "+
+                        np.str(self.tau*c/4*100)+" cm")
+        self.tb1.append("    R.m.s. energy spread is: "+
+                        np.str(0.5*self.dE_b/self.kinetic_energy)+"")
+        self.tb1.append("    Longitudinal emittance is: "+
+                        np.str(self.emittance)+" eVs\n")
 
 
     def bunch_length_from_emittance(self, emittance):
         
         self.emittance_aim = emittance
         
         if self.emittance_aim >= self.bucket_area:
             self.tb1.append("Chosen emittance too large for this bucket. Aborting!")
-            #PhaseSpaceError
             raise RuntimeError("Chosen emittance too large for this bucket. Aborting!")
-        self.tb1.append("Calculating 4-sigma bunch length for an emittance of " 
-                               + np.str(self.emittance_aim) + " eVs")
+        self.tb1.append("Calculating 4-sigma bunch length for an emittance of "
+                        +np.str(self.emittance_aim)+" eVs")
 
         # Make a guess, iterate to get closer
-        self.tau = self.dt_max / 2. 
+        self.tau = self.dt_max/2.
         while (np.fabs((self.emittance - self.emittance_aim)
-                       / self.emittance_aim) > 0.001):   
-            self.tau *= np.sqrt(self.emittance_aim / self.emittance)
+                       /self.emittance_aim) > 0.001):
+            self.tau *= np.sqrt(self.emittance_aim/self.emittance)
+
+        self.tb1.append("    Bunch length is: "+np.str(self.tau*1.e9)+" ns")
+        self.tb1.append("    Corresponding matched rms relative momentum offset: "+
+                        np.str(self.delta_b)+"")
+        self.tb1.append("    Emittance contour in phase: "+
+                        np.str(self.phi_b)+" rad")
 
-        self.tb1.append("    Bunch length is: " 
-                               + np.str(self.tau * 1.e9) + " ns")
-        self.tb1.append("    Corresponding matched rms relative momentum offset: " 
-                               + np.str(self.delta_b) + "")
-        self.tb1.append("    Emittance contour in phase: " 
-                               + np.str(self.phi_b) + " rad")
-    
-    
     
     def setupUi(self, mainWindow):
         
         mainWindow.setObjectName("mainWindow")
         mainWindow.resize(586, 611)
         mainWindow.setWindowOpacity(1.0)
         mainWindow.setFixedSize(mainWindow.size())
-#         mainWindow.setModal(True)
-        
+
+        # Label "Machine/Optics"
         self.lbMachine = QtWidgets.QLabel(mainWindow)
-        self.lbMachine.setGeometry(QtCore.QRect(20, 20, 70, 17))
+        self.lbMachine.setGeometry(QtCore.QRect(20, 20, 120, 17))
         self.lbMachine.setMinimumSize(QtCore.QSize(70, 0))
         self.lbMachine.setMaximumSize(QtCore.QSize(16777215, 17))
         self.lbMachine.setObjectName("lbMachine")
+
+        # Label "Energy"
         self.lbEnergy = QtWidgets.QLabel(mainWindow)
         self.lbEnergy.setGeometry(QtCore.QRect(20, 80, 70, 17))
         self.lbEnergy.setObjectName("lbEnergy")
+        # Custom energy box
         self.leCustom = QtWidgets.QLineEdit(mainWindow)
         self.leCustom.setEnabled(True)
-        self.leCustom.setGeometry(QtCore.QRect(125, 100, 71, 25))
+        self.leCustom.setGeometry(QtCore.QRect(145, 100, 70, 25))
         self.leCustom.setStyleSheet("background-color: rgb(255, 255, 255);\n"
 "border-color: rgb(0, 0, 0);")
         self.leCustom.hide()
         self.leCustom.setText("")
         self.leCustom.setObjectName("leCustom")
+        # Custom energy label (unit)
         self.lbEV1 = QtWidgets.QLabel(mainWindow)
         self.lbEV1.setEnabled(True)
-        self.lbEV1.setGeometry(QtCore.QRect(200, 100, 30, 25))
+        self.lbEV1.setGeometry(QtCore.QRect(220, 100, 30, 25))
         self.lbEV1.setObjectName("lbEV1")
         self.lbEV1.hide()
+
+        # Label "Gamma Transition"
+        self.rbGammaT = QtWidgets.QLabel(mainWindow)
+        self.rbGammaT.setGeometry(QtCore.QRect(260, 80, 120, 17))
+        self.rbGammaT.setObjectName("rbGammaT")
+        # Custom gamma_t box
+        self.reCustom = QtWidgets.QLineEdit(mainWindow)
+        self.reCustom.setEnabled(True)
+        self.reCustom.setGeometry(QtCore.QRect(385, 100, 70, 25))
+        self.reCustom.setStyleSheet("background-color: rgb(255, 255, 255);\n"
+                                    "border-color: rgb(0, 0, 0);")
+        self.reCustom.hide()
+        self.reCustom.setText("")
+        self.reCustom.setObjectName("reCustom")
+
+        # Label "Voltage" with units
         self.lbVoltage = QtWidgets.QLabel(mainWindow)
         self.lbVoltage.setGeometry(QtCore.QRect(20, 160, 70, 25))
         self.lbVoltage.setObjectName("lbVoltage")
         self.lbEV2 = QtWidgets.QLabel(mainWindow)
         self.lbEV2.setGeometry(QtCore.QRect(150, 160, 31, 25))
         self.lbEV2.setObjectName("lbEV2")
         self.leVoltage = QtWidgets.QLineEdit(mainWindow)
         self.leVoltage.setGeometry(QtCore.QRect(80, 155, 70, 25))
         self.leVoltage.setStyleSheet("background-color: rgb(255, 255, 255);\n"
 "border-color: rgb(0, 0, 0);")
         self.leVoltage.setText("")
         self.leVoltage.setObjectName("leVoltage")
+
+        # Label "Optional"
         self.lbOptional = QtWidgets.QLabel(mainWindow)
         self.lbOptional.setGeometry(QtCore.QRect(20, 230, 70, 17))
         self.lbOptional.setObjectName("lbOptional")
-        
+
+        # Label "Emittance" with units
         self.leEmittance = QtWidgets.QLineEdit(mainWindow)
         self.leEmittance.setGeometry(QtCore.QRect(130, 270, 70, 25))
         self.leEmittance.setStyleSheet("background-color: rgb(255, 255, 255);\n"
 "border-color: rgb(0, 0, 0);")
         self.leEmittance.setText("")
         self.leEmittance.setObjectName("leEmittance")
         self.lbEVS1 = QtWidgets.QLabel(mainWindow)
         self.lbEVS1.setGeometry(QtCore.QRect(200, 275, 41, 25))
         self.lbEVS1.setObjectName("lbEVS1")
         self.lbEVS2 = QtWidgets.QLabel(mainWindow)
         self.lbEVS2.setGeometry(QtCore.QRect(330, 275, 41, 25))
         self.lbEVS2.setObjectName("lbEVS2")
+
+        # Label "Bunch Length" with units
         self.leBunchLength = QtWidgets.QLineEdit(mainWindow)
         self.leBunchLength.setGeometry(QtCore.QRect(260, 270, 70, 25))
         self.leBunchLength.setStyleSheet("background-color: rgb(255, 255, 255);\n"
 "border-color: rgb(0, 0, 0);")
         self.leBunchLength.setText("")
         self.leBunchLength.setObjectName("leBunchLength")
-        
+
+        # "Submit" button
         self.pbSubmit = QtWidgets.QPushButton(mainWindow)
         self.pbSubmit.setGeometry(QtCore.QRect(230, 320, 101, 27))
         self.pbSubmit.setObjectName("pbSumbit")
         self.tb1 = QtWidgets.QTextBrowser(mainWindow)
         self.tb1.setGeometry(QtCore.QRect(10, 350, 561, 241))
         self.tb1.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOn)
         self.tb1.setObjectName("tb1")
+
+        # Drop-down menus Machine/Optics, Energy, Gamma Transition
         self.cbMachine = QtWidgets.QComboBox(mainWindow)
-        self.cbMachine.setGeometry(QtCore.QRect(20, 40, 83, 25))
+        self.cbMachine.setGeometry(QtCore.QRect(20, 40, 115, 25))
         self.cbMachine.setEditable(False)
         self.cbMachine.setObjectName("cbMachine")
-        self.cbMachine.addItem("")
-        self.cbMachine.addItem("")
-        self.cbMachine.addItem("")
-        self.cbMachine.addItem("")
-        self.cbMachine.addItem("")
+        for i in range(len(gamma_ts)):
+            self.cbMachine.addItem("")
         self.cbEnergy = QtWidgets.QComboBox(mainWindow)
-        self.cbEnergy.setGeometry(QtCore.QRect(20, 100, 100, 25))
+        self.cbEnergy.setGeometry(QtCore.QRect(20, 100, 115, 25))
         self.cbEnergy.setObjectName("cbEnergy")
         self.cbEnergy.addItem("")
         self.cbEnergy.addItem("")
         self.cbEnergy.addItem("")
-        
+        self.cbGammaT = QtWidgets.QComboBox(mainWindow)
+        self.cbGammaT.setGeometry(QtCore.QRect(260, 100, 115, 25))
+        self.cbGammaT.setObjectName("cbGammaT")
+        self.cbGammaT.addItem("")
+        self.cbGammaT.addItem("")
+
+        # Radio button Bunch Length
         self.rbBunchLength = QtWidgets.QRadioButton(mainWindow)
         self.rbBunchLength.setGeometry(QtCore.QRect(260, 250, 140, 22))
         self.rbBunchLength.setObjectName("rbBunchLength")
         
+        # Radio button Emittance
         self.rbEmittance = QtWidgets.QRadioButton(mainWindow)
         self.rbEmittance.setGeometry(QtCore.QRect(130, 250, 100, 22))
         self.rbEmittance.setObjectName("rbEmittance")
         
+        # Radio button No option
         self.rbNoOption = QtWidgets.QRadioButton(mainWindow)
         self.rbNoOption.setGeometry(QtCore.QRect(20, 250, 100, 22))
         self.rbNoOption.setObjectName('rbNoOption')
         self.rbNoOption.setChecked(True)
-#         self.rbLayout = QHBoxLayout()
-#         self.rbLayout.addWidget(self.rbBunchLength)
-#         self.rbLayout.addWidget(self.rbEmittance)
-#         self.rbLayout.addWidget(self.rbNoOptioin)
-#         self.rbLayout.setGeometry(QtCore.QRect(10, 10, 10, 10))
-#         self.rbLayout.addStretch(1)
-#         
-#         self.rbGroupBox = QGroupBox()
-#         self.rbGroupBox.setLayout(self.rbLayout)
-#         self.rbGroupBox.setGeometry(QtCore.QRect(10, 10, 10, 10))
-#         
+
         self.retranslateUi(mainWindow)
         QtCore.QMetaObject.connectSlotsByName(mainWindow)
         self.addactions(mainWindow)
-        
+
+
     def retranslateUi(self, mainWindow):
+
         _translate = QtCore.QCoreApplication.translate
-        mainWindow.setWindowTitle(_translate("mainWindow", "Parameter Scaling"))
-        self.lbMachine.setText(_translate("mainWindow", "Machine"))
+
+        # Label texts
+        mainWindow.setWindowTitle(_translate("mainWindow", "Bunch Parameter Calculator"))
+        self.lbMachine.setText(_translate("mainWindow", "Machine, Optics"))
         self.lbEnergy.setText(_translate("mainWindow", "Energy"))
         self.lbEV1.setText(_translate("mainWindow", "[eV]"))
+        self.rbGammaT.setText(_translate("mainWindow", "Transition Gamma"))
         self.lbVoltage.setText(_translate("mainWindow", "Voltage"))
         self.lbEV2.setText(_translate("mainWindow", "[V]"))
         self.lbOptional.setText(_translate("mainWindow", "Optional"))
         self.rbEmittance.setText(_translate("mainWindow", "Emittance"))
         self.lbEVS1.setText(_translate("mainWindow", "[eVs]"))
         self.lbEVS2.setText(_translate("mainWindow", "[s]"))
         self.rbBunchLength.setText(_translate("mainWindow", "Bunch Length"))
         self.rbNoOption.setText(_translate("mainWindow", "No Options"))
-
         self.pbSubmit.setText(_translate("mainWindow", "Submit"))
-        self.cbEnergy.setCurrentText(_translate("mainWindow", "LHC"))
-        self.cbMachine.setItemText(0, _translate("mainWindow", "LHC"))
-        self.cbMachine.setItemText(1, _translate("mainWindow", "PSB"))
-        self.cbMachine.setItemText(2, _translate("mainWindow", "SPS, Q20"))
-        self.cbMachine.setItemText(3, _translate("mainWindow", "SPS, Q26"))
-        self.cbMachine.setItemText(4, _translate("mainWindow", "CPS"))
+
+        # Options in roll-down menu
+        for i, key in enumerate(set_ups.keys()):
+            self.cbMachine.setItemText(i, _translate("mainWindow", key))
         self.cbEnergy.setItemText(0, _translate("mainWindow", "Flat bottom"))
         self.cbEnergy.setItemText(1, _translate("mainWindow", "Flat top"))
         self.cbEnergy.setItemText(2, _translate("mainWindow", "Custom"))
-    
+        self.cbGammaT.setItemText(0, _translate("mainWindow", "Default"))
+        self.cbGammaT.setItemText(1, _translate("mainWindow", "Custom"))
+
     
     def addactions(self, mainWindow):
+
         self.pbSubmit.clicked.connect(self.pbHandler)
         self.cbEnergy.activated[str].connect(self.cbEnergyHandler)
-    
+        self.cbGammaT.activated[str].connect(self.cbGammaTHandler)
+
     def pbHandler(self):
-#         self.tb1.append('pbSubmit was clicked!')
-        
+
         self.machine = str(self.cbMachine.currentText())
-#         self.tb1.append('machine is ' + self.machine)
-        
+        self.setup = set_ups[self.machine]
+
         self.energy_type = self.cbEnergy.currentText()
-        if(self.energy_type == 'Custom'):
+        if self.energy_type == 'Custom':
             self.custom_energy = self.leCustom.text()
             try:
                 self.energy = np.double(self.custom_energy)
             except ValueError:
                 self.tb1.append("Energy not recognized!")
                 return
-                # raise RuntimeError('Energy not recognized. Aborting!')
-#             self.tb1.append('custom_energy is ' + self.custom_energy)
-            
-#         self.tb1.append('energy_type is ' + self.energy_type)
-        
-        
+
+        self.gamma_t = gamma_ts[self.setup]
+        self.gamma_t_type = self.cbGammaT.currentText()
+        if self.gamma_t_type == 'Custom':
+            self.custom_gamma_t = self.reCustom.text()
+            try:
+                self.gamma_t = np.double(self.custom_gamma_t)
+            except ValueError:
+                self.tb1.append("Gamma transition not recognized!")
+                return
+
         self.voltage = self.leVoltage.text()
-#         self.tb1.append('voltage is ' + self.voltage)
-        
         self.emittance_target = self.leEmittance.text()
-#         self.tb1.append('emittance_target is ' + self.emittance_target)
-        
         self.bunch_length_target = self.leBunchLength.text()
-#         self.tb1.append('bunch_length_target is ' + self.bunch_length_target)
         
-        
-        self.tb1.append("Input -- chosen machine: " + 
-                               np.str(self.machine) + "\n")
-
-        # Machine-dependent parameters [SI-units] -----------------------------
-        gamma_ts = {'PSB': 4.0767, 'CPS': np.sqrt(37.2), 'SPS, Q20': 18.,
-                   'SPS, Q26': 22.83, 'LHC': 55.759505}
-        harmonics = {'PSB': 1, 'CPS': 21, 'SPS, Q20': 4620, 'SPS, Q26': 4620,
-                     'LHC': 35640}
-        circumferences = {'PSB': 2 * np.pi * 25, 'CPS': 2 * np.pi * 100.,
-                          'SPS, Q20': 2 * np.pi * 1100.009,
-                          'SPS, Q26': 2 * np.pi * 1100.009, 'LHC': 26658.883}
-        energies_fb = {'PSB': (50.e6 + m_p * c ** 2 / e), 'CPS': 1.4e9, 'SPS, Q20': 25.94e9,
-                       'SPS-Q26': 25.94e9, 'LHC': 450.e9}
-        energies_ft = {'PSB': (1.4e9 + m_p * c ** 2 / e), 'CPS': 25.92e9, 'SPS, Q20': 450.e9,
-                       'SPS, Q26': 450.e9, 'LHC': 6.5e12}
-        # Machine-dependent parameters [SI-units] -----------------------------
-              
-        self.gamma_t = gamma_ts[self.machine]
-        self.alpha = 1. / (self.gamma_t) ** 2
-        self.tb1.append("    * with relativistic gamma at transition: " 
-                               + np.str(self.gamma_t) + "")
-        self.tb1.append("    * with momentum compaction factor: " 
-                               + np.str(self.alpha) + "")
-        
-        self.harmonic = harmonics[self.machine]
-        self.tb1.append("    * with main harmonic: " 
-                               + np.str(self.harmonic) + "")
-        
-        self.circumference = circumferences[self.machine]
-        self.tb1.append("    * and machine circumference: " 
-                               + np.str(self.circumference) + " m\n")
+        self.tb1.append("\n\n"+"**************************** BEAM PARAMETER CALCULATOR ****************************"+"\n")
+        self.tb1.append("Input -- chosen machine/optics: "+
+                        np.str(self.machine)+"\n")
+
+        # Derived parameters --------------------------------------------------
+
+        self.alpha = 1./self.gamma_t**2
+        self.tb1.append("    * with relativistic gamma at transition: "+
+                        np.str(self.gamma_t)+"")
+        self.tb1.append("    * with momentum compaction factor: "+
+                        np.str(self.alpha)+"")
+        
+        self.harmonic = harmonics[self.setup]
+        self.tb1.append("    * with main harmonic: " +np.str(self.harmonic)+"")
+        
+        self.circumference = circumferences[self.setup]
+        self.tb1.append("    * and machine circumference: "+
+                        np.str(self.circumference)+" m\n")
         
         if self.energy_type == 'Flat bottom':
-            self.energy = energies_fb[self.machine]
+            self.energy = energies_fb[self.setup]
         elif self.energy_type == 'Flat top':
-            self.energy = energies_ft[self.machine]
-        
-        self.tb1.append("Input -- synchronous total energy: " 
-                               + np.str(self.energy * 1.e-6) + " MeV")
+            self.energy = energies_ft[self.setup]
+        self.tb1.append("Input -- synchronous total energy: "+
+                        np.str(self.energy*1.e-6)+" MeV")
 
         try:
             self.voltage = np.double(self.voltage)
         except ValueError:
             self.tb1.append("Voltage not recognised!")
             return
-            # raise RuntimeError('Voltage not recognised. Aborting!')
-        self.tb1.append("Input -- RF voltage: " 
-                               + np.str(self.voltage * 1.e-6) + " MV")
-
-        self.mass = m_p * c ** 2 / e
-        self.tb1.append("Input -- particle mass: " 
-                               + np.str(self.mass * 1.e-6) + " MeV\n")
+        self.tb1.append("Input -- RF voltage: "+
+                        np.str(self.voltage*1.e-6)+" MV")
+
+        self.mass = m_p*c**2/e
+        self.tb1.append("Input -- particle mass: "+
+                        np.str(self.mass*1.e-6)+" MeV\n")
                 
         # Derived quantities --------------------------------------------------
         self.relativistic_quantities()
         self.frequencies()
         self.tune()
         self.bucket_parameters()
         
         if self.rbEmittance.isChecked():
             try:
                 self.emittance_target = np.double(self.emittance_target)
             except ValueError:
                 self.tb1.append("Target emittance not recognised!")
                 return 
-                # raise RuntimeError('Target emittance not recognised. Aborting!')
             self.bunch_length_from_emittance(self.emittance_target)
         elif self.rbBunchLength.isChecked():
             try:
                 self.bunch_length_target = np.double(self.bunch_length_target)
             except ValueError:
                 self.tb1.append("Target bunch length not recognised!")
                 return 
-                #raise RuntimeError('Target bunch length not recognised. Aborting!')
             self.emittance_from_bunch_length(self.bunch_length_target)
 
     
     def cbEnergyHandler(self, text):
-#         self.tb1.append('cbEnergy changed to ' + text)
         if text == 'Custom':
             self.leCustom.show()
             self.lbEV1.show()
         else:
             self.leCustom.hide()
             self.lbEV1.hide()
             
 
+    def cbGammaTHandler(self, text):
+        if text == 'Custom':
+            self.reCustom.show()
+        else:
+            self.reCustom.hide()
+
+
+
 if __name__ == "__main__":
     import sys
     app = QtWidgets.QApplication(sys.argv)
     mainWindow = QtWidgets.QMainWindow()
     ui = ParameterScaling()
     ui.setupUi(mainWindow)
     mainWindow.show()
     sys.exit(app.exec_())
-    
-    
+
+
```

### Comparing `blond-2.0.11/blond/toolbox/tomoscope.py` & `blond-2.0.12/blond/toolbox/tomoscope.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/trackers/utilities.py` & `blond-2.0.12/blond/trackers/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from __future__ import division, print_function
 from builtins import range, object
 import warnings
 import numpy as np
 import copy
 from scipy.constants import c
 from scipy.integrate import cumtrapz
-
+from ..utils import bmath as bm
 
 
 def synchrotron_frequency_distribution(Beam, FullRingAndRF, main_harmonic_option = 'lowest_freq', 
                                  turn = 0, TotalInducedVoltage = None, smoothOption = None):
     '''
     *Function to compute the frequency distribution of a distribution for a certain
     RF system and optional intensity effects. The potential well (and induced
@@ -48,18 +48,18 @@
     number of pixels to smooth with smoothOption = N.*
     
     *The particle distribution in synchrotron frequencies of the beam is also
     outputed.*
     '''
     
     # Initialize variables depending on the accelerator parameters
-    slippage_factor = FullRingAndRF.RingAndRFSection_list[0].eta_0[0]
+    slippage_factor = FullRingAndRF.RingAndRFSection_list[0].rf_params.eta_0[0]
                         
     eom_factor_dE = abs(slippage_factor) / (2*Beam.beta**2. * Beam.energy)
-    eom_factor_potential = np.sign(slippage_factor) * Beam.Particle.charge / (FullRingAndRF.RingAndRFSection_list[0].t_rev[0])
+    eom_factor_potential = np.sign(slippage_factor) * Beam.Particle.charge / (FullRingAndRF.RingAndRFSection_list[0].rf_params.t_rev[0])
 
     # Generate potential well
     n_points_potential = int(1e4)
     FullRingAndRF.potential_well_generation(n_points = n_points_potential, 
                                             turn = turn, dt_margin_percent = 0.05, 
                                             main_harmonic_option = main_harmonic_option)
     potential_well_array = FullRingAndRF.potential_well
@@ -182,157 +182,162 @@
 
 class synchrotron_frequency_tracker(object):
     '''
     *This class can be added to the tracking map to track a certain
     number of particles (defined by the user) and to store the evolution
     of their coordinates in phase space in order to compute their synchrotron
     frequency as a function of their amplitude in theta.*
-    
+
     *As the time step between two turns can change with acceleration, make sure
     that the momentum program is set to be constant when using this function,
     or that beta_rel~1.*
-    
+
     *The user can input the minimum and maximum theta for the theta_coordinate_range
     option as [min, max]. The input n_macroparticles will be generated with
     linear spacing between these values. One can also input the theta_coordinate_range
-    as the coordinates of all particles, but the length of the array should 
+    as the coordinates of all particles, but the length of the array should
     match the n_macroparticles value.*
     '''
 
-    def __init__(self, Ring, n_macroparticles, theta_coordinate_range, FullRingAndRF, 
-                 TotalInducedVoltage = None):
-        
+    def __init__(self, Ring, n_macroparticles, theta_coordinate_range, FullRingAndRF,
+                 TotalInducedVoltage=None):
+
         #: *Number of macroparticles used in the synchrotron_frequency_tracker method*
         self.n_macroparticles = int(n_macroparticles)
-        
+
         #: *Copy of the input FullRingAndRF object to retrieve the accelerator programs*
         self.FullRingAndRF = copy.deepcopy(FullRingAndRF)
-        
+
         #: *Copy of the input TotalInducedVoltage object to retrieve the intensity effects
         #: (the synchrotron_frequency_tracker particles are not contributing to the
         #: induced voltage).*
         self.TotalInducedVoltage = None
         if TotalInducedVoltage is not None:
             self.TotalInducedVoltage = TotalInducedVoltage
             intensity = TotalInducedVoltage.profiles.Beam.intensity
         else:
             intensity = 0.
-            
-        from beam.beam import Beam
+
         #: *Beam object containing the same physical information as the real beam,
-        #: but containing only the coordinates of the particles for which the 
+        #: but containing only the coordinates of the particles for which the
         #: synchrotron frequency are computed.*
+        from ..beam.beam import Beam
         self.Beam = Beam(Ring, n_macroparticles, intensity)
-        
+
+        # Ring object for the ring radius
+        self.Ring = Ring
+
         # Generating the distribution from the user input
         if len(theta_coordinate_range) == 2:
             self.Beam.dt = np.linspace(float(theta_coordinate_range[0]),
-                                       float(theta_coordinate_range[1]), n_macroparticles)\
-                                       * (self.Beam.ring_radius/(self.Beam.beta*c))
+                                       float(theta_coordinate_range[1]), n_macroparticles) \
+                           * (self.Ring.ring_radius / (self.Beam.beta * c))
         else:
             if len(theta_coordinate_range) != n_macroparticles:
-                #SynchrotronMotionError
+                # SynchrotronMotionError
                 raise RuntimeError('The input n_macroparticles does not match with the length of the theta_coordinates')
             else:
-                self.Beam.dt = np.array(theta_coordinate_range) * (self.Beam.ring_radius/(self.Beam.beta*c))
-                        
+                self.Beam.dt = np.array(theta_coordinate_range) * (self.Ring.ring_radius / (self.Beam.beta * c))
+
         self.Beam.dE = np.zeros(int(n_macroparticles))
- 
+
         for RFsection in self.FullRingAndRF.RingAndRFSection_list:
             RFsection.beam = self.Beam
-        
+
         #: *Revolution period in [s]*
         self.timeStep = Ring.t_rev[0]
-        
+
         #: *Number of turns of the simulation (+1 to include the input parameters)*
-        self.nTurns = Ring.n_turns+1
-        
+        self.nTurns = Ring.n_turns + 1
+
         #: *Saving the theta coordinates of the particles while tracking*
         self.theta_save = np.zeros((self.nTurns, int(n_macroparticles)))
-        
+
         #: *Saving the dE coordinates of the particles while tracking*
         self.dE_save = np.zeros((self.nTurns, int(n_macroparticles)))
-        
+
         #: *Tracking counter*
         self.counter = 0
-          
-        # The first save coordinates are the input coordinates      
-        self.theta_save[self.counter] = self.Beam.dt / (self.Beam.ring_radius/(self.Beam.beta*c))
+
+        # The first save coordinates are the input coordinates
+        self.theta_save[self.counter] = self.Beam.dt / (self.Ring.ring_radius / (self.Beam.beta * c))
         self.dE_save[self.counter] = self.Beam.dE
-    
-            
+
     def track(self):
         '''
         *Method to track the particles with or without intensity effects.*
         '''
-    
+
         self.FullRingAndRF.track()
-        
+
         if self.TotalInducedVoltage is not None:
             self.TotalInducedVoltage.track_ghosts_particles(self.Beam)
-            
+
         self.counter = self.counter + 1
-        
-        self.theta_save[self.counter] = self.Beam.dt / (self.Beam.ring_radius/(self.Beam.beta*c))
+
+        self.theta_save[self.counter] = self.Beam.dt / (self.Ring.ring_radius / (self.Beam.beta * c))
         self.dE_save[self.counter] = self.Beam.dE
-        
-            
-    def frequency_calculation(self, n_sampling=100000, start_turn = None, end_turn = None):
+
+    def frequency_calculation(self, n_sampling=100000, start_turn=None, end_turn=None):
         '''
         *Method to compute the fft of the particle oscillations in theta and dE
         to obtain their synchrotron frequencies. The particles for which
         the amplitude of oscillations is extending the minimum and maximum
         theta from user input are considered to be lost and their synchrotron
-        frequencies are not calculated.*
+        frequencies are not calculated.
         '''
-        
+
         n_sampling = int(n_sampling)
-        
+
         #: *Saving the synchrotron frequency from the theta oscillations for each particle*
         self.frequency_theta_save = np.zeros(int(self.n_macroparticles))
-        
+
         #: *Saving the synchrotron frequency from the dE oscillations for each particle*
         self.frequency_dE_save = np.zeros(int(self.n_macroparticles))
-        
-        #: *Saving the maximum of oscillations in theta for each particle 
+
+        #: *Saving the maximum of oscillations in theta for each particle
         #: (theta amplitude on the right side of the bunch)*
         self.max_theta_save = np.zeros(int(self.n_macroparticles))
-        
-        #: *Saving the minimum of oscillations in theta for each particle 
+
+        #: *Saving the minimum of oscillations in theta for each particle
         #: (theta amplitude on the left side of the bunch)*
         self.min_theta_save = np.zeros(int(self.n_macroparticles))
-        
-        # Maximum theta for which the particles are considered to be lost        
-        max_theta_range = np.max(self.theta_save[0,:])
-        
+
+        # Maximum theta for which the particles are considered to be lost
+        max_theta_range = np.max(self.theta_save[0, :])
+
         # Minimum theta for which the particles are considered to be lost
-        min_theta_range = np.min(self.theta_save[0,:])
-        
+        min_theta_range = np.min(self.theta_save[0, :])
+
         #: *Frequency array for the synchrotron frequency distribution*
         self.frequency_array = np.fft.rfftfreq(n_sampling, self.timeStep)
-        
+
         if start_turn is None:
             start_turn = 0
-        
+
         if end_turn is None:
             end_turn = self.nTurns + 1
-        
+
         # Computing the synchrotron frequency of each particle from the maximum
         # peak of the FFT.
         for indexParticle in range(0, self.n_macroparticles):
-            self.max_theta_save[indexParticle] = np.max(self.theta_save[start_turn:end_turn,indexParticle])
-            self.min_theta_save[indexParticle] = np.min(self.theta_save[start_turn:end_turn,indexParticle])
-            
-            if (self.max_theta_save[indexParticle]<max_theta_range) and (self.min_theta_save[indexParticle]>min_theta_range):
-            
-                theta_save_fft = abs(np.fft.rfft(self.theta_save[start_turn:end_turn,indexParticle] - np.mean(self.theta_save[start_turn:end_turn,indexParticle]), n_sampling))
-                dE_save_fft = abs(np.fft.rfft(self.dE_save[start_turn:end_turn,indexParticle] - np.mean(self.dE_save[start_turn:end_turn,indexParticle]), n_sampling))
-        
-                self.frequency_theta_save[indexParticle] = self.frequency_array[theta_save_fft==np.max(theta_save_fft)]
-                self.frequency_dE_save[indexParticle] = self.frequency_array[dE_save_fft==np.max(dE_save_fft)]
+            self.max_theta_save[indexParticle] = np.max(self.theta_save[start_turn:end_turn, indexParticle])
+            self.min_theta_save[indexParticle] = np.min(self.theta_save[start_turn:end_turn, indexParticle])
+
+            if (self.max_theta_save[indexParticle] < max_theta_range) and (
+                    self.min_theta_save[indexParticle] > min_theta_range):
+                theta_save_fft = abs(np.fft.rfft(self.theta_save[start_turn:end_turn, indexParticle] - np.mean(
+                    self.theta_save[start_turn:end_turn, indexParticle]), n_sampling))
+                dE_save_fft = abs(np.fft.rfft(self.dE_save[start_turn:end_turn, indexParticle] - np.mean(
+                    self.dE_save[start_turn:end_turn, indexParticle]), n_sampling))
+
+                self.frequency_theta_save[indexParticle] = self.frequency_array[
+                    np.argmax(theta_save_fft == np.max(theta_save_fft))]
+                self.frequency_dE_save[indexParticle] = self.frequency_array[
+                    np.argmax(dE_save_fft == np.max(dE_save_fft))]
 
 
 
 def total_voltage(RFsection_list, harmonic = 'first'):
     """
     Total voltage from all the RF stations and systems in the ring.
     To be generalized.
@@ -378,17 +383,17 @@
     if RFStation.n_rf > 1:
         warnings.warn("WARNING: The Hamiltonian will be calculated for the first harmonic only!")
 
          
     counter = RFStation.counter[0]
     h0 = RFStation.harmonic[0,counter]
     if total_voltage == None:
-        V0 = RFStation.voltage[0,counter]
+        V0 = float(RFStation.voltage[0,counter])
     else: 
-        V0 = total_voltage[counter]
+        V0 = float(total_voltage[counter])
     V0 *= RFStation.Particle.charge
     
     c1 = RFStation.eta_tracking(Beam, counter, dE)*c*np.pi/ \
          (Ring.ring_circumference*Beam.beta*Beam.energy )
     c2 = c*Beam.beta*V0/(h0*Ring.ring_circumference)
      
     phi_s = RFStation.phi_s[counter] 
@@ -399,16 +404,16 @@
     
     # Modulo 2 Pi of bunch phase
     if eta0 < 0:
         phi_b = phase_modulo_below_transition(phi_b)
     elif eta0 > 0:
         phi_b = phase_modulo_above_transition(phi_b)    
 
-    return c1 * dE**2 + c2 * (np.cos(phi_b) - np.cos(phi_s) + 
-                               (phi_b - phi_s) * np.sin(phi_s))
+    return c1 * dE**2 + c2 * (bm.cos(phi_b) - bm.cos(phi_s) + 
+                               (phi_b - phi_s) * bm.sin(phi_s))
          
  
  
 def separatrix(Ring, RFStation, dt):
     r""" Function to calculate the ideal separatrix without intensity effects.
     For single or multiple RF systems. For the time being, multiple RF sections
     are not yet implemented.
@@ -564,16 +569,16 @@
     counter = RFStation.counter[0]
     dt_sep = (np.pi - RFStation.phi_s[counter] 
               - RFStation.phi_rf_d[0,counter])/ \
               RFStation.omega_rf[0,counter]
      
     Hsep = hamiltonian(Ring, RFStation, Beam, dt_sep, 0, 
                        total_voltage = None) 
-    isin = np.fabs(hamiltonian(Ring, RFStation, Beam, 
-                               dt, dE, total_voltage = None)) < np.fabs(Hsep)
+    isin = bm.fabs(hamiltonian(Ring, RFStation, Beam, 
+                               dt, dE, total_voltage = None)) < bm.fabs(Hsep)
      
     return isin
         
 
 
 def minmax_location(x,f):
     '''
@@ -688,26 +693,26 @@
     return time_potential_sep, potential_well_sep
 
 def phase_modulo_above_transition(phi):
     '''
     *Projects a phase array into the range -Pi/2 to +3*Pi/2.*
     '''
     
-    return phi - 2.*np.pi*np.floor(phi/(2.*np.pi))
+    return phi - 2.*np.pi*bm.floor(phi/(2.*np.pi))
 
 
  
 def phase_modulo_below_transition(phi):
     '''
     *Projects a phase array into the range -Pi/2 to +3*Pi/2.*
     '''
     
-    return phi - 2.*np.pi*(np.floor(phi/(2.*np.pi) + 0.5))
+    return phi - 2.*np.pi*(bm.floor(phi/(2.*np.pi) + 0.5))
         
 
 
 def time_modulo(dt, dt_offset, T):
     '''
     *Returns dt projected onto the desired interval.*
     '''
     
-    return dt - T*np.floor((dt + dt_offset)/T)
+    return dt - T*bm.floor((dt + dt_offset)/T)
```

### Comparing `blond-2.0.11/blond/utils/data_check.py` & `blond-2.0.12/blond/utils/data_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/utils/exceptions.py` & `blond-2.0.12/blond/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/utils/track_iteration.py` & `blond-2.0.12/blond/utils/track_iteration.py`

 * *Files identical despite different names*

### Comparing `blond-2.0.11/blond/sanity_check.py` & `blond-2.0.12/blond/sanity_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,18 @@
         if docs:
             self.compile_docs()
         print("*** END SANITY CHECK ***")
 
     def compile_docs(self):
 
         print("COMPILING DOCUMENTATION...")
-        os.chdir("__doc")
+        if os.path.isdir("__doc"):
+            os.chdir("__doc")
+        else:
+            os.chdir("../__doc")
         os.system("make html")
         os.chdir("..")
         print("DOCUMENTATION COMPILED")
         print("")
 
     def pep8_test(self, pep8Files):
 
@@ -58,15 +61,15 @@
         # Ignore E303 too many blank lines (3)
         # Ignore E128 continuation line under-indented for visual indent
 
         def command(x):
             try:
                 print("~~~ EXECUTING PEP8 CHECK ON: %s ~~~" % x)
                 subprocess.check_output(
-                    ['pep8', '--ignore', 'W291,W293,W391,E303,E128', x])
+                    ['pycodestyle', '--ignore', 'W291,W293,W391,E303,E128', x])
             except subprocess.CalledProcessError as e:
                 print(e.output.decode())
         files = []
         if isinstance(pep8Files, str) and (pep8Files == ''):
             print("EXECUTING PEP8 CHECK ON THE ENTIRE BLOND PROJECT\n")
 
             for path, _, Files in os.walk("."):
@@ -153,15 +156,18 @@
                         help='Run all unit-tests (default) or only ' +
                         'unit-tests found in the given files/directories')
 
     args = parser.parse_args()
 
     # Passing a default option if no argument is given
     if len(sys.argv) == 1:
-        args.unitTests = 'unitTests'
+        if os.path.isdir('unittests'):
+            args.unitTests = 'unittests'
+        else:
+            args.unitTests = '../unittests'
 
     # Call the actual sanity check
     SanityCheck(args.all, args.docs, args.pep8Files, args.unitTests)
 
 
 if __name__ == "__main__":
     try:
```

