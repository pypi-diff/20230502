# Comparing `tmp/dkist_processing_visp-2.0.2.tar.gz` & `tmp/dkist_processing_visp-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_visp-2.0.2.tar", last modified: Mon Apr 24 18:20:10 2023, max compression
+gzip compressed data, was "dkist_processing_visp-2.1.0.tar", last modified: Tue May  2 18:17:13 2023, max compression
```

## Comparing `dkist_processing_visp-2.0.2.tar` & `dkist_processing_visp-2.1.0.tar`

### file list

```diff
@@ -1,107 +1,109 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:20:10.375461 dkist_processing_visp-2.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     2455 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    19176 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-04-24 18:20:10.375461 dkist_processing_visp-2.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5645 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3694 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/SCIENCE_CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3428 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:20:10.367461 dkist_processing_visp-2.0.2/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:20:10.367461 dkist_processing_visp-2.0.2/dkist_processing_visp/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:20:10.367461 dkist_processing_visp-2.0.2/dkist_processing_visp/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/fonts/Lato-Regular.ttf
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:20:10.371461 dkist_processing_visp-2.0.2/dkist_processing_visp/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3440 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    10093 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:20:10.371461 dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5370 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/polarimeter_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/raster_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/visp_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/visp_l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:20:10.371461 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    15383 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4137 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)    38179 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    18995 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5343 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     7068 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:20:10.371461 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/mixin/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     7112 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    10422 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     4499 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     7944 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    28173 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)    27922 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7259 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:20:10.375461 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16170 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     6595 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/e2e_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    17553 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/e2e_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    19981 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_build_quality_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5272 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)    13876 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    11145 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)     5651 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    11821 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    16234 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    19734 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     9883 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_submit_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     5097 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_visp_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     5752 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:20:10.375461 dkist_processing_visp-2.0.2/dkist_processing_visp/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/dkist_processing_visp/workflows/single_task_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:20:10.367461 dkist_processing_visp-2.0.2/dkist_processing_visp.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-04-24 18:20:10.000000 dkist_processing_visp-2.0.2/dkist_processing_visp.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3510 2023-04-24 18:20:10.000000 dkist_processing_visp-2.0.2/dkist_processing_visp.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-24 18:20:10.000000 dkist_processing_visp-2.0.2/dkist_processing_visp.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-04-24 18:20:10.000000 dkist_processing_visp-2.0.2/dkist_processing_visp.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-24 18:20:10.000000 dkist_processing_visp-2.0.2/dkist_processing_visp.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:20:10.375461 dkist_processing_visp-2.0.2/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/docs/background_light.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     6427 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/docs/gain_correction.rst
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/docs/l0_to_l1_visp.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     4995 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/docs/polarization_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/docs/science_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/docs/scientific_changelog.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 18:20:10.375461 dkist_processing_visp-2.0.2/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/science_towncrier.sh
--rw-rw-rw-   0 root         (0) root         (0)     1705 2023-04-24 18:20:10.379461 dkist_processing_visp-2.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-04-24 18:20:04.000000 dkist_processing_visp-2.0.2/towncrier_science.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 18:17:13.067526 dkist_processing_visp-2.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    19829 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-05-02 18:17:13.067526 dkist_processing_visp-2.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5645 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3652 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3428 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 18:17:13.055526 dkist_processing_visp-2.1.0/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 18:17:13.055526 dkist_processing_visp-2.1.0/dkist_processing_visp/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 18:17:13.055526 dkist_processing_visp-2.1.0/dkist_processing_visp/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/fonts/Lato-Regular.ttf
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 18:17:13.055526 dkist_processing_visp-2.1.0/dkist_processing_visp/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3440 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    10418 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 18:17:13.059526 dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5370 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/polarimeter_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/raster_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/visp_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/visp_l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 18:17:13.059526 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3296 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    14365 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4137 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    38179 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    20011 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5343 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7068 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 18:17:13.059526 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/mixin/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/mixin/downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)     7112 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10422 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4499 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     7944 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    28173 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)    27922 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6846 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 18:17:13.063526 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16212 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6595 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/e2e_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    17553 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/e2e_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    18443 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_build_quality_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)    13876 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    12613 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)     5651 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    11821 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    16234 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    19734 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     9883 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_submit_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     5097 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_visp_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     5752 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 18:17:13.063526 dkist_processing_visp-2.1.0/dkist_processing_visp/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/dkist_processing_visp/workflows/single_task_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 18:17:13.055526 dkist_processing_visp-2.1.0/dkist_processing_visp.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-05-02 18:17:12.000000 dkist_processing_visp-2.1.0/dkist_processing_visp.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3605 2023-05-02 18:17:13.000000 dkist_processing_visp-2.1.0/dkist_processing_visp.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-02 18:17:12.000000 dkist_processing_visp-2.1.0/dkist_processing_visp.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-05-02 18:17:12.000000 dkist_processing_visp-2.1.0/dkist_processing_visp.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-02 18:17:12.000000 dkist_processing_visp-2.1.0/dkist_processing_visp.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 18:17:13.067526 dkist_processing_visp-2.1.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/docs/background_light.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6427 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/docs/gain_correction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/docs/l0_to_l1_visp.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     4995 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/docs/polarization_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/docs/science_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-02 18:17:13.067526 dkist_processing_visp-2.1.0/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1705 2023-05-02 18:17:13.067526 dkist_processing_visp-2.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-05-02 18:17:07.000000 dkist_processing_visp-2.1.0/towncrier_science.toml
```

### Comparing `dkist_processing_visp-2.0.2/.gitignore` & `dkist_processing_visp-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/.pre-commit-config.yaml` & `dkist_processing_visp-2.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/CHANGELOG.rst` & `dkist_processing_visp-2.1.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v2.1.0 (2023-05-02)
+===================
+
+Features
+--------
+
+- Support for a parameter that sets the number of spatial bins used when computing demodulation matrices. This is mostly to speed up testing and deployment; real science data will probably not be binned at all. (`#112 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/112>`__)
+
+
+Misc
+----
+
+- Offload calculation of "WAVEMIN/MAX" in L1 headers to new functionality in `*-common` that uses the already-defined `get_wavelength_range`. The result is that this logic now only lives in one place. (`#113 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/113>`__)
+
+
 v2.0.2 (2023-04-24)
 ===================
 
 Misc
 ----
 
 - Update `dkist-fits-specifications` to include new header keys.
