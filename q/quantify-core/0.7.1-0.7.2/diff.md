# Comparing `tmp/quantify-core-0.7.1.tar.gz` & `tmp/quantify-core-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantify-core-0.7.1.tar", last modified: Thu Mar  9 20:59:07 2023, max compression
+gzip compressed data, was "quantify-core-0.7.2.tar", last modified: Tue May  2 14:25:03 2023, max compression
```

## Comparing `quantify-core-0.7.1.tar` & `quantify-core-0.7.2.tar`

### file list

```diff
@@ -1,256 +1,256 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.065135 quantify-core-0.7.1/
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-03-09 20:58:47.000000 quantify-core-0.7.1/AUTHORS.md
--rw-rw-rw-   0 root         (0) root         (0)    23257 2023-03-09 20:58:47.000000 quantify-core-0.7.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    14586 2023-03-09 20:58:47.000000 quantify-core-0.7.1/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-03-09 20:58:47.000000 quantify-core-0.7.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-03-09 20:58:47.000000 quantify-core-0.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4978 2023-03-09 20:59:07.065135 quantify-core-0.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3403 2023-03-09 20:58:47.000000 quantify-core-0.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.995129 quantify-core-0.7.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     3610 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/api_reference.md
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/authors.md
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/changelog.md
--rwxrwxrwx   0 root         (0) root         (0)    12702 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/contributing.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.995129 quantify-core-0.7.1/docs/images/
--rw-rw-rw-   0 root         (0) root         (0)     2254 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/images/QUANTIFY-FAVICON_16.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.002129 quantify-core-0.7.1/docs/images/install/
--rw-rw-rw-   0 root         (0) root         (0)  2452484 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/images/install/conda_activate.gif
--rw-rw-rw-   0 root         (0) root         (0)   858347 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/images/install/conda_install.gif
--rw-rw-rw-   0 root         (0) root         (0)  1669689 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/images/install/conda_source_installed_all_users.gif
--rw-rw-rw-   0 root         (0) root         (0)    27025 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/images/surface-7-sched.png
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/index.md
--rw-rw-rw-   0 root         (0) root         (0)    12213 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/installation.md
--rw-rw-rw-   0 root         (0) root         (0)     1244 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.960126 quantify-core-0.7.1/docs/technical_notes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.006130 quantify-core-0.7.1/docs/technical_notes/dataset_design/
--rw-rw-rw-   0 root         (0) root         (0)    10751 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/technical_notes/dataset_design/Quantify dataset - advanced examples.md
--rw-rw-rw-   0 root         (0) root         (0)    15748 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/technical_notes/dataset_design/Quantify dataset - examples.md
--rw-rw-rw-   0 root         (0) root         (0)    13349 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/technical_notes/dataset_design/Quantify dataset - specification.md
--rw-rw-rw-   0 root         (0) root         (0)     4651 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/technical_notes/dataset_design/Xarray introduction.md
--rw-rw-rw-   0 root         (0) root         (0)      532 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/technical_notes/dataset_design/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.008130 quantify-core-0.7.1/docs/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)    11536 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/tutorials/Tutorial 1. Controlling a basic experiment using MeasurementControl.md
--rw-rw-rw-   0 root         (0) root         (0)    12972 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/tutorials/Tutorial 2. Advanced capabilities of the MeasurementControl.md
--rw-rw-rw-   0 root         (0) root         (0)    20406 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/tutorials/Tutorial 3. Building custom analyses - the data analysis framework.md
--rw-rw-rw-   0 root         (0) root         (0)     8886 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/tutorials/Tutorial 4. Adaptive Measurements.md
--rw-rw-rw-   0 root         (0) root         (0)    10860 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/tutorials/Tutorial 5. Plot monitor.md
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/tutorials/index.md
--rw-rw-rw-   0 root         (0) root         (0)    30879 2023-03-09 20:58:47.000000 quantify-core-0.7.1/docs/usage.md
--rw-rw-rw-   0 root         (0) root         (0)    17471 2023-03-09 20:58:47.000000 quantify-core-0.7.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.066135 quantify-core-0.7.1/quantify_core/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)       60 2023-03-09 20:59:07.066135 quantify-core-0.7.1/quantify_core/_static_version.py
--rw-rw-rw-   0 root         (0) root         (0)     5795 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.016131 quantify-core-0.7.1/quantify_core/analysis/
--rw-rw-rw-   0 root         (0) root         (0)      693 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    34947 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/analysis/base_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     8117 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/analysis/calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     3413 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/analysis/cosine_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    19691 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/analysis/fitting_models.py
--rw-rw-rw-   0 root         (0) root         (0)     2573 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/analysis/interpolation_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4339 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/analysis/optimization_analysis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.017131 quantify-core-0.7.1/quantify_core/analysis/schemas/
--rw-rw-rw-   0 root         (0) root         (0)     1152 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/analysis/schemas/AnalysisSettings.json
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/analysis/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26708 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/analysis/single_qubit_timedomain.py
--rw-rw-rw-   0 root         (0) root         (0)     7072 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/analysis/spectroscopy_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/analysis/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.020131 quantify-core-0.7.1/quantify_core/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5853 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/data/dataset_adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    15150 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/data/dataset_attrs.py
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/data/experiment.py
--rw-rw-rw-   0 root         (0) root         (0)    42981 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/data/handling.py
--rw-rw-rw-   0 root         (0) root         (0)     2961 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/data/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.022131 quantify-core-0.7.1/quantify_core/measurement/
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/measurement/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42537 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/measurement/control.py
--rw-rw-rw-   0 root         (0) root         (0)      946 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/measurement/gettables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.023131 quantify-core-0.7.1/quantify_core/measurement/schemas/
--rw-rw-rw-   0 root         (0) root         (0)     2516 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/measurement/schemas/Gettable.json
--rw-rw-rw-   0 root         (0) root         (0)     1646 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/measurement/schemas/Settable.json
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/measurement/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3094 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/measurement/types.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.027132 quantify-core-0.7.1/quantify_core/utilities/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1849 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/utilities/_docs_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1209 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/utilities/_tests_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    19486 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/utilities/dataset_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     7263 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/utilities/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)    12932 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/utilities/examples_support.py
--rw-rw-rw-   0 root         (0) root         (0)     9164 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/utilities/experiment_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     5882 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/utilities/general.py
--rw-rw-rw-   0 root         (0) root         (0)     3223 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/utilities/inspect_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.030132 quantify-core-0.7.1/quantify_core/visualization/
--rw-rw-rw-   0 root         (0) root         (0)    14046 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/visualization/SI_utilities.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/visualization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/visualization/_appnope.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/visualization/color_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.031132 quantify-core-0.7.1/quantify_core/visualization/ins_mon_widget/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/visualization/ins_mon_widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9743 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/visualization/ins_mon_widget/qc_snapshot_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     8852 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/visualization/instrument_monitor.py
--rw-rw-rw-   0 root         (0) root         (0)    20681 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/visualization/mpl_plotting.py
--rw-rw-rw-   0 root         (0) root         (0)     4368 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/visualization/plot_interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)    10576 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/visualization/pyqt_plotmon.py
--rw-rw-rw-   0 root         (0) root         (0)    28735 2023-03-09 20:58:47.000000 quantify-core-0.7.1/quantify_core/visualization/pyqt_plotmon_remote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.013130 quantify-core-0.7.1/quantify_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4978 2023-03-09 20:59:06.000000 quantify-core-0.7.1/quantify_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9006 2023-03-09 20:59:06.000000 quantify-core-0.7.1/quantify_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 20:59:06.000000 quantify-core-0.7.1/quantify_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 20:58:55.000000 quantify-core-0.7.1/quantify_core.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      597 2023-03-09 20:59:06.000000 quantify-core-0.7.1/quantify_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-09 20:59:06.000000 quantify-core-0.7.1/quantify_core.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-09 20:59:07.066135 quantify-core-0.7.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      667 2023-03-09 20:58:47.000000 quantify-core-0.7.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.032132 quantify-core-0.7.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.035132 quantify-core-0.7.1/tests/analysis/
--rw-rw-rw-   0 root         (0) root         (0)     9901 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/analysis/test_base_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     3385 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/analysis/test_calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     3176 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/analysis/test_fitting_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1134 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/analysis/test_interpolation_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/analysis/test_optimization_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18050 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/analysis/test_single_qubit_timedomain.py
--rw-rw-rw-   0 root         (0) root         (0)     3628 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/analysis/test_spectroscopy_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     1415 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/analysis/test_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.036132 quantify-core-0.7.1/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29501 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/data/test_data_handling.py
--rw-rw-rw-   0 root         (0) root         (0)     3534 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/data/test_experiment.py
--rw-rw-rw-   0 root         (0) root         (0)     1849 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/data/test_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.038133 quantify-core-0.7.1/tests/measurement/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/measurement/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    51340 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/measurement/test_measurement_control.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/measurement/test_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.039133 quantify-core-0.7.1/tests/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.966127 quantify-core-0.7.1/tests/test_data/20200430/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.039133 quantify-core-0.7.1/tests/test_data/20200430/20200430-170837-001-315f36-Cosine test/
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20200430/20200430-170837-001-315f36-Cosine test/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.967126 quantify-core-0.7.1/tests/test_data/20200504/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.039133 quantify-core-0.7.1/tests/test_data/20200504/20200504-191556-002-4209ee-2D Cosine test/
--rw-rw-rw-   0 root         (0) root         (0)    13868 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20200504/20200504-191556-002-4209ee-2D Cosine test/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.968127 quantify-core-0.7.1/tests/test_data/20200814/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.040133 quantify-core-0.7.1/tests/test_data/20200814/20200814-134652-492-fbf254-save/
--rw-rw-rw-   0 root         (0) root         (0)     4037 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20200814/20200814-134652-492-fbf254-save/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.970127 quantify-core-0.7.1/tests/test_data/20201124/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.040133 quantify-core-0.7.1/tests/test_data/20201124/20201124-184709-137-8a5112-(0) Spec IF=0.000 MHz/
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20201124/20201124-184709-137-8a5112-(0) Spec IF=0.000 MHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.041133 quantify-core-0.7.1/tests/test_data/20201124/20201124-184716-237-918bee-(1) Spec IF=20.000 MHz/
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20201124/20201124-184716-237-918bee-(1) Spec IF=20.000 MHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.041133 quantify-core-0.7.1/tests/test_data/20201124/20201124-184722-988-0463d4-(2) Spec IF=-20.000 MHz/
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20201124/20201124-184722-988-0463d4-(2) Spec IF=-20.000 MHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.041133 quantify-core-0.7.1/tests/test_data/20201124/20201124-184729-618-85970f-(3) Spec IF=40.000 MHz/
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20201124/20201124-184729-618-85970f-(3) Spec IF=40.000 MHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.042133 quantify-core-0.7.1/tests/test_data/20201124/20201124-184736-341-3628d4-(4) Spec IF=-40.000 MHz/
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20201124/20201124-184736-341-3628d4-(4) Spec IF=-40.000 MHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.970127 quantify-core-0.7.1/tests/test_data/20210118/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.043133 quantify-core-0.7.1/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/
--rw-rw-rw-   0 root         (0) root         (0)   240636 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/dataset.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    36780 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.971127 quantify-core-0.7.1/tests/test_data/20210126/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.044133 quantify-core-0.7.1/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/
--rw-rw-rw-   0 root         (0) root         (0)   244060 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/dataset.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    30350 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.972127 quantify-core-0.7.1/tests/test_data/20210227/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.045133 quantify-core-0.7.1/tests/test_data/20210227/20210227-172939-723-53d82c-Resonator_power_id6_4.612GHz/
--rw-rw-rw-   0 root         (0) root         (0)    73496 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210227/20210227-172939-723-53d82c-Resonator_power_id6_4.612GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.045133 quantify-core-0.7.1/tests/test_data/20210227/20210227-174714-680-31df85-Resonator_id7_4.660GHz/
--rw-rw-rw-   0 root         (0) root         (0)    13616 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210227/20210227-174714-680-31df85-Resonator_id7_4.660GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.046133 quantify-core-0.7.1/tests/test_data/20210305/
--rw-rw-rw-   0 root         (0) root         (0)    10244 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210305/.DS_Store
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.046133 quantify-core-0.7.1/tests/test_data/20210305/20210305-152943-497-ad8670-Resonator_id2_4.483GHz/
--rw-rw-rw-   0 root         (0) root         (0)    12464 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210305/20210305-152943-497-ad8670-Resonator_id2_4.483GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.046133 quantify-core-0.7.1/tests/test_data/20210305/20210305-154735-413-142768-Resonator_id2_4.483GHz/
--rw-rw-rw-   0 root         (0) root         (0)    27568 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210305/20210305-154735-413-142768-Resonator_id2_4.483GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.047133 quantify-core-0.7.1/tests/test_data/20210305/20210305-160157-184-3c17e9-Resonator_id4_4.541GHz/
--rw-rw-rw-   0 root         (0) root         (0)    27568 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210305/20210305-160157-184-3c17e9-Resonator_id4_4.541GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.047133 quantify-core-0.7.1/tests/test_data/20210305/20210305-161550-671-982c6d-Resonator_id5_4.577GHz/
--rw-rw-rw-   0 root         (0) root         (0)    27568 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210305/20210305-161550-671-982c6d-Resonator_id5_4.577GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.974127 quantify-core-0.7.1/tests/test_data/20210319/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.048133 quantify-core-0.7.1/tests/test_data/20210319/20210319-094728-327-69b211-load_settings_test/
--rw-rw-rw-   0 root         (0) root         (0)     2674 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210319/20210319-094728-327-69b211-load_settings_test/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.975127 quantify-core-0.7.1/tests/test_data/20210322/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.048133 quantify-core-0.7.1/tests/test_data/20210322/20210322-205253-758-6689ca-T1 at 4.715GHz/
--rw-rw-rw-   0 root         (0) root         (0)    11464 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210322/20210322-205253-758-6689ca-T1 at 4.715GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.976127 quantify-core-0.7.1/tests/test_data/20210331/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.049133 quantify-core-0.7.1/tests/test_data/20210331/20210331-133734-718-aa9c83 AllXY q0/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210331/20210331-133734-718-aa9c83 AllXY q0/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.977127 quantify-core-0.7.1/tests/test_data/20210419/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.049133 quantify-core-0.7.1/tests/test_data/20210419/20210419-153127-883-fa4508-Rabi oscillation at 4.515GHz/
--rw-rw-rw-   0 root         (0) root         (0)    11464 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210419/20210419-153127-883-fa4508-Rabi oscillation at 4.515GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.049133 quantify-core-0.7.1/tests/test_data/20210419/20210419-170747-902-9c5a05-Offset_calibration/
--rw-rw-rw-   0 root         (0) root         (0)    13176 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210419/20210419-170747-902-9c5a05-Offset_calibration/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.050134 quantify-core-0.7.1/tests/test_data/20210419/20210419-173649-456-23c5f3-AllXY q0/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210419/20210419-173649-456-23c5f3-AllXY q0/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.978128 quantify-core-0.7.1/tests/test_data/20210420/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.050134 quantify-core-0.7.1/tests/test_data/20210420/20210420-001339-580-97bdef-Echo at 4.715GHz/
--rw-rw-rw-   0 root         (0) root         (0)    12928 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210420/20210420-001339-580-97bdef-Echo at 4.715GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.978128 quantify-core-0.7.1/tests/test_data/20210422/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.051133 quantify-core-0.7.1/tests/test_data/20210422/20210422-104958-297-7d6034-Ramsey oscillation at 4.715GHz/
--rw-rw-rw-   0 root         (0) root         (0)    11464 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210422/20210422-104958-297-7d6034-Ramsey oscillation at 4.715GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.978128 quantify-core-0.7.1/tests/test_data/20210827/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.051133 quantify-core-0.7.1/tests/test_data/20210827/20210827-174946-357-70a986-T1 experiment q0/
--rw-rw-rw-   0 root         (0) root         (0)    12024 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210827/20210827-174946-357-70a986-T1 experiment q0/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.052134 quantify-core-0.7.1/tests/test_data/20210827/20210827-175004-087-ab1aab-Ramsey oscillation q0 at 4.9969 GHz/
--rw-rw-rw-   0 root         (0) root         (0)    12024 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210827/20210827-175004-087-ab1aab-Ramsey oscillation q0 at 4.9969 GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.052134 quantify-core-0.7.1/tests/test_data/20210827/20210827-175021-521-251f28-Echo experiment q0/
--rw-rw-rw-   0 root         (0) root         (0)    12024 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210827/20210827-175021-521-251f28-Echo experiment q0/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.980128 quantify-core-0.7.1/tests/test_data/20210901/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.052134 quantify-core-0.7.1/tests/test_data/20210901/20210901-132357-561-5c3ef7-Ramsey oscillation q0 at 6.1400 GHz/
--rw-rw-rw-   0 root         (0) root         (0)    13848 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20210901/20210901-132357-561-5c3ef7-Ramsey oscillation q0 at 6.1400 GHz/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.982128 quantify-core-0.7.1/tests/test_data/20211029/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.053134 quantify-core-0.7.1/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.054134 quantify-core-0.7.1/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/
--rw-rw-rw-   0 root         (0) root         (0)    12032 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    14504 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/dataset.hdf5
--rw-rw-rw-   0 root         (0) root         (0)   175606 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.055134 quantify-core-0.7.1/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.055134 quantify-core-0.7.1/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/
--rw-rw-rw-   0 root         (0) root         (0)    12032 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    14504 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/dataset.hdf5
--rw-rw-rw-   0 root         (0) root         (0)   175607 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.056134 quantify-core-0.7.1/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.057134 quantify-core-0.7.1/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/
--rw-rw-rw-   0 root         (0) root         (0)    12032 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    14504 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/dataset.hdf5
--rw-rw-rw-   0 root         (0) root         (0)   175605 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.983128 quantify-core-0.7.1/tests/test_data/20220409/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.058134 quantify-core-0.7.1/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/
--rw-rw-rw-   0 root         (0) root         (0)    13096 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/dataset.hdf5
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.984128 quantify-core-0.7.1/tests/test_data/20220509/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.058134 quantify-core-0.7.1/tests/test_data/20220509/20220509-204728-327-69b211-load_settings_test_nested/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20220509/20220509-204728-327-69b211-load_settings_test_nested/snapshot.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:06.986128 quantify-core-0.7.1/tests/test_data/20220930/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.058134 quantify-core-0.7.1/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.059134 quantify-core-0.7.1/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/analysis_QubitSpectroscopyAnalysis/
--rw-rw-rw-   0 root         (0) root         (0)    12032 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    16000 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.059134 quantify-core-0.7.1/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.060134 quantify-core-0.7.1/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/analysis_QubitSpectroscopyAnalysis/
--rw-rw-rw-   0 root         (0) root         (0)    12032 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    16000 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/dataset.hdf5
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.060134 quantify-core-0.7.1/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.061134 quantify-core-0.7.1/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/analysis_QubitSpectroscopyAnalysis/
--rw-rw-rw-   0 root         (0) root         (0)    12032 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
--rw-rw-rw-   0 root         (0) root         (0)    16000 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/dataset.hdf5
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.061134 quantify-core-0.7.1/tests/test_data/empty/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/empty/nothing
--rw-rw-rw-   0 root         (0) root         (0)     1538 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_data/transmon_test_config.json
--rw-rw-rw-   0 root         (0) root         (0)     2210 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/test_headers_and_copyright.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.063135 quantify-core-0.7.1/tests/utilities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4296 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/utilities/test_deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     9201 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/utilities/test_experiment_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2788 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/utilities/test_general.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/utilities/test_inspect_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 20:59:07.065135 quantify-core-0.7.1/tests/visualization/
--rw-rw-rw-   0 root         (0) root         (0)     9133 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/visualization/test_SI_utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     7151 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/visualization/test_instrument_monitor.py
--rw-rw-rw-   0 root         (0) root         (0)     4860 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/visualization/test_mpl_plotting.py
--rw-rw-rw-   0 root         (0) root         (0)     8018 2023-03-09 20:58:47.000000 quantify-core-0.7.1/tests/visualization/test_pyqt_plotmon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.557025 quantify-core-0.7.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-05-02 14:24:43.000000 quantify-core-0.7.2/AUTHORS.md
+-rw-rw-rw-   0 root         (0) root         (0)    23823 2023-05-02 14:24:43.000000 quantify-core-0.7.2/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    14586 2023-05-02 14:24:43.000000 quantify-core-0.7.2/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-05-02 14:24:43.000000 quantify-core-0.7.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-02 14:24:43.000000 quantify-core-0.7.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4980 2023-05-02 14:25:03.557025 quantify-core-0.7.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3405 2023-05-02 14:24:43.000000 quantify-core-0.7.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.490017 quantify-core-0.7.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     3610 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/api_reference.md
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/authors.md
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/changelog.md
+-rwxrwxrwx   0 root         (0) root         (0)    12702 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/contributing.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.491017 quantify-core-0.7.2/docs/images/
+-rw-rw-rw-   0 root         (0) root         (0)     2254 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/images/QUANTIFY-FAVICON_16.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.496018 quantify-core-0.7.2/docs/images/install/
+-rw-rw-rw-   0 root         (0) root         (0)  2452484 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/images/install/conda_activate.gif
+-rw-rw-rw-   0 root         (0) root         (0)   858347 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/images/install/conda_install.gif
+-rw-rw-rw-   0 root         (0) root         (0)  1669689 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/images/install/conda_source_installed_all_users.gif
+-rw-rw-rw-   0 root         (0) root         (0)    27025 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/images/surface-7-sched.png
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/index.md
+-rw-rw-rw-   0 root         (0) root         (0)    12583 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/installation.md
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.456013 quantify-core-0.7.2/docs/technical_notes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.499018 quantify-core-0.7.2/docs/technical_notes/dataset_design/
+-rw-rw-rw-   0 root         (0) root         (0)    10751 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/technical_notes/dataset_design/Quantify dataset - advanced examples.md
+-rw-rw-rw-   0 root         (0) root         (0)    15748 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/technical_notes/dataset_design/Quantify dataset - examples.md
+-rw-rw-rw-   0 root         (0) root         (0)    13349 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/technical_notes/dataset_design/Quantify dataset - specification.md
+-rw-rw-rw-   0 root         (0) root         (0)     4651 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/technical_notes/dataset_design/Xarray introduction.md
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/technical_notes/dataset_design/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.502019 quantify-core-0.7.2/docs/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)    11536 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/tutorials/Tutorial 1. Controlling a basic experiment using MeasurementControl.md
+-rw-rw-rw-   0 root         (0) root         (0)    12972 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/tutorials/Tutorial 2. Advanced capabilities of the MeasurementControl.md
+-rw-rw-rw-   0 root         (0) root         (0)    20406 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/tutorials/Tutorial 3. Building custom analyses - the data analysis framework.md
+-rw-rw-rw-   0 root         (0) root         (0)     8886 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/tutorials/Tutorial 4. Adaptive Measurements.md
+-rw-rw-rw-   0 root         (0) root         (0)    10860 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/tutorials/Tutorial 5. Plot monitor.md
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/tutorials/index.md
+-rw-rw-rw-   0 root         (0) root         (0)    30879 2023-05-02 14:24:43.000000 quantify-core-0.7.2/docs/usage.md
+-rw-rw-rw-   0 root         (0) root         (0)    17490 2023-05-02 14:24:43.000000 quantify-core-0.7.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.557025 quantify-core-0.7.2/quantify_core/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-02 14:25:03.557025 quantify-core-0.7.2/quantify_core/_static_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5795 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.509019 quantify-core-0.7.2/quantify_core/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)      693 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/analysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    34981 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/analysis/base_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8117 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/analysis/calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     3413 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/analysis/cosine_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    19691 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/analysis/fitting_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2573 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/analysis/interpolation_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4339 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/analysis/optimization_analysis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.510019 quantify-core-0.7.2/quantify_core/analysis/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)     1152 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/analysis/schemas/AnalysisSettings.json
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/analysis/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26708 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/analysis/single_qubit_timedomain.py
+-rw-rw-rw-   0 root         (0) root         (0)     7072 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/analysis/spectroscopy_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/analysis/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.512020 quantify-core-0.7.2/quantify_core/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5853 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/data/dataset_adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)    15150 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/data/dataset_attrs.py
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/data/experiment.py
+-rw-rw-rw-   0 root         (0) root         (0)    42997 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/data/handling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2961 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/data/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.514020 quantify-core-0.7.2/quantify_core/measurement/
+-rw-rw-rw-   0 root         (0) root         (0)      725 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/measurement/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42537 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/measurement/control.py
+-rw-rw-rw-   0 root         (0) root         (0)      946 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/measurement/gettables.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.515020 quantify-core-0.7.2/quantify_core/measurement/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)     2516 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/measurement/schemas/Gettable.json
+-rw-rw-rw-   0 root         (0) root         (0)     1646 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/measurement/schemas/Settable.json
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/measurement/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3094 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/measurement/types.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.519020 quantify-core-0.7.2/quantify_core/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/utilities/_docs_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/utilities/_tests_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    19486 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/utilities/dataset_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     7263 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/utilities/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)    12926 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/utilities/examples_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     8694 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/utilities/experiment_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5882 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/utilities/general.py
+-rw-rw-rw-   0 root         (0) root         (0)     3223 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/utilities/inspect_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.522021 quantify-core-0.7.2/quantify_core/visualization/
+-rw-rw-rw-   0 root         (0) root         (0)    14166 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/visualization/SI_utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/visualization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/visualization/_appnope.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/visualization/color_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.523021 quantify-core-0.7.2/quantify_core/visualization/ins_mon_widget/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/visualization/ins_mon_widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9725 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/visualization/ins_mon_widget/qc_snapshot_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     8852 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/visualization/instrument_monitor.py
+-rw-rw-rw-   0 root         (0) root         (0)    20681 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/visualization/mpl_plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)     4368 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/visualization/plot_interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)    10576 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/visualization/pyqt_plotmon.py
+-rw-rw-rw-   0 root         (0) root         (0)    28735 2023-05-02 14:24:43.000000 quantify-core-0.7.2/quantify_core/visualization/pyqt_plotmon_remote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.506019 quantify-core-0.7.2/quantify_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4980 2023-05-02 14:25:03.000000 quantify-core-0.7.2/quantify_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9006 2023-05-02 14:25:03.000000 quantify-core-0.7.2/quantify_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 14:25:03.000000 quantify-core-0.7.2/quantify_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 14:24:51.000000 quantify-core-0.7.2/quantify_core.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      609 2023-05-02 14:25:03.000000 quantify-core-0.7.2/quantify_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-02 14:25:03.000000 quantify-core-0.7.2/quantify_core.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 14:25:03.557025 quantify-core-0.7.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      667 2023-05-02 14:24:43.000000 quantify-core-0.7.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.524021 quantify-core-0.7.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.527021 quantify-core-0.7.2/tests/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)     9901 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/analysis/test_base_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     3385 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/analysis/test_calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     3176 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/analysis/test_fitting_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/analysis/test_interpolation_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/analysis/test_optimization_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18050 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/analysis/test_single_qubit_timedomain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3628 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/analysis/test_spectroscopy_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/analysis/test_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.529022 quantify-core-0.7.2/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29501 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/data/test_data_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)     3534 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/data/test_experiment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/data/test_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.530022 quantify-core-0.7.2/tests/measurement/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/measurement/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    51340 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/measurement/test_measurement_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/measurement/test_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.531022 quantify-core-0.7.2/tests/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.462014 quantify-core-0.7.2/tests/test_data/20200430/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.531022 quantify-core-0.7.2/tests/test_data/20200430/20200430-170837-001-315f36-Cosine test/
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20200430/20200430-170837-001-315f36-Cosine test/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.462014 quantify-core-0.7.2/tests/test_data/20200504/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.532022 quantify-core-0.7.2/tests/test_data/20200504/20200504-191556-002-4209ee-2D Cosine test/
+-rw-rw-rw-   0 root         (0) root         (0)    13868 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20200504/20200504-191556-002-4209ee-2D Cosine test/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.463014 quantify-core-0.7.2/tests/test_data/20200814/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.532022 quantify-core-0.7.2/tests/test_data/20200814/20200814-134652-492-fbf254-save/
+-rw-rw-rw-   0 root         (0) root         (0)     4037 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20200814/20200814-134652-492-fbf254-save/snapshot.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.465014 quantify-core-0.7.2/tests/test_data/20201124/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.533022 quantify-core-0.7.2/tests/test_data/20201124/20201124-184709-137-8a5112-(0) Spec IF=0.000 MHz/
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20201124/20201124-184709-137-8a5112-(0) Spec IF=0.000 MHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.533022 quantify-core-0.7.2/tests/test_data/20201124/20201124-184716-237-918bee-(1) Spec IF=20.000 MHz/
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20201124/20201124-184716-237-918bee-(1) Spec IF=20.000 MHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.534022 quantify-core-0.7.2/tests/test_data/20201124/20201124-184722-988-0463d4-(2) Spec IF=-20.000 MHz/
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20201124/20201124-184722-988-0463d4-(2) Spec IF=-20.000 MHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.534022 quantify-core-0.7.2/tests/test_data/20201124/20201124-184729-618-85970f-(3) Spec IF=40.000 MHz/
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20201124/20201124-184729-618-85970f-(3) Spec IF=40.000 MHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.534022 quantify-core-0.7.2/tests/test_data/20201124/20201124-184736-341-3628d4-(4) Spec IF=-40.000 MHz/
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20201124/20201124-184736-341-3628d4-(4) Spec IF=-40.000 MHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.465014 quantify-core-0.7.2/tests/test_data/20210118/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.535022 quantify-core-0.7.2/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/
+-rw-rw-rw-   0 root         (0) root         (0)   240636 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/dataset.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)    36780 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/snapshot.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.466014 quantify-core-0.7.2/tests/test_data/20210126/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.537022 quantify-core-0.7.2/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/
+-rw-rw-rw-   0 root         (0) root         (0)   244060 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/dataset.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)    30350 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/snapshot.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.467015 quantify-core-0.7.2/tests/test_data/20210227/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.537022 quantify-core-0.7.2/tests/test_data/20210227/20210227-172939-723-53d82c-Resonator_power_id6_4.612GHz/
+-rw-rw-rw-   0 root         (0) root         (0)    73496 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210227/20210227-172939-723-53d82c-Resonator_power_id6_4.612GHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.537022 quantify-core-0.7.2/tests/test_data/20210227/20210227-174714-680-31df85-Resonator_id7_4.660GHz/
+-rw-rw-rw-   0 root         (0) root         (0)    13616 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210227/20210227-174714-680-31df85-Resonator_id7_4.660GHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.538023 quantify-core-0.7.2/tests/test_data/20210305/
+-rw-rw-rw-   0 root         (0) root         (0)    10244 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210305/.DS_Store
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.538023 quantify-core-0.7.2/tests/test_data/20210305/20210305-152943-497-ad8670-Resonator_id2_4.483GHz/
+-rw-rw-rw-   0 root         (0) root         (0)    12464 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210305/20210305-152943-497-ad8670-Resonator_id2_4.483GHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.539023 quantify-core-0.7.2/tests/test_data/20210305/20210305-154735-413-142768-Resonator_id2_4.483GHz/
+-rw-rw-rw-   0 root         (0) root         (0)    27568 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210305/20210305-154735-413-142768-Resonator_id2_4.483GHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.539023 quantify-core-0.7.2/tests/test_data/20210305/20210305-160157-184-3c17e9-Resonator_id4_4.541GHz/
+-rw-rw-rw-   0 root         (0) root         (0)    27568 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210305/20210305-160157-184-3c17e9-Resonator_id4_4.541GHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.540023 quantify-core-0.7.2/tests/test_data/20210305/20210305-161550-671-982c6d-Resonator_id5_4.577GHz/
+-rw-rw-rw-   0 root         (0) root         (0)    27568 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210305/20210305-161550-671-982c6d-Resonator_id5_4.577GHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.469015 quantify-core-0.7.2/tests/test_data/20210319/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.540023 quantify-core-0.7.2/tests/test_data/20210319/20210319-094728-327-69b211-load_settings_test/
+-rw-rw-rw-   0 root         (0) root         (0)     2674 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210319/20210319-094728-327-69b211-load_settings_test/snapshot.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.470015 quantify-core-0.7.2/tests/test_data/20210322/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.540023 quantify-core-0.7.2/tests/test_data/20210322/20210322-205253-758-6689ca-T1 at 4.715GHz/
+-rw-rw-rw-   0 root         (0) root         (0)    11464 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210322/20210322-205253-758-6689ca-T1 at 4.715GHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.471015 quantify-core-0.7.2/tests/test_data/20210331/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.541023 quantify-core-0.7.2/tests/test_data/20210331/20210331-133734-718-aa9c83 AllXY q0/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210331/20210331-133734-718-aa9c83 AllXY q0/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.472015 quantify-core-0.7.2/tests/test_data/20210419/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.541023 quantify-core-0.7.2/tests/test_data/20210419/20210419-153127-883-fa4508-Rabi oscillation at 4.515GHz/
+-rw-rw-rw-   0 root         (0) root         (0)    11464 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210419/20210419-153127-883-fa4508-Rabi oscillation at 4.515GHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.542023 quantify-core-0.7.2/tests/test_data/20210419/20210419-170747-902-9c5a05-Offset_calibration/
+-rw-rw-rw-   0 root         (0) root         (0)    13176 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210419/20210419-170747-902-9c5a05-Offset_calibration/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.542023 quantify-core-0.7.2/tests/test_data/20210419/20210419-173649-456-23c5f3-AllXY q0/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210419/20210419-173649-456-23c5f3-AllXY q0/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.473015 quantify-core-0.7.2/tests/test_data/20210420/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.542023 quantify-core-0.7.2/tests/test_data/20210420/20210420-001339-580-97bdef-Echo at 4.715GHz/
+-rw-rw-rw-   0 root         (0) root         (0)    12928 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210420/20210420-001339-580-97bdef-Echo at 4.715GHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.473015 quantify-core-0.7.2/tests/test_data/20210422/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.543023 quantify-core-0.7.2/tests/test_data/20210422/20210422-104958-297-7d6034-Ramsey oscillation at 4.715GHz/
+-rw-rw-rw-   0 root         (0) root         (0)    11464 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210422/20210422-104958-297-7d6034-Ramsey oscillation at 4.715GHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.475015 quantify-core-0.7.2/tests/test_data/20210827/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.543023 quantify-core-0.7.2/tests/test_data/20210827/20210827-174946-357-70a986-T1 experiment q0/
+-rw-rw-rw-   0 root         (0) root         (0)    12024 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210827/20210827-174946-357-70a986-T1 experiment q0/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.544023 quantify-core-0.7.2/tests/test_data/20210827/20210827-175004-087-ab1aab-Ramsey oscillation q0 at 4.9969 GHz/
+-rw-rw-rw-   0 root         (0) root         (0)    12024 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210827/20210827-175004-087-ab1aab-Ramsey oscillation q0 at 4.9969 GHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.544023 quantify-core-0.7.2/tests/test_data/20210827/20210827-175021-521-251f28-Echo experiment q0/
+-rw-rw-rw-   0 root         (0) root         (0)    12024 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210827/20210827-175021-521-251f28-Echo experiment q0/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.475015 quantify-core-0.7.2/tests/test_data/20210901/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.544023 quantify-core-0.7.2/tests/test_data/20210901/20210901-132357-561-5c3ef7-Ramsey oscillation q0 at 6.1400 GHz/
+-rw-rw-rw-   0 root         (0) root         (0)    13848 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20210901/20210901-132357-561-5c3ef7-Ramsey oscillation q0 at 6.1400 GHz/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.477016 quantify-core-0.7.2/tests/test_data/20211029/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.545023 quantify-core-0.7.2/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.546023 quantify-core-0.7.2/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/
+-rw-rw-rw-   0 root         (0) root         (0)    12032 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)    14504 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/dataset.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)   175606 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/snapshot.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.547024 quantify-core-0.7.2/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.547024 quantify-core-0.7.2/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/
+-rw-rw-rw-   0 root         (0) root         (0)    12032 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)    14504 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/dataset.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)   175607 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/snapshot.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.548024 quantify-core-0.7.2/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.548024 quantify-core-0.7.2/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/
+-rw-rw-rw-   0 root         (0) root         (0)    12032 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)    14504 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/dataset.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)   175605 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/snapshot.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.478016 quantify-core-0.7.2/tests/test_data/20220409/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.549024 quantify-core-0.7.2/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/
+-rw-rw-rw-   0 root         (0) root         (0)    13096 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/dataset.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/snapshot.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.479016 quantify-core-0.7.2/tests/test_data/20220509/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.550024 quantify-core-0.7.2/tests/test_data/20220509/20220509-204728-327-69b211-load_settings_test_nested/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20220509/20220509-204728-327-69b211-load_settings_test_nested/snapshot.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.481016 quantify-core-0.7.2/tests/test_data/20220930/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.550024 quantify-core-0.7.2/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.551024 quantify-core-0.7.2/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/analysis_QubitSpectroscopyAnalysis/
+-rw-rw-rw-   0 root         (0) root         (0)    12032 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)    16000 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.551024 quantify-core-0.7.2/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.551024 quantify-core-0.7.2/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/analysis_QubitSpectroscopyAnalysis/
+-rw-rw-rw-   0 root         (0) root         (0)    12032 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)    16000 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/dataset.hdf5
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.552024 quantify-core-0.7.2/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.552024 quantify-core-0.7.2/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/analysis_QubitSpectroscopyAnalysis/
+-rw-rw-rw-   0 root         (0) root         (0)    12032 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)    16000 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/dataset.hdf5
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.553024 quantify-core-0.7.2/tests/test_data/empty/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/empty/nothing
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_data/transmon_test_config.json
+-rw-rw-rw-   0 root         (0) root         (0)     2210 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/test_headers_and_copyright.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.555024 quantify-core-0.7.2/tests/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4296 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/utilities/test_deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9368 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/utilities/test_experiment_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2788 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/utilities/test_general.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/utilities/test_inspect_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:25:03.556025 quantify-core-0.7.2/tests/visualization/
+-rw-rw-rw-   0 root         (0) root         (0)     9131 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/visualization/test_SI_utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     7151 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/visualization/test_instrument_monitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4860 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/visualization/test_mpl_plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)     8018 2023-05-02 14:24:43.000000 quantify-core-0.7.2/tests/visualization/test_pyqt_plotmon.py
```

### Comparing `quantify-core-0.7.1/AUTHORS.md` & `quantify-core-0.7.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/CHANGELOG.md` & `quantify-core-0.7.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## 0.7.2 (2023-05-02)
+
+### Merged branches and closed issues
+
+- Analysis - Allow adding additional arguments to `create_figures()` method of classes that inherit from `BaseAnalysis` (#364, !454)
+- Git - Change back to default merge strategy for CHANGELOG.md (!449)
+- Linting - minor changes to satisfy pyright (!445)
+- QCoDeS - Add qcodes-loop as dependency to ensure `InstrumentMonitor` runs correctly (!452)
+- Utilities - Fix bug and clean up code in `load_settings_onto_instrument` by only trying to get and set parameters in `_try_to_set_par_safe` (!447, #360)
+
 ## 0.7.1 (2023-03-09)
 
 ### Breaking changes
 
 - Requirements - `quantify-core` requires `qcodes>=0.37` (!439)
 
 ### Merged branches and closed issues
```

### Comparing `quantify-core-0.7.1/CONTRIBUTING.md` & `quantify-core-0.7.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/LICENSE` & `quantify-core-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/PKG-INFO` & `quantify-core-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantify-core
-Version: 0.7.1
+Version: 0.7.2
 Summary: Quantify-core is a unified quantum computing, solid-state and pulse sequencing physical experimentation framework.
 Maintainer-email: Edgar Reehuis <ereehuis@qblox.com>, Robert Sokolewicz <rsokolewicz@qblox.com>, Tobias Bonsen <tobias@orangeqs.com>, Viacheslav Ostroukh <viacheslav@orangeqs.com>
 License: BSD-3-Clause
 Project-URL: Documentation, https://quantify-quantify-core.readthedocs-hosted.com
 Project-URL: Source, https://gitlab.com/quantify-os/quantify-core
 Project-URL: Issue tracker, https://gitlab.com/quantify-os/quantify-core/-/issues
 Project-URL: Changelog, https://gitlab.com/quantify-os/quantify-core/-/blob/main/CHANGELOG.md
@@ -46,15 +46,15 @@
 Quantify is a Python-based data acquisition framework focused on Quantum Computing and
 solid-state physics experiments.
 The framework consists of [quantify-core](https://pypi.org/project/quantify-core/) ([git repo](https://gitlab.com/quantify-os/quantify-core/))
 and [quantify-scheduler](https://pypi.org/project/quantify-scheduler/) ([git repo](https://gitlab.com/quantify-os/quantify-scheduler/)).
 It is built on top of [QCoDeS](https://qcodes.github.io/Qcodes/)
 and is a spiritual successor of [PycQED](https://github.com/DiCarloLab-Delft/PycQED_py3).
 
-Quantify-core is the core module that contains all basic functionality to control experiments. This includes:
+`quantify-core` is the core module that contains all basic functionality to control experiments. This includes:
 
 - A framework to control instruments.
 - A data-acquisition loop.
 - Data storage and analysis.
 - Parameter monitoring and live visualization of experiments.
 
 Take a look at the [latest documentation for quantify-core](https://quantify-quantify-core.readthedocs-hosted.com/)
```

### Comparing `quantify-core-0.7.1/README.md` & `quantify-core-0.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Quantify is a Python-based data acquisition framework focused on Quantum Computing and
 solid-state physics experiments.
 The framework consists of [quantify-core](https://pypi.org/project/quantify-core/) ([git repo](https://gitlab.com/quantify-os/quantify-core/))
 and [quantify-scheduler](https://pypi.org/project/quantify-scheduler/) ([git repo](https://gitlab.com/quantify-os/quantify-scheduler/)).
 It is built on top of [QCoDeS](https://qcodes.github.io/Qcodes/)
 and is a spiritual successor of [PycQED](https://github.com/DiCarloLab-Delft/PycQED_py3).
 
-Quantify-core is the core module that contains all basic functionality to control experiments. This includes:
+`quantify-core` is the core module that contains all basic functionality to control experiments. This includes:
 
 - A framework to control instruments.
 - A data-acquisition loop.
 - Data storage and analysis.
 - Parameter monitoring and live visualization of experiments.
 
 Take a look at the [latest documentation for quantify-core](https://quantify-quantify-core.readthedocs-hosted.com/)
```

### Comparing `quantify-core-0.7.1/docs/Makefile` & `quantify-core-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/api_reference.md` & `quantify-core-0.7.2/docs/api_reference.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/conf.py` & `quantify-core-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/images/QUANTIFY-FAVICON_16.png` & `quantify-core-0.7.2/docs/images/QUANTIFY-FAVICON_16.png`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/images/install/conda_activate.gif` & `quantify-core-0.7.2/docs/images/install/conda_activate.gif`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/images/install/conda_install.gif` & `quantify-core-0.7.2/docs/images/install/conda_install.gif`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/images/install/conda_source_installed_all_users.gif` & `quantify-core-0.7.2/docs/images/install/conda_source_installed_all_users.gif`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/images/surface-7-sched.png` & `quantify-core-0.7.2/docs/images/surface-7-sched.png`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/installation.md` & `quantify-core-0.7.2/docs/installation.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,758 +7,781 @@
 00000060: 6e73 7461 6c6c 2051 7561 6e74 6966 792c  nstall Quantify,
 00000070: 2061 7320 6974 2077 696c 6c20 616c 7761   as it will alwa
 00000080: 7973 2069 6e73 7461 6c6c 2074 6865 206d  ys install the m
 00000090: 6f73 7420 7265 6365 6e74 2073 7461 626c  ost recent stabl
 000000a0: 6520 7265 6c65 6173 652e 0a49 6620 796f  e release..If yo
 000000b0: 7520 7761 6e74 2074 6f20 636f 6e74 7269  u want to contri
 000000c0: 6275 7465 2074 6f20 5175 616e 7469 6679  bute to Quantify
-000000d0: 2c20 7365 6520 5b53 6574 7469 6e67 2075  , see [Setting u
-000000e0: 7020 666f 7220 6c6f 6361 6c20 6465 7665  p for local deve
-000000f0: 6c6f 706d 656e 745d 2e0a 0a23 2323 204f  lopment]...### O
-00000100: 6e20 5769 6e64 6f77 7320 616e 6420 6d61  n Windows and ma
-00000110: 634f 5320 2841 6e61 636f 6e64 6129 0a0a  cOS (Anaconda)..
-00000120: 7b6d 6f64 7d60 7175 616e 7469 6679 2d63  {mod}`quantify-c
-00000130: 6f72 6560 2068 6173 2074 6869 7264 2070  ore` has third p
-00000140: 6172 7479 2064 6570 656e 6465 6e63 6965  arty dependencie
-00000150: 7320 7468 6174 2063 616e 2068 6176 6520  s that can have 
-00000160: 656e 7669 726f 6e6d 656e 742d 7370 6563  environment-spec
-00000170: 6966 6963 2070 726f 626c 656d 732e 0a57  ific problems..W
-00000180: 6520 7265 636f 6d6d 656e 6420 7573 696e  e recommend usin
-00000190: 6720 7468 6520 5b41 6e61 636f 6e64 615d  g the [Anaconda]
-000001a0: 2868 7474 7073 3a2f 2f77 7777 2e61 6e61  (https://www.ana
-000001b0: 636f 6e64 612e 636f 6d2f 7072 6f64 7563  conda.com/produc
-000001c0: 7473 2f69 6e64 6976 6964 7561 6c23 446f  ts/individual#Do
-000001d0: 776e 6c6f 6164 7329 2050 7974 686f 6e20  wnloads) Python 
-000001e0: 6469 7374 7269 6275 7469 6f6e 2077 6869  distribution whi
-000001f0: 6368 2077 6f72 6b73 206f 7574 206f 6620  ch works out of 
-00000200: 7468 6520 626f 7820 6f6e 206d 6f73 7420  the box on most 
-00000210: 7379 7374 656d 732e 0a0a 4966 2079 6f75  systems...If you
-00000220: 2061 7265 2066 616d 696c 6961 7220 7769   are familiar wi
-00000230: 7468 2073 6f66 7477 6172 6520 6465 7665  th software deve
-00000240: 6c6f 706d 656e 7420 2870 6163 6b61 6765  lopment (package
-00000250: 206d 616e 6167 6572 2c20 6769 742c 2074   manager, git, t
-00000260: 6572 6d69 6e61 6c2c 2050 7974 686f 6e2c  erminal, Python,
-00000270: 2065 7463 2e29 2074 6865 2066 6f6c 6c6f   etc.) the follo
-00000280: 7769 6e67 2073 686f 756c 6420 6765 7420  wing should get 
-00000290: 796f 7520 7275 6e6e 696e 6720 696e 206e  you running in n
-000002a0: 6f20 7469 6d65 2e20 4f74 6865 7277 6973  o time. Otherwis
-000002b0: 652c 2066 6f6c 6c6f 7720 7468 6520 5b44  e, follow the [D
-000002c0: 6574 6169 6c65 6420 696e 7374 7275 6374  etailed instruct
-000002d0: 696f 6e73 5d20 616e 6420 6c65 6172 6e20  ions] and learn 
-000002e0: 6120 6665 7720 7072 6f64 7563 7469 7669  a few productivi
-000002f0: 7479 2074 6970 7320 6f6e 2079 6f75 7220  ty tips on your 
-00000300: 7761 792e 0a0a 312e 2049 6e73 7461 6c6c  way...1. Install
-00000310: 205b 416e 6163 6f6e 6461 5d28 6874 7470   [Anaconda](http
-00000320: 733a 2f2f 7777 772e 616e 6163 6f6e 6461  s://www.anaconda
-00000330: 2e63 6f6d 2f70 726f 6475 6374 732f 696e  .com/products/in
-00000340: 6469 7669 6475 616c 2344 6f77 6e6c 6f61  dividual#Downloa
-00000350: 6473 292e 0a0a 322e 2049 6e73 7461 6c6c  ds)...2. Install
-00000360: 2051 7561 6e74 6966 7920 2861 6e64 204a   Quantify (and J
-00000370: 7570 7974 6572 4c61 6229 2069 6e20 6120  upyterLab) in a 
-00000380: 6e65 7720 636f 6e64 6120 656e 7669 726f  new conda enviro
-00000390: 6e6d 656e 742c 2073 6565 2061 6c73 6f20  nment, see also 
-000003a0: 7468 6520 5b43 6f6e 6461 2063 6865 6174  the [Conda cheat
-000003b0: 2073 6865 6574 5d28 6874 7470 733a 2f2f   sheet](https://
-000003c0: 646f 6373 2e63 6f6e 6461 2e69 6f2f 7072  docs.conda.io/pr
-000003d0: 6f6a 6563 7473 2f63 6f6e 6461 2f65 6e2f  ojects/conda/en/
-000003e0: 6c61 7465 7374 2f75 7365 722d 6775 6964  latest/user-guid
-000003f0: 652f 6368 6561 7473 6865 6574 2e68 746d  e/cheatsheet.htm
-00000400: 6c29 2e0a 0a20 2020 3e20 4e2e 422e 2049  l)...   > N.B. I
-00000410: 6620 796f 7520 6172 6520 696e 7465 7265  f you are intere
-00000420: 7374 6564 2074 6f20 636f 6e74 7269 6275  sted to contribu
-00000430: 7465 2074 6f20 7b6d 6f64 7d60 7175 616e  te to {mod}`quan
-00000440: 7469 6679 2d63 6f72 6560 2061 6e64 2f6f  tify-core` and/o
-00000450: 7220 7b6d 6f64 7d60 7175 616e 7469 6679  r {mod}`quantify
-00000460: 2d73 6368 6564 756c 6572 6020 796f 7520  -scheduler` you 
-00000470: 7368 6f75 6c64 207b 7265 667d 6073 6574  should {ref}`set
-00000480: 2074 6865 6d20 7570 2066 6f72 206c 6f63   them up for loc
-00000490: 616c 2064 6576 656c 6f70 6d65 6e74 2069  al development i
-000004a0: 6e73 7465 6164 203c 5365 7474 696e 6720  nstead <Setting 
-000004b0: 7570 2066 6f72 206c 6f63 616c 2064 6576  up for local dev
-000004c0: 656c 6f70 6d65 6e74 3e60 2e0a 2020 203e  elopment>`..   >
-000004d0: 0a20 2020 3e20 6060 600a 2020 203e 2024  .   > ```.   > $
-000004e0: 2023 2072 756e 2074 6865 2066 6f6c 6c6f   # run the follo
-000004f0: 7769 6e67 2063 6f6d 6d61 6e64 7320 7374  wing commands st
-00000500: 6570 2062 7920 7374 6570 210a 2020 203e  ep by step!.   >
-00000510: 0a20 2020 3e20 2420 636f 6e64 6120 6372  .   > $ conda cr
-00000520: 6561 7465 202d 2d6e 616d 6520 7175 616e  eate --name quan
-00000530: 7469 6679 2d65 6e76 2070 7974 686f 6e3d  tify-env python=
-00000540: 332e 380a 2020 203e 2024 2063 6f6e 6461  3.8.   > $ conda
-00000550: 2061 6374 6976 6174 6520 7175 616e 7469   activate quanti
-00000560: 6679 2d65 6e76 0a20 2020 3e20 2420 636f  fy-env.   > $ co
-00000570: 6e64 6120 696e 7374 616c 6c20 2d63 2063  nda install -c c
-00000580: 6f6e 6461 2d66 6f72 6765 206a 7570 7974  onda-forge jupyt
-00000590: 6572 6c61 620a 2020 203e 2024 2070 7974  erlab.   > $ pyt
-000005a0: 686f 6e20 2d6d 2069 7079 6b65 726e 656c  hon -m ipykernel
-000005b0: 2069 6e73 7461 6c6c 202d 2d75 7365 7220   install --user 
-000005c0: 2d2d 6e61 6d65 3d71 7561 6e74 6966 792d  --name=quantify-
-000005d0: 656e 7620 202d 2d64 6973 706c 6179 2d6e  env  --display-n
-000005e0: 616d 653d 2250 7974 686f 6e20 3320 5175  ame="Python 3 Qu
-000005f0: 616e 7469 6679 2045 6e76 220a 2020 203e  antify Env".   >
-00000600: 2024 2070 6970 2069 6e73 7461 6c6c 2071   $ pip install q
-00000610: 7561 6e74 6966 792d 636f 7265 0a20 2020  uantify-core.   
-00000620: 3e0a 2020 203e 2024 2023 2028 4f70 7469  >.   > $ # (Opti
-00000630: 6f6e 616c 6c79 2920 696e 7374 616c 6c20  onally) install 
-00000640: 7175 616e 7469 6679 2d73 6368 6564 756c  quantify-schedul
-00000650: 6572 3a0a 2020 203e 0a20 2020 3e20 2420  er:.   >.   > $ 
-00000660: 7069 7020 696e 7374 616c 6c20 7175 616e  pip install quan
-00000670: 7469 6679 2d73 6368 6564 756c 6572 0a20  tify-scheduler. 
-00000680: 2020 3e20 2420 6a75 7079 7465 7220 6c61    > $ jupyter la
-00000690: 6265 7874 656e 7369 6f6e 2069 6e73 7461  bextension insta
-000006a0: 6c6c 206a 7570 7974 6572 6c61 622d 706c  ll jupyterlab-pl
-000006b0: 6f74 6c79 202d 2d6e 6f2d 6275 696c 640a  otly --no-build.
-000006c0: 2020 203e 2024 2023 2074 6869 7320 6d69     > $ # this mi
-000006d0: 6768 7420 7461 6b65 2061 2066 6577 206d  ght take a few m
-000006e0: 696e 7574 6573 0a20 2020 3e20 2420 6a75  inutes.   > $ ju
-000006f0: 7079 7465 7220 6c61 6265 7874 656e 7369  pyter labextensi
-00000700: 6f6e 2069 6e73 7461 6c6c 2040 6a75 7079  on install @jupy
-00000710: 7465 722d 7769 6467 6574 732f 6a75 7079  ter-widgets/jupy
-00000720: 7465 726c 6162 2d6d 616e 6167 6572 2070  terlab-manager p
-00000730: 6c6f 746c 7977 6964 6765 740a 2020 203e  lotlywidget.   >
-00000740: 2060 6060 0a0a 332e 2059 6f75 2061 7265   ```..3. You are
-00000750: 2067 6f6f 6420 746f 2067 6f21 2048 6561   good to go! Hea
-00000760: 6420 6f76 6572 2074 6f20 7468 6520 7b72  d over to the {r
-00000770: 6566 7d60 5573 6572 2067 7569 6465 203c  ef}`User guide <
-00000780: 7573 6572 2d67 7569 6465 3e60 2074 6f20  user-guide>` to 
-00000790: 6765 7420 7374 6172 7465 642e 0a0a 2323  get started...##
-000007a0: 2323 2044 6574 6169 6c65 6420 696e 7374  ## Detailed inst
-000007b0: 7275 6374 696f 6e73 0a0a 312e 2049 6e73  ructions..1. Ins
-000007c0: 7461 6c6c 205b 416e 6163 6f6e 6461 5d28  tall [Anaconda](
-000007d0: 6874 7470 733a 2f2f 7777 772e 616e 6163  https://www.anac
-000007e0: 6f6e 6461 2e63 6f6d 2f70 726f 6475 6374  onda.com/product
-000007f0: 732f 696e 6469 7669 6475 616c 2344 6f77  s/individual#Dow
-00000800: 6e6c 6f61 6473 292e 0a0a 2020 203e 204f  nloads)...   > O
-00000810: 6e20 5769 6e64 6f77 732c 2064 7572 696e  n Windows, durin
-00000820: 6720 7468 6520 696e 7374 616c 6c61 7469  g the installati
-00000830: 6f6e 2c20 7765 2072 6563 6f6d 6d65 6e64  on, we recommend
-00000840: 2074 6f20 7365 6c65 6374 2074 6865 206f   to select the o
-00000850: 7074 696f 6e73 3a0a 2020 203e 0a20 2020  ptions:.   >.   
-00000860: 3e20 2d20 496e 7374 616c 6c20 666f 7220  > - Install for 
-00000870: 6041 6c6c 2055 7365 7273 2028 7265 7175  `All Users (requ
-00000880: 6972 6573 2061 646d 696e 2070 7269 7669  ires admin privi
-00000890: 6c65 6765 7329 603b 2061 6e64 0a20 2020  leges)`; and.   
-000008a0: 3e20 2d20 6041 6464 2041 6e61 636f 6e64  > - `Add Anacond
-000008b0: 6133 2074 6865 2073 7973 7465 6d20 5041  a3 the system PA
-000008c0: 5448 2065 6e76 6972 6f6e 6d65 6e74 2076  TH environment v
-000008d0: 6172 6961 626c 6560 2e0a 2020 203e 0a20  ariable`..   >. 
-000008e0: 2020 3e20 6060 6060 6060 7b61 646d 6f6e    > ``````{admon
-000008f0: 6974 696f 6e7d 2049 6e73 7472 7563 7469  ition} Instructi
-00000900: 6f6e 733a 2041 6e61 636f 6e64 6120 696e  ons: Anaconda in
-00000910: 7374 616c 6c20 2857 696e 646f 7773 290a  stall (Windows).
-00000920: 2020 203e 203a 636c 6173 733a 2064 726f     > :class: dro
-00000930: 7064 6f77 6e2c 2069 6e66 6f0a 2020 203e  pdown, info.   >
-00000940: 0a20 2020 3e20 6060 607b 6669 6775 7265  .   > ```{figure
-00000950: 7d20 2f69 6d61 6765 732f 696e 7374 616c  } /images/instal
-00000960: 6c2f 636f 6e64 615f 696e 7374 616c 6c2e  l/conda_install.
-00000970: 6769 660a 2020 203e 203a 6e61 6d65 3a20  gif.   > :name: 
-00000980: 636f 6e64 615f 696e 7374 616c 6c0a 2020  conda_install.  
-00000990: 203e 203a 7769 6474 683a 2038 3030 0a20   > :width: 800. 
-000009a0: 2020 3e20 6060 600a 2020 203e 2060 6060    > ```.   > ```
-000009b0: 6060 600a 0a32 2e20 2857 696e 646f 7773  ```..2. (Windows
-000009c0: 206f 6e6c 7929 2049 6e73 7461 6c6c 205b   only) Install [
-000009d0: 4769 7420 4241 5348 5d28 6874 7470 733a  Git BASH](https:
-000009e0: 2f2f 6769 7466 6f72 7769 6e64 6f77 732e  //gitforwindows.
-000009f0: 6f72 672f 2920 746f 2068 6176 6520 6120  org/) to have a 
-00000a00: 756e 6978 2d6c 696b 6520 6261 7368 2074  unix-like bash t
-00000a10: 6572 6d69 6e61 6c20 2864 6566 6175 6c74  erminal (default
-00000a20: 206f 7074 696f 6e73 2064 7572 696e 6720   options during 
-00000a30: 696e 7374 616c 6c61 7469 6f6e 2073 686f  installation sho
-00000a40: 756c 6420 776f 726b 2077 656c 6c20 6f6e  uld work well on
-00000a50: 206d 6f73 7420 7365 7475 7073 292e 0a0a   most setups)...
-00000a60: 2020 203e 2060 6060 7b74 6970 7d0a 2020     > ```{tip}.  
-00000a70: 203e 2055 7365 7273 2063 616e 2072 6967   > Users can rig
-00000a80: 6874 2063 6c69 636b 2061 6e79 2066 6f6c  ht click any fol
-00000a90: 6465 7220 696e 2077 696e 646f 7773 2061  der in windows a
-00000aa0: 6e64 206f 7065 6e20 4769 7420 4241 5348  nd open Git BASH
-00000ab0: 2069 6e20 7468 6174 206c 6f63 6174 696f   in that locatio
-00000ac0: 6e2e 0a20 2020 3e20 6060 600a 2020 203e  n..   > ```.   >
-00000ad0: 0a20 2020 3e20 6060 607b 6e6f 7465 7d0a  .   > ```{note}.
-00000ae0: 2020 203e 2042 6520 6177 6172 6520 7468     > Be aware th
-00000af0: 6174 2061 2075 6e69 782d 6c69 6b65 2074  at a unix-like t
-00000b00: 6572 6d69 6e61 6c20 6f6e 2077 696e 646f  erminal on windo
-00000b10: 7773 2068 6173 2073 6f6d 6520 6361 7665  ws has some cave
-00000b20: 6174 732e 2054 6f20 6176 6f69 6420 7468  ats. To avoid th
-00000b30: 656d 2c20 7765 2072 6563 6f6d 6d65 6e64  em, we recommend
-00000b40: 2074 6f20 7275 6e20 616e 7920 7079 7468   to run any pyth
-00000b50: 6f6e 2063 6f64 6520 7573 696e 6720 5b4a  on code using [J
-00000b60: 7570 7974 6572 4c61 625d 2868 7474 7073  upyterLab](https
-00000b70: 3a2f 2f6a 7570 7974 6572 6c61 622e 7265  ://jupyterlab.re
-00000b80: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00000b90: 7374 6162 6c65 2f29 2028 696e 7374 616c  stable/) (instal
-00000ba0: 6c61 7469 6f6e 2073 7465 7073 2062 656c  lation steps bel
-00000bb0: 6f77 292e 0a20 2020 3e20 6060 600a 0a33  ow)..   > ```..3
-00000bc0: 2e20 2857 696e 646f 7773 206f 6e6c 7929  . (Windows only)
-00000bd0: 2041 6464 207b 636f 6465 7d60 736f 7572   Add {code}`sour
-00000be0: 6365 202f 7061 7468 2f74 6f2f 416e 6163  ce /path/to/Anac
-00000bf0: 6f6e 6461 332f 6574 632f 7072 6f66 696c  onda3/etc/profil
-00000c00: 652e 642f 636f 6e64 612e 7368 6020 696e  e.d/conda.sh` in
-00000c10: 2074 6865 2060 2e62 6173 6872 6360 2028   the `.bashrc` (
-00000c20: 6f72 2069 6e20 7468 6520 602e 6261 7368  or in the `.bash
-00000c30: 5f70 726f 6669 6c65 6029 2074 6f20 6578  _profile`) to ex
-00000c40: 706f 7365 2074 6865 2061 6e61 636f 6e64  pose the anacond
-00000c50: 6120 696e 2062 6173 6820 7465 726d 696e  a in bash termin
-00000c60: 616c 2028 7365 6520 696e 7374 7275 6374  al (see instruct
-00000c70: 696f 6e20 6265 6c6f 7720 6966 2079 6f75  ion below if you
-00000c80: 206e 6565 6420 6865 6c70 292e 0a0a 2020   need help)...  
-00000c90: 203e 2060 6060 7b74 6970 7d0a 2020 203e   > ```{tip}.   >
-00000ca0: 2049 6620 796f 7520 666f 6c6c 6f77 6564   If you followed
-00000cb0: 2074 6865 2064 6566 6175 6c74 2061 6e61   the default ana
-00000cc0: 636f 6e64 6120 696e 7374 616c 6c61 7469  conda installati
-00000cd0: 6f6e 2074 6865 2070 6174 6820 746f 2069  on the path to i
-00000ce0: 7420 7769 6c6c 2062 6520 7369 6d69 6c61  t will be simila
-00000cf0: 7220 746f 0a20 2020 3e20 7b63 6f64 657d  r to.   > {code}
-00000d00: 602f 632f 5573 6572 732f 3c59 4f55 525f  `/c/Users/<YOUR_
-00000d10: 5553 4552 4e41 4d45 3e2f 616e 6163 6f6e  USERNAME>/anacon
-00000d20: 6461 332f 6574 632f 7072 6f66 696c 652e  da3/etc/profile.
-00000d30: 642f 636f 6e64 612e 7368 6020 6f72 207b  d/conda.sh` or {
-00000d40: 636f 6465 7d60 2f63 2f50 726f 6772 616d  code}`/c/Program
-00000d50: 4461 7461 2f41 6e61 636f 6e64 6133 2f65  Data/Anaconda3/e
-00000d60: 7463 2f70 726f 6669 6c65 2e64 2f63 6f6e  tc/profile.d/con
-00000d70: 6461 2e73 6860 2e0a 2020 203e 0a20 2020  da.sh`..   >.   
-00000d80: 3e20 5072 6f20 7469 703a 2079 6f75 2063  > Pro tip: you c
-00000d90: 616e 2064 7261 6720 616e 6420 6472 6f70  an drag and drop
-00000da0: 2061 2066 696c 6520 6672 6f6d 2074 6865   a file from the
-00000db0: 2066 696c 6520 6578 706c 6f72 6572 2069   file explorer i
-00000dc0: 6e74 6f20 7468 6520 7465 726d 696e 616c  nto the terminal
-00000dd0: 2061 6e64 2067 6574 2074 6865 2070 6174   and get the pat
-00000de0: 6820 6f66 2074 6865 2066 696c 6520 2869  h of the file (i
-00000df0: 6e73 7465 6164 206f 6620 7479 7069 6e67  nstead of typing
-00000e00: 2069 7420 6d61 6e75 616c 6c79 292e 0a20   it manually).. 
-00000e10: 2020 3e20 6060 600a 2020 203e 0a20 2020    > ```.   >.   
-00000e20: 3e20 6060 6060 6060 7b61 646d 6f6e 6974  > ``````{admonit
-00000e30: 696f 6e7d 2049 6e73 7472 7563 7469 6f6e  ion} Instruction
-00000e40: 733a 2065 7870 6f73 6520 616e 6163 6f6e  s: expose anacon
-00000e50: 6461 2069 6e20 7468 6520 6261 7368 2074  da in the bash t
-00000e60: 6572 6d69 6e61 6c0a 2020 203e 203a 636c  erminal.   > :cl
-00000e70: 6173 733a 2064 726f 7064 6f77 6e2c 2069  ass: dropdown, i
-00000e80: 6e66 6f0a 2020 203e 0a20 2020 3e20 4265  nfo.   >.   > Be
-00000e90: 6c6f 7720 7765 2069 6c6c 7573 7472 6174  low we illustrat
-00000ea0: 6520 7468 6973 2070 726f 6365 7373 2069  e this process i
-00000eb0: 6e20 4769 7420 4261 7368 2e20 596f 7520  n Git Bash. You 
-00000ec0: 6361 6e20 6669 6e64 2064 6574 6169 6c65  can find detaile
-00000ed0: 6420 7374 6570 2d62 792d 7374 6570 2069  d step-by-step i
-00000ee0: 6e73 7472 7563 7469 6f6e 7320 5b68 6572  nstructions [her
-00000ef0: 655d 2868 7474 7073 3a2f 2f73 7570 6572  e](https://super
-00000f00: 7573 6572 2e63 6f6d 2f61 2f36 3032 3839  user.com/a/60289
-00000f10: 3629 2e0a 2020 203e 0a20 2020 3e20 6060  6)..   >.   > ``
-00000f20: 607b 6669 6775 7265 7d20 2f69 6d61 6765  `{figure} /image
-00000f30: 732f 696e 7374 616c 6c2f 636f 6e64 615f  s/install/conda_
-00000f40: 736f 7572 6365 5f69 6e73 7461 6c6c 6564  source_installed
-00000f50: 5f61 6c6c 5f75 7365 7273 2e67 6966 0a20  _all_users.gif. 
-00000f60: 2020 3e20 3a6e 616d 653a 2063 6f6e 6461    > :name: conda
-00000f70: 5f73 6f75 7263 650a 2020 203e 203a 7769  _source.   > :wi
-00000f80: 6474 683a 2038 3030 0a20 2020 3e20 6060  dth: 800.   > ``
-00000f90: 600a 2020 203e 2060 6060 6060 600a 2020  `.   > ``````.  
-00000fa0: 203e 0a20 2020 3e20 6060 607b 6e6f 7465   >.   > ```{note
-00000fb0: 7d0a 2020 203e 2054 6f20 636f 6e66 6972  }.   > To confir
-00000fc0: 6d20 796f 7520 6861 7665 2061 2066 756e  m you have a fun
-00000fd0: 6374 696f 6e61 6c20 696e 7374 616c 6c61  ctional installa
-00000fe0: 7469 6f6e 206f 6620 616e 6163 6f6e 6461  tion of anaconda
-00000ff0: 2c20 7275 6e20 7b63 6f64 657d 6063 6f6e  , run {code}`con
-00001000: 6461 6020 696e 2074 6865 2074 6572 6d69  da` in the termi
-00001010: 6e61 6c2e 2054 6869 7320 7769 6c6c 2070  nal. This will p
-00001020: 7269 6e74 2074 6865 2063 6f6e 6461 2068  rint the conda h
-00001030: 656c 7020 6d65 7373 6167 6520 7768 6963  elp message whic
-00001040: 6820 6973 2061 6e20 696e 6469 6361 7469  h is an indicati
-00001050: 6f6e 206f 6620 6120 776f 726b 696e 6720  on of a working 
-00001060: 696e 7374 616c 6c61 7469 6f6e 2e0a 2020  installation..  
-00001070: 203e 2060 6060 0a0a 342e 2043 7265 6174   > ```..4. Creat
-00001080: 6520 6120 636f 6e64 6120 656e 7669 726f  e a conda enviro
-00001090: 6e6d 656e 742c 2073 6565 2061 6c73 6f20  nment, see also 
-000010a0: 7468 6520 5b43 6f6e 6461 2063 6865 6174  the [Conda cheat
-000010b0: 2073 6865 6574 5d28 6874 7470 733a 2f2f   sheet](https://
-000010c0: 646f 6373 2e63 6f6e 6461 2e69 6f2f 7072  docs.conda.io/pr
-000010d0: 6f6a 6563 7473 2f63 6f6e 6461 2f65 6e2f  ojects/conda/en/
-000010e0: 6c61 7465 7374 2f75 7365 722d 6775 6964  latest/user-guid
-000010f0: 652f 6368 6561 7473 6865 6574 2e68 746d  e/cheatsheet.htm
-00001100: 6c29 2e0a 0a20 2020 3e20 6060 600a 2020  l)...   > ```.  
-00001110: 203e 2024 2063 6f6e 6461 2063 7265 6174   > $ conda creat
-00001120: 6520 2d2d 6e61 6d65 2071 7561 6e74 6966  e --name quantif
-00001130: 792d 656e 7620 7079 7468 6f6e 3d33 2e38  y-env python=3.8
-00001140: 2020 2023 2063 7265 6174 6520 7468 6520     # create the 
-00001150: 636f 6e64 6120 656e 7669 726f 6e6d 656e  conda environmen
-00001160: 742c 2079 6f75 2063 616e 2072 6570 6c61  t, you can repla
-00001170: 6365 2060 7175 616e 7469 6679 2d65 6e76  ce `quantify-env
-00001180: 6020 6966 2079 6f75 2077 6973 680a 2020  ` if you wish.  
-00001190: 203e 2024 2063 6f6e 6461 2061 6374 6976   > $ conda activ
-000011a0: 6174 6520 7175 616e 7469 6679 2d65 6e76  ate quantify-env
-000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011c0: 2020 2023 2061 6374 6976 6174 6573 2074     # activates t
-000011d0: 6865 2063 6f6e 6461 2065 6e76 6972 6f6e  he conda environ
-000011e0: 6d65 6e74 0a20 2020 3e20 6060 600a 2020  ment.   > ```.  
-000011f0: 203e 0a20 2020 3e20 6060 607b 7469 707d   >.   > ```{tip}
-00001200: 0a20 2020 3e20 596f 7520 6361 6e20 6164  .   > You can ad
-00001210: 6420 7b63 6f64 657d 6063 6f6e 6461 2061  d {code}`conda a
-00001220: 6374 6976 6174 6520 7175 616e 7469 6679  ctivate quantify
-00001230: 2d65 6e76 6020 6174 2074 6865 2065 6e64  -env` at the end
-00001240: 206f 6620 7468 6520 602e 6261 7368 7263   of the `.bashrc
-00001250: 6020 286f 7220 602e 6261 7368 5f70 726f  ` (or `.bash_pro
-00001260: 6669 6c65 6029 2069 6620 796f 7520 7769  file`) if you wi
-00001270: 7368 2066 6f72 2074 6869 7320 656e 7669  sh for this envi
-00001280: 726f 6e6d 656e 7420 746f 2062 6520 6163  ronment to be ac
-00001290: 7469 7661 7465 6420 6175 746f 6d61 7469  tivated automati
-000012a0: 6361 6c6c 7920 696e 2074 6865 2074 6572  cally in the ter
-000012b0: 6d69 6e61 6c20 7768 656e 2069 7420 6973  minal when it is
-000012c0: 206f 7065 6e65 6420 2873 6565 2069 6e73   opened (see ins
-000012d0: 7472 7563 7469 6f6e 7320 6265 6c6f 7729  tructions below)
-000012e0: 2e0a 2020 203e 2060 6060 0a20 2020 3e0a  ..   > ```.   >.
-000012f0: 2020 203e 2060 6060 6060 607b 6164 6d6f     > ``````{admo
-00001300: 6e69 7469 6f6e 7d20 496e 7374 7275 6374  nition} Instruct
-00001310: 696f 6e73 3a20 6372 6561 7465 2063 6f6e  ions: create con
-00001320: 6461 2065 6e76 2061 6e64 2061 7574 6f2d  da env and auto-
-00001330: 6163 7469 7661 7465 2028 5769 6e64 6f77  activate (Window
-00001340: 7329 0a20 2020 3e20 3a63 6c61 7373 3a20  s).   > :class: 
-00001350: 6472 6f70 646f 776e 2c20 696e 666f 0a20  dropdown, info. 
-00001360: 2020 3e0a 2020 203e 2060 6060 7b66 6967    >.   > ```{fig
-00001370: 7572 657d 202f 696d 6167 6573 2f69 6e73  ure} /images/ins
-00001380: 7461 6c6c 2f63 6f6e 6461 5f61 6374 6976  tall/conda_activ
-00001390: 6174 652e 6769 660a 2020 203e 203a 6e61  ate.gif.   > :na
-000013a0: 6d65 3a20 636f 6e64 615f 6163 7469 7661  me: conda_activa
-000013b0: 7465 0a20 2020 3e20 3a77 6964 7468 3a20  te.   > :width: 
-000013c0: 3830 300a 2020 203e 2060 6060 0a20 2020  800.   > ```.   
-000013d0: 3e20 6060 6060 6060 0a0a 352e 2049 6e73  > ``````..5. Ins
-000013e0: 7461 6c6c 2060 6a75 7079 7465 722d 6c61  tall `jupyter-la
-000013f0: 6260 2069 6e20 7468 6520 6e65 7720 656e  b` in the new en
-00001400: 7669 726f 6e6d 656e 7420 7573 696e 673a  vironment using:
-00001410: 0a0a 2020 2060 6060 0a20 2020 2420 636f  ..   ```.   $ co
-00001420: 6e64 6120 696e 7374 616c 6c20 2d63 2063  nda install -c c
-00001430: 6f6e 6461 2d66 6f72 6765 206a 7570 7974  onda-forge jupyt
-00001440: 6572 6c61 6220 2023 2069 6e73 7461 6c6c  erlab  # install
-00001450: 206a 7570 7974 6572 206c 6162 0a20 2020   jupyter lab.   
-00001460: 2420 2320 6164 6420 7468 6520 656e 7669  $ # add the envi
-00001470: 726f 6e6d 656e 7420 6173 2061 6e20 6176  ronment as an av
-00001480: 6169 6c61 626c 6520 6b65 726e 656c 2066  ailable kernel f
-00001490: 6f72 206a 7570 7974 6572 206e 6f74 6562  or jupyter noteb
-000014a0: 6f6f 6b20 7769 7468 696e 206a 7570 7974  ook within jupyt
-000014b0: 6572 2d6c 6162 2e0a 2020 2024 2070 7974  er-lab..   $ pyt
-000014c0: 686f 6e20 2d6d 2069 7079 6b65 726e 656c  hon -m ipykernel
-000014d0: 2069 6e73 7461 6c6c 202d 2d75 7365 7220   install --user 
-000014e0: 2d2d 6e61 6d65 3d71 7561 6e74 6966 792d  --name=quantify-
-000014f0: 656e 7620 202d 2d64 6973 706c 6179 2d6e  env  --display-n
-00001500: 616d 653d 2250 7974 686f 6e20 3320 5175  ame="Python 3 Qu
-00001510: 616e 7469 6679 2045 6e76 220a 2020 2060  antify Env".   `
-00001520: 6060 0a0a 362e 2049 6e73 7461 6c6c 207b  ``..6. Install {
-00001530: 6d6f 647d 6071 7561 6e74 6966 792d 636f  mod}`quantify-co
-00001540: 7265 6020 6672 6f6d 2070 7970 690a 0a20  re` from pypi.. 
-00001550: 2020 3e20 4966 2079 6f75 2061 7265 2069    > If you are i
-00001560: 6e74 6572 6573 7465 6420 746f 2063 6f6e  nterested to con
-00001570: 7472 6962 7574 6520 746f 2051 7561 6e74  tribute to Quant
-00001580: 6966 792d 636f 7265 2079 6f75 2073 686f  ify-core you sho
-00001590: 756c 6420 7b72 6566 7d60 7365 7420 6974  uld {ref}`set it
-000015a0: 2075 7020 666f 7220 6c6f 6361 6c20 6465   up for local de
-000015b0: 7665 6c6f 706d 656e 7420 696e 7374 6561  velopment instea
-000015c0: 6420 3c53 6574 7469 6e67 2075 7020 666f  d <Setting up fo
-000015d0: 7220 6c6f 6361 6c20 6465 7665 6c6f 706d  r local developm
-000015e0: 656e 743e 602e 0a20 2020 3e0a 2020 203e  ent>`..   >.   >
-000015f0: 2060 6060 0a20 2020 3e20 2420 7069 7020   ```.   > $ pip 
-00001600: 696e 7374 616c 6c20 7175 616e 7469 6679  install quantify
-00001610: 2d63 6f72 650a 2020 203e 2060 6060 0a20  -core.   > ```. 
-00001620: 2020 3e0a 2020 203e 2060 6060 7b6e 6f74    >.   > ```{not
-00001630: 657d 0a20 2020 3e20 5765 2063 7572 7265  e}.   > We curre
-00001640: 6e74 6c79 2064 6f20 6e6f 7420 6861 7665  ntly do not have
-00001650: 2061 2063 6f6e 6461 2072 6563 6970 6520   a conda recipe 
-00001660: 666f 7220 696e 7374 616c 6c61 7469 6f6e  for installation
-00001670: 2c20 696e 7374 6561 6420 7765 2072 6566  , instead we ref
-00001680: 6572 2074 6f20 7468 6520 6465 6661 756c  er to the defaul
-00001690: 7420 7069 7020 696e 7374 616c 6c61 7469  t pip installati
-000016a0: 6f6e 2077 6974 6869 6e20 6120 636f 6e64  on within a cond
-000016b0: 6120 656e 7669 726f 6e6d 656e 742e 0a20  a environment.. 
-000016c0: 2020 3e20 6060 600a 0a37 2e20 284f 7074    > ```..7. (Opt
-000016d0: 696f 6e61 6c6c 7929 2069 6e73 7461 6c6c  ionally) install
-000016e0: 207b 6d6f 647d 6071 7561 6e74 6966 792d   {mod}`quantify-
-000016f0: 7363 6865 6475 6c65 7260 0a0a 2020 203e  scheduler`..   >
-00001700: 2049 6620 796f 7520 6172 6520 696e 7465   If you are inte
-00001710: 7265 7374 6564 2074 6f20 636f 6e74 7269  rested to contri
-00001720: 6275 7465 2074 6f20 7b6d 6f64 7d60 7175  bute to {mod}`qu
-00001730: 616e 7469 6679 2d73 6368 6564 756c 6572  antify-scheduler
-00001740: 6020 796f 7520 7368 6f75 6c64 207b 7265  ` you should {re
-00001750: 667d 6073 6574 2069 7420 7570 2066 6f72  f}`set it up for
-00001760: 206c 6f63 616c 2064 6576 656c 6f70 6d65   local developme
-00001770: 6e74 2069 6e73 7465 6164 203c 5365 7474  nt instead <Sett
-00001780: 696e 6720 7570 2066 6f72 206c 6f63 616c  ing up for local
-00001790: 2064 6576 656c 6f70 6d65 6e74 3e60 2e20   development>`. 
-000017a0: 596f 7520 6f6e 6c79 206e 6565 6420 746f  You only need to
-000017b0: 2072 6570 6c61 6365 207b 6d6f 647d 6071   replace {mod}`q
-000017c0: 7561 6e74 6966 792d 636f 7265 6020 7769  uantify-core` wi
-000017d0: 7468 207b 6d6f 647d 6071 7561 6e74 6966  th {mod}`quantif
-000017e0: 792d 7363 6865 6475 6c65 7260 2069 6e20  y-scheduler` in 
-000017f0: 7468 6520 7072 6f76 6964 6564 2063 6f6d  the provided com
-00001800: 6d61 6e64 732e 0a20 2020 3e0a 2020 203e  mands..   >.   >
-00001810: 2060 6060 0a20 2020 3e20 2420 7069 7020   ```.   > $ pip 
-00001820: 696e 7374 616c 6c20 7175 616e 7469 6679  install quantify
-00001830: 2d73 6368 6564 756c 6572 0a20 2020 3e20  -scheduler.   > 
-00001840: 2420 6a75 7079 7465 7220 6c61 6265 7874  $ jupyter labext
-00001850: 656e 7369 6f6e 2069 6e73 7461 6c6c 206a  ension install j
-00001860: 7570 7974 6572 6c61 622d 706c 6f74 6c79  upyterlab-plotly
-00001870: 202d 2d6e 6f2d 6275 696c 640a 2020 203e   --no-build.   >
-00001880: 2024 2023 2074 6869 7320 6d69 6768 7420   $ # this might 
-00001890: 7461 6b65 2061 2066 6577 206d 696e 7574  take a few minut
-000018a0: 6573 0a20 2020 3e20 2420 6a75 7079 7465  es.   > $ jupyte
-000018b0: 7220 6c61 6265 7874 656e 7369 6f6e 2069  r labextension i
-000018c0: 6e73 7461 6c6c 2040 6a75 7079 7465 722d  nstall @jupyter-
-000018d0: 7769 6467 6574 732f 6a75 7079 7465 726c  widgets/jupyterl
-000018e0: 6162 2d6d 616e 6167 6572 2070 6c6f 746c  ab-manager plotl
-000018f0: 7977 6964 6765 740a 2020 203e 2060 6060  ywidget.   > ```
-00001900: 0a0a 2323 2320 4f74 6865 7220 7379 7374  ..### Other syst
-00001910: 656d 730a 0a0a 436f 6e66 6972 6d20 7468  ems...Confirm th
-00001920: 6174 2079 6f75 2068 6176 6520 6120 636f  at you have a co
-00001930: 6d70 6174 6962 6c65 2077 6f72 6b69 6e67  mpatible working
-00001940: 2070 7974 686f 6e20 696e 7465 7270 7265   python interpre
-00001950: 7465 7220 6279 2072 756e 6e69 6e67 2074  ter by running t
-00001960: 6865 2066 6f6c 6c6f 7769 6e67 2069 6e20  he following in 
-00001970: 796f 7572 2074 6572 6d69 6e61 6c20 6f66  your terminal of
-00001980: 2063 686f 6963 653a 0a0a 6060 600a 2420   choice:..```.$ 
-00001990: 7079 7468 6f6e 202d 2d76 6572 7369 6f6e  python --version
-000019a0: 0a50 7974 686f 6e20 332e 382e 3130 0a60  .Python 3.8.10.`
-000019b0: 6060 0a45 7861 6374 2076 6572 7369 6f6e  ``.Exact version
-000019c0: 206d 6179 2062 6520 6469 6666 6572 656e   may be differen
-000019d0: 742c 2063 6865 636b 2074 6865 206c 6973  t, check the lis
-000019e0: 7420 6f66 2073 7570 706f 7274 6564 2076  t of supported v
-000019f0: 6572 7369 6f6e 7320 696e 2074 6865 2060  ersions in the `
-00001a00: 7365 7475 702e 7079 6020 6669 6c65 2e0a  setup.py` file..
-00001a10: 0a49 6e73 7461 6c6c 2051 7561 6e74 6966  .Install Quantif
-00001a20: 793a 0a0a 6060 600a 2420 7069 7020 696e  y:..```.$ pip in
-00001a30: 7374 616c 6c20 7175 616e 7469 6679 2d63  stall quantify-c
-00001a40: 6f72 650a 6060 600a 0a49 6620 796f 7520  ore.```..If you 
-00001a50: 646f 6e27 7420 6861 7665 205b 7069 705d  don't have [pip]
-00001a60: 2069 6e73 7461 6c6c 6564 2c20 7468 6973   installed, this
-00001a70: 205b 5079 7468 6f6e 2069 6e73 7461 6c6c   [Python install
-00001a80: 6174 696f 6e20 6775 6964 655d 2063 616e  ation guide] can
-00001a90: 2067 7569 6465 0a79 6f75 2074 6872 6f75   guide.you throu
-00001aa0: 6768 2074 6865 2070 726f 6365 7373 2e0a  gh the process..
-00001ab0: 0a23 2320 5570 6461 7465 2074 6f20 7468  .## Update to th
-00001ac0: 6520 6c61 7465 7374 2076 6572 7369 6f6e  e latest version
-00001ad0: 0a0a 546f 2075 7064 6174 6520 5175 616e  ..To update Quan
-00001ae0: 7469 6679 2074 6f20 7468 6520 6c61 7465  tify to the late
-00001af0: 7374 2076 6572 7369 6f6e 3a0a 0a60 6060  st version:..```
-00001b00: 0a24 2070 6970 2069 6e73 7461 6c6c 202d  .$ pip install -
-00001b10: 2d75 7067 7261 6465 2071 7561 6e74 6966  -upgrade quantif
-00001b20: 792d 636f 7265 0a60 6060 0a0a 2323 2053  y-core.```..## S
-00001b30: 6574 7469 6e67 2075 7020 666f 7220 6c6f  etting up for lo
-00001b40: 6361 6c20 6465 7665 6c6f 706d 656e 740a  cal development.
-00001b50: 0a52 6561 6479 2074 6f20 636f 6e74 7269  .Ready to contri
-00001b60: 6275 7465 3f20 4865 7265 2773 2068 6f77  bute? Here's how
-00001b70: 2074 6f20 7365 7420 7570 2051 7561 6e74   to set up Quant
-00001b80: 6966 7920 666f 7220 6c6f 6361 6c20 6465  ify for local de
-00001b90: 7665 6c6f 706d 656e 742e 0a0a 3030 2e20  velopment...00. 
-00001ba0: 466f 6c6c 6f77 2074 6865 205b 496e 7374  Follow the [Inst
-00001bb0: 616c 6c61 7469 6f6e 5d20 7374 6570 7320  allation] steps 
-00001bc0: 666f 7220 796f 7572 2073 7973 7465 6d20  for your system 
-00001bd0: 736b 6970 7069 6e67 2074 6865 206c 6173  skipping the las
-00001be0: 7420 7374 6570 2028 7b63 6f64 657d 6070  t step ({code}`p
-00001bf0: 6970 2069 6e73 7461 6c6c 202e 2e2e 6029  ip install ...`)
-00001c00: 2e0a 0a30 312e 2046 6f72 6b20 7468 6520  ...01. Fork the 
-00001c10: 6071 7561 6e74 6966 792d 636f 7265 6020  `quantify-core` 
-00001c20: 7265 706f 206f 6e20 4769 744c 6162 2e0a  repo on GitLab..
-00001c30: 0a30 322e 2043 6c6f 6e65 2079 6f75 7220  .02. Clone your 
-00001c40: 666f 726b 206c 6f63 616c 6c79 3a0a 0a20  fork locally:.. 
-00001c50: 2020 2060 6060 0a20 2020 2024 2067 6974     ```.    $ git
-00001c60: 2063 6c6f 6e65 2067 6974 4067 6974 6c61   clone git@gitla
-00001c70: 622e 636f 6d3a 796f 7572 5f6e 616d 655f  b.com:your_name_
-00001c80: 6865 7265 2f71 7561 6e74 6966 792d 636f  here/quantify-co
-00001c90: 7265 2e67 6974 0a20 2020 2060 6060 0a0a  re.git.    ```..
-00001ca0: 3033 2e20 496e 7374 616c 6c20 7b6d 6f64  03. Install {mod
-00001cb0: 7d60 7175 616e 7469 6679 2d63 6f72 6560  }`quantify-core`
-00001cc0: 206c 6f63 616c 6c79 3a0a 0a20 2020 2060   locally:..    `
-00001cd0: 6060 0a20 2020 2024 2063 6420 7175 616e  ``.    $ cd quan
-00001ce0: 7469 6679 2d63 6f72 652f 0a20 2020 2024  tify-core/.    $
-00001cf0: 2070 6970 2069 6e73 7461 6c6c 202d 6520   pip install -e 
-00001d00: 222e 5b64 6576 5d22 0a20 2020 2060 6060  ".[dev]".    ```
-00001d10: 0a0a 3034 2e20 284f 7074 696f 6e61 6c29  ..04. (Optional)
-00001d20: 2049 6e73 7461 6c6c 2060 7072 652d 636f   Install `pre-co
-00001d30: 6d6d 6974 6020 7768 6963 6820 7769 6c6c  mmit` which will
-00001d40: 2061 7574 6f6d 6174 6963 616c 6c79 2066   automatically f
-00001d50: 6f72 6d61 7420 7468 6520 636f 6465 2075  ormat the code u
-00001d60: 7369 6e67 205b 626c 6163 6b5d 2868 7474  sing [black](htt
-00001d70: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001d80: 7073 662f 626c 6163 6b29 3a0a 0a20 2020  psf/black):..   
-00001d90: 203e 2060 6060 0a20 2020 203e 2024 2070   > ```.    > $ p
-00001da0: 7265 2d63 6f6d 6d69 7420 696e 7374 616c  re-commit instal
-00001db0: 6c0a 2020 2020 3e20 6060 600a 2020 2020  l.    > ```.    
-00001dc0: 3e0a 2020 2020 3e20 6060 607b 6e6f 7465  >.    > ```{note
-00001dd0: 7d0a 2020 2020 3e20 5768 656e 2074 6865  }.    > When the
-00001de0: 2063 6f64 6520 6973 206e 6f74 2077 656c   code is not wel
-00001df0: 6c20 666f 726d 6174 7465 6420 6120 6067  l formatted a `g
-00001e00: 6974 2063 6f6d 6d69 7460 2077 696c 6c20  it commit` will 
-00001e10: 6661 696c 2e20 596f 7520 6f6e 6c79 206e  fail. You only n
-00001e20: 6565 6420 746f 2072 756e 2069 7420 6167  eed to run it ag
-00001e30: 6169 6e2e 2054 6869 7320 7365 636f 6e64  ain. This second
-00001e40: 2074 696d 6520 7468 6520 636f 6465 2077   time the code w
-00001e50: 696c 6c20 6265 2061 6c72 6561 6479 202a  ill be already *
-00001e60: 626c 6163 6b2a 2d63 6f6d 706c 6961 6e74  black*-compliant
-00001e70: 2e0a 2020 2020 3e20 6060 600a 0a30 352e  ..    > ```..05.
-00001e80: 2043 7265 6174 6520 6120 6272 616e 6368   Create a branch
-00001e90: 2066 6f72 206c 6f63 616c 2064 6576 656c   for local devel
-00001ea0: 6f70 6d65 6e74 3a0a 0a20 2020 2060 6060  opment:..    ```
-00001eb0: 0a20 2020 2024 2067 6974 2063 6865 636b  .    $ git check
-00001ec0: 6f75 7420 2d62 206e 616d 652d 6f66 2d79  out -b name-of-y
-00001ed0: 6f75 722d 6275 6766 6978 2d6f 722d 6665  our-bugfix-or-fe
-00001ee0: 6174 7572 650a 2020 2020 6060 600a 0a20  ature.    ```.. 
-00001ef0: 2020 204e 6f77 2079 6f75 2063 616e 206d     Now you can m
-00001f00: 616b 6520 796f 7572 2063 6861 6e67 6573  ake your changes
-00001f10: 206c 6f63 616c 6c79 2e0a 0a30 362e 2054   locally...06. T
-00001f20: 6f20 656e 7375 7265 2067 6f6f 6420 7175  o ensure good qu
-00001f30: 616c 6974 7920 636f 6465 2072 756e 205b  ality code run [
-00001f40: 7079 6c69 6e74 5d28 6874 7470 733a 2f2f  pylint](https://
-00001f50: 7079 6c69 6e74 2e72 6561 6474 6865 646f  pylint.readthedo
-00001f60: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00001f70: 696e 6465 782e 6874 6d6c 2920 6f6e 2079  index.html) on y
-00001f80: 6f75 7220 636f 6465 2061 6e64 2061 6464  our code and add
-00001f90: 7265 7373 2061 6e79 2072 6561 736f 6e61  ress any reasona
-00001fa0: 626c 6520 636f 6465 2071 7561 6c69 7479  ble code quality
-00001fb0: 2069 7373 7565 732e 2053 6565 205b 4564   issues. See [Ed
-00001fc0: 6974 6f72 2061 6e64 2049 4445 2069 6e74  itor and IDE int
-00001fd0: 6567 7261 7469 6f6e 5d28 6874 7470 733a  egration](https:
-00001fe0: 2f2f 7079 6c69 6e74 2e72 6561 6474 6865  //pylint.readthe
-00001ff0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00002000: 742f 7573 6572 5f67 7569 6465 2f69 6465  t/user_guide/ide
-00002010: 2d69 6e74 6567 7261 7469 6f6e 2e68 746d  -integration.htm
-00002020: 6c29 2066 6f72 2074 6970 7320 6f6e 2068  l) for tips on h
-00002030: 6f77 2074 6f20 696e 7465 6772 6174 6520  ow to integrate 
-00002040: 7079 6c69 6e74 2069 6e20 796f 7572 2065  pylint in your e
-00002050: 6469 746f 7220 6f72 2049 4445 2e0a 0a30  ditor or IDE...0
-00002060: 372e 2057 6865 6e20 796f 7520 6172 6520  7. When you are 
-00002070: 646f 6e65 206d 616b 696e 6720 6368 616e  done making chan
-00002080: 6765 732c 2061 7574 6f2d 666f 726d 6174  ges, auto-format
-00002090: 2074 6865 2072 6570 6f73 6974 6f72 7920   the repository 
-000020a0: 7769 7468 2060 626c 6163 6b60 2061 6e64  with `black` and
-000020b0: 2065 6e73 7572 6520 7465 7374 2063 6f76   ensure test cov
-000020c0: 6572 6167 650a 0a20 2020 203e 2060 6060  erage..    > ```
-000020d0: 0a20 2020 203e 2024 2062 6c61 636b 202e  .    > $ black .
-000020e0: 0a20 2020 203e 2024 2070 7974 6573 7420  .    > $ pytest 
-000020f0: 2d2d 636f 760a 2020 2020 3e20 6060 600a  --cov.    > ```.
-00002100: 2020 2020 3e0a 2020 2020 3e20 6060 6060      >.    > ````
-00002110: 6060 7b74 6970 7d0a 2020 2020 3e20 5275  ``{tip}.    > Ru
-00002120: 6e6e 696e 6720 7061 7274 7320 6f66 2074  nning parts of t
-00002130: 6865 2074 6573 7420 7375 6974 650a 2020  he test suite.  
-00002140: 2020 3e0a 2020 2020 3e20 546f 2072 756e    >.    > To run
-00002150: 206f 6e6c 7920 7061 7274 7320 6f66 2074   only parts of t
-00002160: 6865 2074 6573 7420 7375 6974 652c 2073  he test suite, s
-00002170: 7065 6369 6679 2074 6865 2066 6f6c 6465  pecify the folde
-00002180: 7220 696e 2077 6869 6368 2074 6f20 6c6f  r in which to lo
-00002190: 6f6b 2066 6f72 0a20 2020 203e 2074 6573  ok for.    > tes
-000021a0: 7473 2061 7320 616e 2061 7267 756d 656e  ts as an argumen
-000021b0: 7420 746f 2070 7974 6573 742e 2054 6865  t to pytest. The
-000021c0: 2066 6f6c 6c6f 7769 6e67 2065 7861 6d70   following examp
-000021d0: 6c65 0a20 2020 203e 0a20 2020 203e 2060  le.    >.    > `
-000021e0: 6060 0a20 2020 203e 2024 2070 792e 7465  ``.    > $ py.te
-000021f0: 7374 2074 6573 7473 2f6d 6561 7375 7265  st tests/measure
-00002200: 6d65 6e74 202d 2d63 6f76 2071 7561 6e74  ment --cov quant
-00002210: 6966 795f 636f 7265 2f6d 6561 7375 7265  ify_core/measure
-00002220: 6d65 6e74 0a20 2020 203e 2060 6060 0a20  ment.    > ```. 
-00002230: 2020 203e 0a20 2020 203e 2077 696c 6c20     >.    > will 
-00002240: 6c6f 6f6b 2066 6f72 2074 6573 7473 206c  look for tests l
-00002250: 6f63 6174 6564 2069 6e20 7468 6520 7465  ocated in the te
-00002260: 7374 732f 6d65 6173 7572 656d 656e 7420  sts/measurement 
-00002270: 6469 7265 6374 6f72 7920 616e 6420 7265  directory and re
-00002280: 706f 7274 2074 6573 7420 636f 7665 7261  port test covera
-00002290: 6765 206f 6620 7468 6520 7175 616e 7469  ge of the quanti
-000022a0: 6679 5f63 6f72 652f 6d65 6173 7572 656d  fy_core/measurem
-000022b0: 656e 7420 6d6f 6475 6c65 2e0a 2020 2020  ent module..    
-000022c0: 3e20 6060 6060 6060 0a20 2020 203e 0a20  > ``````.    >. 
-000022d0: 2020 203e 2060 6060 6060 607b 7469 707d     > ``````{tip}
-000022e0: 0a20 2020 203e 2053 7065 6564 2075 7020  .    > Speed up 
-000022f0: 7465 7374 7320 7769 7468 2070 6172 616c  tests with paral
-00002300: 6c65 6c20 6578 6563 7574 696f 6e0a 2020  lel execution.  
-00002310: 2020 3e0a 2020 2020 3e20 6060 600a 2020    >.    > ```.  
-00002320: 2020 3e20 2420 7079 2e74 6573 7420 2d6e    > $ py.test -n
-00002330: 2032 2023 2077 6865 7265 2032 2069 7320   2 # where 2 is 
-00002340: 7468 6520 6e75 6d62 6572 206f 6620 636f  the number of co
-00002350: 7265 7320 6f66 2079 6f75 7220 4350 550a  res of your CPU.
-00002360: 2020 2020 3e20 6060 600a 2020 2020 3e20      > ```.    > 
-00002370: 6060 6060 6060 0a0a 3038 2e20 4275 696c  ``````..08. Buil
-00002380: 6469 6e67 2074 6865 2064 6f63 756d 656e  ding the documen
-00002390: 7461 7469 6f6e 0a0a 2020 2020 3e20 4966  tation..    > If
-000023a0: 2079 6f75 2068 6176 6520 776f 726b 6564   you have worked
-000023b0: 206f 6e20 646f 6375 6d65 6e74 6174 696f   on documentatio
-000023c0: 6e20 6f72 205b 646f 6373 7472 696e 6773  n or [docstrings
-000023d0: 5d28 6874 7470 733a 2f2f 7777 772e 7079  ](https://www.py
-000023e0: 7468 6f6e 2e6f 7267 2f64 6576 2f70 6570  thon.org/dev/pep
-000023f0: 732f 7065 702d 3032 3537 2f29 2079 6f75  s/pep-0257/) you
-00002400: 206e 6565 6420 746f 2072 6576 6965 7720   need to review 
-00002410: 686f 7720 796f 7572 2064 6f63 7320 6c6f  how your docs lo
-00002420: 6f6b 206c 6f63 616c 6c79 2061 6e64 2065  ok locally and e
-00002430: 6e73 7572 6520 2a6e 6f20 6572 726f 7220  nsure *no error 
-00002440: 6f72 2077 6172 6e69 6e67 7320 6172 6520  or warnings are 
-00002450: 7261 6973 6564 2a2e 0a20 2020 203e 2059  raised*..    > Y
-00002460: 6f75 2063 616e 2062 7569 6c64 2074 6865  ou can build the
-00002470: 2064 6f63 7320 6c6f 6361 6c6c 7920 7573   docs locally us
-00002480: 696e 673a 0a20 2020 203e 0a20 2020 203e  ing:.    >.    >
-00002490: 2060 6060 0a20 2020 203e 2024 2063 6420   ```.    > $ cd 
-000024a0: 646f 6373 0a20 2020 203e 0a20 2020 203e  docs.    >.    >
-000024b0: 2024 2023 2075 6e69 780a 2020 2020 3e20   $ # unix.    > 
-000024c0: 2420 6d61 6b65 2068 746d 6c0a 2020 2020  $ make html.    
-000024d0: 3e0a 2020 2020 3e20 2420 2320 7769 6e64  >.    > $ # wind
-000024e0: 6f77 730a 2020 2020 3e20 2420 2e2f 6d61  ows.    > $ ./ma
-000024f0: 6b65 2e62 6174 2068 746d 6c0a 2020 2020  ke.bat html.    
-00002500: 3e20 6060 600a 2020 2020 3e0a 2020 2020  > ```.    >.    
-00002510: 3e20 5468 6520 646f 6373 2077 696c 6c20  > The docs will 
-00002520: 6265 206c 6f63 6174 6564 2069 6e20 6071  be located in `q
-00002530: 7561 6e74 6966 795f 636f 7265 2f64 6f63  uantify_core/doc
-00002540: 732f 5f62 7569 6c64 602e 0a20 2020 203e  s/_build`..    >
-00002550: 0a20 2020 203e 2060 6060 6060 607b 7469  .    > ``````{ti
-00002560: 707d 0a20 2020 203e 2049 6620 796f 7520  p}.    > If you 
-00002570: 6172 6520 776f 726b 696e 6720 6f6e 2064  are working on d
-00002580: 6f63 756d 656e 7461 7469 6f6e 2069 7420  ocumentation it 
-00002590: 6361 6e20 6265 2075 7365 6675 6c20 746f  can be useful to
-000025a0: 2061 7574 6f6d 6174 6963 616c 6c79 2072   automatically r
-000025b0: 6562 7569 6c64 2074 6865 2064 6f63 7320  ebuild the docs 
-000025c0: 6166 7465 7220 6576 6572 7920 6368 616e  after every chan
-000025d0: 6765 2e0a 2020 2020 3e20 5468 6973 2063  ge..    > This c
-000025e0: 616e 2062 6520 646f 6e65 2075 7369 6e67  an be done using
-000025f0: 2074 6865 2060 7370 6869 6e78 2d61 7574   the `sphinx-aut
-00002600: 6f62 7569 6c64 6020 7061 636b 6167 652e  obuild` package.
-00002610: 2054 6872 6f75 6768 2074 6865 2066 6f6c   Through the fol
-00002620: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0a  lowing command:.
-00002630: 2020 2020 3e0a 2020 2020 3e20 6060 600a      >.    > ```.
-00002640: 2020 2020 3e20 2420 7370 6869 6e78 2d61      > $ sphinx-a
-00002650: 7574 6f62 7569 6c64 2064 6f63 7320 646f  utobuild docs do
-00002660: 6373 2f5f 6275 696c 642f 6874 6d6c 0a20  cs/_build/html. 
-00002670: 2020 203e 2060 6060 0a20 2020 203e 0a20     > ```.    >. 
-00002680: 2020 203e 2054 6865 2064 6f63 756d 656e     > The documen
-00002690: 7461 7469 6f6e 2077 696c 6c20 7468 656e  tation will then
-000026a0: 2062 6520 686f 7374 6564 206f 6e20 606c   be hosted on `l
-000026b0: 6f63 616c 686f 7374 3a38 3030 3060 0a20  ocalhost:8000`. 
-000026c0: 2020 203e 2060 6060 6060 600a 2020 2020     > ``````.    
-000026d0: 3e0a 2020 2020 3e20 6060 607b 7469 707d  >.    > ```{tip}
-000026e0: 0a20 2020 203e 2042 7569 6c64 696e 6720  .    > Building 
-000026f0: 7468 6520 7475 746f 7269 616c 7320 6361  the tutorials ca
-00002700: 6e20 6265 2074 696d 6520 636f 6e73 756d  n be time consum
-00002710: 696e 672c 2069 6620 796f 7520 6172 6520  ing, if you are 
-00002720: 6e6f 7420 6564 6974 696e 6720 7468 656d  not editing them
-00002730: 2c20 6665 656c 2066 7265 6520 746f 2064  , feel free to d
-00002740: 656c 6574 6520 796f 7572 206c 6f63 616c  elete your local
-00002750: 2063 6f70 7920 6f66 2074 6865 2060 7175   copy of the `qu
-00002760: 616e 7469 6679 2d63 6f72 652f 646f 6373  antify-core/docs
-00002770: 2f74 7574 6f72 6961 6c73 6020 746f 2073  /tutorials` to s
-00002780: 6b69 7020 7468 6569 7220 6275 696c 642e  kip their build.
-00002790: 2059 6f75 2063 616e 2072 6563 6f76 6572   You can recover
-000027a0: 2074 6865 2066 696c 6573 2075 7369 6e67   the files using
-000027b0: 2067 6974 2028 646f 206e 6f74 2063 6f6d   git (do not com
-000027c0: 6d69 7420 7468 6520 6465 6c65 7465 6420  mit the deleted 
-000027d0: 6669 6c65 7329 2e0a 2020 2020 3e20 6060  files)..    > ``
-000027e0: 600a 0a30 392e 2043 6f6d 6d69 7420 796f  `..09. Commit yo
-000027f0: 7572 2063 6861 6e67 6573 2061 6e64 2070  ur changes and p
-00002800: 7573 6820 796f 7572 2062 7261 6e63 6820  ush your branch 
-00002810: 746f 2047 6974 4c61 623a 0a0a 2020 2020  to GitLab:..    
-00002820: 6060 600a 2020 2020 2420 6769 7420 6164  ```.    $ git ad
-00002830: 6420 2e0a 2020 2020 2420 6769 7420 636f  d ..    $ git co
-00002840: 6d6d 6974 202d 6d20 2259 6f75 7220 6465  mmit -m "Your de
-00002850: 7461 696c 6564 2064 6573 6372 6970 7469  tailed descripti
-00002860: 6f6e 206f 6620 796f 7572 2063 6861 6e67  on of your chang
-00002870: 6573 2e22 0a20 2020 2024 2067 6974 2070  es.".    $ git p
-00002880: 7573 6820 6f72 6967 696e 206e 616d 652d  ush origin name-
-00002890: 6f66 2d79 6f75 722d 6275 6766 6978 2d6f  of-your-bugfix-o
-000028a0: 722d 6665 6174 7572 650a 2020 2020 6060  r-feature.    ``
-000028b0: 600a 0a31 302e 2052 6576 6965 7720 7468  `..10. Review th
-000028c0: 6520 7b72 6566 7d60 4d65 7267 6520 5265  e {ref}`Merge Re
-000028d0: 7175 6573 7420 4775 6964 656c 696e 6573  quest Guidelines
-000028e0: 6020 616e 6420 7375 626d 6974 2061 206d  ` and submit a m
-000028f0: 6572 6765 2072 6571 7565 7374 2074 6872  erge request thr
-00002900: 6f75 6768 2074 6865 2047 6974 4c61 6220  ough the GitLab 
-00002910: 7765 6273 6974 652e 0a0a 3131 2e20 4164  website...11. Ad
-00002920: 6420 6120 7368 6f72 7420 656e 7472 7920  d a short entry 
-00002930: 696e 2074 6865 2060 4348 414e 4745 4c4f  in the `CHANGELO
-00002940: 472e 6d64 6020 756e 6465 7220 6055 6e72  G.md` under `Unr
-00002950: 656c 6561 7365 6460 2c20 636f 6d6d 6974  eleased`, commit
-00002960: 2061 6e64 2070 7573 682e 0a0a 2323 2054   and push...## T
-00002970: 726f 7562 6c65 7368 6f6f 7469 6e67 0a0a  roubleshooting..
-00002980: 4966 2066 6f72 2073 6f6d 6520 7265 6173  If for some reas
-00002990: 6f6e 2079 6f75 2061 7265 206e 6f74 2061  on you are not a
-000029a0: 626c 6520 746f 2069 6e73 7461 6c6c 206f  ble to install o
-000029b0: 7220 7573 6520 5175 616e 7469 6679 2075  r use Quantify u
-000029c0: 7369 6e67 2074 6865 2070 7265 7363 7269  sing the prescri
-000029d0: 6265 6420 7761 7973 2069 6e64 6963 6174  bed ways indicat
-000029e0: 6564 2061 626f 7665 2c20 6d61 6b65 2073  ed above, make s
-000029f0: 7572 6520 796f 7520 6861 7665 2061 2077  ure you have a w
-00002a00: 6f72 6b69 6e67 2070 7974 686f 6e20 656e  orking python en
-00002a10: 7669 726f 6e6d 656e 7420 2865 2e67 2e20  vironment (e.g. 
-00002a20: 796f 7520 6361 6e20 7275 6e20 616e 2060  you can run an `
-00002a30: 4950 7974 686f 6e60 2074 6572 6d69 6e61  IPython` termina
-00002a40: 6c29 2e20 466f 6c6c 6f77 2074 6865 206e  l). Follow the n
-00002a50: 6578 7420 7374 6570 7320 7468 6174 2061  ext steps that a
-00002a60: 696d 2061 7420 696e 7374 616c 6c69 6e67  im at installing
-00002a70: 2051 7561 6e74 6966 7920 6672 6f6d 2073   Quantify from s
-00002a80: 6f75 7263 6520 616e 6420 7275 6e6e 696e  ource and runnin
-00002a90: 6720 6974 7320 7465 7374 732e 0a0a 302e  g its tests...0.
-00002aa0: 2055 6e69 6e73 7461 6c6c 207b 6d6f 647d   Uninstall {mod}
-00002ab0: 6071 7561 6e74 6966 792d 636f 7265 603a  `quantify-core`:
-00002ac0: 0a0a 2020 2060 6060 0a20 2020 2420 7069  ..   ```.   $ pi
-00002ad0: 7020 756e 696e 7374 616c 6c20 7175 616e  p uninstall quan
-00002ae0: 7469 6679 2d63 6f72 650a 2020 2060 6060  tify-core.   ```
-00002af0: 0a0a 312e 2049 6e73 7461 6c6c 2066 726f  ..1. Install fro
-00002b00: 6d20 736f 7572 6365 2028 7275 6e20 6c69  m source (run li
-00002b10: 6e65 2062 7920 6c69 6e65 293a 0a0a 2020  ne by line):..  
-00002b20: 2060 6060 0a20 2020 2420 6769 7420 636c   ```.   $ git cl
-00002b30: 6f6e 6520 6874 7470 733a 2f2f 6769 746c  one https://gitl
-00002b40: 6162 2e63 6f6d 2f71 7561 6e74 6966 792d  ab.com/quantify-
-00002b50: 6f73 2f71 7561 6e74 6966 792d 636f 7265  os/quantify-core
-00002b60: 2e67 6974 3b20 6364 2071 7561 6e74 6966  .git; cd quantif
-00002b70: 792d 636f 7265 0a20 2020 2420 7069 7020  y-core.   $ pip 
-00002b80: 696e 7374 616c 6c20 2d2d 7570 6772 6164  install --upgrad
-00002b90: 6520 2d2d 7570 6772 6164 652d 7374 7261  e --upgrade-stra
-00002ba0: 7465 6779 2065 6167 6572 2022 2e5b 6465  tegy eager ".[de
-00002bb0: 765d 220a 2020 2024 2070 7974 6573 7420  v]".   $ pytest 
-00002bc0: 2d76 0a20 2020 6060 600a 0a32 2e20 5468  -v.   ```..2. Th
-00002bd0: 6520 7465 7374 7320 7769 6c6c 2065 6974  e tests will eit
-00002be0: 6865 7220 7061 7373 206f 7220 6e6f 742e  her pass or not.
-00002bf0: 2049 6e20 616e 7920 6361 7365 2c20 706c   In any case, pl
-00002c00: 6561 7365 2072 6570 6f72 7420 796f 7572  ease report your
-00002c10: 2065 7870 6572 6965 6e63 6520 616e 6420   experience and 
-00002c20: 7768 6963 6820 7465 7374 2064 6f20 6e6f  which test do no
-00002c30: 7420 7061 7373 2062 7920 6372 6561 7469  t pass by creati
-00002c40: 6e67 2061 2060 4e65 7720 6973 7375 6560  ng a `New issue`
-00002c50: 206f 6e20 7468 6520 5b69 7373 7565 2074   on the [issue t
-00002c60: 7261 636b 6572 5d28 6874 7470 733a 2f2f  racker](https://
-00002c70: 6769 746c 6162 2e63 6f6d 2f71 7561 6e74  gitlab.com/quant
-00002c80: 6966 792d 6f73 2f71 7561 6e74 6966 792d  ify-os/quantify-
-00002c90: 636f 7265 2f2d 2f69 7373 7565 7329 2c20  core/-/issues), 
-00002ca0: 796f 7572 2065 6666 6f72 7473 2061 7265  your efforts are
-00002cb0: 206d 7563 6820 6170 7072 6563 6961 7465   much appreciate
-00002cc0: 6420 616e 6420 7769 6c6c 2068 656c 7020  d and will help 
-00002cd0: 7573 2074 6f20 756e 6465 7273 7461 6e64  us to understand
-00002ce0: 2074 6865 2070 726f 626c 656d 7320 796f   the problems yo
-00002cf0: 7520 6d69 6768 7420 6265 2066 6163 696e  u might be facin
-00002d00: 672e 0a0a 2323 2320 446f 776e 6772 6164  g...### Downgrad
-00002d10: 6520 746f 2061 2073 7065 6369 6669 6320  e to a specific 
-00002d20: 7665 7273 696f 6e0a 0a49 6620 666f 7220  version..If for 
-00002d30: 616e 7920 7265 6173 6f6e 2079 6f75 2072  any reason you r
-00002d40: 6571 7569 7265 2061 2073 7065 6369 6669  equire a specifi
-00002d50: 6320 7665 7273 696f 6e20 6f66 2074 6865  c version of the
-00002d60: 2070 6163 6b61 6765 2c20 652e 672e 2030   package, e.g. 0
-00002d70: 2e33 2e30 2c20 7275 6e3a 0a0a 6060 600a  .3.0, run:..```.
-00002d80: 2420 7069 7020 696e 7374 616c 6c20 2d2d  $ pip install --
-00002d90: 7570 6772 6164 6520 7175 616e 7469 6679  upgrade quantify
-00002da0: 2d63 6f72 653d 3d30 2e33 2e30 0a60 6060  -core==0.3.0.```
-00002db0: 0a0a 2323 2320 506f 7465 6e74 6961 6c20  ..### Potential 
-00002dc0: 6973 7375 6573 3a20 5079 5174 4772 6170  issues: PyQtGrap
-00002dd0: 6820 616e 6420 5079 5174 350a 0a7b 6d6f  h and PyQt5..{mo
-00002de0: 647d 6071 7561 6e74 6966 792d 636f 7265  d}`quantify-core
-00002df0: 6020 6861 7320 6120 6465 7065 6e64 656e  ` has a dependen
-00002e00: 6379 206f 6e20 7468 6520 6050 7951 7435  cy on the `PyQt5
-00002e10: 6020 7061 636b 6167 652c 2077 6869 6368  ` package, which
-00002e20: 2069 7473 656c 6620 6861 7320 6120 6465   itself has a de
-00002e30: 7065 6e64 656e 6379 206f 6e20 7468 6520  pendency on the 
-00002e40: 6051 7435 6020 7275 6e74 696d 652e 0a4f  `Qt5` runtime..O
-00002e50: 6e20 6d6f 7374 2073 7973 7465 6d73 2c20  n most systems, 
-00002e60: 7468 6520 7374 616e 6461 7264 2069 6e73  the standard ins
-00002e70: 7461 6c6c 6174 696f 6e20 7072 6f63 6573  tallation proces
-00002e80: 7320 7769 6c6c 2063 6f72 7265 6374 6c79  s will correctly
-00002e90: 2069 6e73 7461 6c6c 2051 742e 0a54 6865   install Qt..The
-00002ea0: 2041 6e61 636f 6e64 6120 696e 7374 616c   Anaconda instal
-00002eb0: 6c61 7469 6f6e 2073 686f 756c 6420 7265  lation should re
-00002ec0: 736f 6c76 6520 6973 7375 6573 2077 6974  solve issues wit
-00002ed0: 6820 696e 7374 616c 6c61 7469 6f6e 206f  h installation o
-00002ee0: 6e20 5769 6e64 6f77 7320 6f72 206d 6163  n Windows or mac
-00002ef0: 4f53 2e0a 596f 7520 6d61 7920 6e65 6564  OS..You may need
-00002f00: 2074 6f20 636f 6e73 756c 7420 6120 7365   to consult a se
-00002f10: 6172 6368 2065 6e67 696e 6520 6966 2079  arch engine if y
-00002f20: 6f75 2068 6176 6520 6120 6d6f 7265 2065  ou have a more e
-00002f30: 786f 7469 6320 7379 7374 656d 2e0a 0a5b  xotic system...[
-00002f40: 7069 705d 3a20 6874 7470 733a 2f2f 7069  pip]: https://pi
-00002f50: 702e 7079 7061 2e69 6f0a 5b70 7974 686f  p.pypa.io.[pytho
-00002f60: 6e20 696e 7374 616c 6c61 7469 6f6e 2067  n installation g
-00002f70: 7569 6465 5d3a 2068 7474 703a 2f2f 646f  uide]: http://do
-00002f80: 6373 2e70 7974 686f 6e2d 6775 6964 652e  cs.python-guide.
-00002f90: 6f72 672f 656e 2f6c 6174 6573 742f 7374  org/en/latest/st
-00002fa0: 6172 7469 6e67 2f69 6e73 7461 6c6c 6174  arting/installat
-00002fb0: 696f 6e2f 0a                             ion/.
+000000d0: 2c20 7365 6520 7b72 6566 7d60 5365 7474  , see {ref}`Sett
+000000e0: 696e 6720 7570 2066 6f72 206c 6f63 616c  ing up for local
+000000f0: 2064 6576 656c 6f70 6d65 6e74 602e 0a0a   development`...
+00000100: 2323 2320 4f6e 2057 696e 646f 7773 2061  ### On Windows a
+00000110: 6e64 206d 6163 4f53 2028 416e 6163 6f6e  nd macOS (Anacon
+00000120: 6461 290a 0a7b 6d6f 647d 6071 7561 6e74  da)..{mod}`quant
+00000130: 6966 792d 636f 7265 6020 6861 7320 7468  ify-core` has th
+00000140: 6972 6420 7061 7274 7920 6465 7065 6e64  ird party depend
+00000150: 656e 6369 6573 2074 6861 7420 6361 6e20  encies that can 
+00000160: 6861 7665 2065 6e76 6972 6f6e 6d65 6e74  have environment
+00000170: 2d73 7065 6369 6669 6320 7072 6f62 6c65  -specific proble
+00000180: 6d73 2e0a 5765 2072 6563 6f6d 6d65 6e64  ms..We recommend
+00000190: 2075 7369 6e67 2074 6865 205b 416e 6163   using the [Anac
+000001a0: 6f6e 6461 5d28 6874 7470 733a 2f2f 7777  onda](https://ww
+000001b0: 772e 616e 6163 6f6e 6461 2e63 6f6d 2f70  w.anaconda.com/p
+000001c0: 726f 6475 6374 732f 696e 6469 7669 6475  roducts/individu
+000001d0: 616c 2344 6f77 6e6c 6f61 6473 2920 5079  al#Downloads) Py
+000001e0: 7468 6f6e 2064 6973 7472 6962 7574 696f  thon distributio
+000001f0: 6e20 7768 6963 6820 776f 726b 7320 6f75  n which works ou
+00000200: 7420 6f66 2074 6865 2062 6f78 206f 6e20  t of the box on 
+00000210: 6d6f 7374 2073 7973 7465 6d73 2e0a 0a49  most systems...I
+00000220: 6620 796f 7520 6172 6520 6661 6d69 6c69  f you are famili
+00000230: 6172 2077 6974 6820 736f 6674 7761 7265  ar with software
+00000240: 2064 6576 656c 6f70 6d65 6e74 2028 7061   development (pa
+00000250: 636b 6167 6520 6d61 6e61 6765 722c 2067  ckage manager, g
+00000260: 6974 2c20 7465 726d 696e 616c 2c20 5079  it, terminal, Py
+00000270: 7468 6f6e 2c20 6574 632e 2920 7468 6520  thon, etc.) the 
+00000280: 666f 6c6c 6f77 696e 6720 7368 6f75 6c64  following should
+00000290: 2067 6574 2079 6f75 2072 756e 6e69 6e67   get you running
+000002a0: 2069 6e20 6e6f 2074 696d 652e 204f 7468   in no time. Oth
+000002b0: 6572 7769 7365 2c20 666f 6c6c 6f77 2074  erwise, follow t
+000002c0: 6865 207b 7265 667d 6044 6574 6169 6c65  he {ref}`Detaile
+000002d0: 6420 696e 7374 7275 6374 696f 6e73 6020  d instructions` 
+000002e0: 616e 6420 6c65 6172 6e20 6120 6665 7720  and learn a few 
+000002f0: 7072 6f64 7563 7469 7669 7479 2074 6970  productivity tip
+00000300: 7320 6f6e 2079 6f75 7220 7761 792e 0a0a  s on your way...
+00000310: 312e 2049 6e73 7461 6c6c 205b 416e 6163  1. Install [Anac
+00000320: 6f6e 6461 5d28 6874 7470 733a 2f2f 7777  onda](https://ww
+00000330: 772e 616e 6163 6f6e 6461 2e63 6f6d 2f70  w.anaconda.com/p
+00000340: 726f 6475 6374 732f 696e 6469 7669 6475  roducts/individu
+00000350: 616c 2344 6f77 6e6c 6f61 6473 292e 0a0a  al#Downloads)...
+00000360: 322e 2049 6e73 7461 6c6c 2051 7561 6e74  2. Install Quant
+00000370: 6966 7920 2861 6e64 204a 7570 7974 6572  ify (and Jupyter
+00000380: 4c61 6229 2069 6e20 6120 6e65 7720 636f  Lab) in a new co
+00000390: 6e64 6120 656e 7669 726f 6e6d 656e 742c  nda environment,
+000003a0: 2073 6565 2061 6c73 6f20 7468 6520 5b43   see also the [C
+000003b0: 6f6e 6461 2063 6865 6174 2073 6865 6574  onda cheat sheet
+000003c0: 5d28 6874 7470 733a 2f2f 646f 6373 2e63  ](https://docs.c
+000003d0: 6f6e 6461 2e69 6f2f 7072 6f6a 6563 7473  onda.io/projects
+000003e0: 2f63 6f6e 6461 2f65 6e2f 6c61 7465 7374  /conda/en/latest
+000003f0: 2f75 7365 722d 6775 6964 652f 6368 6561  /user-guide/chea
+00000400: 7473 6865 6574 2e68 746d 6c29 2e0a 0a20  tsheet.html)... 
+00000410: 2020 3e20 6060 607b 6164 6d6f 6e69 7469    > ```{admoniti
+00000420: 6f6e 7d20 5375 7070 6f72 7465 6420 5079  on} Supported Py
+00000430: 7468 6f6e 2076 6572 7369 6f6e 730a 2020  thon versions.  
+00000440: 203e 2043 6865 636b 2074 6865 2073 7570   > Check the sup
+00000450: 706f 7274 6564 2050 7974 686f 6e20 7665  ported Python ve
+00000460: 7273 696f 6e73 206f 6e20 5079 5069 3a20  rsions on PyPi: 
+00000470: 5b71 7561 6e74 6966 792d 636f 7265 5d28  [quantify-core](
+00000480: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000490: 2f70 726f 6a65 6374 2f71 7561 6e74 6966  /project/quantif
+000004a0: 792d 636f 7265 2f29 207c 205b 7175 616e  y-core/) | [quan
+000004b0: 7469 6679 2d73 6368 6564 756c 6572 5d28  tify-scheduler](
+000004c0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+000004d0: 2f70 726f 6a65 6374 2f71 7561 6e74 6966  /project/quantif
+000004e0: 792d 7363 6865 6475 6c65 722f 290a 2020  y-scheduler/).  
+000004f0: 203e 2060 6060 0a0a 2020 203e 204e 2e42   > ```..   > N.B
+00000500: 2e20 4966 2079 6f75 2061 7265 2069 6e74  . If you are int
+00000510: 6572 6573 7465 6420 746f 2063 6f6e 7472  erested to contr
+00000520: 6962 7574 6520 746f 207b 6d6f 647d 6071  ibute to {mod}`q
+00000530: 7561 6e74 6966 792d 636f 7265 6020 616e  uantify-core` an
+00000540: 642f 6f72 207b 6d6f 647d 6071 7561 6e74  d/or {mod}`quant
+00000550: 6966 792d 7363 6865 6475 6c65 7260 2079  ify-scheduler` y
+00000560: 6f75 2073 686f 756c 6420 7b72 6566 7d60  ou should {ref}`
+00000570: 7365 7420 7468 656d 2075 7020 666f 7220  set them up for 
+00000580: 6c6f 6361 6c20 6465 7665 6c6f 706d 656e  local developmen
+00000590: 7420 696e 7374 6561 6420 3c53 6574 7469  t instead <Setti
+000005a0: 6e67 2075 7020 666f 7220 6c6f 6361 6c20  ng up for local 
+000005b0: 6465 7665 6c6f 706d 656e 743e 602e 0a20  development>`.. 
+000005c0: 2020 3e0a 2020 203e 2060 6060 0a20 2020    >.   > ```.   
+000005d0: 3e20 2420 2320 7275 6e20 7468 6520 666f  > $ # run the fo
+000005e0: 6c6c 6f77 696e 6720 636f 6d6d 616e 6473  llowing commands
+000005f0: 2073 7465 7020 6279 2073 7465 7021 0a20   step by step!. 
+00000600: 2020 3e0a 2020 203e 2024 2063 6f6e 6461    >.   > $ conda
+00000610: 2063 7265 6174 6520 2d2d 6e61 6d65 2071   create --name q
+00000620: 7561 6e74 6966 792d 656e 7620 7079 7468  uantify-env pyth
+00000630: 6f6e 3d33 2e38 0a20 2020 3e20 2420 636f  on=3.8.   > $ co
+00000640: 6e64 6120 6163 7469 7661 7465 2071 7561  nda activate qua
+00000650: 6e74 6966 792d 656e 760a 2020 203e 2024  ntify-env.   > $
+00000660: 2063 6f6e 6461 2069 6e73 7461 6c6c 202d   conda install -
+00000670: 6320 636f 6e64 612d 666f 7267 6520 6a75  c conda-forge ju
+00000680: 7079 7465 726c 6162 0a20 2020 3e20 2420  pyterlab.   > $ 
+00000690: 7079 7468 6f6e 202d 6d20 6970 796b 6572  python -m ipyker
+000006a0: 6e65 6c20 696e 7374 616c 6c20 2d2d 7573  nel install --us
+000006b0: 6572 202d 2d6e 616d 653d 7175 616e 7469  er --name=quanti
+000006c0: 6679 2d65 6e76 2020 2d2d 6469 7370 6c61  fy-env  --displa
+000006d0: 792d 6e61 6d65 3d22 5079 7468 6f6e 2033  y-name="Python 3
+000006e0: 2051 7561 6e74 6966 7920 456e 7622 0a20   Quantify Env". 
+000006f0: 2020 3e20 2420 7069 7020 696e 7374 616c    > $ pip instal
+00000700: 6c20 7175 616e 7469 6679 2d63 6f72 650a  l quantify-core.
+00000710: 2020 203e 0a20 2020 3e20 2420 2320 284f     >.   > $ # (O
+00000720: 7074 696f 6e61 6c6c 7929 2069 6e73 7461  ptionally) insta
+00000730: 6c6c 2071 7561 6e74 6966 792d 7363 6865  ll quantify-sche
+00000740: 6475 6c65 723a 0a20 2020 3e0a 2020 203e  duler:.   >.   >
+00000750: 2024 2070 6970 2069 6e73 7461 6c6c 2071   $ pip install q
+00000760: 7561 6e74 6966 792d 7363 6865 6475 6c65  uantify-schedule
+00000770: 720a 2020 203e 2024 206a 7570 7974 6572  r.   > $ jupyter
+00000780: 206c 6162 6578 7465 6e73 696f 6e20 696e   labextension in
+00000790: 7374 616c 6c20 6a75 7079 7465 726c 6162  stall jupyterlab
+000007a0: 2d70 6c6f 746c 7920 2d2d 6e6f 2d62 7569  -plotly --no-bui
+000007b0: 6c64 0a20 2020 3e20 2420 2320 7468 6973  ld.   > $ # this
+000007c0: 206d 6967 6874 2074 616b 6520 6120 6665   might take a fe
+000007d0: 7720 6d69 6e75 7465 730a 2020 203e 2024  w minutes.   > $
+000007e0: 206a 7570 7974 6572 206c 6162 6578 7465   jupyter labexte
+000007f0: 6e73 696f 6e20 696e 7374 616c 6c20 406a  nsion install @j
+00000800: 7570 7974 6572 2d77 6964 6765 7473 2f6a  upyter-widgets/j
+00000810: 7570 7974 6572 6c61 622d 6d61 6e61 6765  upyterlab-manage
+00000820: 7220 706c 6f74 6c79 7769 6467 6574 0a20  r plotlywidget. 
+00000830: 2020 3e20 6060 600a 0a33 2e20 596f 7520    > ```..3. You 
+00000840: 6172 6520 676f 6f64 2074 6f20 676f 2120  are good to go! 
+00000850: 4865 6164 206f 7665 7220 746f 2074 6865  Head over to the
+00000860: 207b 7265 667d 6055 7365 7220 6775 6964   {ref}`User guid
+00000870: 6520 3c75 7365 722d 6775 6964 653e 6020  e <user-guide>` 
+00000880: 746f 2067 6574 2073 7461 7274 6564 2e0a  to get started..
+00000890: 0a23 2323 2320 4465 7461 696c 6564 2069  .#### Detailed i
+000008a0: 6e73 7472 7563 7469 6f6e 730a 0a31 2e20  nstructions..1. 
+000008b0: 496e 7374 616c 6c20 5b41 6e61 636f 6e64  Install [Anacond
+000008c0: 615d 2868 7474 7073 3a2f 2f77 7777 2e61  a](https://www.a
+000008d0: 6e61 636f 6e64 612e 636f 6d2f 7072 6f64  naconda.com/prod
+000008e0: 7563 7473 2f69 6e64 6976 6964 7561 6c23  ucts/individual#
+000008f0: 446f 776e 6c6f 6164 7329 2e0a 0a20 2020  Downloads)...   
+00000900: 3e20 4f6e 2057 696e 646f 7773 2c20 6475  > On Windows, du
+00000910: 7269 6e67 2074 6865 2069 6e73 7461 6c6c  ring the install
+00000920: 6174 696f 6e2c 2077 6520 7265 636f 6d6d  ation, we recomm
+00000930: 656e 6420 746f 2073 656c 6563 7420 7468  end to select th
+00000940: 6520 6f70 7469 6f6e 733a 0a20 2020 3e0a  e options:.   >.
+00000950: 2020 203e 202d 2049 6e73 7461 6c6c 2066     > - Install f
+00000960: 6f72 2060 416c 6c20 5573 6572 7320 2872  or `All Users (r
+00000970: 6571 7569 7265 7320 6164 6d69 6e20 7072  equires admin pr
+00000980: 6976 696c 6567 6573 2960 3b20 616e 640a  ivileges)`; and.
+00000990: 2020 203e 202d 2060 4164 6420 416e 6163     > - `Add Anac
+000009a0: 6f6e 6461 3320 7468 6520 7379 7374 656d  onda3 the system
+000009b0: 2050 4154 4820 656e 7669 726f 6e6d 656e   PATH environmen
+000009c0: 7420 7661 7269 6162 6c65 602e 0a20 2020  t variable`..   
+000009d0: 3e0a 2020 203e 2060 6060 6060 607b 6164  >.   > ``````{ad
+000009e0: 6d6f 6e69 7469 6f6e 7d20 496e 7374 7275  monition} Instru
+000009f0: 6374 696f 6e73 3a20 416e 6163 6f6e 6461  ctions: Anaconda
+00000a00: 2069 6e73 7461 6c6c 2028 5769 6e64 6f77   install (Window
+00000a10: 7329 0a20 2020 3e20 3a63 6c61 7373 3a20  s).   > :class: 
+00000a20: 6472 6f70 646f 776e 2c20 696e 666f 0a20  dropdown, info. 
+00000a30: 2020 3e0a 2020 203e 2060 6060 7b66 6967    >.   > ```{fig
+00000a40: 7572 657d 202f 696d 6167 6573 2f69 6e73  ure} /images/ins
+00000a50: 7461 6c6c 2f63 6f6e 6461 5f69 6e73 7461  tall/conda_insta
+00000a60: 6c6c 2e67 6966 0a20 2020 3e20 3a6e 616d  ll.gif.   > :nam
+00000a70: 653a 2063 6f6e 6461 5f69 6e73 7461 6c6c  e: conda_install
+00000a80: 0a20 2020 3e20 3a77 6964 7468 3a20 3530  .   > :width: 50
+00000a90: 300a 2020 203e 2060 6060 0a20 2020 3e20  0.   > ```.   > 
+00000aa0: 6060 6060 6060 0a0a 322e 2028 5769 6e64  ``````..2. (Wind
+00000ab0: 6f77 7320 6f6e 6c79 2920 496e 7374 616c  ows only) Instal
+00000ac0: 6c20 5b47 6974 2042 4153 485d 2868 7474  l [Git BASH](htt
+00000ad0: 7073 3a2f 2f67 6974 666f 7277 696e 646f  ps://gitforwindo
+00000ae0: 7773 2e6f 7267 2f29 2074 6f20 6861 7665  ws.org/) to have
+00000af0: 2061 2075 6e69 782d 6c69 6b65 2062 6173   a unix-like bas
+00000b00: 6820 7465 726d 696e 616c 2028 6465 6661  h terminal (defa
+00000b10: 756c 7420 6f70 7469 6f6e 7320 6475 7269  ult options duri
+00000b20: 6e67 2069 6e73 7461 6c6c 6174 696f 6e20  ng installation 
+00000b30: 7368 6f75 6c64 2077 6f72 6b20 7765 6c6c  should work well
+00000b40: 206f 6e20 6d6f 7374 2073 6574 7570 7329   on most setups)
+00000b50: 2e0a 0a20 2020 3e20 6060 607b 7469 707d  ...   > ```{tip}
+00000b60: 0a20 2020 3e20 5573 6572 7320 6361 6e20  .   > Users can 
+00000b70: 7269 6768 7420 636c 6963 6b20 616e 7920  right click any 
+00000b80: 666f 6c64 6572 2069 6e20 7769 6e64 6f77  folder in window
+00000b90: 7320 616e 6420 6f70 656e 2047 6974 2042  s and open Git B
+00000ba0: 4153 4820 696e 2074 6861 7420 6c6f 6361  ASH in that loca
+00000bb0: 7469 6f6e 2e0a 2020 203e 2060 6060 0a20  tion..   > ```. 
+00000bc0: 2020 3e0a 2020 203e 2060 6060 7b6e 6f74    >.   > ```{not
+00000bd0: 657d 0a20 2020 3e20 4265 2061 7761 7265  e}.   > Be aware
+00000be0: 2074 6861 7420 6120 756e 6978 2d6c 696b   that a unix-lik
+00000bf0: 6520 7465 726d 696e 616c 206f 6e20 7769  e terminal on wi
+00000c00: 6e64 6f77 7320 6861 7320 736f 6d65 2063  ndows has some c
+00000c10: 6176 6561 7473 2e20 546f 2061 766f 6964  aveats. To avoid
+00000c20: 2074 6865 6d2c 2077 6520 7265 636f 6d6d   them, we recomm
+00000c30: 656e 6420 746f 2072 756e 2061 6e79 2050  end to run any P
+00000c40: 7974 686f 6e20 636f 6465 2075 7369 6e67  ython code using
+00000c50: 205b 4a75 7079 7465 724c 6162 5d28 6874   [JupyterLab](ht
+00000c60: 7470 733a 2f2f 6a75 7079 7465 726c 6162  tps://jupyterlab
+00000c70: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000c80: 656e 2f73 7461 626c 652f 2920 2869 6e73  en/stable/) (ins
+00000c90: 7461 6c6c 6174 696f 6e20 7374 6570 7320  tallation steps 
+00000ca0: 6265 6c6f 7729 2e0a 2020 203e 2060 6060  below)..   > ```
+00000cb0: 0a0a 332e 2028 5769 6e64 6f77 7320 6f6e  ..3. (Windows on
+00000cc0: 6c79 2920 4164 6420 7b63 6f64 657d 6073  ly) Add {code}`s
+00000cd0: 6f75 7263 6520 2f70 6174 682f 746f 2f41  ource /path/to/A
+00000ce0: 6e61 636f 6e64 6133 2f65 7463 2f70 726f  naconda3/etc/pro
+00000cf0: 6669 6c65 2e64 2f63 6f6e 6461 2e73 6860  file.d/conda.sh`
+00000d00: 2069 6e20 7468 6520 602e 6261 7368 7263   in the `.bashrc
+00000d10: 6020 286f 7220 696e 2074 6865 2060 2e62  ` (or in the `.b
+00000d20: 6173 685f 7072 6f66 696c 6560 2920 746f  ash_profile`) to
+00000d30: 2065 7870 6f73 6520 7468 6520 616e 6163   expose the anac
+00000d40: 6f6e 6461 2069 6e20 6261 7368 2074 6572  onda in bash ter
+00000d50: 6d69 6e61 6c20 2873 6565 2069 6e73 7472  minal (see instr
+00000d60: 7563 7469 6f6e 2062 656c 6f77 2069 6620  uction below if 
+00000d70: 796f 7520 6e65 6564 2068 656c 7029 2e0a  you need help)..
+00000d80: 0a20 2020 3e20 6060 607b 7469 707d 0a20  .   > ```{tip}. 
+00000d90: 2020 3e20 4966 2079 6f75 2066 6f6c 6c6f    > If you follo
+00000da0: 7765 6420 7468 6520 6465 6661 756c 7420  wed the default 
+00000db0: 616e 6163 6f6e 6461 2069 6e73 7461 6c6c  anaconda install
+00000dc0: 6174 696f 6e20 7468 6520 7061 7468 2074  ation the path t
+00000dd0: 6f20 6974 2077 696c 6c20 6265 2073 696d  o it will be sim
+00000de0: 696c 6172 2074 6f0a 2020 203e 207b 636f  ilar to.   > {co
+00000df0: 6465 7d60 2f63 2f55 7365 7273 2f3c 594f  de}`/c/Users/<YO
+00000e00: 5552 5f55 5345 524e 414d 453e 2f61 6e61  UR_USERNAME>/ana
+00000e10: 636f 6e64 6133 2f65 7463 2f70 726f 6669  conda3/etc/profi
+00000e20: 6c65 2e64 2f63 6f6e 6461 2e73 6860 206f  le.d/conda.sh` o
+00000e30: 7220 7b63 6f64 657d 602f 632f 5072 6f67  r {code}`/c/Prog
+00000e40: 7261 6d44 6174 612f 416e 6163 6f6e 6461  ramData/Anaconda
+00000e50: 332f 6574 632f 7072 6f66 696c 652e 642f  3/etc/profile.d/
+00000e60: 636f 6e64 612e 7368 602e 0a20 2020 3e0a  conda.sh`..   >.
+00000e70: 2020 203e 2050 726f 2074 6970 3a20 796f     > Pro tip: yo
+00000e80: 7520 6361 6e20 6472 6167 2061 6e64 2064  u can drag and d
+00000e90: 726f 7020 6120 6669 6c65 2066 726f 6d20  rop a file from 
+00000ea0: 7468 6520 6669 6c65 2065 7870 6c6f 7265  the file explore
+00000eb0: 7220 696e 746f 2074 6865 2074 6572 6d69  r into the termi
+00000ec0: 6e61 6c20 616e 6420 6765 7420 7468 6520  nal and get the 
+00000ed0: 7061 7468 206f 6620 7468 6520 6669 6c65  path of the file
+00000ee0: 2028 696e 7374 6561 6420 6f66 2074 7970   (instead of typ
+00000ef0: 696e 6720 6974 206d 616e 7561 6c6c 7929  ing it manually)
+00000f00: 2e0a 2020 203e 2060 6060 0a20 2020 3e0a  ..   > ```.   >.
+00000f10: 2020 203e 2060 6060 6060 607b 6164 6d6f     > ``````{admo
+00000f20: 6e69 7469 6f6e 7d20 496e 7374 7275 6374  nition} Instruct
+00000f30: 696f 6e73 3a20 6578 706f 7365 2061 6e61  ions: expose ana
+00000f40: 636f 6e64 6120 696e 2074 6865 2062 6173  conda in the bas
+00000f50: 6820 7465 726d 696e 616c 0a20 2020 3e20  h terminal.   > 
+00000f60: 3a63 6c61 7373 3a20 6472 6f70 646f 776e  :class: dropdown
+00000f70: 2c20 696e 666f 0a20 2020 3e0a 2020 203e  , info.   >.   >
+00000f80: 2042 656c 6f77 2077 6520 696c 6c75 7374   Below we illust
+00000f90: 7261 7465 2074 6869 7320 7072 6f63 6573  rate this proces
+00000fa0: 7320 696e 2047 6974 2042 6173 682e 2059  s in Git Bash. Y
+00000fb0: 6f75 2063 616e 2066 696e 6420 6465 7461  ou can find deta
+00000fc0: 696c 6564 2073 7465 702d 6279 2d73 7465  iled step-by-ste
+00000fd0: 7020 696e 7374 7275 6374 696f 6e73 205b  p instructions [
+00000fe0: 6865 7265 5d28 6874 7470 733a 2f2f 7375  here](https://su
+00000ff0: 7065 7275 7365 722e 636f 6d2f 612f 3630  peruser.com/a/60
+00001000: 3238 3936 292e 0a20 2020 3e0a 2020 203e  2896)..   >.   >
+00001010: 2060 6060 7b66 6967 7572 657d 202f 696d   ```{figure} /im
+00001020: 6167 6573 2f69 6e73 7461 6c6c 2f63 6f6e  ages/install/con
+00001030: 6461 5f73 6f75 7263 655f 696e 7374 616c  da_source_instal
+00001040: 6c65 645f 616c 6c5f 7573 6572 732e 6769  led_all_users.gi
+00001050: 660a 2020 203e 203a 6e61 6d65 3a20 636f  f.   > :name: co
+00001060: 6e64 615f 736f 7572 6365 0a20 2020 3e20  nda_source.   > 
+00001070: 3a77 6964 7468 3a20 3530 300a 2020 203e  :width: 500.   >
+00001080: 2060 6060 0a20 2020 3e20 6060 6060 6060   ```.   > ``````
+00001090: 0a20 2020 3e0a 2020 203e 2060 6060 7b6e  .   >.   > ```{n
+000010a0: 6f74 657d 0a20 2020 3e20 546f 2063 6f6e  ote}.   > To con
+000010b0: 6669 726d 2079 6f75 2068 6176 6520 6120  firm you have a 
+000010c0: 6675 6e63 7469 6f6e 616c 2069 6e73 7461  functional insta
+000010d0: 6c6c 6174 696f 6e20 6f66 2061 6e61 636f  llation of anaco
+000010e0: 6e64 612c 2072 756e 207b 636f 6465 7d60  nda, run {code}`
+000010f0: 636f 6e64 6160 2069 6e20 7468 6520 7465  conda` in the te
+00001100: 726d 696e 616c 2e20 5468 6973 2077 696c  rminal. This wil
+00001110: 6c20 7072 696e 7420 7468 6520 636f 6e64  l print the cond
+00001120: 6120 6865 6c70 206d 6573 7361 6765 2077  a help message w
+00001130: 6869 6368 2069 7320 616e 2069 6e64 6963  hich is an indic
+00001140: 6174 696f 6e20 6f66 2061 2077 6f72 6b69  ation of a worki
+00001150: 6e67 2069 6e73 7461 6c6c 6174 696f 6e2e  ng installation.
+00001160: 0a20 2020 3e20 6060 600a 0a34 2e20 4372  .   > ```..4. Cr
+00001170: 6561 7465 2061 2063 6f6e 6461 2065 6e76  eate a conda env
+00001180: 6972 6f6e 6d65 6e74 2c20 7365 6520 616c  ironment, see al
+00001190: 736f 2074 6865 205b 436f 6e64 6120 6368  so the [Conda ch
+000011a0: 6561 7420 7368 6565 745d 2868 7474 7073  eat sheet](https
+000011b0: 3a2f 2f64 6f63 732e 636f 6e64 612e 696f  ://docs.conda.io
+000011c0: 2f70 726f 6a65 6374 732f 636f 6e64 612f  /projects/conda/
+000011d0: 656e 2f6c 6174 6573 742f 7573 6572 2d67  en/latest/user-g
+000011e0: 7569 6465 2f63 6865 6174 7368 6565 742e  uide/cheatsheet.
+000011f0: 6874 6d6c 292e 0a0a 2020 203e 2060 6060  html)...   > ```
+00001200: 0a20 2020 3e20 2420 636f 6e64 6120 6372  .   > $ conda cr
+00001210: 6561 7465 202d 2d6e 616d 6520 7175 616e  eate --name quan
+00001220: 7469 6679 2d65 6e76 2070 7974 686f 6e3d  tify-env python=
+00001230: 332e 3820 2020 2320 6372 6561 7465 2074  3.8   # create t
+00001240: 6865 2063 6f6e 6461 2065 6e76 6972 6f6e  he conda environ
+00001250: 6d65 6e74 2c20 796f 7520 6361 6e20 7265  ment, you can re
+00001260: 706c 6163 6520 6071 7561 6e74 6966 792d  place `quantify-
+00001270: 656e 7660 2069 6620 796f 7520 7769 7368  env` if you wish
+00001280: 0a20 2020 3e20 2420 636f 6e64 6120 6163  .   > $ conda ac
+00001290: 7469 7661 7465 2071 7561 6e74 6966 792d  tivate quantify-
+000012a0: 656e 7620 2020 2020 2020 2020 2020 2020  env             
+000012b0: 2020 2020 2020 2320 6163 7469 7661 7465        # activate
+000012c0: 7320 7468 6520 636f 6e64 6120 656e 7669  s the conda envi
+000012d0: 726f 6e6d 656e 740a 2020 203e 2060 6060  ronment.   > ```
+000012e0: 0a20 2020 3e0a 2020 203e 2060 6060 7b74  .   >.   > ```{t
+000012f0: 6970 7d0a 2020 203e 2059 6f75 2063 616e  ip}.   > You can
+00001300: 2061 6464 207b 636f 6465 7d60 636f 6e64   add {code}`cond
+00001310: 6120 6163 7469 7661 7465 2071 7561 6e74  a activate quant
+00001320: 6966 792d 656e 7660 2061 7420 7468 6520  ify-env` at the 
+00001330: 656e 6420 6f66 2074 6865 2060 2e62 6173  end of the `.bas
+00001340: 6872 6360 2028 6f72 2060 2e62 6173 685f  hrc` (or `.bash_
+00001350: 7072 6f66 696c 6560 2920 6966 2079 6f75  profile`) if you
+00001360: 2077 6973 6820 666f 7220 7468 6973 2065   wish for this e
+00001370: 6e76 6972 6f6e 6d65 6e74 2074 6f20 6265  nvironment to be
+00001380: 2061 6374 6976 6174 6564 2061 7574 6f6d   activated autom
+00001390: 6174 6963 616c 6c79 2069 6e20 7468 6520  atically in the 
+000013a0: 7465 726d 696e 616c 2077 6865 6e20 6974  terminal when it
+000013b0: 2069 7320 6f70 656e 6564 2028 7365 6520   is opened (see 
+000013c0: 696e 7374 7275 6374 696f 6e73 2062 656c  instructions bel
+000013d0: 6f77 292e 0a20 2020 3e20 6060 600a 2020  ow)..   > ```.  
+000013e0: 203e 0a20 2020 3e20 6060 6060 6060 7b61   >.   > ``````{a
+000013f0: 646d 6f6e 6974 696f 6e7d 2049 6e73 7472  dmonition} Instr
+00001400: 7563 7469 6f6e 733a 2063 7265 6174 6520  uctions: create 
+00001410: 636f 6e64 6120 656e 7620 616e 6420 6175  conda env and au
+00001420: 746f 2d61 6374 6976 6174 6520 2857 696e  to-activate (Win
+00001430: 646f 7773 290a 2020 203e 203a 636c 6173  dows).   > :clas
+00001440: 733a 2064 726f 7064 6f77 6e2c 2069 6e66  s: dropdown, inf
+00001450: 6f0a 2020 203e 0a20 2020 3e20 6060 607b  o.   >.   > ```{
+00001460: 6669 6775 7265 7d20 2f69 6d61 6765 732f  figure} /images/
+00001470: 696e 7374 616c 6c2f 636f 6e64 615f 6163  install/conda_ac
+00001480: 7469 7661 7465 2e67 6966 0a20 2020 3e20  tivate.gif.   > 
+00001490: 3a6e 616d 653a 2063 6f6e 6461 5f61 6374  :name: conda_act
+000014a0: 6976 6174 650a 2020 203e 203a 7769 6474  ivate.   > :widt
+000014b0: 683a 2035 3030 0a20 2020 3e20 6060 600a  h: 500.   > ```.
+000014c0: 2020 203e 2060 6060 6060 600a 0a35 2e20     > ``````..5. 
+000014d0: 496e 7374 616c 6c20 606a 7570 7974 6572  Install `jupyter
+000014e0: 2d6c 6162 6020 696e 2074 6865 206e 6577  -lab` in the new
+000014f0: 2065 6e76 6972 6f6e 6d65 6e74 2075 7369   environment usi
+00001500: 6e67 3a0a 0a20 2020 6060 600a 2020 2024  ng:..   ```.   $
+00001510: 2063 6f6e 6461 2069 6e73 7461 6c6c 202d   conda install -
+00001520: 6320 636f 6e64 612d 666f 7267 6520 6a75  c conda-forge ju
+00001530: 7079 7465 726c 6162 2020 2320 696e 7374  pyterlab  # inst
+00001540: 616c 6c20 6a75 7079 7465 7220 6c61 620a  all jupyter lab.
+00001550: 2020 2024 2023 2061 6464 2074 6865 2065     $ # add the e
+00001560: 6e76 6972 6f6e 6d65 6e74 2061 7320 616e  nvironment as an
+00001570: 2061 7661 696c 6162 6c65 206b 6572 6e65   available kerne
+00001580: 6c20 666f 7220 6a75 7079 7465 7220 6e6f  l for jupyter no
+00001590: 7465 626f 6f6b 2077 6974 6869 6e20 6a75  tebook within ju
+000015a0: 7079 7465 722d 6c61 622e 0a20 2020 2420  pyter-lab..   $ 
+000015b0: 7079 7468 6f6e 202d 6d20 6970 796b 6572  python -m ipyker
+000015c0: 6e65 6c20 696e 7374 616c 6c20 2d2d 7573  nel install --us
+000015d0: 6572 202d 2d6e 616d 653d 7175 616e 7469  er --name=quanti
+000015e0: 6679 2d65 6e76 2020 2d2d 6469 7370 6c61  fy-env  --displa
+000015f0: 792d 6e61 6d65 3d22 5079 7468 6f6e 2033  y-name="Python 3
+00001600: 2051 7561 6e74 6966 7920 456e 7622 0a20   Quantify Env". 
+00001610: 2020 6060 600a 0a36 2e20 496e 7374 616c    ```..6. Instal
+00001620: 6c20 7b6d 6f64 7d60 7175 616e 7469 6679  l {mod}`quantify
+00001630: 2d63 6f72 6560 2066 726f 6d20 7079 7069  -core` from pypi
+00001640: 0a0a 2020 203e 2049 6620 796f 7520 6172  ..   > If you ar
+00001650: 6520 696e 7465 7265 7374 6564 2074 6f20  e interested to 
+00001660: 636f 6e74 7269 6275 7465 2074 6f20 5175  contribute to Qu
+00001670: 616e 7469 6679 2d63 6f72 6520 796f 7520  antify-core you 
+00001680: 7368 6f75 6c64 207b 7265 667d 6073 6574  should {ref}`set
+00001690: 2069 7420 7570 2066 6f72 206c 6f63 616c   it up for local
+000016a0: 2064 6576 656c 6f70 6d65 6e74 2069 6e73   development ins
+000016b0: 7465 6164 203c 5365 7474 696e 6720 7570  tead <Setting up
+000016c0: 2066 6f72 206c 6f63 616c 2064 6576 656c   for local devel
+000016d0: 6f70 6d65 6e74 3e60 2e0a 2020 203e 0a20  opment>`..   >. 
+000016e0: 2020 3e20 6060 600a 2020 203e 2024 2070    > ```.   > $ p
+000016f0: 6970 2069 6e73 7461 6c6c 2071 7561 6e74  ip install quant
+00001700: 6966 792d 636f 7265 0a20 2020 3e20 6060  ify-core.   > ``
+00001710: 600a 2020 203e 0a20 2020 3e20 6060 607b  `.   >.   > ```{
+00001720: 6e6f 7465 7d0a 2020 203e 2057 6520 6375  note}.   > We cu
+00001730: 7272 656e 746c 7920 646f 206e 6f74 2068  rrently do not h
+00001740: 6176 6520 6120 636f 6e64 6120 7265 6369  ave a conda reci
+00001750: 7065 2066 6f72 2069 6e73 7461 6c6c 6174  pe for installat
+00001760: 696f 6e2c 2069 6e73 7465 6164 2077 6520  ion, instead we 
+00001770: 7265 6665 7220 746f 2074 6865 2064 6566  refer to the def
+00001780: 6175 6c74 2070 6970 2069 6e73 7461 6c6c  ault pip install
+00001790: 6174 696f 6e20 7769 7468 696e 2061 2063  ation within a c
+000017a0: 6f6e 6461 2065 6e76 6972 6f6e 6d65 6e74  onda environment
+000017b0: 2e0a 2020 203e 2060 6060 0a0a 372e 2028  ..   > ```..7. (
+000017c0: 4f70 7469 6f6e 616c 6c79 2920 696e 7374  Optionally) inst
+000017d0: 616c 6c20 7b6d 6f64 7d60 7175 616e 7469  all {mod}`quanti
+000017e0: 6679 2d73 6368 6564 756c 6572 600a 0a20  fy-scheduler`.. 
+000017f0: 2020 3e20 4966 2079 6f75 2061 7265 2069    > If you are i
+00001800: 6e74 6572 6573 7465 6420 746f 2063 6f6e  nterested to con
+00001810: 7472 6962 7574 6520 746f 207b 6d6f 647d  tribute to {mod}
+00001820: 6071 7561 6e74 6966 792d 7363 6865 6475  `quantify-schedu
+00001830: 6c65 7260 2079 6f75 2073 686f 756c 6420  ler` you should 
+00001840: 7b72 6566 7d60 7365 7420 6974 2075 7020  {ref}`set it up 
+00001850: 666f 7220 6c6f 6361 6c20 6465 7665 6c6f  for local develo
+00001860: 706d 656e 7420 696e 7374 6561 6420 3c53  pment instead <S
+00001870: 6574 7469 6e67 2075 7020 666f 7220 6c6f  etting up for lo
+00001880: 6361 6c20 6465 7665 6c6f 706d 656e 743e  cal development>
+00001890: 602e 2059 6f75 206f 6e6c 7920 6e65 6564  `. You only need
+000018a0: 2074 6f20 7265 706c 6163 6520 7b6d 6f64   to replace {mod
+000018b0: 7d60 7175 616e 7469 6679 2d63 6f72 6560  }`quantify-core`
+000018c0: 2077 6974 6820 7b6d 6f64 7d60 7175 616e   with {mod}`quan
+000018d0: 7469 6679 2d73 6368 6564 756c 6572 6020  tify-scheduler` 
+000018e0: 696e 2074 6865 2070 726f 7669 6465 6420  in the provided 
+000018f0: 636f 6d6d 616e 6473 2e0a 2020 203e 0a20  commands..   >. 
+00001900: 2020 3e20 6060 600a 2020 203e 2024 2070    > ```.   > $ p
+00001910: 6970 2069 6e73 7461 6c6c 2071 7561 6e74  ip install quant
+00001920: 6966 792d 7363 6865 6475 6c65 720a 2020  ify-scheduler.  
+00001930: 203e 2024 206a 7570 7974 6572 206c 6162   > $ jupyter lab
+00001940: 6578 7465 6e73 696f 6e20 696e 7374 616c  extension instal
+00001950: 6c20 6a75 7079 7465 726c 6162 2d70 6c6f  l jupyterlab-plo
+00001960: 746c 7920 2d2d 6e6f 2d62 7569 6c64 0a20  tly --no-build. 
+00001970: 2020 3e20 2420 2320 7468 6973 206d 6967    > $ # this mig
+00001980: 6874 2074 616b 6520 6120 6665 7720 6d69  ht take a few mi
+00001990: 6e75 7465 730a 2020 203e 2024 206a 7570  nutes.   > $ jup
+000019a0: 7974 6572 206c 6162 6578 7465 6e73 696f  yter labextensio
+000019b0: 6e20 696e 7374 616c 6c20 406a 7570 7974  n install @jupyt
+000019c0: 6572 2d77 6964 6765 7473 2f6a 7570 7974  er-widgets/jupyt
+000019d0: 6572 6c61 622d 6d61 6e61 6765 7220 706c  erlab-manager pl
+000019e0: 6f74 6c79 7769 6467 6574 0a20 2020 3e20  otlywidget.   > 
+000019f0: 6060 600a 0a23 2323 204f 7468 6572 206f  ```..### Other o
+00001a00: 7065 7261 7469 6e67 2073 7973 7465 6d73  perating systems
+00001a10: 0a0a 436f 6e66 6972 6d20 7468 6174 2079  ..Confirm that y
+00001a20: 6f75 2068 6176 6520 6120 636f 6d70 6174  ou have a compat
+00001a30: 6962 6c65 2077 6f72 6b69 6e67 2050 7974  ible working Pyt
+00001a40: 686f 6e20 696e 7465 7270 7265 7465 7220  hon interpreter 
+00001a50: 6279 2072 756e 6e69 6e67 2074 6865 2066  by running the f
+00001a60: 6f6c 6c6f 7769 6e67 2069 6e20 796f 7572  ollowing in your
+00001a70: 2074 6572 6d69 6e61 6c20 6f66 2063 686f   terminal of cho
+00001a80: 6963 653a 0a60 6060 0a24 2070 7974 686f  ice:.```.$ pytho
+00001a90: 6e20 2d2d 7665 7273 696f 6e0a 5079 7468  n --version.Pyth
+00001aa0: 6f6e 2033 2e38 2e31 300a 6060 600a 6060  on 3.8.10.```.``
+00001ab0: 607b 6164 6d6f 6e69 7469 6f6e 7d20 5375  `{admonition} Su
+00001ac0: 7070 6f72 7465 6420 5079 7468 6f6e 2076  pported Python v
+00001ad0: 6572 7369 6f6e 730a 4368 6563 6b20 7468  ersions.Check th
+00001ae0: 6520 7375 7070 6f72 7465 6420 5079 7468  e supported Pyth
+00001af0: 6f6e 2076 6572 7369 6f6e 7320 6f6e 2050  on versions on P
+00001b00: 7950 693a 205b 7175 616e 7469 6679 2d63  yPi: [quantify-c
+00001b10: 6f72 655d 2868 7474 7073 3a2f 2f70 7970  ore](https://pyp
+00001b20: 692e 6f72 672f 7072 6f6a 6563 742f 7175  i.org/project/qu
+00001b30: 616e 7469 6679 2d63 6f72 652f 2920 7c20  antify-core/) | 
+00001b40: 5b71 7561 6e74 6966 792d 7363 6865 6475  [quantify-schedu
+00001b50: 6c65 725d 2868 7474 7073 3a2f 2f70 7970  ler](https://pyp
+00001b60: 692e 6f72 672f 7072 6f6a 6563 742f 7175  i.org/project/qu
+00001b70: 616e 7469 6679 2d73 6368 6564 756c 6572  antify-scheduler
+00001b80: 2f29 0a60 6060 0a0a 496e 7374 616c 6c20  /).```..Install 
+00001b90: 5175 616e 7469 6679 3a0a 0a60 6060 0a24  Quantify:..```.$
+00001ba0: 2070 6970 2069 6e73 7461 6c6c 2071 7561   pip install qua
+00001bb0: 6e74 6966 792d 636f 7265 0a60 6060 0a0a  ntify-core.```..
+00001bc0: 4966 2079 6f75 2064 6f6e 2774 2068 6176  If you don't hav
+00001bd0: 6520 5b70 6970 5d20 696e 7374 616c 6c65  e [pip] installe
+00001be0: 642c 2074 6869 7320 5b50 7974 686f 6e20  d, this [Python 
+00001bf0: 696e 7374 616c 6c61 7469 6f6e 2067 7569  installation gui
+00001c00: 6465 5d20 6361 6e20 6775 6964 650a 796f  de] can guide.yo
+00001c10: 7520 7468 726f 7567 6820 7468 6520 7072  u through the pr
+00001c20: 6f63 6573 732e 0a0a 2323 2055 7064 6174  ocess...## Updat
+00001c30: 6520 746f 2074 6865 206c 6174 6573 7420  e to the latest 
+00001c40: 7665 7273 696f 6e0a 0a54 6f20 7570 6461  version..To upda
+00001c50: 7465 2051 7561 6e74 6966 7920 746f 2074  te Quantify to t
+00001c60: 6865 206c 6174 6573 7420 7665 7273 696f  he latest versio
+00001c70: 6e3a 0a0a 6060 600a 2420 7069 7020 696e  n:..```.$ pip in
+00001c80: 7374 616c 6c20 7175 616e 7469 6679 2d63  stall quantify-c
+00001c90: 6f72 650a 6060 600a 0a23 2320 5365 7474  ore.```..## Sett
+00001ca0: 696e 6720 7570 2066 6f72 206c 6f63 616c  ing up for local
+00001cb0: 2064 6576 656c 6f70 6d65 6e74 0a0a 5265   development..Re
+00001cc0: 6164 7920 746f 2063 6f6e 7472 6962 7574  ady to contribut
+00001cd0: 653f 2048 6572 6527 7320 686f 7720 746f  e? Here's how to
+00001ce0: 2073 6574 2075 7020 5175 616e 7469 6679   set up Quantify
+00001cf0: 2066 6f72 206c 6f63 616c 2064 6576 656c   for local devel
+00001d00: 6f70 6d65 6e74 2e0a 0a30 302e 2046 6f6c  opment...00. Fol
+00001d10: 6c6f 7720 7468 6520 7b72 6566 7d60 496e  low the {ref}`In
+00001d20: 7374 616c 6c61 7469 6f6e 6020 7374 6570  stallation` step
+00001d30: 7320 666f 7220 796f 7572 2073 7973 7465  s for your syste
+00001d40: 6d20 736b 6970 7069 6e67 2074 6865 206c  m skipping the l
+00001d50: 6173 7420 7374 6570 2028 7b63 6f64 657d  ast step ({code}
+00001d60: 6070 6970 2069 6e73 7461 6c6c 202e 2e2e  `pip install ...
+00001d70: 6029 2e0a 0a30 312e 2046 6f72 6b20 7468  `)...01. Fork th
+00001d80: 6520 6071 7561 6e74 6966 792d 636f 7265  e `quantify-core
+00001d90: 6020 7265 706f 206f 6e20 4769 744c 6162  ` repo on GitLab
+00001da0: 2e0a 0a30 322e 2043 6c6f 6e65 2079 6f75  ...02. Clone you
+00001db0: 7220 666f 726b 206c 6f63 616c 6c79 3a0a  r fork locally:.
+00001dc0: 0a20 2020 2060 6060 0a20 2020 2024 2067  .    ```.    $ g
+00001dd0: 6974 2063 6c6f 6e65 2067 6974 4067 6974  it clone git@git
+00001de0: 6c61 622e 636f 6d3a 796f 7572 5f6e 616d  lab.com:your_nam
+00001df0: 655f 6865 7265 2f71 7561 6e74 6966 792d  e_here/quantify-
+00001e00: 636f 7265 2e67 6974 0a20 2020 2060 6060  core.git.    ```
+00001e10: 0a0a 3033 2e20 496e 7374 616c 6c20 7b6d  ..03. Install {m
+00001e20: 6f64 7d60 7175 616e 7469 6679 2d63 6f72  od}`quantify-cor
+00001e30: 6560 206c 6f63 616c 6c79 3a0a 0a20 2020  e` locally:..   
+00001e40: 2060 6060 0a20 2020 2024 2063 6420 7175   ```.    $ cd qu
+00001e50: 616e 7469 6679 2d63 6f72 652f 0a20 2020  antify-core/.   
+00001e60: 2024 2070 6970 2069 6e73 7461 6c6c 202d   $ pip install -
+00001e70: 6520 222e 5b64 6576 5d22 0a20 2020 2060  e ".[dev]".    `
+00001e80: 6060 0a0a 3034 2e20 284f 7074 696f 6e61  ``..04. (Optiona
+00001e90: 6c29 2049 6e73 7461 6c6c 2060 7072 652d  l) Install `pre-
+00001ea0: 636f 6d6d 6974 6020 7768 6963 6820 7769  commit` which wi
+00001eb0: 6c6c 2061 7574 6f6d 6174 6963 616c 6c79  ll automatically
+00001ec0: 2066 6f72 6d61 7420 7468 6520 636f 6465   format the code
+00001ed0: 2075 7369 6e67 205b 626c 6163 6b5d 2868   using [black](h
+00001ee0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001ef0: 6d2f 7073 662f 626c 6163 6b29 3a0a 0a20  m/psf/black):.. 
+00001f00: 2020 203e 2060 6060 0a20 2020 203e 2024     > ```.    > $
+00001f10: 2070 7265 2d63 6f6d 6d69 7420 696e 7374   pre-commit inst
+00001f20: 616c 6c0a 2020 2020 3e20 6060 600a 2020  all.    > ```.  
+00001f30: 2020 3e0a 2020 2020 3e20 6060 607b 6e6f    >.    > ```{no
+00001f40: 7465 7d0a 2020 2020 3e20 5768 656e 2074  te}.    > When t
+00001f50: 6865 2063 6f64 6520 6973 206e 6f74 2077  he code is not w
+00001f60: 656c 6c20 666f 726d 6174 7465 6420 6120  ell formatted a 
+00001f70: 6067 6974 2063 6f6d 6d69 7460 2077 696c  `git commit` wil
+00001f80: 6c20 6661 696c 2e20 596f 7520 6f6e 6c79  l fail. You only
+00001f90: 206e 6565 6420 746f 2072 756e 2069 7420   need to run it 
+00001fa0: 6167 6169 6e2e 2054 6869 7320 7365 636f  again. This seco
+00001fb0: 6e64 2074 696d 6520 7468 6520 636f 6465  nd time the code
+00001fc0: 2077 696c 6c20 6265 2061 6c72 6561 6479   will be already
+00001fd0: 202a 626c 6163 6b2a 2d63 6f6d 706c 6961   *black*-complia
+00001fe0: 6e74 2e0a 2020 2020 3e20 6060 600a 0a30  nt..    > ```..0
+00001ff0: 352e 2043 7265 6174 6520 6120 6272 616e  5. Create a bran
+00002000: 6368 2066 6f72 206c 6f63 616c 2064 6576  ch for local dev
+00002010: 656c 6f70 6d65 6e74 3a0a 0a20 2020 2060  elopment:..    `
+00002020: 6060 0a20 2020 2024 2067 6974 2063 6865  ``.    $ git che
+00002030: 636b 6f75 7420 2d62 206e 616d 652d 6f66  ckout -b name-of
+00002040: 2d79 6f75 722d 6275 6766 6978 2d6f 722d  -your-bugfix-or-
+00002050: 6665 6174 7572 650a 2020 2020 6060 600a  feature.    ```.
+00002060: 0a20 2020 204e 6f77 2079 6f75 2063 616e  .    Now you can
+00002070: 206d 616b 6520 796f 7572 2063 6861 6e67   make your chang
+00002080: 6573 206c 6f63 616c 6c79 2e0a 0a30 362e  es locally...06.
+00002090: 2054 6f20 656e 7375 7265 2067 6f6f 6420   To ensure good 
+000020a0: 7175 616c 6974 7920 636f 6465 2072 756e  quality code run
+000020b0: 205b 7079 6c69 6e74 5d28 6874 7470 733a   [pylint](https:
+000020c0: 2f2f 7079 6c69 6e74 2e72 6561 6474 6865  //pylint.readthe
+000020d0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+000020e0: 742f 696e 6465 782e 6874 6d6c 2920 6f6e  t/index.html) on
+000020f0: 2079 6f75 7220 636f 6465 2061 6e64 2061   your code and a
+00002100: 6464 7265 7373 2061 6e79 2072 6561 736f  ddress any reaso
+00002110: 6e61 626c 6520 636f 6465 2071 7561 6c69  nable code quali
+00002120: 7479 2069 7373 7565 732e 2053 6565 205b  ty issues. See [
+00002130: 4564 6974 6f72 2061 6e64 2049 4445 2069  Editor and IDE i
+00002140: 6e74 6567 7261 7469 6f6e 5d28 6874 7470  ntegration](http
+00002150: 733a 2f2f 7079 6c69 6e74 2e72 6561 6474  s://pylint.readt
+00002160: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00002170: 6573 742f 7573 6572 5f67 7569 6465 2f69  est/user_guide/i
+00002180: 6465 2d69 6e74 6567 7261 7469 6f6e 2e68  de-integration.h
+00002190: 746d 6c29 2066 6f72 2074 6970 7320 6f6e  tml) for tips on
+000021a0: 2068 6f77 2074 6f20 696e 7465 6772 6174   how to integrat
+000021b0: 6520 7079 6c69 6e74 2069 6e20 796f 7572  e pylint in your
+000021c0: 2065 6469 746f 7220 6f72 2049 4445 2e0a   editor or IDE..
+000021d0: 0a30 372e 2057 6865 6e20 796f 7520 6172  .07. When you ar
+000021e0: 6520 646f 6e65 206d 616b 696e 6720 6368  e done making ch
+000021f0: 616e 6765 732c 2061 7574 6f2d 666f 726d  anges, auto-form
+00002200: 6174 2074 6865 2072 6570 6f73 6974 6f72  at the repositor
+00002210: 7920 7769 7468 2060 626c 6163 6b60 2061  y with `black` a
+00002220: 6e64 2065 6e73 7572 6520 7465 7374 2063  nd ensure test c
+00002230: 6f76 6572 6167 650a 0a20 2020 203e 2060  overage..    > `
+00002240: 6060 0a20 2020 203e 2024 2062 6c61 636b  ``.    > $ black
+00002250: 202e 0a20 2020 203e 2024 2070 7974 6573   ..    > $ pytes
+00002260: 7420 2d2d 636f 760a 2020 2020 3e20 6060  t --cov.    > ``
+00002270: 600a 2020 2020 3e0a 2020 2020 3e20 6060  `.    >.    > ``
+00002280: 6060 6060 7b74 6970 7d0a 2020 2020 3e20  ````{tip}.    > 
+00002290: 5275 6e6e 696e 6720 7061 7274 7320 6f66  Running parts of
+000022a0: 2074 6865 2074 6573 7420 7375 6974 650a   the test suite.
+000022b0: 2020 2020 3e0a 2020 2020 3e20 546f 2072      >.    > To r
+000022c0: 756e 206f 6e6c 7920 7061 7274 7320 6f66  un only parts of
+000022d0: 2074 6865 2074 6573 7420 7375 6974 652c   the test suite,
+000022e0: 2073 7065 6369 6679 2074 6865 2066 6f6c   specify the fol
+000022f0: 6465 7220 696e 2077 6869 6368 2074 6f20  der in which to 
+00002300: 6c6f 6f6b 2066 6f72 0a20 2020 203e 2074  look for.    > t
+00002310: 6573 7473 2061 7320 616e 2061 7267 756d  ests as an argum
+00002320: 656e 7420 746f 2070 7974 6573 742e 2054  ent to pytest. T
+00002330: 6865 2066 6f6c 6c6f 7769 6e67 2065 7861  he following exa
+00002340: 6d70 6c65 0a20 2020 203e 0a20 2020 203e  mple.    >.    >
+00002350: 2060 6060 0a20 2020 203e 2024 2070 792e   ```.    > $ py.
+00002360: 7465 7374 2074 6573 7473 2f6d 6561 7375  test tests/measu
+00002370: 7265 6d65 6e74 202d 2d63 6f76 2071 7561  rement --cov qua
+00002380: 6e74 6966 795f 636f 7265 2f6d 6561 7375  ntify_core/measu
+00002390: 7265 6d65 6e74 0a20 2020 203e 2060 6060  rement.    > ```
+000023a0: 0a20 2020 203e 0a20 2020 203e 2077 696c  .    >.    > wil
+000023b0: 6c20 6c6f 6f6b 2066 6f72 2074 6573 7473  l look for tests
+000023c0: 206c 6f63 6174 6564 2069 6e20 7468 6520   located in the 
+000023d0: 7465 7374 732f 6d65 6173 7572 656d 656e  tests/measuremen
+000023e0: 7420 6469 7265 6374 6f72 7920 616e 6420  t directory and 
+000023f0: 7265 706f 7274 2074 6573 7420 636f 7665  report test cove
+00002400: 7261 6765 206f 6620 7468 6520 7175 616e  rage of the quan
+00002410: 7469 6679 5f63 6f72 652f 6d65 6173 7572  tify_core/measur
+00002420: 656d 656e 7420 6d6f 6475 6c65 2e0a 2020  ement module..  
+00002430: 2020 3e20 6060 6060 6060 0a20 2020 203e    > ``````.    >
+00002440: 0a20 2020 203e 2060 6060 6060 607b 7469  .    > ``````{ti
+00002450: 707d 0a20 2020 203e 2053 7065 6564 2075  p}.    > Speed u
+00002460: 7020 7465 7374 7320 7769 7468 2070 6172  p tests with par
+00002470: 616c 6c65 6c20 6578 6563 7574 696f 6e0a  allel execution.
+00002480: 2020 2020 3e0a 2020 2020 3e20 6060 600a      >.    > ```.
+00002490: 2020 2020 3e20 2420 7079 2e74 6573 7420      > $ py.test 
+000024a0: 2d6e 2032 2023 2077 6865 7265 2032 2069  -n 2 # where 2 i
+000024b0: 7320 7468 6520 6e75 6d62 6572 206f 6620  s the number of 
+000024c0: 636f 7265 7320 6f66 2079 6f75 7220 4350  cores of your CP
+000024d0: 550a 2020 2020 3e20 6060 600a 2020 2020  U.    > ```.    
+000024e0: 3e20 6060 6060 6060 0a0a 3038 2e20 4275  > ``````..08. Bu
+000024f0: 696c 6469 6e67 2074 6865 2064 6f63 756d  ilding the docum
+00002500: 656e 7461 7469 6f6e 0a0a 2020 2020 3e20  entation..    > 
+00002510: 4966 2079 6f75 2068 6176 6520 776f 726b  If you have work
+00002520: 6564 206f 6e20 646f 6375 6d65 6e74 6174  ed on documentat
+00002530: 696f 6e20 6f72 205b 646f 6373 7472 696e  ion or [docstrin
+00002540: 6773 5d28 6874 7470 733a 2f2f 7777 772e  gs](https://www.
+00002550: 7079 7468 6f6e 2e6f 7267 2f64 6576 2f70  python.org/dev/p
+00002560: 6570 732f 7065 702d 3032 3537 2f29 2079  eps/pep-0257/) y
+00002570: 6f75 206e 6565 6420 746f 2072 6576 6965  ou need to revie
+00002580: 7720 686f 7720 796f 7572 2064 6f63 7320  w how your docs 
+00002590: 6c6f 6f6b 206c 6f63 616c 6c79 2061 6e64  look locally and
+000025a0: 2065 6e73 7572 6520 2a6e 6f20 6572 726f   ensure *no erro
+000025b0: 7220 6f72 2077 6172 6e69 6e67 7320 6172  r or warnings ar
+000025c0: 6520 7261 6973 6564 2a2e 0a20 2020 203e  e raised*..    >
+000025d0: 2059 6f75 2063 616e 2062 7569 6c64 2074   You can build t
+000025e0: 6865 2064 6f63 7320 6c6f 6361 6c6c 7920  he docs locally 
+000025f0: 7573 696e 673a 0a20 2020 203e 0a20 2020  using:.    >.   
+00002600: 203e 2060 6060 0a20 2020 203e 2024 2063   > ```.    > $ c
+00002610: 6420 646f 6373 0a20 2020 203e 0a20 2020  d docs.    >.   
+00002620: 203e 2024 2023 2075 6e69 780a 2020 2020   > $ # unix.    
+00002630: 3e20 2420 6d61 6b65 2068 746d 6c0a 2020  > $ make html.  
+00002640: 2020 3e0a 2020 2020 3e20 2420 2320 7769    >.    > $ # wi
+00002650: 6e64 6f77 730a 2020 2020 3e20 2420 2e2f  ndows.    > $ ./
+00002660: 6d61 6b65 2e62 6174 2068 746d 6c0a 2020  make.bat html.  
+00002670: 2020 3e20 6060 600a 2020 2020 3e0a 2020    > ```.    >.  
+00002680: 2020 3e20 5468 6520 646f 6373 2077 696c    > The docs wil
+00002690: 6c20 6265 206c 6f63 6174 6564 2069 6e20  l be located in 
+000026a0: 6071 7561 6e74 6966 795f 636f 7265 2f64  `quantify_core/d
+000026b0: 6f63 732f 5f62 7569 6c64 602e 0a20 2020  ocs/_build`..   
+000026c0: 203e 0a20 2020 203e 2060 6060 6060 607b   >.    > ``````{
+000026d0: 7469 707d 0a20 2020 203e 2049 6620 796f  tip}.    > If yo
+000026e0: 7520 6172 6520 776f 726b 696e 6720 6f6e  u are working on
+000026f0: 2064 6f63 756d 656e 7461 7469 6f6e 2069   documentation i
+00002700: 7420 6361 6e20 6265 2075 7365 6675 6c20  t can be useful 
+00002710: 746f 2061 7574 6f6d 6174 6963 616c 6c79  to automatically
+00002720: 2072 6562 7569 6c64 2074 6865 2064 6f63   rebuild the doc
+00002730: 7320 6166 7465 7220 6576 6572 7920 6368  s after every ch
+00002740: 616e 6765 2e0a 2020 2020 3e20 5468 6973  ange..    > This
+00002750: 2063 616e 2062 6520 646f 6e65 2075 7369   can be done usi
+00002760: 6e67 2074 6865 2060 7370 6869 6e78 2d61  ng the `sphinx-a
+00002770: 7574 6f62 7569 6c64 6020 7061 636b 6167  utobuild` packag
+00002780: 652e 2054 6872 6f75 6768 2074 6865 2066  e. Through the f
+00002790: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+000027a0: 3a0a 2020 2020 3e0a 2020 2020 3e20 6060  :.    >.    > ``
+000027b0: 600a 2020 2020 3e20 2420 7370 6869 6e78  `.    > $ sphinx
+000027c0: 2d61 7574 6f62 7569 6c64 2064 6f63 7320  -autobuild docs 
+000027d0: 646f 6373 2f5f 6275 696c 642f 6874 6d6c  docs/_build/html
+000027e0: 0a20 2020 203e 2060 6060 0a20 2020 203e  .    > ```.    >
+000027f0: 0a20 2020 203e 2054 6865 2064 6f63 756d  .    > The docum
+00002800: 656e 7461 7469 6f6e 2077 696c 6c20 7468  entation will th
+00002810: 656e 2062 6520 686f 7374 6564 206f 6e20  en be hosted on 
+00002820: 606c 6f63 616c 686f 7374 3a38 3030 3060  `localhost:8000`
+00002830: 0a20 2020 203e 2060 6060 6060 600a 2020  .    > ``````.  
+00002840: 2020 3e0a 2020 2020 3e20 6060 607b 7469    >.    > ```{ti
+00002850: 707d 0a20 2020 203e 2042 7569 6c64 696e  p}.    > Buildin
+00002860: 6720 7468 6520 7475 746f 7269 616c 7320  g the tutorials 
+00002870: 6361 6e20 6265 2074 696d 6520 636f 6e73  can be time cons
+00002880: 756d 696e 672c 2069 6620 796f 7520 6172  uming, if you ar
+00002890: 6520 6e6f 7420 6564 6974 696e 6720 7468  e not editing th
+000028a0: 656d 2c20 6665 656c 2066 7265 6520 746f  em, feel free to
+000028b0: 2064 656c 6574 6520 796f 7572 206c 6f63   delete your loc
+000028c0: 616c 2063 6f70 7920 6f66 2074 6865 2060  al copy of the `
+000028d0: 7175 616e 7469 6679 2d63 6f72 652f 646f  quantify-core/do
+000028e0: 6373 2f74 7574 6f72 6961 6c73 6020 746f  cs/tutorials` to
+000028f0: 2073 6b69 7020 7468 6569 7220 6275 696c   skip their buil
+00002900: 642e 2059 6f75 2063 616e 2072 6563 6f76  d. You can recov
+00002910: 6572 2074 6865 2066 696c 6573 2075 7369  er the files usi
+00002920: 6e67 2067 6974 2028 646f 206e 6f74 2063  ng git (do not c
+00002930: 6f6d 6d69 7420 7468 6520 6465 6c65 7465  ommit the delete
+00002940: 6420 6669 6c65 7329 2e0a 2020 2020 3e20  d files)..    > 
+00002950: 6060 600a 0a30 392e 2043 6f6d 6d69 7420  ```..09. Commit 
+00002960: 796f 7572 2063 6861 6e67 6573 2061 6e64  your changes and
+00002970: 2070 7573 6820 796f 7572 2062 7261 6e63   push your branc
+00002980: 6820 746f 2047 6974 4c61 623a 0a0a 2020  h to GitLab:..  
+00002990: 2020 6060 600a 2020 2020 2420 6769 7420    ```.    $ git 
+000029a0: 6164 6420 2e0a 2020 2020 2420 6769 7420  add ..    $ git 
+000029b0: 636f 6d6d 6974 202d 6d20 2259 6f75 7220  commit -m "Your 
+000029c0: 6465 7461 696c 6564 2064 6573 6372 6970  detailed descrip
+000029d0: 7469 6f6e 206f 6620 796f 7572 2063 6861  tion of your cha
+000029e0: 6e67 6573 2e22 0a20 2020 2024 2067 6974  nges.".    $ git
+000029f0: 2070 7573 6820 6f72 6967 696e 206e 616d   push origin nam
+00002a00: 652d 6f66 2d79 6f75 722d 6275 6766 6978  e-of-your-bugfix
+00002a10: 2d6f 722d 6665 6174 7572 650a 2020 2020  -or-feature.    
+00002a20: 6060 600a 0a31 302e 2052 6576 6965 7720  ```..10. Review 
+00002a30: 7468 6520 7b72 6566 7d60 4d65 7267 6520  the {ref}`Merge 
+00002a40: 5265 7175 6573 7420 4775 6964 656c 696e  Request Guidelin
+00002a50: 6573 6020 616e 6420 7375 626d 6974 2061  es` and submit a
+00002a60: 206d 6572 6765 2072 6571 7565 7374 2074   merge request t
+00002a70: 6872 6f75 6768 2074 6865 2047 6974 4c61  hrough the GitLa
+00002a80: 6220 7765 6273 6974 652e 0a0a 3131 2e20  b website...11. 
+00002a90: 4164 6420 6120 7368 6f72 7420 656e 7472  Add a short entr
+00002aa0: 7920 696e 2074 6865 2060 4348 414e 4745  y in the `CHANGE
+00002ab0: 4c4f 472e 6d64 6020 756e 6465 7220 6055  LOG.md` under `U
+00002ac0: 6e72 656c 6561 7365 6460 2c20 636f 6d6d  nreleased`, comm
+00002ad0: 6974 2061 6e64 2070 7573 682e 0a0a 2323  it and push...##
+00002ae0: 2054 726f 7562 6c65 7368 6f6f 7469 6e67   Troubleshooting
+00002af0: 0a0a 4966 2066 6f72 2073 6f6d 6520 7265  ..If for some re
+00002b00: 6173 6f6e 2079 6f75 2061 7265 206e 6f74  ason you are not
+00002b10: 2061 626c 6520 746f 2069 6e73 7461 6c6c   able to install
+00002b20: 206f 7220 7573 6520 5175 616e 7469 6679   or use Quantify
+00002b30: 2075 7369 6e67 2074 6865 2070 7265 7363   using the presc
+00002b40: 7269 6265 6420 7761 7973 2069 6e64 6963  ribed ways indic
+00002b50: 6174 6564 2061 626f 7665 2c20 6d61 6b65  ated above, make
+00002b60: 2073 7572 6520 796f 7520 6861 7665 2061   sure you have a
+00002b70: 2077 6f72 6b69 6e67 2050 7974 686f 6e20   working Python 
+00002b80: 656e 7669 726f 6e6d 656e 7420 2865 2e67  environment (e.g
+00002b90: 2e20 796f 7520 6361 6e20 7275 6e20 616e  . you can run an
+00002ba0: 2060 4950 7974 686f 6e60 2074 6572 6d69   `IPython` termi
+00002bb0: 6e61 6c29 2e20 466f 6c6c 6f77 2074 6865  nal). Follow the
+00002bc0: 206e 6578 7420 7374 6570 7320 7468 6174   next steps that
+00002bd0: 2061 696d 2061 7420 696e 7374 616c 6c69   aim at installi
+00002be0: 6e67 2051 7561 6e74 6966 7920 6672 6f6d  ng Quantify from
+00002bf0: 2073 6f75 7263 6520 616e 6420 7275 6e6e   source and runn
+00002c00: 696e 6720 6974 7320 7465 7374 732e 0a0a  ing its tests...
+00002c10: 302e 2055 6e69 6e73 7461 6c6c 207b 6d6f  0. Uninstall {mo
+00002c20: 647d 6071 7561 6e74 6966 792d 636f 7265  d}`quantify-core
+00002c30: 603a 0a0a 2020 2060 6060 0a20 2020 2420  `:..   ```.   $ 
+00002c40: 7069 7020 756e 696e 7374 616c 6c20 7175  pip uninstall qu
+00002c50: 616e 7469 6679 2d63 6f72 650a 2020 2060  antify-core.   `
+00002c60: 6060 0a0a 312e 2049 6e73 7461 6c6c 2066  ``..1. Install f
+00002c70: 726f 6d20 736f 7572 6365 2028 7275 6e20  rom source (run 
+00002c80: 6c69 6e65 2062 7920 6c69 6e65 293a 0a0a  line by line):..
+00002c90: 2020 2060 6060 0a20 2020 2420 6769 7420     ```.   $ git 
+00002ca0: 636c 6f6e 6520 6874 7470 733a 2f2f 6769  clone https://gi
+00002cb0: 746c 6162 2e63 6f6d 2f71 7561 6e74 6966  tlab.com/quantif
+00002cc0: 792d 6f73 2f71 7561 6e74 6966 792d 636f  y-os/quantify-co
+00002cd0: 7265 2e67 6974 3b20 6364 2071 7561 6e74  re.git; cd quant
+00002ce0: 6966 792d 636f 7265 0a20 2020 2420 7069  ify-core.   $ pi
+00002cf0: 7020 696e 7374 616c 6c20 2d2d 7570 6772  p install --upgr
+00002d00: 6164 6520 2d2d 7570 6772 6164 652d 7374  ade --upgrade-st
+00002d10: 7261 7465 6779 2065 6167 6572 2022 2e5b  rategy eager ".[
+00002d20: 6465 765d 220a 2020 2024 2070 7974 6573  dev]".   $ pytes
+00002d30: 7420 2d76 0a20 2020 6060 600a 0a32 2e20  t -v.   ```..2. 
+00002d40: 5468 6520 7465 7374 7320 7769 6c6c 2065  The tests will e
+00002d50: 6974 6865 7220 7061 7373 206f 7220 6e6f  ither pass or no
+00002d60: 742e 2049 6e20 616e 7920 6361 7365 2c20  t. In any case, 
+00002d70: 706c 6561 7365 2072 6570 6f72 7420 796f  please report yo
+00002d80: 7572 2065 7870 6572 6965 6e63 6520 616e  ur experience an
+00002d90: 6420 7768 6963 6820 7465 7374 2064 6f20  d which test do 
+00002da0: 6e6f 7420 7061 7373 2062 7920 6372 6561  not pass by crea
+00002db0: 7469 6e67 2061 2060 4e65 7720 6973 7375  ting a `New issu
+00002dc0: 6560 206f 6e20 7468 6520 5b69 7373 7565  e` on the [issue
+00002dd0: 2074 7261 636b 6572 5d28 6874 7470 733a   tracker](https:
+00002de0: 2f2f 6769 746c 6162 2e63 6f6d 2f71 7561  //gitlab.com/qua
+00002df0: 6e74 6966 792d 6f73 2f71 7561 6e74 6966  ntify-os/quantif
+00002e00: 792d 636f 7265 2f2d 2f69 7373 7565 7329  y-core/-/issues)
+00002e10: 2c20 796f 7572 2065 6666 6f72 7473 2061  , your efforts a
+00002e20: 7265 206d 7563 6820 6170 7072 6563 6961  re much apprecia
+00002e30: 7465 6420 616e 6420 7769 6c6c 2068 656c  ted and will hel
+00002e40: 7020 7573 2074 6f20 756e 6465 7273 7461  p us to understa
+00002e50: 6e64 2074 6865 2070 726f 626c 656d 7320  nd the problems 
+00002e60: 796f 7520 6d69 6768 7420 6265 2066 6163  you might be fac
+00002e70: 696e 672e 0a0a 2323 2320 446f 776e 6772  ing...### Downgr
+00002e80: 6164 6520 746f 2061 2073 7065 6369 6669  ade to a specifi
+00002e90: 6320 7665 7273 696f 6e0a 0a49 6620 666f  c version..If fo
+00002ea0: 7220 616e 7920 7265 6173 6f6e 2079 6f75  r any reason you
+00002eb0: 2072 6571 7569 7265 2061 2073 7065 6369   require a speci
+00002ec0: 6669 6320 7665 7273 696f 6e20 6f66 2074  fic version of t
+00002ed0: 6865 2070 6163 6b61 6765 2c20 652e 672e  he package, e.g.
+00002ee0: 2030 2e33 2e30 2c20 7275 6e3a 0a0a 6060   0.3.0, run:..``
+00002ef0: 600a 2420 7069 7020 696e 7374 616c 6c20  `.$ pip install 
+00002f00: 2d2d 7570 6772 6164 6520 7175 616e 7469  --upgrade quanti
+00002f10: 6679 2d63 6f72 653d 3d30 2e33 2e30 0a60  fy-core==0.3.0.`
+00002f20: 6060 0a0a 2323 2320 506f 7465 6e74 6961  ``..### Potentia
+00002f30: 6c20 6973 7375 6573 3a20 5079 5174 4772  l issues: PyQtGr
+00002f40: 6170 6820 616e 6420 5079 5174 350a 0a7b  aph and PyQt5..{
+00002f50: 6d6f 647d 6071 7561 6e74 6966 792d 636f  mod}`quantify-co
+00002f60: 7265 6020 6861 7320 6120 6465 7065 6e64  re` has a depend
+00002f70: 656e 6379 206f 6e20 7468 6520 6050 7951  ency on the `PyQ
+00002f80: 7435 6020 7061 636b 6167 652c 2077 6869  t5` package, whi
+00002f90: 6368 2069 7473 656c 6620 6861 7320 6120  ch itself has a 
+00002fa0: 6465 7065 6e64 656e 6379 206f 6e20 7468  dependency on th
+00002fb0: 6520 6051 7435 6020 7275 6e74 696d 652e  e `Qt5` runtime.
+00002fc0: 0a4f 6e20 6d6f 7374 2073 7973 7465 6d73  .On most systems
+00002fd0: 2c20 7468 6520 7374 616e 6461 7264 2069  , the standard i
+00002fe0: 6e73 7461 6c6c 6174 696f 6e20 7072 6f63  nstallation proc
+00002ff0: 6573 7320 7769 6c6c 2063 6f72 7265 6374  ess will correct
+00003000: 6c79 2069 6e73 7461 6c6c 2051 742e 0a54  ly install Qt..T
+00003010: 6865 2041 6e61 636f 6e64 6120 696e 7374  he Anaconda inst
+00003020: 616c 6c61 7469 6f6e 2073 686f 756c 6420  allation should 
+00003030: 7265 736f 6c76 6520 6973 7375 6573 2077  resolve issues w
+00003040: 6974 6820 696e 7374 616c 6c61 7469 6f6e  ith installation
+00003050: 206f 6e20 5769 6e64 6f77 7320 6f72 206d   on Windows or m
+00003060: 6163 4f53 2e0a 596f 7520 6d61 7920 6e65  acOS..You may ne
+00003070: 6564 2074 6f20 636f 6e73 756c 7420 6120  ed to consult a 
+00003080: 7365 6172 6368 2065 6e67 696e 6520 6966  search engine if
+00003090: 2079 6f75 2068 6176 6520 6120 6d6f 7265   you have a more
+000030a0: 2065 786f 7469 6320 7379 7374 656d 2e0a   exotic system..
+000030b0: 0a5b 7069 705d 3a20 6874 7470 733a 2f2f  .[pip]: https://
+000030c0: 7069 702e 7079 7061 2e69 6f0a 5b70 7974  pip.pypa.io.[pyt
+000030d0: 686f 6e20 696e 7374 616c 6c61 7469 6f6e  hon installation
+000030e0: 2067 7569 6465 5d3a 2068 7474 703a 2f2f   guide]: http://
+000030f0: 646f 6373 2e70 7974 686f 6e2d 6775 6964  docs.python-guid
+00003100: 652e 6f72 672f 656e 2f6c 6174 6573 742f  e.org/en/latest/
+00003110: 7374 6172 7469 6e67 2f69 6e73 7461 6c6c  starting/install
+00003120: 6174 696f 6e2f 0a                        ation/.
```

### Comparing `quantify-core-0.7.1/docs/make.bat` & `quantify-core-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/technical_notes/dataset_design/Quantify dataset - advanced examples.md` & `quantify-core-0.7.2/docs/technical_notes/dataset_design/Quantify dataset - advanced examples.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/technical_notes/dataset_design/Quantify dataset - examples.md` & `quantify-core-0.7.2/docs/technical_notes/dataset_design/Quantify dataset - examples.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/technical_notes/dataset_design/Quantify dataset - specification.md` & `quantify-core-0.7.2/docs/technical_notes/dataset_design/Quantify dataset - specification.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/technical_notes/dataset_design/Xarray introduction.md` & `quantify-core-0.7.2/docs/technical_notes/dataset_design/Xarray introduction.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/technical_notes/dataset_design/index.md` & `quantify-core-0.7.2/docs/technical_notes/dataset_design/index.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/tutorials/Tutorial 1. Controlling a basic experiment using MeasurementControl.md` & `quantify-core-0.7.2/docs/tutorials/Tutorial 1. Controlling a basic experiment using MeasurementControl.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/tutorials/Tutorial 2. Advanced capabilities of the MeasurementControl.md` & `quantify-core-0.7.2/docs/tutorials/Tutorial 2. Advanced capabilities of the MeasurementControl.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/tutorials/Tutorial 3. Building custom analyses - the data analysis framework.md` & `quantify-core-0.7.2/docs/tutorials/Tutorial 3. Building custom analyses - the data analysis framework.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/tutorials/Tutorial 4. Adaptive Measurements.md` & `quantify-core-0.7.2/docs/tutorials/Tutorial 4. Adaptive Measurements.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/tutorials/Tutorial 5. Plot monitor.md` & `quantify-core-0.7.2/docs/tutorials/Tutorial 5. Plot monitor.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/docs/usage.md` & `quantify-core-0.7.2/docs/usage.md`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/pyproject.toml` & `quantify-core-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 ]
 license = { text = "BSD-3-Clause" }
 dynamic = ["version", "readme"]
 requires-python = ">=3.8"
 dependencies = [
     "numpy !=1.19.4",  # 1.19.4 not allowed because of a bug on windows https://github.com/numpy/numpy/issues/17726
     "qcodes >=0.37.0", # 0.37.0 replaces deprecated pyqtgraph functionality
+    "qcodes-loop",
     "scipy >=1.5.0, !=1.6.0",
     "h5netcdf",
     "xarray >=0.19.0",
     "matplotlib !=3.5.0",
     "lmfit >=1.0.3", # Bugfix for lmfit (https://github.com/lmfit/lmfit-py/pull/758)
     "pyqt5 >5.15.2",  # 5.15.2 has known bug, #170, https://bugreports.qt.io/browse/PYSIDE-1473
     "pyqtgraph",
```

### Comparing `quantify-core-0.7.1/quantify_core/_version.py` & `quantify-core-0.7.2/quantify_core/_version.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/analysis/__init__.py` & `quantify-core-0.7.2/quantify_core/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/analysis/base_analysis.py` & `quantify-core-0.7.2/quantify_core/analysis/base_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,18 +132,18 @@
 
     def __new__(cls, name, bases, namespace, /, **kwargs) -> AnalysisMeta:
         if "create_figures" in namespace.keys():
             namespace = dict(namespace)
             create_figures_orig = namespace.pop("create_figures")
 
             @wraps(create_figures_orig)
-            def create_figures_patched(self):
+            def create_figures_patched(self, *args, **kwargs):
                 self._analyses_figures_cache().initialized = True
                 self._creating_figures = True
-                create_figures_orig(self)
+                create_figures_orig(self, *args, **kwargs)
                 self._creating_figures = False
 
             def _figs_axs_mpl(self):
                 cache = self._analyses_figures_cache()
                 if not cache.initialized and not self._creating_figures:
                     create_figures_patched(self)
                 return cache
```

### Comparing `quantify-core-0.7.1/quantify_core/analysis/calibration.py` & `quantify-core-0.7.2/quantify_core/analysis/calibration.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/analysis/cosine_analysis.py` & `quantify-core-0.7.2/quantify_core/analysis/cosine_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/analysis/fitting_models.py` & `quantify-core-0.7.2/quantify_core/analysis/fitting_models.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/analysis/interpolation_analysis.py` & `quantify-core-0.7.2/quantify_core/analysis/interpolation_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/analysis/optimization_analysis.py` & `quantify-core-0.7.2/quantify_core/analysis/optimization_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/analysis/schemas/AnalysisSettings.json` & `quantify-core-0.7.2/quantify_core/analysis/schemas/AnalysisSettings.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/analysis/single_qubit_timedomain.py` & `quantify-core-0.7.2/quantify_core/analysis/single_qubit_timedomain.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/analysis/spectroscopy_analysis.py` & `quantify-core-0.7.2/quantify_core/analysis/spectroscopy_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/analysis/types.py` & `quantify-core-0.7.2/quantify_core/analysis/types.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/data/dataset_adapters.py` & `quantify-core-0.7.2/quantify_core/data/dataset_adapters.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/data/dataset_attrs.py` & `quantify-core-0.7.2/quantify_core/data/dataset_attrs.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/data/experiment.py` & `quantify-core-0.7.2/quantify_core/data/experiment.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/data/handling.py` & `quantify-core-0.7.2/quantify_core/data/handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,17 @@
     FileNotFoundError
         No data found for specified date.
     """
     with open(_locate_experiment_file(tuid, datadir, file)) as snap:
         return json.load(snap, cls=dh.DecodeToNumpy, list_to_ndarray=list_to_ndarray)
 
 
-def create_exp_folder(tuid: TUID, name: str = "", datadir: str = None) -> str:
+def create_exp_folder(
+    tuid: TUID, name: str | None = None, datadir: str | None = None
+) -> str:
     """
     Creates an empty folder to store an experiment container.
 
     If the folder already exists, simply returns the experiment folder corresponding to
     the :class:`~quantify_core.data.types.TUID`.
 
     Parameters
@@ -461,15 +463,15 @@
         ``/datadir/YYYYmmDD/YYYYmmDD-HHMMSS-sss-******-name/``.
     """
     TUID.is_valid(tuid)
 
     if datadir is None:
         datadir = get_datadir()
     exp_folder = os.path.join(datadir, tuid[:8], tuid)
-    if name != "":
+    if name:
         exp_folder += "-" + name
 
     os.makedirs(exp_folder, exist_ok=True)
     return exp_folder
 
 
 # pylint: disable=too-many-locals
```

### Comparing `quantify-core-0.7.1/quantify_core/data/types.py` & `quantify-core-0.7.2/quantify_core/data/types.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/measurement/__init__.py` & `quantify-core-0.7.2/quantify_core/measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/measurement/control.py` & `quantify-core-0.7.2/quantify_core/measurement/control.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/measurement/gettables.py` & `quantify-core-0.7.2/quantify_core/measurement/gettables.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/measurement/schemas/Gettable.json` & `quantify-core-0.7.2/quantify_core/measurement/schemas/Gettable.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/measurement/schemas/Settable.json` & `quantify-core-0.7.2/quantify_core/measurement/schemas/Settable.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/measurement/types.py` & `quantify-core-0.7.2/quantify_core/measurement/types.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/utilities/_docs_helpers.py` & `quantify-core-0.7.2/quantify_core/utilities/_docs_helpers.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/utilities/_tests_helpers.py` & `quantify-core-0.7.2/quantify_core/utilities/_tests_helpers.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/utilities/dataset_examples.py` & `quantify-core-0.7.2/quantify_core/utilities/dataset_examples.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/utilities/deprecation.py` & `quantify-core-0.7.2/quantify_core/utilities/deprecation.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/utilities/examples_support.py` & `quantify-core-0.7.2/quantify_core/utilities/examples_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,10 +404,10 @@
     return attrs
 
 
 def round_trip_dataset(dataset: xr.Dataset) -> xr.Dataset:
     """Writes a dataset to disk and loads it back returning it."""
 
     tuid = dataset.tuid
-    assert tuid != ""
+    assert tuid
     dh.write_dataset(Path(dh.create_exp_folder(tuid)) / dh.DATASET_NAME, dataset)
     return dh.load_dataset(tuid)
```

### Comparing `quantify-core-0.7.1/quantify_core/utilities/experiment_helpers.py` & `quantify-core-0.7.2/quantify_core/utilities/experiment_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Repository: https://gitlab.com/quantify-os/quantify-core
 # Licensed according to the LICENCE file on the main branch
 """Helpers for performing experiments."""
+from __future__ import annotations
 import warnings
 from typing import Any, Optional, Union, Dict, List, Literal
 
 import numpy as np
 from qcodes.instrument import Instrument, InstrumentChannel
 from qcodes.parameters import Parameter
 
@@ -12,15 +13,15 @@
 from quantify_core.data.types import TUID
 from quantify_core.visualization.pyqt_plotmon import PlotMonitor_pyqt
 
 
 # pylint: disable=broad-except
 def load_settings_onto_instrument(
     instrument: Union[Instrument, InstrumentChannel, Parameter],
-    tuid: TUID = None,
+    tuid: TUID | None = None,
     datadir: str = None,
     exception_handling: Literal["raise", "warn"] = "raise",
 ) -> None:
     """
     Loads settings from a previous experiment onto a current
     :class:`~qcodes.instrument.Instrument`, or any of its submodules or
     parameters. This information is loaded from the 'snapshot.json' file in
@@ -53,14 +54,15 @@
         "instruments"
     ]
 
     def _try_to_set_par_safe(
         instr_mod: Union[Instrument, InstrumentChannel],
         parname: str,
         value: Any,
+        value_np: Any,
     ):
         """Tries to set a parameter and emits a warning if not successful."""
         # do not try to set parameters that are not settable
         if not "set" in dir(instr_mod.parameters[parname]):
             return
         # do not set to None if value is already None. If there is a runtime
         # error when getting the parameter, do not try to set the parameter.
@@ -75,15 +77,18 @@
             )
             return
         if get_val is None and value is None:
             return
 
         # Make sure the parameter is actually a settable
         try:
-            instr_mod.set(parname, value)
+            if isinstance(get_val, np.ndarray):
+                instr_mod.set(parname, value_np)
+            else:
+                instr_mod.set(parname, value)
         except (RuntimeError, KeyError, ValueError, TypeError) as exc:
             warnings.warn(
                 f'Parameter "{parname}" of "{instr_mod.name}" '
                 f'could not be set to "{value}" due to error:\n{exc}'
             )
 
     parents = get_all_parents(instrument)
@@ -112,17 +117,16 @@
         if isinstance(parent, Parameter):
             if parent.name not in instr_mod_snap["parameters"]:
                 address = ".".join([p._short_name for p in parents])
                 raise ValueError(
                     f'Parameter "{address}" not found in snapshot {datadir}:{tuid}'
                 )
             value = instr_mod_snap["parameters"][parent.name]["value"]
-            if isinstance(parent(), np.ndarray):
-                value = instr_mod_snap_numpy_array["parameters"][parent.name]["value"]
-            _try_to_set_par_safe(parents[-2], parent.name, value)
+            value_np = instr_mod_snap_numpy_array["parameters"][parent.name]["value"]
+            _try_to_set_par_safe(parents[-2], parent.name, value, value_np)
             return
 
     def _set_params_instr_mod(
         instr_mod_snap: Dict,
         instr_mod_snap_np: Dict,
         instr_mod: Union[Instrument, InstrumentChannel],
     ):
@@ -130,29 +134,16 @@
         private function to set parameters and recursively set parameters of submodules.
         """
         # iterate over top-level parameters
         for parname, par in instr_mod_snap["parameters"].items():
             # Check that the parameter exists in this instrument
             if parname in instr_mod.parameters:
                 value = par["value"]
-                # If we get a runtime error when getting the parameter, don't try to
-                # set the parameter
-                try:
-                    get_val = instr_mod.parameters[parname]()
-                except Exception as exc:
-                    if exception_handling == "raise":
-                        raise exc
-                    warnings.warn(
-                        f"Could not get value of {parname} parameter due to '{exc}'. "
-                        "We will not try to set this parameter."
-                    )
-                    continue
-                if isinstance(get_val, np.ndarray):
-                    value = instr_mod_snap_np["parameters"][parname]["value"]
-                _try_to_set_par_safe(instr_mod, parname, value)
+                value_np = instr_mod_snap_np["parameters"][parname]["value"]
+                _try_to_set_par_safe(instr_mod, parname, value, value_np)
             else:
                 warnings.warn(
                     f"Could not set parameter {parname} in {instr_mod.name}. "
                     f"{instr_mod.name} does not possess a parameter named {parname}."
                 )
         # recursively call this function for all submodules
         if "submodules" in instr_mod_snap.keys():
```

### Comparing `quantify-core-0.7.1/quantify_core/utilities/general.py` & `quantify-core-0.7.2/quantify_core/utilities/general.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/utilities/inspect_utils.py` & `quantify-core-0.7.2/quantify_core/utilities/inspect_utils.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/visualization/SI_utilities.py` & `quantify-core-0.7.2/quantify_core/visualization/SI_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Repository: https://gitlab.com/quantify-os/quantify-core
 # Licensed according to the LICENCE file on the main branch
 # pylint: disable=invalid-name  # disabled because of capital SI in module name
 """
 Utilities for managing SI units with plotting systems.
 """
+from __future__ import annotations
+
 import re
 import string
 from typing import Optional, Tuple, Union
 import warnings
 
 import lmfit
 import matplotlib
@@ -17,15 +19,17 @@
 
 golden_mean = (np.sqrt(5) - 1.0) / 2.0  # Aesthetic ratio
 single_col_figsize = (3.39, golden_mean * 3.39)
 double_col_figsize = (6.9, golden_mean * 6.9)
 thesis_col_figsize = (12.2 / 2.54, golden_mean * 12.2 / 2.54)
 
 
-def set_xlabel(label, unit=None, axis=None, **kw):
+def set_xlabel(
+    label: str | plt.Axes, unit: str | None = None, axis: plt.Axes | None = None, **kw
+):
     """
     Add a unit aware x-label to an axis object.
 
     Parameters
     ----------
     label
         the desired label
@@ -44,29 +48,31 @@
             stacklevel=2,
         )
         axis, label, unit = label, unit, axis
 
     if axis is None:
         axis = plt.gca()
 
-    if unit is not None and unit != "":
+    if unit:
         xticks = axis.get_xticks()
         scale_factor, unit = SI_prefix_and_scale_factor(val=max(abs(xticks)), unit=unit)
         formatter = matplotlib.ticker.FuncFormatter(
             lambda x, pos: f"{x * scale_factor:.4g}"
         )
 
         axis.xaxis.set_major_formatter(formatter)
         axis.set_xlabel(label + f" [{unit}]", **kw)
     else:
         axis.set_xlabel(label, **kw)
     return axis
 
 
-def set_ylabel(label, unit=None, axis=None, **kw):
+def set_ylabel(
+    label: str | plt.Axes, unit: str | None = None, axis: plt.Axes | None = None, **kw
+):
     """
     Add a unit aware y-label to an axis object.
 
     Parameters
     ----------
     label
         the desired label
@@ -85,45 +91,47 @@
             stacklevel=2,
         )
         axis, label, unit = label, unit, axis
 
     if axis is None:
         axis = plt.gca()
 
-    if unit is not None and unit != "":
+    if unit:
         yticks = axis.get_yticks()
         scale_factor, unit = SI_prefix_and_scale_factor(val=max(abs(yticks)), unit=unit)
         formatter = matplotlib.ticker.FuncFormatter(
             lambda x, pos: f"{x * scale_factor:.6g}"
         )
 
         axis.yaxis.set_major_formatter(formatter)
 
         axis.set_ylabel(label + f" [{unit}]", **kw)
     else:
         axis.set_ylabel(label, **kw)
     return axis
 
 
-def set_cbarlabel(cbar, label, unit=None, **kw):
+def set_cbarlabel(
+    cbar: matplotlib.colorbar.Colorbar, label: str, unit: str | None = None, **kw
+):
     """
     Add a unit aware z-label to a colorbar object
 
     Parameters
     ----------
     cbar
         colorbar object to set label on
     label
         the desired label
     unit
         the unit
     **kw
         keyword argument to be passed to cbar.set_label
     """
-    if unit is not None and unit != "":
+    if unit:
         zticks = cbar.get_ticks()
         scale_factor, unit = SI_prefix_and_scale_factor(val=max(abs(zticks)), unit=unit)
         formatter = matplotlib.ticker.FuncFormatter(
             lambda x, pos: f"{x * scale_factor:.6g}"
         )
         cbar.ax.yaxis.set_major_formatter(formatter)
         cbar.set_label(label + f" [{unit}]")
```

### Comparing `quantify-core-0.7.1/quantify_core/visualization/__init__.py` & `quantify-core-0.7.2/quantify_core/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/visualization/_appnope.py` & `quantify-core-0.7.2/quantify_core/visualization/_appnope.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/visualization/color_utilities.py` & `quantify-core-0.7.2/quantify_core/visualization/color_utilities.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/visualization/ins_mon_widget/qc_snapshot_widget.py` & `quantify-core-0.7.2/quantify_core/visualization/ins_mon_widget/qc_snapshot_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             Unit of parameter
 
         Returns
         -------
         :
             new value and new unit
         """
-        if unit is None or unit == "":
+        if not unit:
             if isinstance(value, Enum):
                 # For Enum, don't show class name
                 return value.name, ""
             return str(value), ""
         return SI_val_to_msg_str(value, unit)
 
     def _add_single_parameter(self, param_snap, param_name, node, node_key):
```

### Comparing `quantify-core-0.7.1/quantify_core/visualization/instrument_monitor.py` & `quantify-core-0.7.2/quantify_core/visualization/instrument_monitor.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/visualization/mpl_plotting.py` & `quantify-core-0.7.2/quantify_core/visualization/mpl_plotting.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/visualization/plot_interpolation.py` & `quantify-core-0.7.2/quantify_core/visualization/plot_interpolation.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/visualization/pyqt_plotmon.py` & `quantify-core-0.7.2/quantify_core/visualization/pyqt_plotmon.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core/visualization/pyqt_plotmon_remote.py` & `quantify-core-0.7.2/quantify_core/visualization/pyqt_plotmon_remote.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core.egg-info/PKG-INFO` & `quantify-core-0.7.2/quantify_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantify-core
-Version: 0.7.1
+Version: 0.7.2
 Summary: Quantify-core is a unified quantum computing, solid-state and pulse sequencing physical experimentation framework.
 Maintainer-email: Edgar Reehuis <ereehuis@qblox.com>, Robert Sokolewicz <rsokolewicz@qblox.com>, Tobias Bonsen <tobias@orangeqs.com>, Viacheslav Ostroukh <viacheslav@orangeqs.com>
 License: BSD-3-Clause
 Project-URL: Documentation, https://quantify-quantify-core.readthedocs-hosted.com
 Project-URL: Source, https://gitlab.com/quantify-os/quantify-core
 Project-URL: Issue tracker, https://gitlab.com/quantify-os/quantify-core/-/issues
 Project-URL: Changelog, https://gitlab.com/quantify-os/quantify-core/-/blob/main/CHANGELOG.md
@@ -46,15 +46,15 @@
 Quantify is a Python-based data acquisition framework focused on Quantum Computing and
 solid-state physics experiments.
 The framework consists of [quantify-core](https://pypi.org/project/quantify-core/) ([git repo](https://gitlab.com/quantify-os/quantify-core/))
 and [quantify-scheduler](https://pypi.org/project/quantify-scheduler/) ([git repo](https://gitlab.com/quantify-os/quantify-scheduler/)).
 It is built on top of [QCoDeS](https://qcodes.github.io/Qcodes/)
 and is a spiritual successor of [PycQED](https://github.com/DiCarloLab-Delft/PycQED_py3).
 
-Quantify-core is the core module that contains all basic functionality to control experiments. This includes:
+`quantify-core` is the core module that contains all basic functionality to control experiments. This includes:
 
 - A framework to control instruments.
 - A data-acquisition loop.
 - Data storage and analysis.
 - Parameter monitoring and live visualization of experiments.
 
 Take a look at the [latest documentation for quantify-core](https://quantify-quantify-core.readthedocs-hosted.com/)
```

### Comparing `quantify-core-0.7.1/quantify_core.egg-info/SOURCES.txt` & `quantify-core-0.7.2/quantify_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/quantify_core.egg-info/requires.txt` & `quantify-core-0.7.2/quantify_core.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 numpy!=1.19.4
 qcodes>=0.37.0
+qcodes-loop
 scipy!=1.6.0,>=1.5.0
 h5netcdf
 xarray>=0.19.0
 matplotlib!=3.5.0
 lmfit>=1.0.3
 pyqt5>5.15.2
 pyqtgraph
```

### Comparing `quantify-core-0.7.1/setup.py` & `quantify-core-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/analysis/test_base_analysis.py` & `quantify-core-0.7.2/tests/analysis/test_base_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/analysis/test_calibration.py` & `quantify-core-0.7.2/tests/analysis/test_calibration.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/analysis/test_fitting_models.py` & `quantify-core-0.7.2/tests/analysis/test_fitting_models.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/analysis/test_interpolation_analysis.py` & `quantify-core-0.7.2/tests/analysis/test_interpolation_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/analysis/test_optimization_analysis.py` & `quantify-core-0.7.2/tests/analysis/test_optimization_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/analysis/test_single_qubit_timedomain.py` & `quantify-core-0.7.2/tests/analysis/test_single_qubit_timedomain.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/analysis/test_spectroscopy_analysis.py` & `quantify-core-0.7.2/tests/analysis/test_spectroscopy_analysis.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/analysis/test_types.py` & `quantify-core-0.7.2/tests/analysis/test_types.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/data/test_data_handling.py` & `quantify-core-0.7.2/tests/data/test_data_handling.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/data/test_experiment.py` & `quantify-core-0.7.2/tests/data/test_experiment.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/data/test_types.py` & `quantify-core-0.7.2/tests/data/test_types.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/measurement/test_measurement_control.py` & `quantify-core-0.7.2/tests/measurement/test_measurement_control.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/measurement/test_types.py` & `quantify-core-0.7.2/tests/measurement/test_types.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20200430/20200430-170837-001-315f36-Cosine test/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20200430/20200430-170837-001-315f36-Cosine test/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20200504/20200504-191556-002-4209ee-2D Cosine test/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20200504/20200504-191556-002-4209ee-2D Cosine test/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20200814/20200814-134652-492-fbf254-save/snapshot.json` & `quantify-core-0.7.2/tests/test_data/20200814/20200814-134652-492-fbf254-save/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20201124/20201124-184709-137-8a5112-(0) Spec IF=0.000 MHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20201124/20201124-184709-137-8a5112-(0) Spec IF=0.000 MHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20201124/20201124-184716-237-918bee-(1) Spec IF=20.000 MHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20201124/20201124-184716-237-918bee-(1) Spec IF=20.000 MHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20201124/20201124-184722-988-0463d4-(2) Spec IF=-20.000 MHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20201124/20201124-184722-988-0463d4-(2) Spec IF=-20.000 MHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20201124/20201124-184729-618-85970f-(3) Spec IF=40.000 MHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20201124/20201124-184729-618-85970f-(3) Spec IF=40.000 MHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20201124/20201124-184736-341-3628d4-(4) Spec IF=-40.000 MHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20201124/20201124-184736-341-3628d4-(4) Spec IF=-40.000 MHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/snapshot.json` & `quantify-core-0.7.2/tests/test_data/20210118/20210118-202044-211-58ddb0-heterodyne_spectroscopy_mockDev/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/snapshot.json` & `quantify-core-0.7.2/tests/test_data/20210126/20210126-162726-170-de4f78-TWPA_pump_8.3300GHz_heterodyne_spectroscopy_mockDevmock-coarse/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210227/20210227-172939-723-53d82c-Resonator_power_id6_4.612GHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210227/20210227-172939-723-53d82c-Resonator_power_id6_4.612GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210227/20210227-174714-680-31df85-Resonator_id7_4.660GHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210227/20210227-174714-680-31df85-Resonator_id7_4.660GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210305/.DS_Store` & `quantify-core-0.7.2/tests/test_data/20210305/.DS_Store`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210305/20210305-152943-497-ad8670-Resonator_id2_4.483GHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210305/20210305-152943-497-ad8670-Resonator_id2_4.483GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210305/20210305-154735-413-142768-Resonator_id2_4.483GHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210305/20210305-154735-413-142768-Resonator_id2_4.483GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210305/20210305-160157-184-3c17e9-Resonator_id4_4.541GHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210305/20210305-160157-184-3c17e9-Resonator_id4_4.541GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210305/20210305-161550-671-982c6d-Resonator_id5_4.577GHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210305/20210305-161550-671-982c6d-Resonator_id5_4.577GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210319/20210319-094728-327-69b211-load_settings_test/snapshot.json` & `quantify-core-0.7.2/tests/test_data/20210319/20210319-094728-327-69b211-load_settings_test/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210322/20210322-205253-758-6689ca-T1 at 4.715GHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210322/20210322-205253-758-6689ca-T1 at 4.715GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210331/20210331-133734-718-aa9c83 AllXY q0/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210331/20210331-133734-718-aa9c83 AllXY q0/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210419/20210419-153127-883-fa4508-Rabi oscillation at 4.515GHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210419/20210419-153127-883-fa4508-Rabi oscillation at 4.515GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210419/20210419-170747-902-9c5a05-Offset_calibration/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210419/20210419-170747-902-9c5a05-Offset_calibration/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210419/20210419-173649-456-23c5f3-AllXY q0/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210419/20210419-173649-456-23c5f3-AllXY q0/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210420/20210420-001339-580-97bdef-Echo at 4.715GHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210420/20210420-001339-580-97bdef-Echo at 4.715GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210422/20210422-104958-297-7d6034-Ramsey oscillation at 4.715GHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210422/20210422-104958-297-7d6034-Ramsey oscillation at 4.715GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210827/20210827-174946-357-70a986-T1 experiment q0/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210827/20210827-174946-357-70a986-T1 experiment q0/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210827/20210827-175004-087-ab1aab-Ramsey oscillation q0 at 4.9969 GHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210827/20210827-175004-087-ab1aab-Ramsey oscillation q0 at 4.9969 GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210827/20210827-175021-521-251f28-Echo experiment q0/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210827/20210827-175021-521-251f28-Echo experiment q0/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20210901/20210901-132357-561-5c3ef7-Ramsey oscillation q0 at 6.1400 GHz/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20210901/20210901-132357-561-5c3ef7-Ramsey oscillation q0 at 6.1400 GHz/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5` & `quantify-core-0.7.2/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/snapshot.json` & `quantify-core-0.7.2/tests/test_data/20211029/20211029-000217-063-ab42e4-Pulsed spectroscopy q4/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5` & `quantify-core-0.7.2/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/snapshot.json` & `quantify-core-0.7.2/tests/test_data/20211029/20211029-001240-717-587536-Pulsed spectroscopy q4/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5` & `quantify-core-0.7.2/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/snapshot.json` & `quantify-core-0.7.2/tests/test_data/20211029/20211029-002303-114-e360dc-Pulsed spectroscopy q4/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/snapshot.json` & `quantify-core-0.7.2/tests/test_data/20220409/20220409-095654-698-b2dc1f-1d with two settables/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20220509/20220509-204728-327-69b211-load_settings_test_nested/snapshot.json` & `quantify-core-0.7.2/tests/test_data/20220509/20220509-204728-327-69b211-load_settings_test_nested/snapshot.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5` & `quantify-core-0.7.2/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20220930/20220930-104634-687-dcc774-Pulsed spectroscopy 0/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5` & `quantify-core-0.7.2/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20220930/20220930-104712-924-d6f761-Pulsed spectroscopy 1/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5` & `quantify-core-0.7.2/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/analysis_QubitSpectroscopyAnalysis/dataset_processed.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/dataset.hdf5` & `quantify-core-0.7.2/tests/test_data/20220930/20220930-104728-848-035150-Pulsed spectroscopy 2/dataset.hdf5`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_data/transmon_test_config.json` & `quantify-core-0.7.2/tests/test_data/transmon_test_config.json`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/test_headers_and_copyright.py` & `quantify-core-0.7.2/tests/test_headers_and_copyright.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/utilities/test_deprecation.py` & `quantify-core-0.7.2/tests/utilities/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/utilities/test_experiment_helpers.py` & `quantify-core-0.7.2/tests/utilities/test_experiment_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 
     def get_func():
         return 20
 
     def _error_param_get():
         raise RuntimeError("An error occured when getting the parameter")
 
+    def _error_param_set(value):
+        raise RuntimeError(f"An error occured when setting the parameter to {value}")
+
     instr = Instrument("DummyInstrument")
 
     # A parameter that is both settable and gettable
     instr.add_parameter(
         "settable_param", initial_value=10, parameter_class=ManualParameter
     )
     # A parameter that is only gettable
@@ -51,16 +54,18 @@
     # A parameter which our function will try to set to a numpy array
     instr.add_parameter(
         "numpy_array_param",
         initial_value=np.array([1]),
         parameter_class=ManualParameter,
         vals=validators.Arrays(),
     )
-    # A parameter that always returns an error when you try to get it
-    instr.add_parameter("error_param", get_cmd=_error_param_get)
+    # A parameter that always returns an error when you try to get or set it
+    instr.add_parameter(
+        "error_param", get_cmd=_error_param_get, set_cmd=_error_param_set
+    )
 
     def cleanup_instruments():
         instr.close()
 
     request.addfinalizer(cleanup_instruments)
 
     return instr
```

### Comparing `quantify-core-0.7.1/tests/utilities/test_general.py` & `quantify-core-0.7.2/tests/utilities/test_general.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/utilities/test_inspect_utils.py` & `quantify-core-0.7.2/tests/utilities/test_inspect_utils.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/visualization/test_SI_utilities.py` & `quantify-core-0.7.2/tests/visualization/test_SI_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     scale_factor, post_unit = SI_prefix_and_scale_factor(val=1000.0, unit=unit)
     assert scale_factor == 1e-3
     assert "$\\Phi_0$" == post_unit
 
     unit = None
     scale_factor, post_unit = SI_prefix_and_scale_factor(val=5000.4, unit=unit)
     assert scale_factor == 1
-    assert "" == post_unit
+    assert not post_unit
 
 
 def test_label_scaling() -> None:
     """
     This test creates a dummy plot and checks if the tick labels are
     rescaled correctly
     """
```

### Comparing `quantify-core-0.7.1/tests/visualization/test_instrument_monitor.py` & `quantify-core-0.7.2/tests/visualization/test_instrument_monitor.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/visualization/test_mpl_plotting.py` & `quantify-core-0.7.2/tests/visualization/test_mpl_plotting.py`

 * *Files identical despite different names*

### Comparing `quantify-core-0.7.1/tests/visualization/test_pyqt_plotmon.py` & `quantify-core-0.7.2/tests/visualization/test_pyqt_plotmon.py`

 * *Files identical despite different names*

