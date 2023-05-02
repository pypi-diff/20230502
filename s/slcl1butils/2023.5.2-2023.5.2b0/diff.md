# Comparing `tmp/slcl1butils-2023.5.2.tar.gz` & `tmp/slcl1butils-2023.5.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slcl1butils-2023.5.2.tar", last modified: Tue May  2 14:19:45 2023, max compression
+gzip compressed data, was "slcl1butils-2023.5.2b0.tar", last modified: Tue May  2 14:32:13 2023, max compression
```

## Comparing `slcl1butils-2023.5.2.tar` & `slcl1butils-2023.5.2b0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:45.119871 slcl1butils-2023.5.2/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      348 2023-04-07 13:30:19.000000 slcl1butils-2023.5.2/.flake8
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:44.947871 slcl1butils-2023.5.2/.github/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      117 2023-04-07 13:30:19.000000 slcl1butils-2023.5.2/.github/dependabot.yml
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:44.947871 slcl1butils-2023.5.2/.github/workflows/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      829 2023-04-07 13:30:19.000000 slcl1butils-2023.5.2/.github/workflows/publish.yml
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     1799 2023-04-07 13:30:19.000000 slcl1butils-2023.5.2/.gitignore
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      957 2023-04-07 13:30:19.000000 slcl1butils-2023.5.2/.pre-commit-config.yaml
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      417 2023-04-07 13:30:19.000000 slcl1butils-2023.5.2/.readthedocs.yml
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    35149 2023-04-07 13:30:19.000000 slcl1butils-2023.5.2/LICENSE
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      398 2023-05-02 14:19:45.119871 slcl1butils-2023.5.2/PKG-INFO
--rw-rw-r--   0 agrouaze (54605) droos    (10042)       66 2023-03-10 13:41:53.000000 slcl1butils-2023.5.2/README.md
--rw-rw-r--   0 agrouaze (54605) droos    (10042)        0 2023-04-07 13:30:19.000000 slcl1butils-2023.5.2/__init__.py
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:44.967871 slcl1butils-2023.5.2/docs/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      744 2023-04-07 13:30:19.000000 slcl1butils-2023.5.2/docs/Makefile
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:44.895871 slcl1butils-2023.5.2/docs/_static/
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:44.975871 slcl1butils-2023.5.2/docs/_static/css/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      126 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/docs/_static/css/slcl1butils.css
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      290 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/docs/basic_api.rst
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     3272 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/docs/conf.py
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:44.987871 slcl1butils-2023.5.2/docs/examples/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     5970 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/docs/examples/display_a_IW_L1B_xspectra.ipynb
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     2306 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
--rw-rw-r--   0 agrouaze (54605) droos    (10042)        0 2023-04-07 13:30:19.000000 slcl1butils-2023.5.2/docs/examples/intro.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     4245 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     5359 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     2043 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/docs/index.rst
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      846 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/docs/installing.rst
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    59687 2023-04-07 13:30:19.000000 slcl1butils-2023.5.2/docs/oceanspectrumSAR.png
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    10438 2023-04-07 11:55:47.000000 slcl1butils-2023.5.2/get_polygons_from_l1b.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     1142 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/pyproject.toml
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      198 2023-04-07 13:30:19.000000 slcl1butils-2023.5.2/requirements_doc.txt
--rw-rw-r--   0 agrouaze (54605) droos    (10042)       38 2023-05-02 14:19:45.119871 slcl1butils-2023.5.2/setup.cfg
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:45.031871 slcl1butils-2023.5.2/slcl1butils/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      223 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/__init__.py
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:45.059872 slcl1butils-2023.5.2/slcl1butils/coloc/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/coloc/__init__.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     9173 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/coloc/coloc.py
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:45.079872 slcl1butils-2023.5.2/slcl1butils/compute/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/compute/__init__.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     3103 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/compute/compute_from_l1b.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     3757 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/compute/cwave.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     1471 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/compute/macs.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     5440 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/compute/stack_iw_l1b.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    11305 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/compute/stack_wv_l1c_monthly.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      189 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/config.yaml
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     4386 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/conversion_polar_cartesian.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     3626 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/cwave_parameters_computation_example.ipynb
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      617 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/get_config.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    10830 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/get_polygons_from_l1b.py
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:45.103871 slcl1butils-2023.5.2/slcl1butils/plotting/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/plotting/__init__.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     1094 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    20411 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/plotting/display_one_spectra.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    12819 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/plotting/display_xspectra_grid.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     2131 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     2216 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      752 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     5776 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/raster_readers.py
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:45.115872 slcl1butils-2023.5.2/slcl1butils/scripts/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    12466 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/scripts/do_L1C_SAFE_from_L1B_SAFE.py
--rwxrwxr-x   0 agrouaze (54605) droos    (10042)      560 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    11790 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     1034 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/spectrum_clockwise_to_trigo.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      729 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/spectrum_rotation.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     1193 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/symmetrize_l1b_spectra.py
--rw-rw-r--   0 agrouaze (54605) droos    (10042)    19569 2023-05-02 14:19:26.000000 slcl1butils-2023.5.2/slcl1butils/utils.py
-drwxrwxr-x   0 agrouaze (54605) droos    (10042)        0 2023-05-02 14:19:45.051871 slcl1butils-2023.5.2/slcl1butils.egg-info/
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      398 2023-05-02 14:19:44.000000 slcl1butils-2023.5.2/slcl1butils.egg-info/PKG-INFO
--rw-rw-r--   0 agrouaze (54605) droos    (10042)     1990 2023-05-02 14:19:44.000000 slcl1butils-2023.5.2/slcl1butils.egg-info/SOURCES.txt
--rw-rw-r--   0 agrouaze (54605) droos    (10042)        1 2023-05-02 14:19:44.000000 slcl1butils-2023.5.2/slcl1butils.egg-info/dependency_links.txt
--rw-rw-r--   0 agrouaze (54605) droos    (10042)      251 2023-05-02 14:19:44.000000 slcl1butils-2023.5.2/slcl1butils.egg-info/entry_points.txt
--rw-rw-r--   0 agrouaze (54605) droos    (10042)       75 2023-05-02 14:19:44.000000 slcl1butils-2023.5.2/slcl1butils.egg-info/requires.txt
--rw-rw-r--   0 agrouaze (54605) droos    (10042)       12 2023-05-02 14:19:44.000000 slcl1butils-2023.5.2/slcl1butils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.234670 slcl1butils-2023.5.2b0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.234670 slcl1butils-2023.5.2b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.234670 slcl1butils-2023.5.2b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.234670 slcl1butils-2023.5.2b0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.234670 slcl1butils-2023.5.2b0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/_static/css/slcl1butils.css
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.234670 slcl1butils-2023.5.2b0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/examples/display_a_IW_L1B_xspectra.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/oceanspectrumSAR.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/get_polygons_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/slcl1butils/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/slcl1butils/coloc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/coloc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/coloc/coloc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/slcl1butils/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/compute/compute_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/compute/cwave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/compute/macs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/compute/stack_iw_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/compute/stack_wv_l1c_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/conversion_polar_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/cwave_parameters_computation_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/get_polygons_from_l1b.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/slcl1butils/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/plotting/display_one_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/plotting/display_xspectra_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/raster_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/slcl1butils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/scripts/do_L1C_SAFE_from_L1B_SAFE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/spectrum_clockwise_to_trigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/spectrum_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/symmetrize_l1b_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19569 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/slcl1butils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-02 14:32:13.000000 slcl1butils-2023.5.2b0/slcl1butils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-02 14:32:13.000000 slcl1butils-2023.5.2b0/slcl1butils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:32:13.000000 slcl1butils-2023.5.2b0/slcl1butils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-02 14:32:13.000000 slcl1butils-2023.5.2b0/slcl1butils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 14:32:13.000000 slcl1butils-2023.5.2b0/slcl1butils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 14:32:13.000000 slcl1butils-2023.5.2b0/slcl1butils.egg-info/top_level.txt
```

### Comparing `slcl1butils-2023.5.2/.github/workflows/publish.yml` & `slcl1butils-2023.5.2b0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/.gitignore` & `slcl1butils-2023.5.2b0/.gitignore`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/.pre-commit-config.yaml` & `slcl1butils-2023.5.2b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/LICENSE` & `slcl1butils-2023.5.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/docs/Makefile` & `slcl1butils-2023.5.2b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/docs/conf.py` & `slcl1butils-2023.5.2b0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/docs/examples/display_a_IW_L1B_xspectra.ipynb` & `slcl1butils-2023.5.2b0/docs/examples/display_a_IW_L1B_xspectra.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb` & `slcl1butils-2023.5.2b0/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2023.5.2b0/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2023.5.2b0/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/docs/index.rst` & `slcl1butils-2023.5.2b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/docs/installing.rst` & `slcl1butils-2023.5.2b0/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/docs/oceanspectrumSAR.png` & `slcl1butils-2023.5.2b0/docs/oceanspectrumSAR.png`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/get_polygons_from_l1b.py` & `slcl1butils-2023.5.2b0/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/pyproject.toml` & `slcl1butils-2023.5.2b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/coloc/coloc.py` & `slcl1butils-2023.5.2b0/slcl1butils/coloc/coloc.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/compute/compute_from_l1b.py` & `slcl1butils-2023.5.2b0/slcl1butils/compute/compute_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/compute/cwave.py` & `slcl1butils-2023.5.2b0/slcl1butils/compute/cwave.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/compute/macs.py` & `slcl1butils-2023.5.2b0/slcl1butils/compute/macs.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/compute/stack_iw_l1b.py` & `slcl1butils-2023.5.2b0/slcl1butils/compute/stack_iw_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/compute/stack_wv_l1c_monthly.py` & `slcl1butils-2023.5.2b0/slcl1butils/compute/stack_wv_l1c_monthly.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/conversion_polar_cartesian.py` & `slcl1butils-2023.5.2b0/slcl1butils/conversion_polar_cartesian.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/cwave_parameters_computation_example.ipynb` & `slcl1butils-2023.5.2b0/slcl1butils/cwave_parameters_computation_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/get_config.py` & `slcl1butils-2023.5.2b0/slcl1butils/get_config.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/get_polygons_from_l1b.py` & `slcl1butils-2023.5.2b0/slcl1butils/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py` & `slcl1butils-2023.5.2b0/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/plotting/display_one_spectra.py` & `slcl1butils-2023.5.2b0/slcl1butils/plotting/display_one_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/plotting/display_xspectra_grid.py` & `slcl1butils-2023.5.2b0/slcl1butils/plotting/display_xspectra_grid.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2023.5.2b0/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2023.5.2b0/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py` & `slcl1butils-2023.5.2b0/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/raster_readers.py` & `slcl1butils-2023.5.2b0/slcl1butils/raster_readers.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/scripts/do_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2023.5.2b0/slcl1butils/scripts/do_L1C_SAFE_from_L1B_SAFE.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs` & `slcl1butils-2023.5.2b0/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2023.5.2b0/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/spectrum_clockwise_to_trigo.py` & `slcl1butils-2023.5.2b0/slcl1butils/spectrum_clockwise_to_trigo.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/spectrum_rotation.py` & `slcl1butils-2023.5.2b0/slcl1butils/spectrum_rotation.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/symmetrize_l1b_spectra.py` & `slcl1butils-2023.5.2b0/slcl1butils/symmetrize_l1b_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils/utils.py` & `slcl1butils-2023.5.2b0/slcl1butils/utils.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2/slcl1butils.egg-info/SOURCES.txt` & `slcl1butils-2023.5.2b0/slcl1butils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