```

### Comparing `dkist_processing_visp-2.0.2/PKG-INFO` & `dkist_processing_visp-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_processing_visp
-Version: 2.0.2
+Version: 2.1.0
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.0.2/README.rst` & `dkist_processing_visp-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/SCIENCE_CHANGELOG.rst` & `dkist_processing_visp-2.1.0/SCIENCE_CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 - Improvements to beam-registration calibration, especially the spectral angle. See the pull request for more information.
   A result is that hairline features are better identified and produce fewer interpolation artifacts. (`#108 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/108>`__)
 - Use `dkist-processing-pac` >= 2.0.0 to correct a bug in how the final coordinate transform was applied. As of now, all
   L1 data are in a coordinate frame consistent with SDO/HMI and Hinode-SP. See :doc:`this page </science_calibration>` for
   more information. (`#109 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/109>`__)
 
 
-v1.3.0 (2023-03-28)
+v1.3.0 (2022-11-14)
 ===================
 
 
 
 
 - Fixed a bug that could cause incorrect calculation of the region overlapped by both beams. It is unlikely this bug was ever encountered in the wild.
 
 
-v1.1.0 (2023-03-28)
+v1.1.0 (2022-11-01)
 ===================
 
 
 
 
-- Uses a new version of the PA&C library that fixes a bug in how the inverse telescope Mueller matrices were computed. Previously, the Mueller matrices did not account for small angular offsets between the as-build telescope mount and the design specificiations.
+- Uses a new version of the PA&C library that fixes a bug in how the inverse telescope Mueller matrices were computed. Previously, the Mueller matrices did not account for small intrinsic rotations between mirror groups.
```

### Comparing `dkist_processing_visp-2.0.2/bitbucket-pipelines.yml` & `dkist_processing_visp-2.1.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/check_changelog_updated.sh` & `dkist_processing_visp-2.1.0/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/fonts/Lato-Regular.ttf` & `dkist_processing_visp-2.1.0/dkist_processing_visp/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/models/constants.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/models/parameters.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/models/parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,14 +164,23 @@
 
     @property
     def polcal_spatial_median_filter_width_px(self) -> int:
         """Return the size of the median filter to apply in the spatial dimension to polcal data."""
         return self._find_most_recent_past_value("visp_polcal_spatial_median_filter_width_px")
 
     @property
