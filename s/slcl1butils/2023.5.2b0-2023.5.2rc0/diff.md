# Comparing `tmp/slcl1butils-2023.5.2b0.tar.gz` & `tmp/slcl1butils-2023.5.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slcl1butils-2023.5.2b0.tar", last modified: Tue May  2 14:32:13 2023, max compression
+gzip compressed data, was "slcl1butils-2023.5.2rc0.tar", last modified: Tue May  2 14:43:54 2023, max compression
```

## Comparing `slcl1butils-2023.5.2b0.tar` & `slcl1butils-2023.5.2rc0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.234670 slcl1butils-2023.5.2b0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.234670 slcl1butils-2023.5.2b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.234670 slcl1butils-2023.5.2b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.234670 slcl1butils-2023.5.2b0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.234670 slcl1butils-2023.5.2b0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/_static/css/slcl1butils.css
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.234670 slcl1butils-2023.5.2b0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/examples/display_a_IW_L1B_xspectra.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/docs/oceanspectrumSAR.png
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/get_polygons_from_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/slcl1butils/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/slcl1butils/coloc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/coloc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/coloc/coloc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/slcl1butils/compute/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/compute/compute_from_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/compute/cwave.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/compute/macs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/compute/stack_iw_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/compute/stack_wv_l1c_monthly.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/conversion_polar_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/cwave_parameters_computation_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/get_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/get_polygons_from_l1b.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/slcl1butils/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
--rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/plotting/display_one_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/plotting/display_xspectra_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/raster_readers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/slcl1butils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/scripts/do_L1C_SAFE_from_L1B_SAFE.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/spectrum_clockwise_to_trigo.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/spectrum_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/symmetrize_l1b_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)    19569 2023-05-02 14:31:57.000000 slcl1butils-2023.5.2b0/slcl1butils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:32:13.238670 slcl1butils-2023.5.2b0/slcl1butils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-02 14:32:13.000000 slcl1butils-2023.5.2b0/slcl1butils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-02 14:32:13.000000 slcl1butils-2023.5.2b0/slcl1butils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:32:13.000000 slcl1butils-2023.5.2b0/slcl1butils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-02 14:32:13.000000 slcl1butils-2023.5.2b0/slcl1butils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 14:32:13.000000 slcl1butils-2023.5.2b0/slcl1butils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 14:32:13.000000 slcl1butils-2023.5.2b0/slcl1butils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:54.951821 slcl1butils-2023.5.2rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:54.939821 slcl1butils-2023.5.2rc0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:54.943821 slcl1butils-2023.5.2rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-02 14:43:54.951821 slcl1butils-2023.5.2rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:54.943821 slcl1butils-2023.5.2rc0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:54.939821 slcl1butils-2023.5.2rc0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:54.943821 slcl1butils-2023.5.2rc0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/docs/_static/css/slcl1butils.css
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:54.943821 slcl1butils-2023.5.2rc0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/docs/examples/display_a_IW_L1B_xspectra.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/docs/oceanspectrumSAR.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/get_polygons_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:43:54.951821 slcl1butils-2023.5.2rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:54.947821 slcl1butils-2023.5.2rc0/slcl1butils/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:54.947821 slcl1butils-2023.5.2rc0/slcl1butils/coloc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/coloc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/coloc/coloc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:54.947821 slcl1butils-2023.5.2rc0/slcl1butils/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/compute/compute_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/compute/cwave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/compute/macs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/compute/stack_iw_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/compute/stack_wv_l1c_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/conversion_polar_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/cwave_parameters_computation_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/get_polygons_from_l1b.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:54.951821 slcl1butils-2023.5.2rc0/slcl1butils/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/plotting/display_one_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/plotting/display_xspectra_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/raster_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:54.951821 slcl1butils-2023.5.2rc0/slcl1butils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/scripts/do_L1C_SAFE_from_L1B_SAFE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/spectrum_clockwise_to_trigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/spectrum_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/symmetrize_l1b_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19569 2023-05-02 14:43:33.000000 slcl1butils-2023.5.2rc0/slcl1butils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:43:54.947821 slcl1butils-2023.5.2rc0/slcl1butils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-02 14:43:54.000000 slcl1butils-2023.5.2rc0/slcl1butils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-02 14:43:54.000000 slcl1butils-2023.5.2rc0/slcl1butils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:43:54.000000 slcl1butils-2023.5.2rc0/slcl1butils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-02 14:43:54.000000 slcl1butils-2023.5.2rc0/slcl1butils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 14:43:54.000000 slcl1butils-2023.5.2rc0/slcl1butils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 14:43:54.000000 slcl1butils-2023.5.2rc0/slcl1butils.egg-info/top_level.txt
```

### Comparing `slcl1butils-2023.5.2b0/.github/workflows/publish.yml` & `slcl1butils-2023.5.2rc0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/.gitignore` & `slcl1butils-2023.5.2rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/.pre-commit-config.yaml` & `slcl1butils-2023.5.2rc0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/LICENSE` & `slcl1butils-2023.5.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/docs/Makefile` & `slcl1butils-2023.5.2rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/docs/conf.py` & `slcl1butils-2023.5.2rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/docs/examples/display_a_IW_L1B_xspectra.ipynb` & `slcl1butils-2023.5.2rc0/docs/examples/display_a_IW_L1B_xspectra.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb` & `slcl1butils-2023.5.2rc0/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2023.5.2rc0/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2023.5.2rc0/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/docs/index.rst` & `slcl1butils-2023.5.2rc0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/docs/installing.rst` & `slcl1butils-2023.5.2rc0/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/docs/oceanspectrumSAR.png` & `slcl1butils-2023.5.2rc0/docs/oceanspectrumSAR.png`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/get_polygons_from_l1b.py` & `slcl1butils-2023.5.2rc0/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/pyproject.toml` & `slcl1butils-2023.5.2rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/coloc/coloc.py` & `slcl1butils-2023.5.2rc0/slcl1butils/coloc/coloc.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/compute/compute_from_l1b.py` & `slcl1butils-2023.5.2rc0/slcl1butils/compute/compute_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/compute/cwave.py` & `slcl1butils-2023.5.2rc0/slcl1butils/compute/cwave.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/compute/macs.py` & `slcl1butils-2023.5.2rc0/slcl1butils/compute/macs.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/compute/stack_iw_l1b.py` & `slcl1butils-2023.5.2rc0/slcl1butils/compute/stack_iw_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/compute/stack_wv_l1c_monthly.py` & `slcl1butils-2023.5.2rc0/slcl1butils/compute/stack_wv_l1c_monthly.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/conversion_polar_cartesian.py` & `slcl1butils-2023.5.2rc0/slcl1butils/conversion_polar_cartesian.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/cwave_parameters_computation_example.ipynb` & `slcl1butils-2023.5.2rc0/slcl1butils/cwave_parameters_computation_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/get_config.py` & `slcl1butils-2023.5.2rc0/slcl1butils/get_config.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/get_polygons_from_l1b.py` & `slcl1butils-2023.5.2rc0/slcl1butils/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py` & `slcl1butils-2023.5.2rc0/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/plotting/display_one_spectra.py` & `slcl1butils-2023.5.2rc0/slcl1butils/plotting/display_one_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/plotting/display_xspectra_grid.py` & `slcl1butils-2023.5.2rc0/slcl1butils/plotting/display_xspectra_grid.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2023.5.2rc0/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2023.5.2rc0/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py` & `slcl1butils-2023.5.2rc0/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/raster_readers.py` & `slcl1butils-2023.5.2rc0/slcl1butils/raster_readers.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/scripts/do_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2023.5.2rc0/slcl1butils/scripts/do_L1C_SAFE_from_L1B_SAFE.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs` & `slcl1butils-2023.5.2rc0/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2023.5.2rc0/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/spectrum_clockwise_to_trigo.py` & `slcl1butils-2023.5.2rc0/slcl1butils/spectrum_clockwise_to_trigo.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/spectrum_rotation.py` & `slcl1butils-2023.5.2rc0/slcl1butils/spectrum_rotation.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/symmetrize_l1b_spectra.py` & `slcl1butils-2023.5.2rc0/slcl1butils/symmetrize_l1b_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils/utils.py` & `slcl1butils-2023.5.2rc0/slcl1butils/utils.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.5.2b0/slcl1butils.egg-info/SOURCES.txt` & `slcl1butils-2023.5.2rc0/slcl1butils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

