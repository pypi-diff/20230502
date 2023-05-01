# Comparing `tmp/cebra-0.1.0rc3.tar.gz` & `tmp/cebra-0.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cebra-0.1.0rc3.tar", last modified: Sun Mar 19 23:28:49 2023, max compression
+gzip compressed data, was "cebra-0.2.0rc3.tar", last modified: Mon May  1 23:42:05 2023, max compression
```

## Comparing `cebra-0.1.0rc3.tar` & `cebra-0.2.0rc3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:28:49.264386 cebra-0.1.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-03-19 23:28:49.264386 cebra-0.1.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:28:49.256386 cebra-0.1.0rc3/cebra/
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:28:49.256386 cebra-0.1.0rc3/cebra/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/data/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/data/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/data/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/data/multi_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/data/single_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:28:49.256386 cebra-0.1.0rc3/cebra/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:28:49.260386 cebra-0.1.0rc3/cebra/datasets/allen/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/allen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/allen/ca_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/allen/ca_movie_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/allen/combined.py
--rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/allen/make_neuropixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/allen/neuropixel_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/allen/neuropixel_movie_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/allen/single_session_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/gaussian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/generate_synthetic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/hippocampus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/make_neuropixel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17257 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/monkey_reaching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/poisson.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/datasets/save_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:28:49.260386 cebra-0.1.0rc3/cebra/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/distributions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/distributions/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/distributions/mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/distributions/multisession.py
--rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:28:49.260386 cebra-0.1.0rc3/cebra/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/integrations/deeplabcut.py
--rw-r--r--   0 runner    (1001) docker     (123)    46351 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/integrations/matplotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:28:49.260386 cebra-0.1.0rc3/cebra/integrations/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/integrations/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55040 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/integrations/sklearn/cebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/integrations/sklearn/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/integrations/sklearn/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/integrations/sklearn/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15791 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/integrations/sklearn/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/integrations/sklearn/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:28:49.260386 cebra-0.1.0rc3/cebra/models/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/models/criterions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22210 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/models/multiobjective.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/models/projector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:28:49.264386 cebra-0.1.0rc3/cebra/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/solver/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/solver/multi_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/solver/single_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/solver/supervised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-03-19 23:28:39.000000 cebra-0.1.0rc3/cebra/solver/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:28:49.256386 cebra-0.1.0rc3/cebra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-03-19 23:28:49.000000 cebra-0.1.0rc3/cebra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-03-19 23:28:49.000000 cebra-0.1.0rc3/cebra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 23:28:49.000000 cebra-0.1.0rc3/cebra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-19 23:28:49.000000 cebra-0.1.0rc3/cebra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-19 23:28:49.000000 cebra-0.1.0rc3/cebra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-19 23:28:49.268386 cebra-0.1.0rc3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 23:28:49.264386 cebra-0.1.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_criterions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_dlc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_integration_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    23539 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    28621 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_sklearn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_sklearn_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-03-19 23:28:40.000000 cebra-0.1.0rc3/tests/test_usecases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.495751 cebra-0.2.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-01 23:42:05.495751 cebra-0.2.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.487751 cebra-0.2.0rc3/cebra/
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.487751 cebra-0.2.0rc3/cebra/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16008 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25366 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/multi_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/single_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.487751 cebra-0.2.0rc3/cebra/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.491751 cebra-0.2.0rc3/cebra/datasets/allen/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/ca_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/ca_movie_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/make_neuropixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/neuropixel_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/neuropixel_movie_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/single_session_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/gaussian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/generate_synthetic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/hippocampus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/make_neuropixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/monkey_reaching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/save_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.491751 cebra-0.2.0rc3/cebra/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/distributions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/distributions/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/distributions/mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9935 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/distributions/multisession.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21964 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.491751 cebra-0.2.0rc3/cebra/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/deeplabcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46689 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/matplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.491751 cebra-0.2.0rc3/cebra/integrations/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55181 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/sklearn/cebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/sklearn/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/sklearn/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/sklearn/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/sklearn/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/sklearn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.491751 cebra-0.2.0rc3/cebra/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/models/criterions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27878 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/models/multiobjective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/models/projector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.495751 cebra-0.2.0rc3/cebra/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/solver/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/solver/multi_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/solver/single_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/solver/supervised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/solver/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.487751 cebra-0.2.0rc3/cebra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-01 23:42:05.000000 cebra-0.2.0rc3/cebra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-01 23:42:05.000000 cebra-0.2.0rc3/cebra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:42:05.000000 cebra-0.2.0rc3/cebra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-01 23:42:05.000000 cebra-0.2.0rc3/cebra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 23:42:05.000000 cebra-0.2.0rc3/cebra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15768 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-01 23:42:05.495751 cebra-0.2.0rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.495751 cebra-0.2.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_criterions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_data_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_dlc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_integration_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23949 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29031 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_sklearn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_sklearn_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_usecases.py
```

### Comparing `cebra-0.1.0rc3/LICENSE.md` & `cebra-0.2.0rc3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cebra-0.1.0rc3/PKG-INFO` & `cebra-0.2.0rc3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cebra
-Version: 0.1.0rc3
+Version: 0.2.0rc3
 Summary: Consistent Embeddings of high-dimensional Recordings using Auxiliary variables
 Home-page: https://github.com/AdaptiveMotorControlLab/CEBRA
 Author: Steffen Schneider, Jin H Lee, Mackenzie W Mathis
 Author-email: stes@hey.com
 Project-URL: Bug Tracker, https://github.com/AdaptiveMotorControlLab/CEBRA/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -37,15 +37,15 @@
 [🚨 News](https://cebra.ai/docs/index.html) |
 [🪲 Reporting Issues](https://github.com/AdaptiveMotorControlLab/CEBRA) 
 
 
 [![Downloads](https://static.pepy.tech/badge/cebra)](https://pepy.tech/project/cebra)
 [![Downloads](https://static.pepy.tech/badge/cebra/month)](https://pepy.tech/project/cebra)
 [![PyPI version](https://badge.fury.io/py/cebra.svg)](https://badge.fury.io/py/cebra)
-![License: Non-Commerical](https://img.shields.io/badge/License-Non--commerical-lightgrey)
+![License: Non-Commercial](https://img.shields.io/badge/License-Non--commercial-lightgrey)
 ![Codecov](https://img.shields.io/codecov/c/github/AdaptiveMotorControlLab/CEBRA)
 [![Twitter Follow](https://img.shields.io/twitter/follow/CEBRAAI.svg?label=CEBRAai&style=social)](https://twitter.com/CEBRAAI)
 
 
 
 </div>
```

### Comparing `cebra-0.1.0rc3/README.md` & `cebra-0.2.0rc3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [🚨 News](https://cebra.ai/docs/index.html) |
 [🪲 Reporting Issues](https://github.com/AdaptiveMotorControlLab/CEBRA) 
 
 
 [![Downloads](https://static.pepy.tech/badge/cebra)](https://pepy.tech/project/cebra)
 [![Downloads](https://static.pepy.tech/badge/cebra/month)](https://pepy.tech/project/cebra)
 [![PyPI version](https://badge.fury.io/py/cebra.svg)](https://badge.fury.io/py/cebra)
-![License: Non-Commerical](https://img.shields.io/badge/License-Non--commerical-lightgrey)
+![License: Non-Commercial](https://img.shields.io/badge/License-Non--commercial-lightgrey)
 ![Codecov](https://img.shields.io/codecov/c/github/AdaptiveMotorControlLab/CEBRA)
 [![Twitter Follow](https://img.shields.io/twitter/follow/CEBRAAI.svg?label=CEBRAai&style=social)](https://twitter.com/CEBRAAI)
 
 
 
 </div>
```

### Comparing `cebra-0.1.0rc3/cebra/__init__.py` & `cebra-0.2.0rc3/cebra/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """CEBRA is a library for estimating Consistent Embeddings of high-dimensional Recordings 
 using Auxiliary variables. It contains self-supervised learning algorithms implemented in
 PyTorch, and has support for a variety of different datasets common in biology and neuroscience.
 """
 
 is_sklearn_available = False
 try:
@@ -22,18 +33,25 @@
 
     is_matplotlib_available = True
 except ImportError as e:
     # silently fail for now
     pass
 
 from cebra.data.load import load as load_data
-from cebra.integrations.deeplabcut import load_deeplabcut
+
+is_load_deeplabcut_available = False
+try:
+    from cebra.integrations.deeplabcut import load_deeplabcut
+    is_load_deeplabcut_available = True
+except (ImportError, NameError):
+    pass
+
 import cebra.integrations.sklearn as sklearn
 
-__version__ = "0.1.0rc3"
+__version__ = "0.2.0rc3"
 __all__ = ["CEBRA"]
 __allow_lazy_imports = False
 __lazy_imports = {}
 
 
 def allow_lazy_imports():
     """Enables lazy imports of all submodules and packages of cebra.
@@ -64,23 +82,22 @@
         return L1LinearRegressor
     elif not key.startswith("_"):
         import importlib
         import warnings
 
         if key not in __lazy_imports:
             # NOTE(celia): condition needed when testing the string examples
-            # so that the function doesn't try to import the testing packages 
-            # (pytest plugins, SetUpModule and TearDownModule) as cebra.{key}. 
+            # so that the function doesn't try to import the testing packages
+            # (pytest plugins, SetUpModule and TearDownModule) as cebra.{key}.
             # We just make sure that pytest is installed.
             if any(name in key.lower()
                    for name in ["pytest", "setup", "module"]):
                 import pytest
 
-                return importlib.import_module(
-                    pytest)
+                return importlib.import_module(pytest)
             __lazy_imports[key] = importlib.import_module(f"{__name__}.{key}")
             if not __allow_lazy_imports:
                 warnings.warn(
                     f"Your code triggered a lazy import of {__name__}.{key}. "
                     f"While this will (likely) work, it is recommended to "
                     f"add an explicit import statement to you code instead. "
                     f"To disable this warning, you can run "
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/__main__.py` & `cebra-0.2.0rc3/cebra/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """CEBRA command line interface.
 
 
 """
 
 import argparse
 import sys
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/config.py` & `cebra-0.2.0rc3/cebra/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,22 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import argparse
 import json
 from dataclasses import MISSING
-from typing import Literal
-from typing import Optional
+from typing import Literal, Optional
 
 import literate_dataclasses as dataclasses
 
 import cebra.data
 import cebra.datasets
 
 
@@ -56,15 +66,15 @@
 
     min_temperature: Optional[float] = dataclasses.field(
         default=None, doc="""Minimum temperature for learnable temperature""")
 
     time_offset: int = dataclasses.field(
         default=10,
         doc=
-        """ Distance (in time) between positive pairs. The intepretation of this parameter depends on
+        """ Distance (in time) between positive pairs. The interpretation of this parameter depends on
         the chosen conditional distribution, but generally a higher time offset increases the difficulty of
         the learning task, and (in a certain range) improves the quality of the representation. The time
         offset would typically be larger than the specified receptive field of the model.""",
     )
 
     delta: float = dataclasses.field(
         default=0.1,
@@ -129,15 +139,15 @@
         default=0.8,
         doc="""Ratio of train dataset. The remaining will be used for
         valid and test split.""",
     )
     valid_ratio: float = dataclasses.field(
         default=0.1,
         doc="""Ratio of validation set after the train data split.
-        The remaing will be test split""",
+        The remaining will be test split""",
     )
 
     @classmethod
     def _add_arguments(cls, parser, **override_kwargs):
         _metavars = {int: "N", float: "val"}
 
         def _json(self):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/data/__init__.py` & `cebra-0.2.0rc3/cebra/data/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Data loaders use distributions and indices to make samples available for training.
 
 This package contains all helper functions and classes for defining and loading datasets
 in the various usage modes of CEBRA, e.g. single- and multi-session datasets.
 It is non-specific to a particular dataset (see :py:mod:`cebra.datasets` for actual dataset
 implementations). However, the base classes for all datasets are defined here, as well as helper
 functions to interact with datasets.
@@ -12,15 +23,15 @@
   have the same feature dimension across the samples (e.g., neural data) and all context
   variables (e.g. behavior, stimuli, etc.).
 - :py:class:`cebra.data.multi_session.MultiSessionDataset` is the abstract base class for a multi session dataset.
   Multi session datasets contain of multiple single session datasets. Crucially, the dimensionality of the
   auxiliary variable dimension needs to match across the sessions, which allows alignment of multiple sessions.
   The dimensionality of the signal variable can vary arbitrarily between sessions.
 
-Note that the actual implemenation of datasets (e.g. for benchmarking) is done in the :py:mod:`cebra.datasets`
+Note that the actual implementation of datasets (e.g. for benchmarking) is done in the :py:mod:`cebra.datasets`
 package.
 
 """
 
 # NOTE(stes): intentional ordering of imports to avoid circular imports
 #             these imports will not be reordered by isort (see .isort.cfg)
 from cebra.data.base import *
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/data/base.py` & `cebra-0.2.0rc3/cebra/data/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Base classes for datasets and loaders."""
 
 import abc
 import collections
 from typing import List
 
 import literate_dataclasses as dataclasses
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/data/datasets.py` & `cebra-0.2.0rc3/cebra/data/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,24 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Pre-defined datasets."""
 
 import abc
 import collections
 import types
-from typing import List
-from typing import Tuple
-from typing import Union
+from typing import List, Tuple, Union
 
 import literate_dataclasses as dataclasses
 import numpy as np
 import numpy.typing as npt
 import torch
 from numpy.typing import NDArray
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/data/datatypes.py` & `cebra-0.2.0rc3/cebra/data/datatypes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import collections
 from typing import Tuple
 
 import torch
 
 __all__ = ["Batch", "BatchIndex", "Offset"]
 
@@ -15,15 +26,15 @@
 
     Attributes:
         reference: The reference samples, typically sampled from the prior
             distribution
         positive: The positive samples, typically sampled from the positive
             conditional distribution depending on the reference samples
         negative: The negative samples, typically sampled from the negative
-            conditional distribution depending (but often indepent) from
+            conditional distribution depending (but often independent) from
             the reference samples
         index: TODO(stes), see docs for multisession training distributions
         index_reversed: TODO(stes), see docs for multisession training distributions
     """
 
     __slots__ = ["reference", "positive", "negative", "index", "index_reversed"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/data/load.py` & `cebra-0.2.0rc3/cebra/data/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,24 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """A simple API for loading various data formats used with CEBRA."""
 
 import abc
 import pathlib
 import warnings
-from typing import IO
-from typing import List
-from typing import Optional
-from typing import Union
+from typing import IO, List, Optional, Union
 
 import numpy as np
 import numpy.typing as npt
 import torch
 
 _IS_H5PY_AVAILABLE = True
 try:
@@ -59,15 +67,16 @@
     warnings.warn(
         "scipy module was not found, be sure it is installed in your env.",
         ImportWarning,
     )
 
 _IS_DLC_INTEGRATION_AVAILABLE = True
 try:
-    from cebra.integrations.deeplabcut import load_deeplabcut
+    if _IS_PANDAS_AVAILABLE:
+        from cebra.integrations.deeplabcut import load_deeplabcut
 except ModuleNotFoundError:
     _IS_DLC_INTEGRATION_AVAILABLE = False
     warnings.warn(
         "DLC integration module was not found, be sure it is installed in your env.",
         ImportWarning,
     )
 
@@ -81,15 +90,15 @@
         key: Optional[Union[str, int]] = None,
         columns: Optional[list] = None,
     ) -> npt.NDArray:
         """Load data from file, at key.
 
         Args:
             file: The path to the given file to load, in a supported format.
-            key: The key referencing the data of interest in the file, if the file has a dictionnary-like structure.
+            key: The key referencing the data of interest in the file, if the file has a dictionary-like structure.
             columns: The part of the data to keep in the output 2D-array. For now, it corresponds to the columns of
                 a DataFrame to keep if the data selected is a DataFrame.
 
         Returns:
             The loaded data.
         """
         raise NotImplementedError()
@@ -616,15 +625,15 @@
         - if no key is provided, the first data structure found upon iteration of the collection will be loaded;
         - if a key is provided, it needs to correspond to an existing item of the collection;
         - if a key is provided, the data value accessed needs to be a data structure;
         - the function loads data for only one data structure, even if the file contains more. The function can be called again with the corresponding key to get the other ones.
 
     Args:
         file: The path to the given file to load, in a supported format.
-        key: The key referencing the data of interest in the file, if the file has a dictionnary-like structure.
+        key: The key referencing the data of interest in the file, if the file has a dictionary-like structure.
         columns: The part of the data to keep in the output 2D-array. For now, it corresponds to the columns of
             a DataFrame to keep if the data selected is a DataFrame.
 
 
     Returns:
         The loaded data.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/data/multi_session.py` & `cebra-0.2.0rc3/cebra/data/multi_session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Datasets and loaders for multi-session training."""
 
 import abc
 import collections
 from typing import List
 
 import literate_dataclasses as dataclasses
@@ -120,23 +131,14 @@
             reference=ref_idx,
             positive=pos_idx,
             negative=neg_idx,
             index=idx,
             index_reversed=idx_rev,
         )
 
-        # return [
-        #    BatchIndex(reference=ref_idx[i],
-        #               positive=pos_idx[i],
-        #               negative=neg_idx[i],
-        #               index=idx,
-        #               index_reversed=idx_rev)
-        #    for i in range(self.dataset.num_sessions)
-        # ]
-
 
 @dataclasses.dataclass
 class ContinuousMultiSessionDataLoader(MultiSessionLoader):
     """Contrastive learning conditioned on a continuous behavior variable."""
 
     conditional: str = "time_delta"
     time_offset: int = dataclasses.field(default=10)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/data/single_session.py` & `cebra-0.2.0rc3/cebra/data/single_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Datasets and loaders for single session training.
 
 All dataloaders should be implemented using ``dataclasses`` for handling
 arguments and configuration values and subclass :py:class:`.base.Loader`.
 """
 
 import abc
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/__init__.py` & `cebra-0.2.0rc3/cebra/datasets/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Pre-defined demo and benchmark datasets.
 
 This package contains actual implementations of datasets. If you want to add a commonly used (and
 public dataset) to CEBRA, this is the right package to do it. Datasets here can be loaded e.g. for testing,
 reproducing reference results and benchmarking. When contributing to this package, you should ensure
 that the data is publicly available under a suitable license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/allen/ca_movie.py` & `cebra-0.2.0rc3/cebra/datasets/allen/ca_movie.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Allen pseudomouse Ca dataset.
 
 References:
     *Deitch, Daniel, Alon Rubin, and Yaniv Ziv. "Representational drift in the mouse visual cortex." Current biology 31.19 (2021): 4327-4339.
     *de Vries, Saskia EJ, et al. "A large-scale standardized physiological survey reveals functional organization of the mouse visual cortex." Nature neuroscience 23.1 (2020): 138-151.
     *https://github.com/zivlab/visual_drift
     *http://observatory.brain-map.org/visualcoding
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/allen/ca_movie_decoding.py` & `cebra-0.2.0rc3/cebra/datasets/allen/ca_movie_decoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Allen pseudomouse Ca decoding dataset with train/test split. 
 
 References:
     *Deitch, Daniel, Alon Rubin, and Yaniv Ziv. "Representational drift in the mouse visual cortex." Current biology 31.19 (2021): 4327-4339.
     *de Vries, Saskia EJ, et al. "A large-scale standardized physiological survey reveals functional organization of the mouse visual cortex." Nature neuroscience 23.1 (2020): 138-151.
     *https://github.com/zivlab/visual_drift
     *http://observatory.brain-map.org/visualcoding
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/allen/combined.py` & `cebra-0.2.0rc3/cebra/datasets/allen/combined.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Joint Allen pseudomouse Ca/Neuropixel datasets.
 
 References:
     *Deitch, Daniel, Alon Rubin, and Yaniv Ziv. "Representational drift in the mouse visual cortex." Current biology 31.19 (2021): 4327-4339.
     *de Vries, Saskia EJ, et al. "A large-scale standardized physiological survey reveals functional organization of the mouse visual cortex." Nature neuroscience 23.1 (2020): 138-151.
     *https://github.com/zivlab/visual_drift
     *http://observatory.brain-map.org/visualcoding
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/allen/make_neuropixel.py` & `cebra-0.2.0rc3/cebra/datasets/allen/make_neuropixel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Generate pseudomouse Neuropixels data.
 
 This script generates the pseudomouse Neuropixels data for each visual cortical area from original Allen ENuropixels Brain observatory 1.1 NWB data.
 We followed the units filtering used in the AllenSDK package.
 
 References:
     *Siegle, Joshua H., et al. "Survey of spiking in the mouse visual system reveals functional hierarchy." Nature 592.7852 (2021): 86-92.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/allen/neuropixel_movie.py` & `cebra-0.2.0rc3/cebra/datasets/allen/neuropixel_movie.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Allen pseudomouse Neuropixels decoding dataset.
 
 References:
     *https://allensdk.readthedocs.io/en/latest/visual_coding_neuropixels.html
     *Siegle, Joshua H., et al. "Survey of spiking in the mouse visual system reveals functional hierarchy." Nature 592.7852 (2021): 86-92.
 
 """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/allen/neuropixel_movie_decoding.py` & `cebra-0.2.0rc3/cebra/datasets/allen/neuropixel_movie_decoding.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Allen pseudomouse Neuropixels decoding dataset with train/test split.
 
 References:
     *https://allensdk.readthedocs.io/en/latest/visual_coding_neuropixels.html
     *Siegle, Joshua H., et al. "Survey of spiking in the mouse visual system reveals functional hierarchy." Nature 592.7852 (2021): 86-92.
 
 """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/allen/single_session_ca.py` & `cebra-0.2.0rc3/cebra/datasets/allen/single_session_ca.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Allen single mouse dataset.
 
 References:
     *Deitch, Daniel, Alon Rubin, and Yaniv Ziv. "Representational drift in the mouse visual cortex." Current biology 31.19 (2021): 4327-4339.
     *de Vries, Saskia EJ, et al. "A large-scale standardized physiological survey reveals functional organization of the mouse visual cortex." Nature neuroscience 23.1 (2020): 138-151.
     *https://github.com/zivlab/visual_drift
     *http://observatory.brain-map.org/visualcoding
@@ -187,15 +198,15 @@
     A dataset of a single mouse 30Hz calcium events from the excitatory neurons in the primary visual cortex
     during the 10 repeats of the MOVIE1 stimulus in session type A. The preprocessed data from *Deitch et al. (2021) are used.
     The continuous labels corresponding to a DINO embedding of each stimulus frame.
     A neural recording during the chosen repeat is used as a test set and the remaining 9 repeats are used as a train set.
 
     Args:
         session_id: The integer value to pick a session among 4 sessions with the largest number of recorded neruons. Choose between 0-3.
-        repeat_no: The nth repeat to use as the test set. Chosse between 0-9.
+        repeat_no: The nth repeat to use as the test set. Choose between 0-9.
         split_flag: The `train`/`test` split to load.
         frame_feature_path: The path of the movie frame features.
         pca: If true, 32 principal components of the PCA transformed calcium data are used as neural input. Default value is `False`.
 
     """
 
     def __init__(
@@ -308,17 +319,15 @@
 
     def __init__(self, repeat_no, split_flag):
         super().__init__(
             *[
                 init(
                     f"allen-movie1-ca-single-session-decoding-{session_id}-repeat-{repeat_no}-{split_flag}"
                 ) for session_id in range(4)
-            ],
-            continuous=True,
-        )
+            ],)
 
 
 @parametrize(
     "allen-movie1-ca-multi-session-leave2out-repeat-{repeat_no}-{split_flag}",
     repeat_no=[0, 2, 4, 6, 8],
     split_flag=["train", "valid", "test"],
 )
@@ -326,36 +335,38 @@
 
     def __init__(self, repeat_no, split_flag):
         super().__init__(
             *[
                 init(
                     f"allen-movie1-ca-single-session-leave2out-{session_id}-repeat-{repeat_no}-{split_flag}"
                 ) for session_id in range(4)
-            ],
-            continuous=True,
-        )
+            ],)
 
 
 @parametrize(
     "allen-movie1-ca-single-session-decoding-corrupt-{session_id}-repeat-{repeat_no}-{split_flag}",
     session_id=range(len(_SINGLE_SESSION_CA)),
     repeat_no=[9],
     split_flag=["train", "test"],
 )
 class SingleSessionAllenCaDecoding(cebra.data.SingleSessionDataset):
     """A corrupted single mouse 30Hz calcium events dataset during the allen MOVIE1 stimulus with train/test splits.
 
-    A dataset of a single mouse 30Hz calcium events from the excitatory neurons in the primary visual cortex
-    during the 10 repeats of the MOVIE1 stimulus in session type A. The preprocessed data from *Deitch et al. (2021) are used.
-    The continuous labels corresponding to a DINO embedding of each stimulus frame, but in randomly shuffled order.
-    A neural recording during the chosen repeat is used as a test set and the remaining 9 repeats are used as a train set.
+    A dataset of a single mouse 30Hz calcium events from the excitatory neurons 
+    in the primary visual cortex during the 10 repeats of the MOVIE1 stimulus 
+    in session type A. The preprocessed data from *Deitch et al. (2021) are used.
+    The continuous labels corresponding to a DINO embedding of each stimulus frame, 
+    but in randomly shuffled order.
+    A neural recording during the chosen repeat is used as a test set and the 
+    remaining 9 repeats are used as a train set.
 
     Args:
-        session_id: The integer value to pick a session among 4 sessions with the largest number of recorded neruons. Choose between 0-3.
-        repeat_no: The nth repeat to use as the test set. Chosse between 0-9.
+        session_id: The integer value to pick a session among 4 sessions with the 
+            largest number of recorded neruons. Choose between 0-3.
+        repeat_no: The nth repeat to use as the test set. Choose between 0-9.
         split_flag: The `train`/`test` split to load.
         frame_feature_path: The path of the movie frame features.
 
     """
 
     def __init__(
         self,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/demo.py` & `cebra-0.2.0rc3/cebra/datasets/demo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Demo datasets for testing CEBRA.
 
 Note that none of the datasets will yield useful embeddings.
 They are exclusively meant for unit tests and benchmarking
 purposes.
 """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/gaussian_mixture.py` & `cebra-0.2.0rc3/cebra/datasets/gaussian_mixture.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 from typing import Tuple
 
 import joblib as jl
 import literate_dataclasses as dataclasses
 import numpy as np
 import sklearn
 import torch
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/generate_synthetic_data.py` & `cebra-0.2.0rc3/cebra/datasets/generate_synthetic_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Generate synthetic datasets for benchmarking embedding quality.
 
 References:
     Adapted from pi-VAE: https://github.com/zhd96/pi-vae/blob/main/code/pi_vae.py
 """
 import argparse
 import os
@@ -10,15 +21,15 @@
 import joblib as jl
 import keras
 import numpy as np
 import poisson
 import scipy.stats
 import tensorflow as tf
 
-import examples.pi_vae.code.pi_vae as pi_vae
+import third_party.pivae.pivae_code.pi_vae as pi_vae
 
 
 def simulate_cont_data_diff_var(length: int, n_dim: int, noise_func: str):
     """Generate a synthetic dataset with the chosen generative process.
 
     Adapted from pi-VAE; https://github.com/zhd96/pi-vae/blob/main/code/pi_vae.py.
     The 1D continuous label u is sampled from uniform distribution defined in [0, 2*pi].
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/hippocampus.py` & `cebra-0.2.0rc3/cebra/datasets/hippocampus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Rat hippocampus dataset
 
 References:
     * Grosmark, A.D., and Buzsáki, G. (2016). Diversity in neural firing dynamics supports both rigid and learned 
        hippocampal sequences. Science 351, 1440–1443.
     * Chen, Z., Grosmark, A.D., Penagos, H., and Wilson, M.A. (2016). Uncovering representations of sleep-associated 
        hippocampal ensemble spike activity. Sci. Rep. 6, 32193.
@@ -105,15 +116,15 @@
     split_no=[0, 1, 2],
 )
 class SingleRatTrialSplitDataset(SingleRatDataset):
     """A single rat hippocampus tetrode recording while the rat navigates on a linear track with 3-fold splits.
 
     Neural data is spike counts binned into 25ms time window and the behavior is position and the running driection (left, right) of a rat.
     The behavior label is structured as 3D array consists of position, right, and left.
-    The neural and behavior recordings are parsed into trials (a round trip from one end of the track) and the trials are split into a train, valid and test set with k=3 nested cross validataion.
+    The neural and behavior recordings are parsed into trials (a round trip from one end of the track) and the trials are split into a train, valid and test set with k=3 nested cross validation.
 
     Args:
         name: The name of a rat to use. Choose among 'achilles', 'buddy', 'cicero' and 'gatsby'.
         split_no: The `k` for k-fold split. Choose among 0, 1, 2.
         split: The split to use. Choose among 'train', 'valid', 'test', 'all', and 'wo_test'(all trials except test split).
 
     """
@@ -226,32 +237,29 @@
              split_no=[0, 1, 2])
 class MultipleRatsTrialSplitDataset(cebra.data.DatasetCollection):
     """4 rats hippocampus tetrode recording while the rat navigates on a linear track with 3-fold splits.
 
     Neural and behavior recordings of 4 rats.
     For each rat, neural data is spike counts binned into 25ms time window and the behavior is position and the running driection (left, right) of a rat.
     The behavior label is structured as 3D array consists of position, right, and left.
-    Neural and behavior recordings of each rat are parsed into trials (a round trip from one end of the track) and the trials are split into a train, valid and test set with k=3 nested cross validataion.
+    Neural and behavior recordings of each rat are parsed into trials (a round trip from one end of the track) and the trials are split into a train, valid and test set with k=3 nested cross validation.
 
     Args:
         split_no: The `k` for k-fold split. Choose among 0, 1, and 2.
         split: The split to use. Choose among 'train', 'valid', 'test', 'all', and 'wo_test'(all trials except test split).
 
     """
 
     def __init__(self, split_no=0, split=None):
         super().__init__(
             *[
                 init(f"rat-hippocampus-{name}-3fold-trial-split-{split_no}",
                      split=split)
                 for name in ["achilles", "buddy", "cicero", "gatsby"]
-            ],
-            continuous=True,
-            discrete=False,
-        )
+            ],)
         self.names = [dataset.name for dataset in self._datasets]
         self.shapes = [dataset.neural.shape for dataset in self._datasets]
         self._split = split
 
     def __repr__(self):
         return (
             f"MultipleRatsTrialSplitDataset(name: {self.names}, shape: {self.shapes})"
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/make_neuropixel.py` & `cebra-0.2.0rc3/cebra/datasets/make_neuropixel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Generate pseudomouse Neuropixels data.
 
 This script generates the pseudomouse Neuropixels data for each visual cortical area from original Allen ENuropixels Brain observatory 1.1 NWB data.
 We followed the units filtering used in the AllenSDK package.
 
 References:
     *Siegle, Joshua H., et al. "Survey of spiking in the mouse visual system reveals functional hierarchy." Nature 592.7852 (2021): 86-92.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/monkey_reaching.py` & `cebra-0.2.0rc3/cebra/datasets/monkey_reaching.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Ephys neural and behavior data used for the monkey reaching experiment. 
 
 References:
     * Chowdhury, Raeed H., Joshua I. Glaser, and Lee E. Miller. "Area 2 of primary somatosensory cortex encodes kinematics of the whole arm." Elife 9 (2020).
     * Chowdhury, Raeed; Miller, Lee (2022) Area2 Bump: macaque somatosensory area 2 spiking activity during reaching with perturbations (Version 0.220113.0359) [Data set]. `DANDI archive <https://doi.org/10.48324/dandi.000127/0.220113.0359>`_
     * Pei, Felix, et al. "Neural Latents Benchmark'21: Evaluating latent variable models of neural population activity." arXiv preprint arXiv:2109.04463 (2021).
 
@@ -121,22 +132,26 @@
     return data_dic
 
 
 @register("area2-bump")
 class Area2BumpDataset(cebra.data.SingleSessionDataset):
     """Base dataclass to generate monkey reaching datasets.
 
-    Ephys and behavior recording from -100ms and 500ms from the movement onset in 1ms bin size.
+    Ephys and behavior recording from -100ms and 500ms from the movement 
+    onset in 1ms bin size.
     Neural recording is smoothened with Gaussian kernel with 40ms std.
-    The behavior labels can include trial types, target directions and the x,y hand positions.
-    After intialization of the dataset, split method can splits the data into 'train', 'valid' and 'test' split.
+    The behavior labels can include trial types, target directions and the 
+    x,y hand positions.
+    After initialization of the dataset, split method can splits the data 
+    into 'train', 'valid' and 'test' split.
 
     Args:
         path: The path to the directory where the preloaded data is.
-        session: The trial type. Choose between 'active', 'passive', 'all', 'active-passive'.
+        session: The trial type. Choose between 'active', 'passive', 
+            'all', 'active-passive'.
 
     """
 
     def __init__(
         self,
         path: str = get_datapath("monkey_reaching_preload_smth_40/"),
         session: str = "active",
@@ -150,16 +165,18 @@
             self.load_session = session
         self.data = jl.load(os.path.join(path, f"{self.load_session}_all.jl"))
         self._post_load()
 
     def split(self, split):
         """Split the dataset.
 
-        The train trials are the same as one defined in Neural Latent Benchmark (NLB) Dataset.
-        The half of the valid trials defined in NLBDataset is used as the valid set and the other half is used as the test set.
+        The train trials are the same as one defined in Neural Latent 
+        Benchmark (NLB) Dataset.
+        The half of the valid trials defined in NLBDataset is used as 
+        the valid set and the other half is used as the test set.
 
         Args:
             split: The split. It can be either `all`, `train`, `valid`, `test`.
 
         """
 
         self.data = jl.load(
@@ -207,36 +224,41 @@
         return self.passive
 
     @property
     def continuous_index(self):
         return self.pos
 
     def __repr__(self):
-        return f"MonkeyArea2BumpDataset(name: Discrete active/passive & continuous hand position, shape: {self.neural.shape})"
+        return f"MonkeyArea2BumpDataset(name: Discrete active/passive & " \
+               f"continuous hand position, shape: {self.neural.shape})"
 
     def __getitem__(self, index):
         index = self.expand_index_in_trial(index,
                                            trial_ids=self.trial_ids,
                                            trial_borders=self.trial_borders)
         return self.neural[index].transpose(2, 1)
 
 
 @register("area2-bump-shuffled")
 class Area2BumpShuffledDataset(Area2BumpDataset):
     """Base dataclass to generate shuffled monkey reaching datasets.
 
-    Ephys and behavior recording from -100ms and 500ms from the movement onset in 1ms bin size.
+    Ephys and behavior recording from -100ms and 500ms from the movement 
+    onset in 1ms bin size.
     Neural recording is smoothened with Gaussian kernel with 40ms std.
-    The shuffled behavior labels can include trial types, target directions and the x,y hand positions.
+    The shuffled behavior labels can include trial types, target directions 
+    and the x,y hand positions.
 
-    After intialization of the dataset, split method can splits the data into 'train', 'valid' and 'test' split.
+    After initialization of the dataset, split method can splits the data 
+    into 'train', 'valid' and 'test' split.
 
     Args:
         path: The path to the directory where the preloaded data is.
-        session: The trial type. Choose between 'active', 'passive', 'all', 'active-passive'.
+        session: The trial type. Choose between 'active', 'passive', 'all', 
+            'active-passive'.
 
     """
 
     def _post_load(self):
         rng = np.random.Generator(np.random.PCG64(1))
 
         self.trial_len = int(self.data["trial_len"])
@@ -271,31 +293,34 @@
         self.trial_indices = torch.from_numpy(self.trial_indices).float()
 
 
 def _create_area2_dataset():
     """Register the monkey reaching datasets of different trial types, behavior labels.
 
     The trial types are 'active', 'passive', 'all' and 'active-passive'.
-    The 'active-passive' type distinguishes movement direction between active, passive (0-7 for active and 8-15 for passive) and 'all' does not (0-7).
+    The 'active-passive' type distinguishes movement direction between active, passive 
+    (0-7 for active and 8-15 for passive) and 'all' does not (0-7).
 
     """
 
     PATH = get_datapath("monkey_reaching_preload_smth_40")
     for session_type in ["active", "passive", "active-passive", "all"]:
 
         @register(f"area2-bump-pos-{session_type}")
         class Dataset(Area2BumpDataset):
             """Monkey reaching dataset with hand position labels.
 
             The dataset loads continuous x,y hand position as behavior labels.
-            For the 'active-passive' trial type, it additionally loads discrete binary label of active(0)/passive(1).
+            For the 'active-passive' trial type, it additionally loads discrete binary 
+            label of active(0)/passive(1).
 
             Args:
                 path: The path to the directory where the preloaded data is.
-                session: The trial type. Choose between 'active', 'passive', 'all', 'active-passive'.
+                session: The trial type. Choose between 'active', 'passive', 'all', 
+                    'active-passive'.
 
             """
 
             def __init__(self, path=PATH, session=session_type):
                 super().__init__(path=path, session=session)
 
             @property
@@ -313,15 +338,16 @@
         class Dataset(Area2BumpDataset):
             """Monkey reaching dataset with target direction labels.
 
             The dataset loads discrete target direction (0-7) as behavior labels.
 
             Args:
                 path: The path to the directory where the preloaded data is.
-                session: The trial type. Choose between 'active', 'passive', 'all', 'active-passive'.
+                session: The trial type. Choose between 'active', 'passive', 'all', 
+                    'active-passive'.
 
             """
 
             def __init__(self, path=PATH, session=session_type):
                 super().__init__(path=path, session=session)
 
             @property
@@ -335,20 +361,23 @@
             def continuous_index(self):
                 return None
 
         @register(f"area2-bump-posdir-{session_type}")
         class Dataset(Area2BumpDataset):
             """Monkey reaching dataset with hand position labels and discrete target labels.
 
-            The dataset loads continuous x,y hand position and discrete target labels (0-7) as behavior labels.
-            For active-passive type, the discrete target labels 0-7 for active and 8-16 for passive are loaded.
+            The dataset loads continuous x,y hand position and discrete target labels (0-7) 
+            as behavior labels.
+            For active-passive type, the discrete target labels 0-7 for active and 8-16 for 
+            passive are loaded.
 
             Args:
                 path: The path to the directory where the preloaded data is.
-                session: The trial type. Choose between 'active', 'passive', 'all', 'active-passive'.
+                session: The trial type. Choose between 'active', 'passive', 'all', 
+                'active-passive'.
 
             """
 
             def __init__(self, path=PATH, session=session_type):
                 super().__init__(path=path, session=session)
 
             @property
@@ -363,30 +392,33 @@
 _create_area2_dataset()
 
 
 def _create_area2_shuffled_dataset():
     """Register the shuffled monkey reaching datasets of different trial types, behavior labels.
 
     The trial types are 'active' and 'active-passive'.
-    The behavior labels are randomly shuffled and the trial types are shuffled in case of 'shuffled-trial' datasets.
+    The behavior labels are randomly shuffled and the trial types are shuffled 
+    in case of 'shuffled-trial' datasets.
 
     """
 
     PATH = get_datapath("monkey_reaching_preload_smth_40/")
     for session_type in ["active", "active-passive"]:
 
         @register(f"area2-bump-pos-{session_type}-shuffled-trial")
         class Dataset(Area2BumpShuffledDataset):
             """Monkey reaching dataset with the shuffled trial type.
 
-            The dataset loads the discrete binary trial type label active(0)/passive(1) in randomly shuffled order.
+            The dataset loads the discrete binary trial type label active(0)/passive(1) 
+            in randomly shuffled order.
 
             Args:
                 path: The path to the directory where the preloaded data is.
-                session: The trial type. Choose between 'active', 'passive', 'all', 'active-passive'.
+                session: The trial type. Choose between 'active', 'passive', 'all', 
+                    'active-passive'.
 
             """
 
             def __init__(self, path=PATH, session=session_type):
                 super().__init__(path=path, session=session)
 
             @property
@@ -401,19 +433,21 @@
                 return self.pos
 
         @register(f"area2-bump-pos-{session_type}-shuffled-position")
         class Dataset(Area2BumpShuffledDataset):
             """Monkey reaching dataset with the shuffled hand position.
 
             The dataset loads continuous x,y hand position in randomly shuffled order.
-            For the 'active-passive' trial type, it additionally loads discrete binary label of active(0)/passive(1).
+            For the 'active-passive' trial type, it additionally loads discrete binary label 
+            of active(0)/passive(1).
 
             Args:
                 path: The path to the directory where the preloaded data is.
-                session: The trial type. Choose between 'active', 'passive', 'all', 'active-passive'.
+                session: The trial type. Choose between 'active', 'passive', 'all', 
+                    'active-passive'.
 
             """
 
             def __init__(self, path=PATH, session=session_type):
                 super().__init__(path=path, session=session)
 
             @property
@@ -427,19 +461,21 @@
             def continuous_index(self):
                 return self.pos_shuffled
 
         @register(f"area2-bump-target-{session_type}-shuffled")
         class Dataset(Area2BumpShuffledDataset):
             """Monkey reaching dataset with the shuffled hand position.
 
-            The dataset loads discrete target direction (0-7 for active and 0-15 for active-passive) in randomly shuffled order.
+            The dataset loads discrete target direction (0-7 for active and 0-15 for active-passive) 
+            in randomly shuffled order.
 
             Args:
                 path: The path to the directory where the preloaded data is.
-                session: The trial type. Choose between 'active', 'passive', 'all', 'active-passive'.
+                session: The trial type. Choose between 'active', 'passive', 'all', 
+                    'active-passive'.
 
             """
 
             def __init__(self, path=PATH, session=session_type):
                 super().__init__(path=path, session=session)
 
             @property
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/poisson.py` & `cebra-0.2.0rc3/cebra/datasets/poisson.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Utilities for simulating spike counts for Poisson-like neuron models."""
 
 import dataclasses
 
 import joblib
 import numpy as np
 import scipy.stats
@@ -153,15 +164,15 @@
         deltas += refractory_period
         spike_times = np.cumsum(deltas, axis=-1)
 
         latest_spike_time = spike_times.max(axis=-1).min()
         if latest_spike_time < self.time_interval:
             raise ValueError(
                 f"The simulated number of spikes were not sufficient to complete the simulation. "
-                f"You specifed a time interval of {self.time_interval}s, but the last spike occurred "
+                f"You specified a time interval of {self.time_interval}s, but the last spike occurred "
                 f"at {latest_spike_time}s. We simulated {max_spike_count} spikes in total. "
                 f"Try to either increase data_range_sigmas (={self.data_range_sigmas}) or to decrease "
                 f"the time_interval.")
 
         return (spike_times < self.time_interval).sum(axis=-1)
 
     def sample_spikes(self, refractory_period: float = 0.0):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/datasets/save_dataset.py` & `cebra-0.2.0rc3/cebra/datasets/save_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import argparse
 import os
 
 import joblib as jl
 
 import cebra.datasets
 from cebra.datasets import get_datapath
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/distributions/__init__.py` & `cebra-0.2.0rc3/cebra/distributions/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Distributions and indexing helper functions for training CEBRA models.
 
 This package contains classes for sampling and indexing of datasets.
 Typically, the functionality of
 classes in this module is guided by the auxiliary variables of CEBRA. A dataset would pass auxiliary
 variables to a sampler, and within the sampler the *indices* of reference, negative and positive 
 samples will be sampled based on the auxiliary information. Custom ways of sampling should therefore
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/distributions/base.py` & `cebra-0.2.0rc3/cebra/distributions/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Abstract base classes for distributions and indices.
 
 Contrastive learning in CEBRA requires a prior and conditional distribution.
 Distributions are defined in terms of _indices_ that reference samples within
 the dataset.
 
 The appropriate base classes are defined in this module: An :py:class:`Index` is the
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/distributions/continuous.py` & `cebra-0.2.0rc3/cebra/distributions/continuous.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,22 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Distributions for sampling from continuously indexed datasets."""
 
+from typing import Literal, Optional
+
 import numpy as np
 import torch
 
 import cebra.data
 import cebra.distributions
 import cebra.distributions.base as abc_
 from cebra.data.datatypes import Offset
@@ -15,22 +28,25 @@
     Given the index, uniformly sample across time steps, i.e.,
     sample from the empirical distribution.
 
     Args:
         continuous: The multi-dimensional continuous index.
     """
 
-    def __init__(self, continuous, device="cpu", seed: int = 0):
+    def __init__(self,
+                 continuous: torch.Tensor,
+                 device: Literal["cpu", "cuda"] = "cpu",
+                 seed: int = 0):
         abc_.HasGenerator.__init__(self, device=device, seed=seed)
         self.continuous = continuous
         self.num_samples = len(self.continuous)
 
     def sample_prior(self,
                      num_samples: int,
-                     offset: Offset = None) -> torch.Tensor:
+                     offset: Optional[Offset] = None) -> torch.Tensor:
         """Return uniformly sampled indices.
 
         Args:
             num_samples: The number of samples to draw from the prior
                 distribution. This will be the length of the returned
                 tensor.
             offset: The :py:class:`cebra.data.datatypes.Offset` offset
@@ -73,19 +89,19 @@
     TODO:
         Implement time contrastive learning across multiple time steps, e.g.
         by sampling the time offset in the conditional distribution.
     """
 
     def __init__(
         self,
-        continuous: torch.Tensor = None,
+        continuous: Optional[torch.Tensor] = None,
         time_offset: int = 1,
-        num_samples: int = None,
-        device: str = "cpu",
-        seed: int = None,
+        num_samples: Optional[int] = None,
+        device: Literal["cpu", "cuda"] = "cpu",
+        seed: Optional[int] = None,
     ):
         abc_.HasGenerator.__init__(self, device=device, seed=seed)
         if continuous is None and num_samples is None:
             raise ValueError(
                 f"Supply either a continuous index (which will be used to infer the dataset size) "
                 f"or alternatively the number of datapoints using the num_samples argument."
             )
@@ -101,15 +117,15 @@
         if self.num_samples <= self.time_offset:
             raise ValueError(
                 f"number of samples has to exceed the time offset, but got {self.num_samples} <= {self.time_offset}."
             )
 
     def sample_prior(self,
                      num_samples: int,
-                     offset: Offset = None) -> torch.Tensor:
+                     offset: Optional[Offset] = None) -> torch.Tensor:
         """Return a random index sample, respecting the given time offset.
 
         Prior samples are uniformly sampled from ``[0, T - t)`` where ``T`` is the total
         number of samples in the index, and ``t`` is the time offset used for sampling.
 
         Args:
             num_samples: Number of time steps to draw uniformly from the
@@ -151,19 +167,19 @@
 class DirectTimedeltaDistribution(TimeContrastive, abc_.HasGenerator):
     """Look up indices with
 
     Todo:
         - This class is work in progress.
     """
 
-    def __init__(self, continuous, time_offset: int = 1):
+    def __init__(self, continuous: torch.Tensor, time_offset: int = 1):
         super().__init__(continuous=continuous, time_offset=time_offset)
         self.index = cebra.distributions.ContinuousIndex(self.data)
 
-    def sample_conditional(self, reference_idx):
+    def sample_conditional(self, reference_idx: torch.Tensor) -> torch.Tensor:
         """Samples from the conditional distribution.
 
         Todo:
             - class and this function is work in progress.
         """
         query_idx = super().sample_conditional(reference_idx)
         query = self.index[query_idx]
@@ -193,30 +209,30 @@
         distance is used in the search). A simple solution is to perform a PCA
         or ICA, or apply CEBRA first before passing the index to this function.
     """
 
     def __init__(self,
                  continuous,
                  time_delta: int = 1,
-                 device: str = "cpu",
-                 seed: int = None):
+                 device: Literal["cpu", "cuda"] = "cpu",
+                 seed: Optional[int] = None):
         abc_.HasGenerator.__init__(self, device=device, seed=seed)
         self.data = continuous
         self.time_delta = time_delta
         self.time_difference = torch.zeros_like(self.data, device=self.device)
         self.time_difference[time_delta:] = (self.data[time_delta:] -
                                              self.data[:-time_delta])
         self.index = cebra.distributions.ContinuousIndex(self.data)
         self.prior = Prior(self.data, device=device, seed=seed)
 
-    def sample_prior(self, num_samples):
+    def sample_prior(self, num_samples: int) -> torch.Tensor:
         """See :py:meth:`.Prior.sample_prior`."""
         return self.prior.sample_prior(num_samples)
 
-    def sample_conditional(self, reference_idx):
+    def sample_conditional(self, reference_idx: torch.Tensor) -> torch.Tensor:
         """Return indices from the conditional distribution."""
 
         if reference_idx.dim() != 1:
             raise ValueError(
                 f"Reference indices have wrong shape: {reference_idx.shape}. "
                 "Pass a 1D array of indices of reference samples.")
 
@@ -234,29 +250,29 @@
     Args:
         continuous: The multidimensional, continuous index
         delta: Standard deviation of Gaussian distribution to sample positive pair
 
     """
 
     def __init__(self,
-                 continuous,
+                 continuous: torch.Tensor,
                  delta: float = 0.1,
-                 device: str = "cpu",
-                 seed: int = None):
+                 device: Literal["cpu", "cuda"] = "cpu",
+                 seed: Optional[int] = None):
         abc_.HasGenerator.__init__(self, device=device, seed=seed)
         self.data = continuous
         self.std = delta
         self.index = cebra.distributions.ContinuousIndex(self.data)
         self.prior = Prior(self.data, device=device, seed=seed)
 
-    def sample_prior(self, num_samples):
+    def sample_prior(self, num_samples: int) -> torch.Tensor:
         """See :py:meth:`.Prior.sample_prior`."""
         return self.prior.sample_prior(num_samples)
 
-    def sample_conditional(self, reference_idx):
+    def sample_conditional(self, reference_idx: torch.Tensor) -> torch.Tensor:
         """Return indices from the conditional distribution."""
 
         if reference_idx.dim() != 1:
             raise ValueError(
                 f"Reference indices have wrong shape: {reference_idx.shape}. "
                 "Pass a 1D array of indices of reference samples.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/distributions/index.py` & `cebra-0.2.0rc3/cebra/distributions/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,23 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Index operations for conditional sampling.
 
 Indexing operations---in contrast to data distributions---exhibit deterministic behavior
 by returning an element closest in the dataset to a given query sample. This module contains
-helper functions for mixed and continuously indexed datsets (i.e., containing discrete and/or
+helper functions for mixed and continuously indexed datasets (i.e., containing discrete and/or
 continuous data).
 
 Discrete data has to come in the format of a single label for each datapoint. Multidimensional
 discrete labels should be converted accordingly.
 """
 
 import numpy as np
@@ -129,15 +140,15 @@
         # TODO(stes) handle offsets
         # + self.dist_matrix.offset.left
 
 
 class ConditionalIndex(cebra_distributions.Index):
     """Index a dataset based on both continuous and discrete information.
 
-    In constrast to the standard :py:class:`.base.Index` class, the :py:class:`ConditionalIndex`
+    In contrast to the standard :py:class:`.base.Index` class, the :py:class:`ConditionalIndex`
     accept both discrete and continuous indexing information.
 
     This index considers the discrete indexing information first to
     identify possible positive pairs. Then among these candidate samples,
     behaves like an :py:class:`.base.Index` and returns the samples closest in terms of
     the information in the continuous index.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/distributions/mixed.py` & `cebra-0.2.0rc3/cebra/distributions/mixed.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,25 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Distributions with a mix of continuous/discrete auxiliary variables.
 
 TODO:
     * API in this package is not yet fully stable, and the docs are quite
       sparse because of this. Extend docs/finalize API.
 """
+from typing import Literal
 
 import numpy as np
 import torch
 
 import cebra.io
 from cebra.distributions.continuous import TimedeltaDistribution
 from cebra.distributions.discrete import DiscreteUniform
@@ -33,30 +45,32 @@
         ],
     }
 
     def __init__(self):
         """Not implemented yet."""
         pass
 
-    def configure_prior(self, distribution="empirical"):
+    def configure_prior(self,
+                        distribution: Literal["empirical",
+                                              "uniform"] = "empirical"):
         """Not implemented yet."""
         pass
 
     def configure_conditional(self):
         """Not implemented yet."""
         pass
 
 
 class Mixed(cebra.io.HasDevice):
     """Distribution over behavior variables.
 
     Class combines sampling across continuous and discrete variables.
     """
 
-    def __init__(self, discrete, continuous):
+    def __init__(self, discrete: torch.Tensor, continuous: torch.Tensor):
         self.uniform_prior = False
         self.prior = DiscreteUniform(discrete)
         self.conditional = ConditionalIndex(discrete, continuous)
 
     def sample_conditional_discrete(self,
                                     discrete: torch.Tensor) -> torch.Tensor:
         """Sample conditional on the discrete samples, marginalized across continuous."""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/distributions/multisession.py` & `cebra-0.2.0rc3/cebra/distributions/multisession.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Continuous variable multi-session sampling."""
 
 import numpy as np
 import torch
 
 import cebra.distributions as cebra_distr
 import cebra.io
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/grid_search.py` & `cebra-0.2.0rc3/cebra/grid_search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,24 @@
-"""Utilties for performing a grid search across CEBRA models."""
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
+"""Utilities for performing a grid search across CEBRA models."""
 
 import copy
 import pathlib
 import pickle
-from typing import Iterable
-from typing import List
-from typing import Literal
-from typing import Optional
-from typing import Tuple
+from typing import Iterable, List, Literal, Optional, Tuple
 
 import matplotlib.axes
 import numpy as np
 import pandas as pd
 import sklearn.model_selection
 import sklearn.utils.validation as sklearn_utils_validation
 import torch
@@ -20,15 +27,15 @@
 import cebra.integrations.sklearn.cebra as cebra_sklearn_cebra
 
 
 class GridSearch:
     """Define and run a grid search on the CEBRA hyperparameters.
 
     Note:
-        We recommand that you use that grid-search implementation for rather small and simple grid-search.
+        We recommend that you use that grid-search implementation for rather small and simple grid-search.
 
     Depending on the usage, one needs to optimize some parameters used in the CEBRA model, e.g., the
     :py:attr:`~.CEBRA.temperature`, the :py:attr:`~.CEBRA.batch_size`, the :py:attr:`~.CEBRA.learning_rate`.
     A grid-search on that set of parameters consists in finding the best combination of values
     for those parameters. For that, models with different combinations of parameters are trained and the
     parameters used to get the best performing model are considered to be the optimal parameters. One can also
     define the fixed parameters, which will stay constant
@@ -50,23 +57,22 @@
             model (second returns).
 
         Example:
 
             >>> import cebra.grid_search
             >>> # 1. Define the parameters for the models
             >>> params_grid = dict(
-            ...     output_dimension = [3, 8, 16],
-            ...     learning_rate = [0.001, 0.002],
-            ...     time_offsets = [5, 10, 20],
-            ...     max_iterations = 100,
-            ...     temperature_mode = "auto",
-            ...     verbose = True)
+            ...     output_dimension = [3, 16],
+            ...     learning_rate = [0.001],
+            ...     time_offsets = 5,
+            ...     max_iterations = 10,
+            ...     verbose = False)
             >>> # 2. Define the grid search and generate the models
             >>> grid_search = cebra.grid_search.GridSearch()
-            >>> models, parameter_grid = grid_search.generate_models()
+            >>> models, parameter_grid = grid_search.generate_models(params=params_grid)
 
         """
         # determine if each param is fixed or to optimize
         fixed_params, variable_params = {}, {}
         for key in list(params.keys()):
             if not isinstance(params[key], list):  # fixed parameters
                 if (isinstance(params[key], dict) or
@@ -74,18 +80,20 @@
                         isinstance(params[key], torch.Tensor) or
                         isinstance(params[key], np.ndarray)):
                     raise ValueError(
                         f"Invalid list of variable parameters, provide a list of values, got {type(params[key])}."
                     )
                 fixed_params[key] = params[key]
             elif len(params[key]) < 2:  # fixed parameters
-                if not isinstance(params[key][0], Iterable):
+                if not isinstance(params[key][0], Iterable) or isinstance(
+                        params[key][0], str):
                     fixed_params[key] = params[key][0]
             elif not any(
-                    isinstance(params[key][i], Iterable)
+                    isinstance(params[key][i], Iterable) or
+                    isinstance(params[key][0], str)
                     for i in range(len(params[key]))):  # variable parameters
                 variable_params[key] = params[key]
             else:
                 raise ValueError(
                     f"Invalid parameter {params[key]} of type {type(params[key])}."
                 )
 
@@ -128,25 +136,28 @@
 
         Returns:
             ``self`` for chaining operations.
 
         Example:
 
             >>> import cebra.grid_search
+            >>> import numpy as np
+            >>> neural_data =  np.random.uniform(0, 1, (300, 30))
             >>> # 1. Define the parameters for the models
             >>> params_grid = dict(
-            ...     output_dimension = [3, 8, 16],
-            ...     learning_rate = [0.001, 0.002],
-            ...     time_offsets = [5, 10, 20],
-            ...     max_iterations = 100,
-            ...     temperature_mode = "auto",
-            ...     verbose = True)
+            ...     output_dimension = [3, 16],
+            ...     learning_rate = [0.001],
+            ...     time_offsets = 5,
+            ...     max_iterations = 10,
+            ...     verbose = False)
             >>> # 2. Fit the models generated from the list of parameters
             >>> grid_search = cebra.grid_search.GridSearch()
-            >>> grid_search.fit_models(datasets=neural_data, params=params_grid, models_dir="saved_models")
+            >>> grid_search = grid_search.fit_models(datasets={"neural_data": neural_data}, 
+            ...                                      params=params_grid,
+            ...                                      models_dir="grid_search_models")
 
         """
         if models_dir is not None:
             models_dir = pathlib.Path(models_dir)
             if not pathlib.Path.exists(models_dir):
                 pathlib.Path.mkdir(models_dir)
         self.models_dir = models_dir
@@ -203,37 +214,40 @@
         return self
 
     @classmethod
     def load(cls, dir: str) -> Tuple[cebra_sklearn_cebra.CEBRA, List[dict]]:
         """Load the *fitted* models and parameter grid present in ``dir``.
 
         Note:
-            It is recommanded to generate the models to iterate over by using :py:meth:`fit_models`, but you can also run
+            It is recommended to generate the models to iterate over by using :py:meth:`fit_models`, but you can also run
             the following function on a folder containing valid *fitted* models **and** the corresponding parameter grid.
 
         Args:
             dir: The directory in which the fitted models are saved.
 
         Returns:
             A dict containing the fitted models (first returns) and a list of dict containing the parameters
             used for each model present in the ``dir`` (second returns).
 
         Example:
 
             >>> import cebra.grid_search
-            >>> models, parameter_grid = cebra.grid_search.GridSearch().load(dir="saved_models")
+            >>> models, parameter_grid = cebra.grid_search.GridSearch().load(dir="grid_search_models")
+        
         """
         dir = pathlib.Path(dir)
         if not pathlib.Path.exists(dir):
             raise ValueError(
                 f"Invalid model directory, provide a directory that exists and contains the models to load, got {dir}."
             )
 
         cosine_files = []
         euclidean_files = []
+        parameter_grid = None
+        models_names = None
         for filename in pathlib.Path.iterdir(dir):
             if (str(filename).endswith(".pth") or str(filename).endswith(".pt")
                ) and not str(filename).startswith(".DS_Store"):
                 if "cosine" in str(filename):
                     cosine_files.append(pathlib.Path(filename))
                 else:
                     euclidean_files.append(pathlib.Path(filename))
@@ -301,25 +315,28 @@
         Returns:
             The :py:class:`cebra.CEBRA` model with the highest performance for a given ``dataset_name``
             (first returns) and its name (second returns).
 
         Example:
 
             >>> import cebra.grid_search
+            >>> import numpy as np
+            >>> neural_data =  np.random.uniform(0, 1, (300, 30))
             >>> # 1. Define the parameters for the models
             >>> params_grid = dict(
-            ...     output_dimension = [3, 8, 16],
-            ...     learning_rate = [0.001, 0.002],
-            ...     time_offsets = [5, 10, 20],
-            ...     max_iterations = 100,
-            ...     temperature_mode = "auto",
-            ...     verbose = True)
+            ...     output_dimension = [3, 16],
+            ...     learning_rate = [0.001],
+            ...     time_offsets = 5,
+            ...     max_iterations = 10,
+            ...     verbose = False)
             >>> # 2. Fit the models generated from the list of parameters
             >>> grid_search = cebra.grid_search.GridSearch()
-            >>> grid_search.fit_models(params=params_grid, models_dir="saved_models")
+            >>> grid_search = grid_search.fit_models(datasets={"neural_data": neural_data},
+            ...                        params=params_grid, 
+            ...                        models_dir="grid_search_models")
             >>> # 3. Get model with the best performances and use it as usual
             >>> best_model, best_model_name = grid_search.get_best_model()
             >>> embedding = best_model.transform(neural_data)
 
         """
 
         if not hasattr(self, "models_dir"):
@@ -362,25 +379,28 @@
             A :py:class:`pandas.DataFrame` in which each row corresponds to a model from the grid search
             and contains the parameters used for the model, the dataset name that was used for fitting and
             the performances obtained with that model.
 
         Example:
 
             >>> import cebra.grid_search
+            >>> import numpy as np
+            >>> neural_data =  np.random.uniform(0, 1, (300, 30))
             >>> # 1. Define the parameters for the models
             >>> params_grid = dict(
-            ...     output_dimension = [3, 8, 16],
-            ...     learning_rate = [0.001, 0.002],
-            ...     time_offsets = [5, 10, 20],
-            ...     max_iterations = 100,
-            ...     temperature_mode = "auto",
-            ...     verbose = True)
+            ...     output_dimension = [3, 16],
+            ...     learning_rate = [0.001],
+            ...     time_offsets = 5,
+            ...     max_iterations = 10,
+            ...     verbose = False)
             >>> # 2. Fit the models generated from the list of parameters
             >>> grid_search = cebra.grid_search.GridSearch()
-            >>> grid_search.fit_models(params=params_grid, models_dir="saved_models")
+            >>> grid_search = grid_search.fit_models(datasets={"neural_data": neural_data},
+            ...                        params=params_grid, 
+            ...                        models_dir="grid_search_models")
             >>> # 3. Get results for all models
             >>> df_results = grid_search.get_df_results()
 
         """
         if not hasattr(self, "models_dir"):
             if models_dir is None:
                 raise ValueError(
@@ -417,25 +437,28 @@
 
         Returns:
             A ``matplotlib.axes.Axes`` on which to generate the plot.
 
         Example:
 
             >>> import cebra.grid_search
+            >>> import numpy as np
+            >>> neural_data =  np.random.uniform(0, 1, (300, 30))
             >>> # 1. Define the parameters for the models
             >>> params_grid = dict(
-            ...     output_dimension = [3, 8, 16],
-            ...     learning_rate = [0.001, 0.002],
-            ...     time_offsets = [5, 10, 20],
-            ...     max_iterations = 100,
-            ...     temperature_mode = "auto",
-            ...     verbose = True)
+            ...     output_dimension = [3, 16],
+            ...     learning_rate = [0.001],
+            ...     time_offsets = 5,
+            ...     max_iterations = 10,
+            ...     verbose = False)
             >>> # 2. Fit the models generated from the list of parameters
             >>> grid_search = cebra.grid_search.GridSearch()
-            >>> grid_search.fit_models(params=params_grid, models_dir="saved_models")
+            >>> grid_search = grid_search.fit_models(datasets={"neural_data": neural_data},
+            ...                        params=params_grid, 
+            ...                        models_dir="grid_search_models")
             >>> # 3. Plot losses for all models
             >>> ax = grid_search.plot_loss_comparison()
 
         """
         if not hasattr(self, "models_dir"):
             if models_dir is None:
                 raise ValueError(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/helper.py` & `cebra-0.2.0rc3/cebra/helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Collection of helper functions that did not fit into own modules."""
 
 import io
 import pathlib
 import tempfile
 import urllib
 import zipfile
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/integrations/deeplabcut.py` & `cebra-0.2.0rc3/cebra/integrations/deeplabcut.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,23 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Helper functions for training embeddings on DeepLabCut outputs."""
 
 import pathlib
 import warnings
-from typing import List
-from typing import Optional
-from typing import Tuple
-from typing import Union
+from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
 
 _IS_PANDAS_AVAILABLE = True
 try:
     import pandas as pd
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/integrations/matplotlib.py` & `cebra-0.2.0rc3/cebra/integrations/matplotlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,23 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Matplotlib interface to CEBRA."""
 
 import abc
 from collections.abc import Iterable
-from typing import List
-from typing import Literal
-from typing import Optional
-from typing import Tuple
-from typing import Union
+from typing import List, Literal, Optional, Tuple, Union
 
 import matplotlib
 import matplotlib.axes
 import matplotlib.cm
 import matplotlib.colors
 import matplotlib.figure
 import matplotlib.pyplot as plt
@@ -1070,15 +1077,15 @@
     between-runs comparison. If the number of pairs still doesn't fit with that comparison, then an error is
     raised, asking the user to make sure that the formats of the scores, datasets and pairs are valid.
 
     .. tip::
         The safer way to use that function is to directly use as inputs the outputs from :py:func:`~.consistency_score`.
 
     The function makes use of :py:func:`matplotlib.pyplot.imshow` and parameters from that function can be provided as part of ``kwargs``.
-    For instance, we recommand that you bound the color bar using ``vmin`` and ``vmax``. The scores are percentages between 0 and 100.
+    For instance, we recommend that you bound the color bar using ``vmin`` and ``vmax``. The scores are percentages between 0 and 100.
 
     Args:
         scores: List of consistency scores obtained by comparing a set of CEBRA embeddings using :py:func:`~.consistency_score`.
         pairs: List of the pairs of datasets/runs whose embeddings were compared in ``scores``.
         datasets: List of the datasets whose embeddings were compared in ``scores``. Each dataset is present once only in the list.
         ax: Optional axis to create the plot on.
         cmap: Color map to use to color the m
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/integrations/sklearn/cebra.py` & `cebra-0.2.0rc3/cebra/integrations/sklearn/cebra.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Define the CEBRA model."""
 
 import copy
-from typing import Callable
-from typing import Iterable
-from typing import List
-from typing import Literal
-from typing import Optional
-from typing import Tuple
-from typing import Union
+from typing import Callable, Iterable, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
 import sklearn.utils.validation as sklearn_utils_validation
 import torch
 from sklearn.base import BaseEstimator
 from sklearn.base import ClassifierMixin
@@ -303,18 +308,14 @@
             single value, or a tuple of values to sample from uniformly. Will only have an effect if
             :py:attr:`~.conditional` is set to ``time`` or ``time_delta``.
         max_iterations (int):
             The number of iterations to train for. To pick the optimal number of iterations, start with
             a lower number (like 1,000) for faster training, and observe the value of the loss function (see
             :py:func:`~.plot_loss` to display the model loss over training). Make sure to pick a number
             of iterations high enough for the loss to converge. |Default:| ``10000``.
-        max_validation_samples (int):
-            The number of samples for evaluating the model. This parameter is only relevant for
-            the :py:func:`~.infonce_loss` method. Higher number of samples will give a more accurate estimate.
-            |Default:| ``500``.
         max_adapt_iterations (int):
             The number of samples for retraining the first layer when adapting the model to a new
             dataset. This parameter is only relevant when ``adapt=True`` in :py:meth:`cebra.CEBRA.fit`.
             |Default:| ``500``.
         batch_size (int):
             The batch size to use for training. If RAM or GPU memory allows, this parameter can be set to
             ``None`` to select batch gradient descent on the whole dataset. If you use mini-batch training,
@@ -411,15 +412,14 @@
         conditional: str = None,
         temperature: float = 1.0,
         temperature_mode: Literal["constant", "auto"] = "constant",
         min_temperature: Optional[float] = 0.1,
         time_offsets: int = 1,
         delta: float = None,
         max_iterations: int = 10000,
-        max_validation_samples: int = 500,
         max_adapt_iterations: int = 500,
         batch_size: int = None,
         learning_rate: float = 3e-4,
         optimizer: str = "adam",
         output_dimension: int = 8,
         verbose: bool = False,
         num_hidden_units: int = 32,
@@ -507,15 +507,15 @@
                 y: A list of tuple, each corresponding to the different indices of the dataset.
 
             Returns:
                 A multisession dataset.
             """
             if y is None or len(y) == 0:
                 raise RuntimeError(
-                    "No label: labels are needed for alignement in the multisession implementation."
+                    "No label: labels are needed for alignment in the multisession implementation."
                 )
 
             # TODO(celia): to make it work for multiple set of index. For now, y should be a tuple of one list only
             if isinstance(y, tuple) and len(y) > 1:
                 raise NotImplementedError(
                     f"Support for multiple set of index is not implemented in multissesion training, "
                     f"got {len(y)} sets of indexes.")
@@ -924,14 +924,16 @@
 
         """
         if callback_frequency is not None:
             if callback is None:
                 raise ValueError(
                     "callback_frequency requires to specify a callback.")
 
+        model.train()
+
         solver.fit(
             loader,
             valid_loader=None,
             save_frequency=callback_frequency,
             valid_frequency=None,
             decode=False,
             logdir=None,
@@ -1118,14 +1120,16 @@
         model, offset = self._select_model(X, session_id)
 
         # Input validation
         X = sklearn_utils.check_input_array(X, min_samples=len(self.offset_))
         input_dtype = X.dtype
 
         with torch.no_grad():
+            model.eval()
+
             if self.pad_before_transform:
                 X = np.pad(X, ((offset.left, offset.right - 1), (0, 0)),
                            mode="edge")
             X = torch.from_numpy(X).float().to(self.device_)
 
             if isinstance(model, cebra.models.ConvolutionalModelMixin):
                 # Fully convolutional evaluation, switch (T, C) -> (1, C, T)
@@ -1216,20 +1220,22 @@
             raise NotImplementedError(f"Unsupported backend: {backend}")
         checkpoint = torch.save(self, filename)
         return checkpoint
 
     @classmethod
     def load(cls,
              filename: str,
-             backend: Literal["torch"] = "torch") -> "CEBRA":
+             backend: Literal["torch"] = "torch",
+             **kwargs) -> "CEBRA":
         """Load a model from disk.
 
         Args:
             filename: The path to the file in which to save the trained model.
             backend: A string identifying the used backend.
+            kwargs: Optional keyword arguments passed directly to the loader.
 
         Return:
             The model to load.
 
         Note:
             Experimental functionality. Do not expect the save/load functionalities to be
             backward compatible yet between CEBRA versions!
@@ -1241,12 +1247,12 @@
             >>> dataset =  np.random.uniform(0, 1, (1000, 20))
             >>> loaded_model = cebra.CEBRA.load('/tmp/foo.pt')
             >>> embedding = loaded_model.transform(dataset)
 
         """
         if backend != "torch":
             raise NotImplementedError(f"Unsupported backend: {backend}")
-        model = torch.load(filename)
+        model = torch.load(filename, **kwargs)
         if not isinstance(model, cls):
             raise RuntimeError("Model loaded from file is not compatible with "
                                "the current CEBRA version.")
         return model
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/integrations/sklearn/dataset.py` & `cebra-0.2.0rc3/cebra/integrations/sklearn/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,21 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Datasets to be used as part of the sklearn framework."""
 
-from typing import Iterable
-from typing import Optional
+from typing import Iterable, Optional
 
 import numpy as np
 import numpy.typing as npt
 import torch
 
 import cebra.data
 import cebra.integrations.sklearn.utils as cebra_sklearn_utils
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/integrations/sklearn/decoder.py` & `cebra-0.2.0rc3/cebra/integrations/sklearn/decoder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Some decoders following the ``scikit-learn`` API."""
 
 import abc
-from typing import Generator
-from typing import Optional
-from typing import Tuple
-from typing import Union
+from typing import Generator, Optional, Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
 import sklearn
 import sklearn.base
 import sklearn.neighbors
 import torch
@@ -65,15 +73,15 @@
 
     Note:
         See `sklearn.neighbors.KNeighborsClassifier <https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html>`_
         and `sklearn.neighbors.KNeighborsRegressor <https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsRegressor.html>`_.
 
     Attributes:
         n_neighbors (int): An integer indicating the K number of neighbors to consider.
-        metric (str): The metric to evalute the KNN decoder's performances.
+        metric (str): The metric to evaluate the KNN decoder's performances.
 
     Examples:
 
         >>> from cebra import KNNDecoder
         >>> import numpy as np
         >>> X = np.random.uniform(0, 1, (100, 50))
         >>> y = np.random.uniform(0, 10, (100, 2))
@@ -138,15 +146,15 @@
     def iter_hyperparams() -> Generator[dict, None, None]:
         """Create sets of parameters.
 
         Note:
             It can be used for parametrized testing.
 
         Yields:
-            A dictionnary containing sets of parameters to be used for
+            A dictionary containing sets of parameters to be used for
             testing.
         """
         for n in np.power(np.arange(1, 6, dtype=int), 2):
             yield dict(n_neighbors=n, metric="cosine")
 
 
 class L1LinearRegressor(Decoder):
@@ -224,12 +232,12 @@
     def iter_hyperparams() -> Generator[dict, None, None]:
         """Create sets of parameters.
 
         Note:
             It can be used for testing.
 
         Yields:
-            A dictionnary containing sets of parameters to be used for
+            A dictionary containing sets of parameters to be used for
             testing.
         """
         for alpha in [0.001, 0.01, 0.1, 1, 10, 100]:
             yield dict(alpha=alpha)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/integrations/sklearn/helpers.py` & `cebra-0.2.0rc3/cebra/integrations/sklearn/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,19 @@
-from typing import List
-from typing import Tuple
-from typing import Union
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
+from typing import List, Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
 import torch
 
 
 def _get_min_max(
@@ -81,15 +90,15 @@
 
     Each embedding has an associated set of labels. During alignment, the labels are
     digitalized so that all sets of digitalized labels contain the same set of values.
     Then the embeddings are quantized based on the new digitalized labels.
 
     Args:
         embeddings: List of embeddings to align on the labels.
-        labels: List of labels corresponding to each embedding and to use for alignement
+        labels: List of labels corresponding to each embedding and to use for alignment
             between them.
         normalize: If True, samples of the embeddings are normalized across dimensions.
         n_bins: Number of values for the digitalized common labels.
 
     Returns:
         The embeddings aligned on the labels.
     """
@@ -116,15 +125,15 @@
             label = label.numpy()
 
         # Only keep non-NaNs values
         valid_ = np.isnan(embedding).any(axis=1)
         valid_embedding = embedding[~valid_]
         valid_labels = label[~valid_]
 
-        # Digitalize the labels so that values are contained into a common set of values
+        # Digitize the labels so that values are contained into a common set of values
         digitized_labels = np.digitize(
             valid_labels, np.linspace(min_labels_value, max_labels_value,
                                       n_bins))
 
         # quantize embedding based on the new labels
         quantized_embedding = [
             _coarse_to_fine(valid_embedding, digitized_labels, bin_idx)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/integrations/sklearn/metrics.py` & `cebra-0.2.0rc3/cebra/integrations/sklearn/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
-from typing import Iterable
-from typing import List
-from typing import Literal
-from typing import Optional
-from typing import Tuple
-from typing import Union
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
+from typing import Iterable, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
 import sklearn.linear_model
 import sklearn.utils.validation as sklearn_utils_validation
 import torch
 
@@ -16,39 +22,44 @@
 
 
 def infonce_loss(
     cebra_model: cebra_sklearn_cebra.CEBRA,
     X: Union[npt.NDArray, torch.Tensor],
     *y,
     session_id: Optional[int] = None,
+    num_batches: int = 500,
     correct_by_batchsize: bool = False,
 ) -> float:
     """Compute the InfoNCE loss on a *single session* dataset on the model.
 
     Args:
         cebra_model: The model to use to compute the InfoNCE loss on the samples.
         X: A 2D data matrix, corresponding to a *single session* recording.
         y: An arbitrary amount of continuous indices passed as 2D matrices, and up to one
             discrete index passed as a 1D array. Each index has to match the length of ``X``.
-        session_id: The session ID, an :py:class:`int` between 0 and :py:attr:`cebra.CEBRA.num_sessions` for
-            multisession, set to ``None`` for single session.
+        session_id: The session ID, an :py:class:`int` between 0 and :py:attr:`cebra.CEBRA.num_sessions`
+            for multisession, set to ``None`` for single session.
+        num_batches: The number of iterations to consider to evaluate the model on the new data.
+            Higher values will give a more accurate estimate. Set it to at least 500 iterations.
         correct_by_batchsize: If True, the loss is corrected by the batch size.
 
     Returns:
-        The average InfoNCE loss estimated over ``max_validation_samples`` samples from the data distribution.
+        The average InfoNCE loss estimated over ``num_batches`` batches from the data distribution.
 
     Example:
 
         >>> import cebra
         >>> import numpy as np
         >>> neural_data = np.random.uniform(0, 1, (1000, 20))
         >>> cebra_model = cebra.CEBRA(max_iterations=10)
         >>> cebra_model.fit(neural_data)
         CEBRA(max_iterations=10)
-        >>> loss = cebra.sklearn.metrics.infonce_loss(cebra_model, neural_data)
+        >>> loss = cebra.sklearn.metrics.infonce_loss(cebra_model, 
+        ...                                           neural_data, 
+        ...                                           num_batches=5)
 
     """
     sklearn_utils_validation.check_is_fitted(cebra_model, "n_features_")
 
     # score is computed on single session dataset only
     if isinstance(X, list) and isinstance(X[0], Iterable) and len(
             X[0].shape) == 2:
@@ -64,15 +75,15 @@
     model, _ = cebra_model._select_model(
         X, session_id)  # check session_id validity and corresponding model
     cebra_model._check_labels_types(y, session_id=session_id)
 
     dataset, is_multisession = cebra_model._prepare_data(X, y)  # single session
     loader, _ = cebra_model._prepare_loader(
         dataset,
-        max_iterations=cebra_model.max_validation_samples,
+        max_iterations=num_batches,
         is_multisession=is_multisession,
     )
 
     cebra_model._configure_for_all(dataset, model, is_multisession)
 
     solver = cebra_model.solver_
     solver.to(cebra_model.device_)
@@ -144,16 +155,16 @@
     from different datasets, so that one-to-one comparison between all provided embeddings is
     performed.
 
     Args:
         embeddings: List of embedding matrices.
         dataset_ids: List of dataset ID associated to each embedding. Multiple embeddings can be
         associated to the same dataset.
-        labels: List of labels corresponding to each embedding and to use for alignement
-        between them.
+        labels: List of labels corresponding to each embedding and to use for alignment
+            between them.
 
     Returns:
         A list of scores obtained between embeddings from different datasets (first element),
         a list of pairs of IDs corresponding to the scores (second element), and a list of the
         datasets (third element).
 
     """
@@ -293,15 +304,15 @@
     labels: Optional[List[Union[npt.NDArray, torch.Tensor]]] = None,
     dataset_ids: Optional[List[Union[int, str, float]]] = None,
 ) -> Tuple[npt.NDArray, npt.NDArray, npt.NDArray]:
     """Compute the consistency score between embeddings, either between runs or between datasets.
 
     Args:
         embeddings: List of embedding matrices.
-        labels: List of labels corresponding to each embedding and to use for alignement
+        labels: List of labels corresponding to each embedding and to use for alignment
             between them. They are only required for a between-datasets comparison.
         dataset_ids: List of dataset ID associated to each embedding. Multiple embeddings can be
             associated to the same dataset. In both modes (``runs`` or ``datasets``), if no ``dataset_ids`` is
             provided, then all the provided embeddings are compared one-to-one. Internally, the function will
             consider that the embeddings are all different runs from the same dataset for between-runs mode and
             on the contrary, that they are all computed on different dataset in the between-datasets mode.
         between: A string describing the type of comparison to perform between the embeddings, either
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/integrations/sklearn/utils.py` & `cebra-0.2.0rc3/cebra/integrations/sklearn/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import warnings
 
 import numpy.typing as npt
 import sklearn.utils.validation as sklearn_utils_validation
 import torch
 
 
@@ -10,17 +21,17 @@
 
     Note:
         If both the deprecated and new arguments are present, then an error is raised,
         else if only the deprecated argument is present, a warning is raised and the
         old argument is used in place of the new one.
 
     Args:
-        old: A dictionnary containing the deprecated arguments.
-        new: A dictionnary containing the new arguments.
-        kwargs: A dictionnary containing all the arguments.
+        old: A dictionary containing the deprecated arguments.
+        new: A dictionary containing the new arguments.
+        kwargs: A dictionary containing all the arguments.
 
     Returns:
         The updated ``kwargs`` set of arguments.
 
     """
     if kwargs[old] is None and kwargs[new] is None:  # none are present
         kwargs[new] = default
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/io.py` & `cebra-0.2.0rc3/cebra/io.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Helper classes and functions for I/O functionality."""
 
 import joblib
 import numpy as np
 import sklearn.decomposition
 import torch
 from torch import nn
@@ -74,15 +85,15 @@
         self._device = device
 
     @property
     def _initialized(self) -> bool:
         """
 
         ``True`` if the instance was either initialized upon creation via
-        passing the ``device`` option to the construtor, or later by setting
+        passing the ``device`` option to the constructor, or later by setting
         any attribute of the instance. The device of the instance will then
         be set to the first element's device.
         """
         return hasattr(self, "_modules")
 
     def _assert_initialized(self, device=None):
         if not self._initialized:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/models/criterions.py` & `cebra-0.2.0rc3/cebra/models/criterions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,33 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Criterions for contrastive learning
 
 Different criterions can be used for learning embeddings with CEBRA. The common
 interface of criterions implementing the generalized InfoNCE metric is given by
 :py:class:`BaseInfoNCE`.
 
 Criterions are available for fixed and learnable temperatures, as well as different
 similarity measures.
 
 Note that criterions can have trainable parameters, which are automatically handled
 by the training loops implemented in :py:class:`cebra.solver.base.Solver` classes.
 """
 
 import math
-from typing import Optional
-from typing import Tuple
-from typing import Union
+from typing import Optional, Tuple, Union
 
 import torch
 from torch import nn
 
 
 @torch.jit.script
 def dot_similarity(ref: torch.Tensor, pos: torch.Tensor,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/models/layers.py` & `cebra-0.2.0rc3/cebra/models/layers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Neural network layers used for building cebra models.
 
 Layers are used in the models defined in :py:mod:`.model`.
 """
 import torch
 import torch.nn.functional as F
 from torch import nn
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/models/multiobjective.py` & `cebra-0.2.0rc3/cebra/models/multiobjective.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Wrappers for using models with multiobjective solvers.
 
 .. note::
 
     Experimental as of Nov 06, 2022.
 """
 
@@ -35,15 +46,15 @@
         module: The module to wrap
         dimensions: A tuple of dimension values to extract from the model's feature embedding.
         renormalize: If True, the individual feature slices will be re-normalized before
             getting returned---this option only makes sense in conjunction with a loss based
             on the cosine distance or dot product.
         output_mode: A mode as defined in ``MultiobjectiveModel.Mode``. Overlapping means that
             when ``dimensions`` are set to `(x0, x1, ...)``, features will be extracted from
-            ``0:x0, 0:x1, ...``. When mode is set to seprate, features are extracted from
+            ``0:x0, 0:x1, ...``. When mode is set to separate, features are extracted from
             ``x0:x1, x1:x2, ...``.
         append_last_dimension: Defaults to True, and will allow to omit the last dimension in
             the ``dimensions`` argument (which should be equal to the output dimension) of the
             given model.
 
     TODO:
         - Update nn.Module type annotation for ``module`` to cebra.models.Model
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/registry.py` & `cebra-0.2.0rc3/cebra/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,33 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """A simple registry for python modules.
 
 This module only exposes a single public function, `add_helper_functions`,
 which takes a python module or module name (or package) as its argument and
 defines the decorator functions
 
 * ``register``
 * ``parametrize``
 
 and the functions
 
 * ``init`` and
 * ``get_options``
 
-within this module. It also (implicitely and lazy) initializes a singleton
+within this module. It also (implicitly and lazy) initializes a singleton
 registry object which holds all registered classes. Typically, the helper
 functions should be added in the first lines of a package ``__init__.py``
 module.
 
 Note that all functions carrying the respective decorators need to be discovered
 by the import system, otherwise they will not be available when calling ``get_options``
 or ``init``.
@@ -26,18 +37,15 @@
 
 import fnmatch
 import itertools
 import sys
 import textwrap
 import types
 import warnings
-from typing import Any
-from typing import Dict
-from typing import List
-from typing import Union
+from typing import Any, Dict, List, Union
 
 
 class _Registry:
     _instance: Dict = None
 
     @classmethod
     def get_instance(cls, module: types.ModuleType) -> _Registry:
@@ -231,15 +239,15 @@
         """Retrieve a list of registered names, optionally filtered.
 
         Args:
             pattern: A glob-like pattern (supporting wildcards ``*`` and ``?`` to
                 filter the options. Optional argument, defaults to no filtering.
             limit: An optional maximum amount of options to return, in the order
                 of finding them with the given query.
-            expand_parametrized: Whether to list classes registred with the
+            expand_parametrized: Whether to list classes registered with the
                 ``parametrize`` decorator in the options.
 
         Returns:
             All matching names. If a ``limit`` was specified, the maximum length
             is given by the limit.
         """
         return _Registry.get_options(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/solver/__init__.py` & `cebra-0.2.0rc3/cebra/solver/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Variants of CEBRA solvers for single- and multi-session training.
 
 This package contains wrappers around training loops. If you want to customize how
 different encoder models are used to transform the reference, positive and negative samples,
 how the loss functions are applied to the data, or adapt specifics on how results are logged,
 extending the classes in this package is the right way to go.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/solver/base.py` & `cebra-0.2.0rc3/cebra/solver/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,32 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """This package contains abstract base classes for different solvers.
 
 Solvers are used to package models, criterions and optimizers and implement training
 loops. When subclassing abstract solvers, in the simplest case only the
 :py:meth:`Solver._inference` needs to be overridden.
 
 For more complex use cases, the :py:meth:`Solver.step` and 
 :py:meth:`Solver.fit` method can be overridden to
 implement larger changes to the training loop.
 """
 
 import abc
 import os
-from typing import Callable
-from typing import Dict
-from typing import List
-from typing import Literal
-from typing import Optional
-from typing import Union
+from typing import Callable, Dict, List, Literal, Optional, Union
 
 import literate_dataclasses as dataclasses
 import torch
 import tqdm
 
 import cebra
 import cebra.data
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/solver/multi_session.py` & `cebra-0.2.0rc3/cebra/solver/multi_session.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,24 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Solver implementations for multi-session datasetes."""
 
 import abc
 import os
 from collections.abc import Iterable
-from typing import List
-from typing import Optional
+from typing import List, Optional
 
 import literate_dataclasses as dataclasses
 import torch
 
 import cebra
 import cebra.data
 import cebra.models
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/solver/single_session.py` & `cebra-0.2.0rc3/cebra/solver/single_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Single session solvers embed a single pair of time series."""
 
 import abc
 import copy
 import os
 from collections.abc import Iterable
 from typing import List
@@ -70,23 +81,26 @@
         """
         return self.model(data)[0].T
 
 
 @register("single-session-aux")
 @dataclasses.dataclass
 class SingleSessionAuxVariableSolver(abc_.Solver):
-    """Single session training with different processing for reference and positive/negative samples.
+    """Single session training for reference and positive/negative samples.
 
-    This solver processes reference samples with a model different from processing the positive and
-    negative samples. Requires that the ``reference_model`` is initialized to be different
-    from the ``model`` used to process the positive and negative samples.
-
-    Besides using an assymetric encoder for the same modality, this solver also allows for e.g.
-    time-contrastive learning across modalities, by using a reference model on modality A, and a different
-    model processing the signal from modality B.
+    This solver processes reference samples with a model different from 
+    processing the positive and
+    negative samples. Requires that the ``reference_model`` is initialized
+    to be different from the ``model`` used to process the positive and 
+    negative samples.
+
+    Besides using an asymmetric encoder for the same modality, this solver 
+    also allows for e.g. time-contrastive learning across modalities, by 
+    using a reference model on modality A, and a different model processing 
+    the signal from modality B.
     """
 
     _variant_name = "single-session-aux"
     reference_model: torch.nn.Module = None
 
     def __post_init__(self):
         super().__post_init__()
@@ -175,20 +189,14 @@
             return super().get_embedding(data)
         else:
             # data has shape (1, d, T)
             # output needs to be (T, d)
             return self.model(data[0].T)
 
     def _inference(self, batch: cebra.data.Batch) -> cebra.data.Batch:
-        # outputs = self.get_embedding(self.neural)
-        # return cebra.data.Batch(outputs[:-5],
-        #                        outputs[5:],
-        #                        outputs[torch.randperm(len(outputs), device = self.device)[5:]]
-        # )
-
         outputs = self.get_embedding(self.neural)
         idc = batch.positive - self.offset.left >= len(outputs)
         batch.positive[idc] = batch.reference[idc]
 
         return cebra.data.Batch(
             outputs[batch.reference - self.offset.left],
             outputs[batch.positive - self.offset.left],
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/solver/supervised.py` & `cebra-0.2.0rc3/cebra/solver/supervised.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Solvers for supervised training
 
 Note:
     It is inclear whether these will be kept. Consider the implementation
     as experimental/outdated, and the API for this particular package unstable.
 """
 import abc
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra/solver/util.py` & `cebra-0.2.0rc3/cebra/solver/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Utility functions for solvers and their training loops."""
 
 from collections.abc import Iterable
 from typing import Dict
 
 import literate_dataclasses as dataclasses
 import tqdm
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/cebra.egg-info/PKG-INFO` & `cebra-0.2.0rc3/cebra.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cebra
-Version: 0.1.0rc3
+Version: 0.2.0rc3
 Summary: Consistent Embeddings of high-dimensional Recordings using Auxiliary variables
 Home-page: https://github.com/AdaptiveMotorControlLab/CEBRA
 Author: Steffen Schneider, Jin H Lee, Mackenzie W Mathis
 Author-email: stes@hey.com
 Project-URL: Bug Tracker, https://github.com/AdaptiveMotorControlLab/CEBRA/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -37,15 +37,15 @@
 [🚨 News](https://cebra.ai/docs/index.html) |
 [🪲 Reporting Issues](https://github.com/AdaptiveMotorControlLab/CEBRA) 
 
 
 [![Downloads](https://static.pepy.tech/badge/cebra)](https://pepy.tech/project/cebra)
 [![Downloads](https://static.pepy.tech/badge/cebra/month)](https://pepy.tech/project/cebra)
 [![PyPI version](https://badge.fury.io/py/cebra.svg)](https://badge.fury.io/py/cebra)
-![License: Non-Commerical](https://img.shields.io/badge/License-Non--commerical-lightgrey)
+![License: Non-Commercial](https://img.shields.io/badge/License-Non--commercial-lightgrey)
 ![Codecov](https://img.shields.io/codecov/c/github/AdaptiveMotorControlLab/CEBRA)
 [![Twitter Follow](https://img.shields.io/twitter/follow/CEBRAAI.svg?label=CEBRAai&style=social)](https://twitter.com/CEBRAAI)
 
 
 
 </div>
```

### Comparing `cebra-0.1.0rc3/cebra.egg-info/SOURCES.txt` & `cebra-0.2.0rc3/cebra.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
-pytest.ini
 setup.cfg
 cebra/__init__.py
 cebra/__main__.py
 cebra/config.py
 cebra/grid_search.py
 cebra/helper.py
 cebra/io.py
@@ -71,14 +70,15 @@
 cebra/solver/supervised.py
 cebra/solver/util.py
 tests/_util.py
 tests/test_api.py
 tests/test_benchmark.py
 tests/test_cli.py
 tests/test_criterions.py
+tests/test_data_helper.py
 tests/test_datasets.py
 tests/test_demo.py
 tests/test_distributions.py
 tests/test_dlc.py
 tests/test_grid_search.py
 tests/test_index.py
 tests/test_integration_train.py
```

### Comparing `cebra-0.1.0rc3/cebra.egg-info/requires.txt` & `cebra-0.2.0rc3/cebra.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 coverage
 pytest
 pytest-benchmark
 pytest-xdist
 pytest-timeout
 pytest-sphinx
 tables
+licenseheaders
+codespell
 
 [docs]
 sphinx==5.3
 sphinx-gallery==0.10.1
 docutils
 pydata-sphinx-theme==0.9.0
 sphinx_autodoc_typehints==1.19
@@ -47,7 +49,8 @@
 ipykernel
 matplotlib<=3.5.2
 pandas
 seaborn
 
 [integrations]
 jupyter
+pandas
```

### Comparing `cebra-0.1.0rc3/setup.cfg` & `cebra-0.2.0rc3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 datasets = 
 	h5py
 	pandas
 	hdf5storage # for creating .mat files in new format
 	openpyxl # for excel file format loading
 integrations = 
 	jupyter
+	pandas
 docs = 
 	sphinx==5.3
 	sphinx-gallery==0.10.1
 	docutils
 	pydata-sphinx-theme==0.9.0
 	sphinx_autodoc_typehints==1.19
 	sphinx_copybutton
@@ -74,14 +75,16 @@
 	coverage
 	pytest
 	pytest-benchmark
 	pytest-xdist
 	pytest-timeout
 	pytest-sphinx
 	tables
+	licenseheaders
+	codespell
 
 [bdist_wheel]
 universal = 1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `cebra-0.1.0rc3/tests/test_benchmark.py` & `cebra-0.2.0rc3/tests/test_benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import numpy as np
 import pytest
 import sklearn
 import sklearn.metrics
 import sklearn.neighbors
 import torch
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/tests/test_criterions.py` & `cebra-0.2.0rc3/tests/test_criterions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import numpy as np
 import pytest
 import torch
 from torch import nn
 
 import cebra.models.criterions as cebra_criterions
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/tests/test_distributions.py` & `cebra-0.2.0rc3/tests/test_distributions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import functools
 
 import numpy as np
 import pytest
 import torch
 
 import cebra.datasets as cebra_datasets
```

### Comparing `cebra-0.1.0rc3/tests/test_dlc.py` & `cebra-0.2.0rc3/tests/test_dlc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import tempfile
 
 import numpy as np
 import pandas as pd
 import pytest
 
 import cebra.helper
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/tests/test_grid_search.py` & `cebra-0.2.0rc3/tests/test_grid_search.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,39 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import numpy as np
 import pytest
 
 import cebra
 import cebra.grid_search
 
 
 def test_grid_search():
     X = np.random.uniform(0, 1, (1000, 50))
     X2 = np.random.uniform(0, 1, (800, 40))
     y_c = np.random.uniform(0, 1, (1000, 10))
     y_d = np.random.randint(0, 10, (1000))
 
     params_grid = dict(
+        model_architecture=["offset10-model"],
         output_dimension=[3, 16],
         learning_rate=[0.001],
         time_offsets=10,
         max_iterations=5,
         batch_size=512,
-        verbose=True,
+        verbose=False,
     )
 
     datasets = {
         "dataset1": X,  # time contrastive learning
         "dataset2": (X, y_c),  # behavioral contrastive learning
         "dataset3": (X, y_d),  # behavioral contrastive learning
         "dataset4": (X, y_c, y_d),  # behavioral contrastive learning - hybrid
@@ -35,14 +47,16 @@
 
     models, parameters = grid_search.load("saved_models")
     assert len(models) == len(parameters)
 
     best_model, best_model_name = grid_search.get_best_model(
         dataset_name="dataset1")
     assert "dataset1" in best_model_name
+    assert best_model.__dict__["model_architecture"] == "offset10-model"
+    assert best_model.__dict__["time_offsets"] == 10
     embedding = best_model.transform(X)
     assert isinstance(embedding, np.ndarray)
 
     best_model, best_model_name = grid_search.get_best_model(
         dataset_name="dataset2")
     assert "dataset2" in best_model_name
     embedding = best_model.transform(X)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/tests/test_load.py` & `cebra-0.2.0rc3/tests/test_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import pathlib
 import pickle
 import tempfile
 
 import h5py
 import hdf5storage
 import joblib as jl
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/tests/test_loader.py` & `cebra-0.2.0rc3/tests/test_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import pytest
 import torch
 
 import cebra.data
 import cebra.io
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/tests/test_models.py` & `cebra-0.2.0rc3/tests/test_models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import itertools
 
 import pytest
 import torch
 from torch import nn
 
 import cebra.models
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/tests/test_plot.py` & `cebra-0.2.0rc3/tests/test_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import copy
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pytest
 import torch
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/tests/test_registry.py` & `cebra-0.2.0rc3/tests/test_registry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import types
 
 import pytest
 
 import cebra.registry
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/tests/test_sklearn.py` & `cebra-0.2.0rc3/tests/test_sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import itertools
 import tempfile
 import warnings
 
 import _util
 import numpy as np
 import pytest
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/tests/test_sklearn_decoder.py` & `cebra-0.2.0rc3/tests/test_sklearn_decoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import numpy as np
 import pytest
 
 import cebra.integrations.sklearn.decoder as cebra_sklearn_decoder
 
 
 def test_imports():
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/tests/test_sklearn_metrics.py` & `cebra-0.2.0rc3/tests/test_sklearn_metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import math
 
 import numpy as np
 import pytest
 import torch
 
 import cebra
@@ -12,18 +23,18 @@
 def test_imports():
     import cebra
 
     assert hasattr(cebra, "sklearn")
 
 
 def test_sklearn_infonce_loss():
+    max_loss_iterations = 2
     cebra_model = cebra_sklearn_cebra.CEBRA(
         model_architecture="offset10-model",
         max_iterations=5,
-        max_validation_samples=5,
         batch_size=128,
     )
 
     # Example data
     X = torch.tensor(np.random.uniform(0, 1, (1000, 50)))
     y_c1 = torch.tensor(np.random.uniform(0, 1, (1000, 5)))
     y_d = np.random.randint(0, 10, (1000,))
@@ -35,126 +46,175 @@
     y_d_test = np.random.randint(0, 10, (500,))
 
     # Single session
     cebra_model.fit(X, y_c1)
     score = cebra.sklearn.metrics.infonce_loss(cebra_model,
                                                X_test,
                                                y_c1_test,
-                                               session_id=0)
-    assert isinstance(score, float)
-    score = cebra.sklearn.metrics.infonce_loss(cebra_model, X_test, y_c1_test)
+                                               session_id=0,
+                                               num_batches=max_loss_iterations)
     assert isinstance(score, float)
     score = cebra.sklearn.metrics.infonce_loss(cebra_model,
                                                X_test,
                                                y_c1_test,
-                                               correct_by_batchsize=True)
+                                               num_batches=max_loss_iterations)
+    assert isinstance(score, float)
+    score = cebra.sklearn.metrics.infonce_loss(
+        cebra_model,
+        X_test,
+        y_c1_test,
+        num_batches=max_loss_iterations,
+        correct_by_batchsize=True,
+    )
     assert isinstance(score, float)
 
     with pytest.raises(RuntimeError, match="Invalid.*session_id"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model,
-                                                   X_test,
-                                                   y_c1_test,
-                                                   session_id=2)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model,
+            X_test,
+            y_c1_test,
+            num_batches=max_loss_iterations,
+            session_id=2,
+        )
     with pytest.raises(ValueError, match="Labels.*invalid"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model,
-                                                   X_test,
-                                                   y_d_test,
-                                                   session_id=0)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model,
+            X_test,
+            y_d_test,
+            num_batches=max_loss_iterations,
+            session_id=0)
     with pytest.raises(ValueError, match="Number.*index.*invalid"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model, X_test)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model, X_test, num_batches=max_loss_iterations)
     with pytest.raises(ValueError, match="Number.*index.*invalid"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model, X_test,
-                                                   y_c1_test, y_d_test)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model,
+            X_test,
+            y_c1_test,
+            y_d_test,
+            num_batches=max_loss_iterations)
     with pytest.raises(ValueError, match="Number.*index.*invalid"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model, X_test,
-                                                   y_c1_test_2, y_d_test)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model,
+            X_test,
+            y_c1_test_2,
+            y_d_test,
+            num_batches=max_loss_iterations)
 
     cebra_model.fit(X, y_d)
-    score = cebra.sklearn.metrics.infonce_loss(cebra_model, X_test, y_d_test)
+    score = cebra.sklearn.metrics.infonce_loss(cebra_model,
+                                               X_test,
+                                               y_d_test,
+                                               num_batches=max_loss_iterations)
     assert isinstance(score, float)
     score = cebra.sklearn.metrics.infonce_loss(cebra_model,
                                                X_test,
                                                y_d_test,
+                                               num_batches=max_loss_iterations,
                                                session_id=0)
     assert isinstance(score, float)
 
     with pytest.raises(RuntimeError, match="Invalid.*session_id"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model,
-                                                   X_test,
-                                                   y_d_test,
-                                                   session_id=2)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model,
+            X_test,
+            y_d_test,
+            num_batches=max_loss_iterations,
+            session_id=2)
     with pytest.raises(ValueError, match="Labels.*invalid"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model,
-                                                   X_test,
-                                                   y_c1_test,
-                                                   session_id=0)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model,
+            X_test,
+            y_c1_test,
+            num_batches=max_loss_iterations,
+            session_id=0,
+        )
     with pytest.raises(ValueError, match="Number.*index.*invalid"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model, X_test)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model, X_test, num_batches=max_loss_iterations)
 
     # Multisession
     cebra_model.fit([X, X], [y_c1, y_c1])
     score = cebra.sklearn.metrics.infonce_loss(cebra_model,
                                                X_test,
                                                y_c1_test,
+                                               num_batches=max_loss_iterations,
                                                session_id=0)
     assert isinstance(score, float)
     score = cebra.sklearn.metrics.infonce_loss(cebra_model,
                                                X_test,
                                                y_c1_test,
+                                               num_batches=max_loss_iterations,
                                                session_id=1)
     assert isinstance(score, float)
 
     with pytest.raises(ValueError, match="Labels.*invalid"):
         cebra.sklearn.metrics.infonce_loss(cebra_model,
                                            X_test,
                                            y_d_test,
+                                           num_batches=max_loss_iterations,
                                            session_id=0)
     with pytest.raises(ValueError, match="shape"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model,
-                                                   X_test_2,
-                                                   y_c1_test,
-                                                   session_id=0)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model,
+            X_test_2,
+            y_c1_test,
+            num_batches=max_loss_iterations,
+            session_id=0,
+        )
     with pytest.raises(RuntimeError, match="No.*session_id"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model, X_test,
-                                                   y_c1_test)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model, X_test, y_c1_test, num_batches=max_loss_iterations)
     with pytest.raises(RuntimeError, match="Invalid.*session_id"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model,
-                                                   X_test,
-                                                   y_c1_test,
-                                                   session_id=3)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model,
+            X_test,
+            y_c1_test,
+            num_batches=max_loss_iterations,
+            session_id=3,
+        )
     with pytest.raises(ValueError, match="Number.*index.*invalid"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model,
-                                                   X_test,
-                                                   session_id=0)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model, X_test, num_batches=max_loss_iterations, session_id=0)
     with pytest.raises(NotImplementedError, match="Data.*invalid"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model,
-                                                   [X_test, X_test_2],
-                                                   y_c1_test,
-                                                   session_id=0)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model,
+            [X_test, X_test_2],
+            y_c1_test,
+            num_batches=max_loss_iterations,
+            session_id=0,
+        )
     with pytest.raises(NotImplementedError, match="Labels.*invalid"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model,
-                                                   X_test,
-                                                   [y_c1_test, y_c1_test],
-                                                   session_id=0)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model,
+            X_test,
+            [y_c1_test, y_c1_test],
+            num_batches=max_loss_iterations,
+            session_id=0,
+        )
 
     # No batch size
     cebra_model_no_bs = cebra_sklearn_cebra.CEBRA(
         model_architecture="offset10-model",
-        max_iterations=5,
-        max_validation_samples=5,
+        max_iterations=max_loss_iterations,
         batch_size=None,
     )
 
     cebra_model_no_bs.fit(X_test)
-    score = cebra.sklearn.metrics.infonce_loss(cebra_model_no_bs, X_test)
+    score = cebra.sklearn.metrics.infonce_loss(cebra_model_no_bs,
+                                               X_test,
+                                               num_batches=max_loss_iterations)
 
     with pytest.raises(ValueError, match="Batch.*size"):
-        score = cebra.sklearn.metrics.infonce_loss(cebra_model_no_bs,
-                                                   X_test,
-                                                   correct_by_batchsize=True)
+        score = cebra.sklearn.metrics.infonce_loss(
+            cebra_model_no_bs,
+            X_test,
+            num_batches=max_loss_iterations,
+            correct_by_batchsize=True,
+        )
 
 
 def test_sklearn_consistency():
     # Example data
     np.random.seed(42)
     embedding1 = np.random.uniform(0, 1, (10000, 4))
     embedding2 = np.random.uniform(0, 1, (10000, 10))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/tests/test_solver.py` & `cebra-0.2.0rc3/tests/test_solver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 import itertools
 
 import pytest
 import torch
 from torch import nn
 
 import cebra.data
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cebra-0.1.0rc3/tests/test_usecases.py` & `cebra-0.2.0rc3/tests/test_usecases.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#
+# (c) All rights reserved. ECOLE POLYTECHNIQUE FÉDÉRALE DE LAUSANNE,
+# Switzerland, Laboratory of Prof. Mackenzie W. Mathis (UPMWMATHIS) and
+# original authors: Steffen Schneider, Jin H Lee, Mackenzie W Mathis. 2023.
+#
+# Source code:
+# https://github.com/AdaptiveMotorControlLab/CEBRA
+#
+# Please see LICENSE.md for the full license document:
+# https://github.com/AdaptiveMotorControlLab/CEBRA/LICENSE.md
+#
 """Integrations tests using various usecases via the sklearn API.
 
 All attempts to reproduce bugs in the sklearn API should be added to this
 file. Existing tests should **not** be changed to ensure backward compatibility.
 
 If breaking changes are introduced, add decorators that skip tests based on the
 cebra version we test against.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