+    def polcal_num_spatial_bins(self) -> int:
+        """
+        Return the number of spatial bins to pass to `dkist-processing-pac`.
+
+        This sets the spatial resolution of the resulting demodulation matrices.
+        """
+        return self._find_most_recent_past_value("visp_polcal_num_spatial_bins")
+
+    @property
     def polcal_demod_spatial_smooth_fit_order(self) -> int:
         """Return the polynomial fit order used to fit/smooth demodulation matrices in the spatial dimension."""
         return self._find_most_recent_past_value("visp_polcal_demod_spatial_smooth_fit_order")
 
     @property
     def polcal_demod_spatial_smooth_min_samples(self) -> float:
         """Return fractional number of samples required for the RANSAC regressor used to smooth demod matrices."""
```

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/models/tags.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/map_repeats.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/polarimeter_mode.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/polarimeter_mode.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/raster_step.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/raster_step.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/task.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/time.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/visp_l0_fits_access.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/visp_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/visp_l1_fits_access.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/visp_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/parsers/wavelength.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/assemble_movie.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/background_light.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/background_light.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_processing_math.transform.binning import resize_arrays
 from logging42 import logger
 
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
+from dkist_processing_visp.tasks.mixin.downsample import DownsampleMixin
 from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 
 
 class BackgroundLightCalibration(
     VispTaskBase,
     IntermediateFrameHelpersMixin,
     InputFrameLoadersMixin,
+    DownsampleMixin,
     CorrectionsMixin,
     QualityMixin,
 ):
     """
     Task class for measuring additive background light that is not captured in the dark frames.
 
     Parameters
@@ -185,15 +187,15 @@
 
                 pol_cal_arrays = [
                     self.input_frame_loaders_get_beam(obj.data, beam=beam) for obj in pol_cal_objs
                 ]
                 input_data = average_numpy_arrays(pol_cal_arrays)
                 dark_subtracted_array = next(subtract_array_from_arrays(input_data, dark_array))
 
-                resampled_array = self.resample_spatial_dimension(
+                resampled_array = self.downsample_spatial_dimension_local_median(
                     dark_subtracted_array,
                     num_spatial_bins=self.parameters.background_num_spatial_bins,
                 )
 
                 array_list.append(resampled_array)
 
         output_array = np.stack(array_list)
@@ -239,34 +241,14 @@
         return background_light
 
     @staticmethod
     def upsample_background_light(small_data: np.ndarray, full_shape: tuple) -> np.ndarray:
         """Resample a background light array to the full ViSP frame."""
         return next(resize_arrays(small_data, output_shape=full_shape, order=1))
 
-    @staticmethod
-    def resample_spatial_dimension(data: np.ndarray, num_spatial_bins: int) -> np.ndarray:
-        """Resample a stack of spectra along the spatial dimension.
-
-        This is a separate function because calling `skimage.measure.block_reduce` on the entire (large) array all at once
-        creates a huge memory strain that is not needed since we're only reducing over one of the dimensions. Instead,
-        this function does some very cool tricks with reshaping and base numpy to keep the memory footprint lower.
-        """
-        # Taken from the amazing answer in
-        #  https://stackoverflow.com/questions/44527579/whats-the-best-way-to-downsample-a-numpy-array
-        num_wave, num_spat_pos = data.shape
-
-        if (num_spat_pos / num_spatial_bins) % 1 != 0:
-            raise ValueError(
-                f"The number of spatial bins must evenly divide the spatial dimension. {num_spatial_bins} bins do not evenly divide {num_spat_pos}."
-            )
-
-        reshaped = data.reshape((num_wave, num_spatial_bins, num_spat_pos // num_spatial_bins))
-        return np.median(reshaped, axis=2)
-
     def setup_fit(
         self, spectra_stack: np.ndarray, continuum_idx: list[int]
     ) -> tuple[np.ndarray, np.ndarray, spo.Bounds]:
         """
         Subsample the wavelength axis, construct and initial guess, and define parameter bounds.
 
         Parameters
```

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/dark.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/geometric.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/geometric.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/instrument_polarization.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/instrument_polarization.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,26 +18,28 @@
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import PolynomialFeatures
 from sklearn.preprocessing import RobustScaler
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
+from dkist_processing_visp.tasks.mixin.downsample import DownsampleMixin
 from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 
 
 class InstrumentPolarizationCalibration(
     VispTaskBase,
     IntermediateFrameHelpersMixin,
     InputFrameLoadersMixin,
     CorrectionsMixin,
+    DownsampleMixin,
     QualityMixin,
 ):
     """
     Task class for instrument polarization for a VISP calibration run.
 
     Parameters
     ----------
@@ -166,14 +168,17 @@
         except StopIteration:
             if self.parameters.background_on:
                 raise ValueError(f"No background light found for {beam = }")
             else:
                 logger.info("Skipping background light correction")
                 background_array = None
 
+        logger.info(
+            f"Data will be downsampled in the spatial dimension to {self.parameters.polcal_num_spatial_bins} pixels."
+        )
         for modstate in range(1, self.constants.num_modstates + 1):
             angle = self.intermediate_frame_helpers_load_angle(beam=beam)
             state_offset = self.intermediate_frame_helpers_load_state_offset(
                 beam=beam, modstate=modstate
             )
             spec_shift = self.intermediate_frame_helpers_load_spec_shift(beam=beam)
 
@@ -299,54 +304,72 @@
 
             spatially_smoothed_array = spnd.median_filter(
                 spectral_binned_array,
                 # The 1 below means we don't smooth in the spectral dimension
                 size=(1, self.parameters.polcal_spatial_median_filter_width_px),
             )
 
+            local_array = self.downsample_spatial_dimension_local_median(
+                spatially_smoothed_array, self.parameters.polcal_num_spatial_bins
+            )
+
             # Add two dummy dimensions just to keep it 2D.
             global_binned_array = np.nanmedian(filtered_array)[None, None]
 
         with self.apm_processing_step(f"Create reduced VispL0FitsAccess for {apm_str}"):
             local_result = VispL0FitsAccess(
-                fits.ImageHDU(spatially_smoothed_array, avg_inst_pol_cal_header),
+                fits.ImageHDU(local_array, avg_inst_pol_cal_header),
                 auto_squeeze=False,
             )
 
             global_result = VispL0FitsAccess(
                 fits.ImageHDU(global_binned_array, avg_inst_pol_cal_header),
                 auto_squeeze=False,
             )
 
         return local_result, global_result
 
     def smooth_demod_matrices(self, demod_matrices: np.ndarray) -> np.ndarray:
         """
         Smooth demodulation matrices in the spatial dimension.
 
+        The output will fully sample the spatial dimension so, as a side effect, this function also up-samples any data
+        that were binned spatially.
+
         Smoothing is done using a RANSAC regression estimator to perform a polynomial fit with high resilience to outliers.
         """
         # We need to smooth the *modulation* (not DEmodulation) matrices to preserve the normalization of the Stokes-I
         # values. linalg.pinv makes this easy
         modulation_matrices = np.linalg.pinv(demod_matrices)
-        smoothed_mod = np.zeros_like(modulation_matrices)
-        num_wave, num_slit_pos, num_mod, num_stokes = modulation_matrices.shape
-        abscissa = np.arange(num_slit_pos)[:, None]  # 2D because sklearn requires it
+
+        num_wave, num_binned_slit_pos, num_mod, num_stokes = modulation_matrices.shape
+        num_full_slit_pos = self.single_beam_shape[1]
+
+        smoothed_mod = np.zeros((num_wave, num_full_slit_pos, num_mod, num_stokes))
+
+        # The binned abscissa is the "x" locations of the bins along the full spatial range
+        # The full abscissa is the "x" locations of all spatial pixels
+        # Add dummy dimensions because sklearn requires it
+        binned_abscissa = np.linspace(
+            start=0, stop=num_full_slit_pos, num=num_binned_slit_pos, endpoint=False
+        )[:, None]
+        full_abscissa = np.arange(num_full_slit_pos)[:, None]
+
         model = self._build_RANSAC_model()
         for w in range(num_wave):
             for m in range(num_mod):
                 for s in range(num_stokes):
                     curve = modulation_matrices[w, :, m, s]
 
                     # Clean weirdo pixels
                     fill_value = np.nanmedian(curve)
                     curve[~np.isfinite(curve)] = fill_value
 
-                    model.fit(abscissa, curve)
-                    fit_curve = model.predict(abscissa)
+                    model.fit(binned_abscissa, curve)
+                    fit_curve = model.predict(full_abscissa)
                     smoothed_mod[w, :, m, s] = fit_curve
 
         # Now compute the inverse again to return the DEmodulation matrices
         smoothed_demod = np.linalg.pinv(smoothed_mod)
 
         return smoothed_demod
 
@@ -412,15 +435,15 @@
 
     def record_polcal_quality_metrics(self, beam: int, polcal_fitter: PolcalFitter):
         """Record various quality metrics from PolCal fits."""
         self.quality_store_polcal_results(
             polcal_fitter=polcal_fitter,
             label=f"Beam {beam}",
             bins_1=1,  # Yes, this is actually hard-coded right now
-            bins_2=self.single_beam_shape[1],
+            bins_2=self.parameters.polcal_num_spatial_bins,
             bin_1_type="spectral",
             bin_2_type="spatial",
             ## This is a bit of a hack and thus needs some explanation
             # By using the ``skip_recording_constant_pars`` switch we DON'T record the "polcal constant parameters" metric
             # for beam 2. This is because both beam 1 and beam 2 will have the same table. The way `*-common` is built
             # it will look for all metrics for both beam 1 and beam 2 so if we did save that metric for beam 2 then the
             # table would show up twice in the quality report. The following line avoids that.
```

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/lamp.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/make_movie_frames.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/mixin/corrections.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/mixin/corrections.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/mixin/input_frame_loaders.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/mixin/input_frame_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/parse.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/quality_metrics.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/science.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/solar.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/visp_base.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tasks/write_l1.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tasks/write_l1.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,21 +70,14 @@
                 header[f"DUNIT{i}"] = header[f"CUNIT{i}"]
             elif axis_type == "AWAV":
                 header[f"DNAXIS{i}"] = header[f"NAXIS{i}"]
                 header[f"DTYPE{i}"] = "SPECTRAL"
                 header[f"DPNAME{i}"] = "dispersion axis"
                 header[f"DWNAME{i}"] = "wavelength"
                 header[f"DUNIT{i}"] = header[f"CUNIT{i}"]
-                # The wavemin and wavemax assume that all frames in a dataset have identical wavelength axes
-                header["WAVEMIN"] = header[f"CRVAL{i}"] - (
-                    header[f"CRPIX{i}"] * header[f"CDELT{i}"]
-                )
-                header["WAVEMAX"] = header[f"CRVAL{i}"] + (
-                    (header[f"NAXIS{i}"] - header[f"CRPIX{i}"]) * header[f"CDELT{i}"]
-                )
             elif axis_type == "HPLN-TAN":
                 header[f"DNAXIS{i}"] = self.constants.num_raster_steps
                 header[f"DTYPE{i}"] = "SPATIAL"
                 header[f"DPNAME{i}"] = "raster scan step number"
                 header[f"DWNAME{i}"] = "helioprojective longitude"
                 header[f"DUNIT{i}"] = header[f"CUNIT{i}"]
                 # Current position in raster scan which counts from zero
```

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/conftest.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,14 +392,15 @@
     visp_solar_zone_bg_order: WavelengthParameter = WavelengthParameter(values=(21, 22, 11, 22))
     visp_solar_zone_normalization_percentile: WavelengthParameter = WavelengthParameter(
         values=(90, 99, 90, 90)
     )
     visp_solar_zone_rel_height: float = 0.97
     visp_max_cs_step_time_sec: float = 20.0
     visp_polcal_spatial_median_filter_width_px: int = 10
+    visp_polcal_num_spatial_bins: int = 5
     visp_polcal_demod_spatial_smooth_fit_order: int = 17
     visp_polcal_demod_spatial_smooth_min_samples: float = 0.9
     visp_polcal_demod_upsample_order: int = 3
     visp_pac_remove_linear_I_trend: bool = True
     visp_pac_fit_mode: str = "use_M12_I_sys_per_step"
     visp_pac_init_set: str = "OCCal_VIS"
```

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/e2e_helpers.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/e2e_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/e2e_test.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/e2e_test.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_assemble_movie.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_background_light.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_background_light.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import datetime
 import json
 
 import numpy as np
 import pytest
-import skimage.measure as skime
 from astropy.io import fits
 from dkist_data_simulator.dataset import key_function
 from dkist_data_simulator.spec122 import Spec122Dataset
 from dkist_header_validator import spec122_validator
 from dkist_header_validator.translator import translate_spec122_to_spec214_l0
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common.tests.conftest import FakeGQLClient
@@ -411,19 +410,14 @@
         except:
             raise
         finally:
             task.scratch.purge()
             task.constants._purge()
 
 
-@pytest.fixture(scope="session")
-def dummy_array() -> np.ndarray:
-    return np.random.random((100, 2560))
-
-
 def test_background_light_calibration_task(
     background_light_calibration_task, background_light, mocker
 ):
     """
     Give: a BackgroundLightCalibrationTask with a valid set of polcal data
     When: running the task
     Then: BACKGROUND intermediate frames are generated for each beam
@@ -513,42 +507,7 @@
     task()
 
     # Test that no BACKGROUND files were created
     beam_1_bg = list(task.read(tags=[VispTag.beam(1), VispTag.task("BACKGROUND")]))
     assert len(beam_1_bg) == 0
     beam_2_bg = list(task.read(tags=[VispTag.beam(2), VispTag.task("BACKGROUND")]))
     assert len(beam_2_bg) == 0
-
-
-def test_looping_spatial_resample(
-    background_light_calibration_task_non_polarimetric_dataset, dummy_array
-):
-    """
-    Given: A 3-dimensional array
-    When: Resampling the last dimension with the looping version of block_reduce in BackgroundLightCaibration
-    Then: The result is the same as calling the method on the large array all at once
-    """
-    task = background_light_calibration_task_non_polarimetric_dataset
-
-    spat_block = dummy_array.shape[-1] // task.parameters.background_num_spatial_bins
-    expected = skime.block_reduce(dummy_array, block_size=(1, spat_block), func=np.median)
-    observed = task.resample_spatial_dimension(
-        dummy_array, task.parameters.background_num_spatial_bins
-    )
-
-    assert np.array_equal(expected, observed)
-
-
-def test_looping_spatial_resample_fail_on_bad_bin_param(
-    background_light_calibration_task_non_polarimetric_dataset, dummy_array
-):
-    """
-    Given: A 3-dimensional array
-    When: Resampling the last dimension with the looping version of block_reduce in BackgroundLightCaibration
-    Then: The result is the same as calling the method on the large array all at once
-    """
-    task = background_light_calibration_task_non_polarimetric_dataset
-
-    bad_bin_number = dummy_array.shape[-1] / 2 + 1
-
-    with pytest.raises(ValueError):
-        observed = task.resample_spatial_dimension(dummy_array, bad_bin_number)
```

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_build_quality_report.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_build_quality_report.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_dark.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_geometric.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_geometric.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_instrument_polarization.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_instrument_polarization.py`

 * *Files 12% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     num_modstates = 2
     num_cs_steps = 2
     exposure_time = 0.01  # From VispHeadersValidPolcalFrames fixture
     intermediate_shape = (10, 10)
     dataset_shape = (num_cs_steps, 20, 10)
     array_shape = (1, 20, 10)
     spatial_size = array_shape[-1]
+    spectral_size = array_shape[-2] // 2  # Divide by two for a single beam
     constants_db = VispConstantsDb(
         POLARIMETER_MODE="observe_polarimetric",
         NUM_MODSTATES=num_modstates,
         NUM_BEAMS=num_beams,
         NUM_CS_STEPS=num_cs_steps,
         POLCAL_EXPOSURE_TIMES=(exposure_time,),
     )
@@ -176,15 +177,15 @@
                             VispTag.cs_step(cs_step),
                             VispTag.input(),
                             VispTag.frame(),
                             VispTag.exposure_time(exposure_time),
                         ],
                     )
 
-            yield task, quality_metric_mocker, spatial_size
+            yield task, quality_metric_mocker, spectral_size, spatial_size, num_modstates
         except:
             raise
         finally:
             task.scratch.purge()
             task.constants._purge()
 
 
@@ -219,14 +220,25 @@
 
 
 @pytest.fixture()
 def multiple_demodulation_matrices() -> np.ndarray:
     return np.arange(2 * 3 * 4 * 10).reshape(2, 3, 4, 10)
 
 
+@pytest.fixture()
+def full_spatial_beam_shape() -> tuple[int, int]:
+    return (1, 256)
+
+
+@pytest.fixture()
+def spatially_binned_demodulation_matrices(full_spatial_beam_shape) -> np.ndarray:
+    num_bins = full_spatial_beam_shape[1] // 4
+    return np.arange(1 * num_bins * 4 * 10).reshape(1, num_bins, 4, 10)
+
+
 @pytest.mark.parametrize(
     "background_on",
     [pytest.param(True, id="Background on"), pytest.param(False, id="Background off")],
 )
 def test_instrument_polarization_calibration_task(instrument_polarization_calibration_task, mocker):
     """
     Given: An InstrumentPolarizationCalibration task
@@ -235,37 +247,67 @@
     """
 
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
 
     # When
-    task, quality_mocker, spatial_size = instrument_polarization_calibration_task
+    (
+        task,
+        quality_mocker,
+        spectral_size,
+        spatial_size,
+        num_mod,
+    ) = instrument_polarization_calibration_task
     task()
 
     # Then
     for beam in [1, 2]:
         tags = [
             VispTag.intermediate(),
             VispTag.task("DEMOD_MATRICES"),
             VispTag.beam(beam),
         ]
-        assert len(list(task.read(tags=tags))) == 1
+        file_list = list(task.read(tags=tags))
+        assert len(file_list) == 1
+        hdul = fits.open(file_list[0])
+        assert len(hdul) == 1
+        data = hdul[0].data
+        assert data.shape == (spectral_size, spatial_size, 4, num_mod)
 
         quality_mocker.assert_any_call(
             polcal_fitter=ANY,
             label=f"Beam {beam}",
             bins_1=1,
-            bins_2=spatial_size,
+            bins_2=task.parameters.polcal_num_spatial_bins,
             bin_1_type="spectral",
             bin_2_type="spatial",
             skip_recording_constant_pars=beam == 2,
         )
 
 
+def test_smooth_demod_matrices(
+    instrument_polarization_calibration_task_with_no_data,
+    spatially_binned_demodulation_matrices,
+    full_spatial_beam_shape,
+):
+    """
+    Given: An InstrumentPolarizationCalibration task and a set of demod matrices binned in the spatial dimension
+    When: Smooth the demodulation matrices
+    Then: Smoothing doesn't fail and the result fully samples the full spatial dimension
+    """
+    instrument_polarization_calibration_task_with_no_data.single_beam_shape = (
+        full_spatial_beam_shape
+    )
+    result = instrument_polarization_calibration_task_with_no_data.smooth_demod_matrices(
+        spatially_binned_demodulation_matrices
+    )
+    assert result.shape == full_spatial_beam_shape + (4, 10)
+
+
 def test_reshape_demod_matrices(
     instrument_polarization_calibration_task_with_no_data,
     multiple_demodulation_matrices,
     full_beam_shape,
 ):
     """
     Given: An InstrumentPolarizationCalibration task and a set of demodulation matrices sampled over the full FOV
```

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_lamp.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_make_movie_frames.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_map_repeats.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_parameters.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_parse.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_quality.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_science.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_solar.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_submit_quality.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_submit_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_visp_base.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_visp_constants.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_visp_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/tests/test_write_l1.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp/workflows/l0_processing.py` & `dkist_processing_visp-2.1.0/dkist_processing_visp/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp.egg-info/PKG-INFO` & `dkist_processing_visp-2.1.0/dkist_processing_visp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-visp
-Version: 2.0.2
+Version: 2.1.0
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp.egg-info/SOURCES.txt` & `dkist_processing_visp-2.1.0/dkist_processing_visp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,24 +45,26 @@
 dkist_processing_visp/tasks/quality_metrics.py
 dkist_processing_visp/tasks/science.py
 dkist_processing_visp/tasks/solar.py
 dkist_processing_visp/tasks/visp_base.py
 dkist_processing_visp/tasks/write_l1.py
 dkist_processing_visp/tasks/mixin/__init__.py
 dkist_processing_visp/tasks/mixin/corrections.py
+dkist_processing_visp/tasks/mixin/downsample.py
 dkist_processing_visp/tasks/mixin/input_frame_loaders.py
 dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
 dkist_processing_visp/tests/__init__.py
 dkist_processing_visp/tests/conftest.py
 dkist_processing_visp/tests/e2e_helpers.py
 dkist_processing_visp/tests/e2e_test.py
 dkist_processing_visp/tests/test_assemble_movie.py
 dkist_processing_visp/tests/test_background_light.py
 dkist_processing_visp/tests/test_build_quality_report.py
 dkist_processing_visp/tests/test_dark.py
+dkist_processing_visp/tests/test_downsample.py
 dkist_processing_visp/tests/test_geometric.py
 dkist_processing_visp/tests/test_instrument_polarization.py
 dkist_processing_visp/tests/test_lamp.py
 dkist_processing_visp/tests/test_make_movie_frames.py
 dkist_processing_visp/tests/test_map_repeats.py
 dkist_processing_visp/tests/test_parameters.py
 dkist_processing_visp/tests/test_parse.py
```

### Comparing `dkist_processing_visp-2.0.2/dkist_processing_visp.egg-info/requires.txt` & `dkist_processing_visp-2.1.0/dkist_processing_visp.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dkist-processing-common==2.4.1
+dkist-processing-common==2.5.0
 dkist-processing-math==1.0.1
 dkist-processing-pac==2.1.0
 dkist-header-validator==3.0.5
 dkist-fits-specifications==3.6.0
 astropy==5.1.1
 numpy==1.23.1
 sunpy==4.1.4
```

### Comparing `dkist_processing_visp-2.0.2/docs/Makefile` & `dkist_processing_visp-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/docs/background_light.rst` & `dkist_processing_visp-2.1.0/docs/background_light.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/docs/conf.py` & `dkist_processing_visp-2.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/docs/gain_correction.rst` & `dkist_processing_visp-2.1.0/docs/gain_correction.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/docs/l0_to_l1_visp.rst` & `dkist_processing_visp-2.1.0/docs/l0_to_l1_visp.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/docs/make.bat` & `dkist_processing_visp-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/docs/polarization_calibration.rst` & `dkist_processing_visp-2.1.0/docs/polarization_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/docs/science_calibration.rst` & `dkist_processing_visp-2.1.0/docs/science_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/licenses/LICENSE.rst` & `dkist_processing_visp-2.1.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/pyproject.toml` & `dkist_processing_visp-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.2/setup.cfg` & `dkist_processing_visp-2.1.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [options]
 python_requires = >=3.10
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 2.4.1
+	dkist-processing-common == 2.5.0
 	dkist-processing-math == 1.0.1
 	dkist-processing-pac == 2.1.0
 	dkist-header-validator == 3.0.5
 	dkist-fits-specifications == 3.6.0
 	astropy == 5.1.1
 	numpy == 1.23.1
 	sunpy == 4.1.4
```

