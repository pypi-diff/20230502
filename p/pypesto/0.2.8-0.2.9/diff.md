# Comparing `tmp/pypesto-0.2.8.tar.gz` & `tmp/pypesto-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypesto-0.2.8.tar", last modified: Thu Oct 28 18:24:19 2021, max compression
+gzip compressed data, was "pypesto-0.2.9.tar", last modified: Fri Nov  5 11:35:53 2021, max compression
```

## Comparing `pypesto-0.2.8.tar` & `pypesto-0.2.9.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 18:24:19.014243 pypesto-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2021-10-28 18:24:07.000000 pypesto-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4363 2021-10-28 18:24:19.014243 pypesto-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2021-10-28 18:24:07.000000 pypesto-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 18:24:18.994242 pypesto-0.2.8/pypesto/
--rw-r--r--   0 runner    (1001) docker     (121)      703 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 18:24:18.998242 pypesto-0.2.8/pypesto/engine/
--rw-r--r--   0 runner    (1001) docker     (121)      401 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/engine/mpi_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/engine/multi_process.py
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/engine/multi_thread.py
--rw-r--r--   0 runner    (1001) docker     (121)      763 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/engine/single_core.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/engine/task.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 18:24:18.998242 pypesto-0.2.8/pypesto/ensemble/
--rw-r--r--   0 runner    (1001) docker     (121)      705 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2602 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/ensemble/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    11728 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/ensemble/covariance_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     8991 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/ensemble/dimension_reduction.py
--rw-r--r--   0 runner    (1001) docker     (121)    39172 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/ensemble/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (121)      900 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/ensemble/task.py
--rw-r--r--   0 runner    (1001) docker     (121)    11242 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/ensemble/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 18:24:19.002242 pypesto-0.2.8/pypesto/objective/
--rw-r--r--   0 runner    (1001) docker     (121)      554 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8375 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/objective/aesara.py
--rw-r--r--   0 runner    (1001) docker     (121)     4260 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/objective/aggregated.py
--rw-r--r--   0 runner    (1001) docker     (121)    19175 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/objective/amici.py
--rw-r--r--   0 runner    (1001) docker     (121)     7637 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/objective/amici_calculator.py
--rw-r--r--   0 runner    (1001) docker     (121)    11817 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/objective/amici_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    21821 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/objective/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/objective/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    22968 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/objective/finite_difference.py
--rw-r--r--   0 runner    (1001) docker     (121)     6967 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/objective/function.py
--rw-r--r--   0 runner    (1001) docker     (121)    42462 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/objective/history.py
--rw-r--r--   0 runner    (1001) docker     (121)     4285 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/objective/pre_post_process.py
--rw-r--r--   0 runner    (1001) docker     (121)    16506 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/objective/priors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1948 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/objective/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 18:24:19.002242 pypesto-0.2.8/pypesto/optimize/
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4417 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/optimize/optimize.py
--rw-r--r--   0 runner    (1001) docker     (121)    33887 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/optimize/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1380 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/optimize/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     3719 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/optimize/result.py
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/optimize/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/optimize/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 18:24:19.002242 pypesto-0.2.8/pypesto/petab/
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/petab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23690 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/petab/importer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/petab/pysb_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 18:24:19.002242 pypesto-0.2.8/pypesto/predict/
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/predict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16882 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/predict/amici_predictor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/predict/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    11390 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/predict/result.py
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/predict/task.py
--rw-r--r--   0 runner    (1001) docker     (121)    17601 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 18:24:19.006243 pypesto-0.2.8/pypesto/profile/
--rw-r--r--   0 runner    (1001) docker     (121)      369 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/profile/approximate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3043 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/profile/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     4571 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/profile/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)    15041 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/profile/profile_next_guess.py
--rw-r--r--   0 runner    (1001) docker     (121)     5608 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/profile/result.py
--rw-r--r--   0 runner    (1001) docker     (121)     2462 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/profile/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     6769 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/profile/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     5403 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/profile/validation_intervals.py
--rw-r--r--   0 runner    (1001) docker     (121)     4118 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/profile/walk_along_profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     5247 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/result.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 18:24:19.006243 pypesto-0.2.8/pypesto/sample/
--rw-r--r--   0 runner    (1001) docker     (121)      734 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5253 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/adaptive_metropolis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/adaptive_parallel_tempering.py
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/auto_correlation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3745 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (121)     4020 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/emcee.py
--rw-r--r--   0 runner    (1001) docker     (121)     5779 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/geweke_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5176 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (121)     5140 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/parallel_tempering.py
--rw-r--r--   0 runner    (1001) docker     (121)     4065 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/pymc3.py
--rw-r--r--   0 runner    (1001) docker     (121)     3518 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/result.py
--rw-r--r--   0 runner    (1001) docker     (121)     2272 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/sample.py
--rw-r--r--   0 runner    (1001) docker     (121)     3849 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2804 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/theano.py
--rw-r--r--   0 runner    (1001) docker     (121)     2512 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/sample/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 18:24:19.010243 pypesto-0.2.8/pypesto/startpoint/
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/startpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4140 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/startpoint/assign.py
--rw-r--r--   0 runner    (1001) docker     (121)     2496 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/startpoint/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2677 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/startpoint/latin_hypercube.py
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/startpoint/uniform.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/startpoint/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 18:24:19.010243 pypesto-0.2.8/pypesto/store/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2389 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/store/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)    12689 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/store/read_from_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)    10405 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/store/save_to_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 18:24:19.014243 pypesto-0.2.8/pypesto/visualize/
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9668 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/clust_color.py
--rw-r--r--   0 runner    (1001) docker     (121)      673 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     9525 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/dimension_reduction.py
--rw-r--r--   0 runner    (1001) docker     (121)    12384 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (121)     9143 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8764 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/model_fit.py
--rw-r--r--   0 runner    (1001) docker     (121)    12848 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/optimization_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/optimizer_convergence.py
--rw-r--r--   0 runner    (1001) docker     (121)    12544 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/optimizer_history.py
--rw-r--r--   0 runner    (1001) docker     (121)    12474 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2698 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/profile_cis.py
--rw-r--r--   0 runner    (1001) docker     (121)    14910 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/profiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     5579 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/reference_points.py
--rw-r--r--   0 runner    (1001) docker     (121)    37762 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/sampling.py
--rw-r--r--   0 runner    (1001) docker     (121)     9379 2021-10-28 18:24:07.000000 pypesto-0.2.8/pypesto/visualize/waterfall.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 18:24:18.994242 pypesto-0.2.8/pypesto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4363 2021-10-28 18:24:18.000000 pypesto-0.2.8/pypesto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3141 2021-10-28 18:24:18.000000 pypesto-0.2.8/pypesto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-28 18:24:18.000000 pypesto-0.2.8/pypesto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2021-10-28 18:24:18.000000 pypesto-0.2.8/pypesto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-10-28 18:24:18.000000 pypesto-0.2.8/pypesto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-10-28 18:24:07.000000 pypesto-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2577 2021-10-28 18:24:19.014243 pypesto-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-10-28 18:24:07.000000 pypesto-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 11:35:53.547159 pypesto-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1484 2021-11-05 11:35:45.000000 pypesto-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4173 2021-11-05 11:35:53.547159 pypesto-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2488 2021-11-05 11:35:45.000000 pypesto-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 11:35:53.535159 pypesto-0.2.9/pypesto/
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 11:35:53.535159 pypesto-0.2.9/pypesto/engine/
+-rw-r--r--   0 runner    (1001) docker     (121)      401 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      579 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1541 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/engine/mpi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2057 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/engine/multi_process.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2036 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/engine/multi_thread.py
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/engine/single_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/engine/task.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 11:35:53.539159 pypesto-0.2.9/pypesto/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2629 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/ensemble/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11700 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/ensemble/covariance_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9195 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/ensemble/dimension_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39508 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/ensemble/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (121)      932 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/ensemble/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11572 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/ensemble/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1274 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 11:35:53.539159 pypesto-0.2.9/pypesto/objective/
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8728 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/objective/aesara.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4677 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/objective/aggregated.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19638 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/objective/amici.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7675 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/objective/amici_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11814 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/objective/amici_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22259 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/objective/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      810 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/objective/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23429 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/objective/finite_difference.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7314 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/objective/function.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44676 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/objective/history.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4358 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/objective/pre_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16592 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/objective/priors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1957 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/objective/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 11:35:53.539159 pypesto-0.2.9/pypesto/optimize/
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4981 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/optimize/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35431 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/optimize/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1936 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/optimize/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3723 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/optimize/result.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2135 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/optimize/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3071 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/optimize/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 11:35:53.539159 pypesto-0.2.9/pypesto/petab/
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/petab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23792 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/petab/importer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1408 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/petab/pysb_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 11:35:53.543159 pypesto-0.2.9/pypesto/predict/
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/predict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16847 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/predict/amici_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2023 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/predict/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11649 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/predict/result.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1289 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/predict/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18029 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 11:35:53.543159 pypesto-0.2.9/pypesto/profile/
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3600 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/profile/approximate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3093 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/profile/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4970 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/profile/profile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15009 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/profile/profile_next_guess.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5625 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/profile/result.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2467 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/profile/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6860 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/profile/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5356 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/profile/validation_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4101 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/profile/walk_along_profile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5224 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/result.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 11:35:53.543159 pypesto-0.2.9/pypesto/sample/
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5340 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/adaptive_metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1375 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/adaptive_parallel_tempering.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1745 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/auto_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3804 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4143 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/emcee.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5813 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/geweke_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6047 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5254 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/parallel_tempering.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4794 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/pymc3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3586 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/result.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2669 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/sample.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3837 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2972 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/theano.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2513 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/sample/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 11:35:53.547159 pypesto-0.2.9/pypesto/startpoint/
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/startpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4144 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/startpoint/assign.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2546 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/startpoint/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2732 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/startpoint/latin_hypercube.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1291 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/startpoint/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/startpoint/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 11:35:53.547159 pypesto-0.2.9/pypesto/store/
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2381 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/store/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12692 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/store/read_from_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10565 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/store/save_to_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 11:35:53.547159 pypesto-0.2.9/pypesto/visualize/
+-rw-r--r--   0 runner    (1001) docker     (121)     1582 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9656 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/clust_color.py
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9582 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/dimension_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12509 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9079 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9079 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/model_fit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12828 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/optimization_stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1905 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/optimizer_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12478 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/optimizer_history.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12438 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2698 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/profile_cis.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15024 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5605 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/reference_points.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37277 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9233 2021-11-05 11:35:45.000000 pypesto-0.2.9/pypesto/visualize/waterfall.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 11:35:53.535159 pypesto-0.2.9/pypesto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4173 2021-11-05 11:35:53.000000 pypesto-0.2.9/pypesto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3141 2021-11-05 11:35:53.000000 pypesto-0.2.9/pypesto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-05 11:35:53.000000 pypesto-0.2.9/pypesto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1477 2021-11-05 11:35:53.000000 pypesto-0.2.9/pypesto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-11-05 11:35:53.000000 pypesto-0.2.9/pypesto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2021-11-05 11:35:45.000000 pypesto-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2617 2021-11-05 11:35:53.547159 pypesto-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2021-11-05 11:35:45.000000 pypesto-0.2.9/setup.py
```

### Comparing `pypesto-0.2.8/LICENSE` & `pypesto-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypesto-0.2.8/PKG-INFO` & `pypesto-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypesto
-Version: 0.2.8
+Version: 0.2.9
 Summary: python-based Parameter EStimation TOolbox
 Home-page: https://github.com/icb-dcm/pypesto
 Author: The pyPESTO developers
 Author-email: yannik.schaelte@gmail.com,jakob.vanhoefer@uni-bonn.de
 Maintainer: Yannik Schaelte, Jakob Vanhoefer
 Maintainer-email: yannik.schaelte@gmail.com,jakob.vanhoefer@uni-bonn.de
 License: BSD-3-Clause
@@ -14,18 +14,19 @@
 Project-URL: Changelog, https://pypesto.readthedocs.io/en/latest/changelog.html
 Keywords: parameter inference,optimization,sampling,profiles,ODE,AMICI,systems biology
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: all_optimizers
 Provides-Extra: amici
 Provides-Extra: petab
 Provides-Extra: ipopt
 Provides-Extra: dlib
@@ -51,15 +52,14 @@
 
 **pyPESTO** is a widely applicable and highly customizable toolbox for
 parameter estimation.
 
 [![PyPI](https://badge.fury.io/py/pypesto.svg)](https://badge.fury.io/py/pypesto)
 [![CI](https://github.com/ICB-DCM/pyPESTO/workflows/CI/badge.svg)](https://github.com/ICB-DCM/pyPESTO/actions)
 [![Coverage](https://codecov.io/gh/ICB-DCM/pyPESTO/branch/master/graph/badge.svg)](https://codecov.io/gh/ICB-DCM/pyPESTO)
-[![Quality](https://api.codacy.com/project/badge/Grade/134432ddad0e464b8494587ff370f661)](https://www.codacy.com/app/dweindl/pyPESTO?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ICB-DCM/pyPESTO&amp;utm_campaign=Badge_Grade)
 [![Documentation](https://readthedocs.org/projects/pypesto/badge/?version=latest)](https://pypesto.readthedocs.io)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2553546.svg)](https://doi.org/10.5281/zenodo.2553546)
 
 ## Feature overview
 
 pyPESTO features include:
```

### Comparing `pypesto-0.2.8/README.md` & `pypesto-0.2.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 **pyPESTO** is a widely applicable and highly customizable toolbox for
 parameter estimation.
 
 [![PyPI](https://badge.fury.io/py/pypesto.svg)](https://badge.fury.io/py/pypesto)
 [![CI](https://github.com/ICB-DCM/pyPESTO/workflows/CI/badge.svg)](https://github.com/ICB-DCM/pyPESTO/actions)
 [![Coverage](https://codecov.io/gh/ICB-DCM/pyPESTO/branch/master/graph/badge.svg)](https://codecov.io/gh/ICB-DCM/pyPESTO)
-[![Quality](https://api.codacy.com/project/badge/Grade/134432ddad0e464b8494587ff370f661)](https://www.codacy.com/app/dweindl/pyPESTO?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ICB-DCM/pyPESTO&amp;utm_campaign=Badge_Grade)
 [![Documentation](https://readthedocs.org/projects/pypesto/badge/?version=latest)](https://pypesto.readthedocs.io)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2553546.svg)](https://doi.org/10.5281/zenodo.2553546)
 
 ## Feature overview
 
 pyPESTO features include:
```

### Comparing `pypesto-0.2.8/pypesto/__init__.py` & `pypesto-0.2.9/pypesto/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: D400,D205
 """
 pyPESTO
 =======
 
 Parameter Estimation TOolbox for python.
 """
```

### Comparing `pypesto-0.2.8/pypesto/engine/base.py` & `pypesto-0.2.9/pypesto/engine/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
+"""Abstract engine base class."""
 from typing import List
 import abc
 
 from .task import Task
 
 
 class Engine(abc.ABC):
-    """
-    Abstract engine base class.
-    """
+    """Abstract engine base class."""
 
     def __init__(self):
         pass
 
     @abc.abstractmethod
     def execute(self, tasks: List[Task], progress_bar: bool = True):
         """Execute tasks.
```

### Comparing `pypesto-0.2.8/pypesto/engine/mpi_pool.py` & `pypesto-0.2.9/pypesto/engine/mpi_pool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Engines with multi-node parallelization."""
 from mpi4py.futures import MPIPoolExecutor
 from mpi4py import MPI
 import cloudpickle as pickle
 import logging
 from tqdm import tqdm
 
 from typing import List
@@ -17,35 +18,35 @@
     """Unpickle and execute task."""
     task = pickle.loads(pickled_task)
     return task.execute()
 
 
 class MPIPoolEngine(Engine):
     """
-    Parallelize the task execution using
-    `mpi4py <https://mpi4py.readthedocs.io/en/stable/>`_.
+    Parallelize the task execution.
 
+    Uses `mpi4py <https://mpi4py.readthedocs.io/en/stable/>`_.
     To be called with:
     ``mpiexec -np #Workers+1 python -m mpi4py.futures YOURFILE.py``
     """
 
     def __init__(self):
         super().__init__()
 
     def execute(self, tasks: List[Task], progress_bar: bool = True):
-        """Pickle tasks and distribute work to workers.
+        """
+        Pickle tasks and distribute work to workers.
 
         Parameters
         ----------
         tasks:
             List of tasks to execute.
         progress_bar:
             Whether to display a progress bar.
         """
-
         pickled_tasks = [pickle.dumps(task) for task in tasks]
 
         n_procs = MPI.COMM_WORLD.Get_size()   # Size of communicator
         logger.info(f"Performing parallel task execution on {n_procs-1} "
                     f"workers with one manager.")
 
         with MPIPoolExecutor() as executor:
```

### Comparing `pypesto-0.2.8/pypesto/engine/multi_process.py` & `pypesto-0.2.9/pypesto/engine/multi_process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Engines with multi-process parallelization."""
 from multiprocessing import Pool
 import cloudpickle as pickle
 import os
 import logging
 from typing import List
 from tqdm import tqdm
```

### Comparing `pypesto-0.2.8/pypesto/engine/multi_thread.py` & `pypesto-0.2.9/pypesto/engine/multi_thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Engines with multi-threading parallelization."""
 from concurrent.futures import ThreadPoolExecutor
 import copy
 import os
 import logging
 from tqdm import tqdm
 from typing import List
```

### Comparing `pypesto-0.2.8/pypesto/engine/single_core.py` & `pypesto-0.2.9/pypesto/engine/single_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+"""Engines without parallelization."""
 from typing import List
 from tqdm import tqdm
 
 from .base import Engine
 from .task import Task
 
 
 class SingleCoreEngine(Engine):
     """
-    Dummy engine for sequential execution on one core. Note that the
-    objective itself may be multithreaded.
+    Dummy engine for sequential execution on one core.
+
+    Note that the objective itself may be multithreaded.
     """
 
     def __init__(self):
         super().__init__()
 
     def execute(self, tasks: List[Task], progress_bar: bool = True):
         """Execute all tasks in a simple for loop sequentially.
```

### Comparing `pypesto-0.2.8/pypesto/ensemble/__init__.py` & `pypesto-0.2.9/pypesto/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.2.8/pypesto/ensemble/constants.py` & `pypesto-0.2.9/pypesto/ensemble/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-This is for (string) constants used in the ensemble module.
-"""
+"""Constants used in the ensemble module."""
 
 
 from enum import Enum
 from typing import Union
 
 from ..predict.constants import (  # noqa: F401
     OUTPUT,
@@ -53,14 +51,16 @@
 
 COLOR_HIT_BOTH_BOUNDS = [0.6, 0., 0., 0.9]
 COLOR_HIT_ONE_BOUND = [0.95, 0.6, 0., 0.9]
 COLOR_HIT_NO_BOUNDS = [0., 0.8, 0., 0.9]
 
 
 class EnsembleType(Enum):
+    """Class to specify the type of ensemble."""
+
     ensemble = 1
     sample = 2
     unprocessed_chain = 3
 
 
 def get_percentile_label(percentile: Union[float, int, str]) -> str:
     """Convert a percentile to a label.
```

### Comparing `pypesto-0.2.8/pypesto/ensemble/covariance_analysis.py` & `pypesto-0.2.9/pypesto/ensemble/covariance_analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,49 +6,46 @@
 
 
 def get_covariance_matrix_parameters(ens: Ensemble) -> np.ndarray:
     """
     Compute the covariance of ensemble parameters.
 
     Parameters
-    ==========
+    ----------
     ens:
         Ensemble object containing a set of parameter vectors
 
     Returns
-    =======
+    -------
     covariance_matrix:
         covariance matrix of ensemble parameters
     """
-
     # call lowlevel routine using the parameter ensemble
     return np.cov(ens.x_vectors.transpose())
 
 
 def get_covariance_matrix_predictions(
         ens: Union[Ensemble, EnsemblePrediction],
         prediction_index: int = 0) -> np.ndarray:
     """
     Compute the covariance of ensemble predictions.
 
     Parameters
-    ==========
+    ----------
     ens:
         Ensemble object containing a set of parameter vectors and a set of
         predictions or EnsemblePrediction object containing only predictions
-
     prediction_index:
         index telling which prediction from the list should be analyzed
 
     Returns
-    =======
+    -------
     covariance_matrix:
         covariance matrix of ensemble predictions
     """
-
     # extract the an array of predictions from either an Ensemble object or an
     # EnsemblePrediction object
     dataset = get_prediction_dataset(ens, prediction_index)
 
     # call lowlevel routine using the prediction ensemble
     return np.cov(dataset)
 
@@ -63,54 +60,46 @@
         cutoff_absolute_identifiable: float = 1e-16,
         cutoff_relative_identifiable: float = 1e-16
 ) -> Tuple[np.ndarray, np.ndarray]:
     """
     Compute the spectral decomposition of ensemble parameters.
 
     Parameters
-    ==========
+    ----------
     ens:
         Ensemble object containing a set of parameter vectors
-
     normalize:
         flag indicating whether the returned Eigenvalues should be normalized
         with respect to the largest Eigenvalue
-
     only_separable_directions:
         return only separable directions according to
         cutoff_[absolute/relative]_separable
-
     cutoff_absolute_separable:
         Consider only eigenvalues of the covariance matrix above this cutoff
         (only applied when only_separable_directions is True)
-
     cutoff_relative_separable:
         Consider only eigenvalues of the covariance matrix above this cutoff,
         when rescaled with the largest eigenvalue
         (only applied when only_separable_directions is True)
-
     only_identifiable_directions:
         return only identifiable directions according to
         cutoff_[absolute/relative]_identifiable
-
     cutoff_absolute_identifiable:
         Consider only low eigenvalues of the covariance matrix with inverses
         above of this cutoff
         (only applied when only_identifiable_directions is True)
-
     cutoff_relative_identifiable:
         Consider only low eigenvalues of the covariance matrix when rescaled
         with the largest eigenvalue with inverses above of this cutoff
         (only applied when only_identifiable_directions is True)
 
     Returns
-    =======
+    -------
     eigenvalues:
         Eigenvalues of the covariance matrix
-
     eigenvectors:
         Eigenvectors of the covariance matrix
     """
     # check inputs
     if sum([only_identifiable_directions, only_separable_directions]) >= 2:
         raise AssertionError(
             "Specify either only identifiable or only separable directions.")
@@ -136,55 +125,47 @@
         cutoff_absolute_identifiable: float = 1e-16,
         cutoff_relative_identifiable: float = 1e-16
 ) -> Tuple[np.ndarray, np.ndarray]:
     """
     Compute the spectral decomposition of ensemble predictions.
 
     Parameters
-    ==========
+    ----------
     ens:
         Ensemble object containing a set of parameter vectors and a set of
         predictions or EnsemblePrediction object containing only predictions
-
     normalize:
         flag indicating whether the returned Eigenvalues should be normalized
         with respect to the largest Eigenvalue
-
     only_separable_directions:
         return only separable directions according to
         cutoff_[absolute/relative]_separable
-
     cutoff_absolute_separable:
         Consider only eigenvalues of the covariance matrix above this cutoff
         (only applied when only_separable_directions is True)
-
     cutoff_relative_separable:
         Consider only eigenvalues of the covariance matrix above this cutoff,
         when rescaled with the largest eigenvalue
         (only applied when only_separable_directions is True)
-
     only_identifiable_directions:
         return only identifiable directions according to
         cutoff_[absolute/relative]_identifiable
-
     cutoff_absolute_identifiable:
         Consider only low eigenvalues of the covariance matrix with inverses
         above of this cutoff
         (only applied when only_identifiable_directions is True)
-
     cutoff_relative_identifiable:
         Consider only low eigenvalues of the covariance matrix when rescaled
         with the largest eigenvalue with inverses above of this cutoff
         (only applied when only_identifiable_directions is True)
 
     Returns
-    =======
+    -------
     eigenvalues:
         Eigenvalues of the covariance matrix
-
     eigenvectors:
         Eigenvectors of the covariance matrix
     """
     covariance = get_covariance_matrix_predictions(ens)
     return get_spectral_decomposition_lowlevel(
         matrix=covariance, normalize=normalize,
         only_separable_directions=only_separable_directions,
@@ -205,59 +186,50 @@
         cutoff_absolute_identifiable: float = 1e-16,
         cutoff_relative_identifiable: float = 1e-16
 ) -> Tuple[np.ndarray, np.ndarray]:
     """
     Compute the spectral decomposition of ensemble parameters or predictions.
 
     Parameters
-    ==========
+    ----------
     matrix:
         symmetric matrix (typically a covariance matrix) of parameters or
         predictions
-
     normalize:
         flag indicating whether the returned Eigenvalues should be normalized
         with respect to the largest Eigenvalue
-
     only_separable_directions:
         return only separable directions according to
         cutoff_[absolute/relative]_separable
-
     cutoff_absolute_separable:
         Consider only eigenvalues of the covariance matrix above this cutoff
         (only applied when only_separable_directions is True)
-
     cutoff_relative_separable:
         Consider only eigenvalues of the covariance matrix above this cutoff,
         when rescaled with the largest eigenvalue
         (only applied when only_separable_directions is True)
-
     only_identifiable_directions:
         return only identifiable directions according to
         cutoff_[absolute/relative]_identifiable
-
     cutoff_absolute_identifiable:
         Consider only low eigenvalues of the covariance matrix with inverses
         above of this cutoff
         (only applied when only_identifiable_directions is True)
-
     cutoff_relative_identifiable:
         Consider only low eigenvalues of the covariance matrix when rescaled
         with the largest eigenvalue with inverses above of this cutoff
         (only applied when only_identifiable_directions is True)
 
     Returns
-    =======
+    -------
     eigenvalues:
         Eigenvalues of the covariance matrix
-
     eigenvectors:
         Eigenvectors of the covariance matrix
     """
-
     # get the eigenvalue decomposition
     eigenvalues, eigenvectors = np.linalg.eigh(matrix)
 
     # get a normalized version
     rel_eigenvalues = eigenvalues / np.max(eigenvalues)
 
     # If no filtering is wanted, we can return
```

### Comparing `pypesto-0.2.8/pypesto/ensemble/dimension_reduction.py` & `pypesto-0.2.9/pypesto/ensemble/dimension_reduction.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,39 +15,37 @@
 
 def get_umap_representation_parameters(
         ens: Ensemble,
         n_components: int = 2,
         normalize_data: bool = False,
         **kwargs) -> Tuple:
     """
+    UMAP of parameter ensemble.
+
     Compute the representation with reduced dimensionality via umap
     (with a given number of umap components) of the parameter ensemble.
     Allows to pass on additional keyword arguments to the umap routine.
 
     Parameters
-    ==========
+    ----------
     ens:
         Ensemble objects containing a set of parameter vectors
-
     n_components:
         number of components for the dimension reduction
-
     normalize_data:
         flag indicating whether the parameter ensemble should be rescaled with
         mean and standard deviation
 
     Returns
-    =======
+    -------
     umap_components:
         first components of the umap embedding
-
     umap_object:
         returned fitted umap object from umap.UMAP()
     """
-
     # call lowlevel routine using the parameter vector ensemble
     return _get_umap_representation_lowlevel(
         dataset=ens.x_vectors.transpose(),
         n_components=n_components,
         normalize_data=normalize_data,
         **kwargs
     )
@@ -56,43 +54,40 @@
 def get_umap_representation_predictions(
         ens: Union[Ensemble, EnsemblePrediction],
         prediction_index: int = 0,
         n_components: int = 2,
         normalize_data: bool = False,
         **kwargs) -> Tuple:
     """
+    UMAP of ensemble prediction.
+
     Compute the representation with reduced dimensionality via umap
     (with a given number of umap components) of the ensemble predictions.
     Allows to pass on additional keyword arguments to the umap routine.
 
     Parameters
-    ==========
+    ----------
     ens:
         Ensemble objects containing a set of parameter vectors and a set of
         predictions or EnsemblePrediction object containing only predictions
-
     prediction_index:
         index telling which prediction from the list should be analyzed
-
     n_components:
         number of components for the dimension reduction
-
     normalize_data:
         flag indicating whether the parameter ensemble should be rescaled with
         mean and standard deviation
 
     Returns
-    =======
+    -------
     umap_components:
         first components of the umap embedding
-
     umap_object:
         returned fitted umap object from umap.UMAP()
     """
-
     # extract the an array of predictions from either an Ensemble object or an
     # EnsemblePrediction object
     dataset = get_prediction_dataset(ens, prediction_index)
 
     # call lowlevel routine using the prediction ensemble
     return _get_umap_representation_lowlevel(
         dataset=dataset,
@@ -105,43 +100,40 @@
 def get_pca_representation_parameters(
         ens: Ensemble,
         n_components: int = 2,
         rescale_data: bool = True,
         rescaler: Union[Callable, None] = None
 ) -> Tuple:
     """
+    PCA of parameter ensemble.
+
     Compute the representation with reduced dimensionality via principal
     component analysis (with a given number of principal components) of the
     parameter ensemble.
 
     Parameters
-    ==========
+    ----------
     ens:
         Ensemble objects containing a set of parameter vectors
-
     n_components:
         number of components for the dimension reduction
-
     rescale_data:
         flag indicating whether the principal components should be rescaled
         using a rescaler function (e.g., an arcsinh function)
-
     rescaler:
         callable function to rescale the output of the PCA (defaults to
         numpy.arcsinh)
 
     Returns
-    =======
+    -------
     principal_components:
         principal components of the parameter vector ensemble
-
     pca_object:
         returned fitted pca object from sklearn.decomposition.PCA()
     """
-
     return _get_pca_representation_lowlevel(
         dataset=ens.x_vectors.transpose(),
         n_components=n_components,
         rescale_data=rescale_data,
         rescaler=rescaler
     )
 
@@ -150,47 +142,43 @@
         ens: Union[Ensemble, EnsemblePrediction],
         prediction_index: int = 0,
         n_components: int = 2,
         rescale_data: bool = True,
         rescaler: Union[Callable, None] = None
 ) -> Tuple:
     """
+    PCA of ensemble prediction.
+
     Compute the representation with reduced dimensionality via principal
     component analysis (with a given number of principal components) of the
     ensemble prediction.
 
     Parameters
-    ==========
+    ----------
     ens:
         Ensemble objects containing a set of parameter vectors and a set of
         predictions or EnsemblePrediction object containing only predictions
-
     prediction_index:
         index telling which prediction from the list should be analyzed
-
     n_components:
         number of components for the dimension reduction
-
     rescale_data:
         flag indicating whether the principal components should be rescaled
         using a rescaler function (e.g., an arcsinh function)
-
     rescaler:
         callable function to rescale the output of the PCA (defaults to
         numpy.arcsinh)
 
     Returns
-    =======
+    -------
     principal_components:
         principal components of the parameter vector ensemble
-
     pca_object:
         returned fitted pca object from sklearn.decomposition.PCA()
     """
-
     # extract the an array of predictions from either an Ensemble object or an
     # EnsemblePrediction object
     dataset = get_prediction_dataset(ens, prediction_index)
 
     # call lowlevel routine using the prediction ensemble
     return _get_pca_representation_lowlevel(
         dataset=dataset,
@@ -202,44 +190,41 @@
 
 def _get_umap_representation_lowlevel(
         dataset: np.ndarray,
         n_components: int = 2,
         normalize_data: bool = False,
         **kwargs) -> Tuple:
     """
-    Compute the representation with reduced dimensionality via principal
-    component analysis (with a given number of principal components) of the
-    parameter ensemble.
+    Low level UMAP of parameter ensemble.
+
+    Compute the representation with reduced dimensionality via uniform
+    manifold approximation and projection (with a given number of principal
+    components) of the parameter ensemble.
 
     Parameters
-    ==========
+    ----------
     dataset:
         numpy array containing either the ensemble predictions or the parameter
         ensemble itself
-
     n_components:
         number of components for the dimension reduction
-
     rescale_data:
         flag indicating whether the principal components should be rescaled
         using a rescaler function (e.g., an arcsinh function)
-
     rescaler:
         callable function to rescale the output of the PCA (defaults to
         numpy.arcsinh)
 
     Returns
-    =======
+    -------
     umap_components:
         first components of the umap embedding
-
     umap_object:
         returned fitted umap object from umap.UMAP()
     """
-
     # create a umap object
     umap_object = umap.UMAP(n_components=n_components, **kwargs)
 
     # normalize data with mean and standard deviation if wanted
     if normalize_data:
         dataset = StandardScaler().fit_transform(dataset)
 
@@ -252,44 +237,41 @@
 def _get_pca_representation_lowlevel(
         dataset: np.ndarray,
         n_components: int = 2,
         rescale_data: bool = True,
         rescaler: Union[Callable, None] = None
 ) -> Tuple:
     """
+    Low level PCA of parameter ensemble.
+
     Compute the representation with reduced dimensionality via principal
     component analysis (with a given number of principal components) of the
     parameter ensemble.
 
     Parameters
-    ==========
+    ----------
     dataset:
         numpy array containing either the ensemble predictions or the parameter
         ensemble itself
-
     n_components:
         number of components for the dimension reduction
-
     rescale_data:
         flag indicating whether the principal components should be rescaled
         using a rescaler function (e.g., an arcsinh function)
-
     rescaler:
         callable function to rescale the output of the PCA (defaults to
         numpy.arcsinh)
 
     Returns
-    =======
+    -------
     principal_components:
         principal components of the parameter vector ensemble
-
     pca_object:
         returned fitted pca object from sklearn.decomposition.PCA()
     """
-
     # create a PCA object and decompose the dataset
     pca_object = sklearn.decomposition.PCA(n_components=n_components)
     pca_object.fit(dataset)
     # get the projection down to the first components
     principal_components = pca_object.transform(dataset)
 
     # rescale the principal components with a non-linear function, if wanted
```

### Comparing `pypesto-0.2.8/pypesto/ensemble/ensemble.py` & `pypesto-0.2.9/pypesto/ensemble/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,28 +28,30 @@
                         WEIGHTED_SIGMA)
 
 logger = logging.getLogger(__name__)
 
 
 class EnsemblePrediction:
     """
-    A ensemble prediction consists of an ensemble, i.e., a set of parameter
+    Class of ensemble prediction.
+
+    An ensemble prediction consists of an ensemble, i.e., a set of parameter
     vectors and their identifiers such as a sample, and a prediction function.
     It can be attached to a ensemble-type object
     """
 
     def __init__(
             self,
             predictor: Optional[Callable[[Sequence], PredictionResult]] = None,
             prediction_id: str = None,
             prediction_results: Sequence[PredictionResult] = None,
             lower_bound: Sequence[np.ndarray] = None,
             upper_bound: Sequence[np.ndarray] = None):
         """
-        Constructor.
+        Initialize.
 
         Parameters
         ----------
         predictor:
             Prediction function, e.g., an AmiciPredictor, which takes a
             parameter vector as input and outputs a PredictionResult object
         prediction_id:
@@ -84,32 +86,35 @@
         self.prediction_summary = {MEAN: None,
                                    STANDARD_DEVIATION: None,
                                    MEDIAN: None,
                                    WEIGHTED_SIGMA: None}
 
     def __iter__(self):
         """
-        __iter__ makes the instances of the class iterable objects, allowing to
-        apply functions such as __dict__ to them.
+        Make the instances of the class iterable objects.
+
+        Allows to apply functions such as __dict__ to them.
         """
         yield PREDICTOR, self.predictor
         yield PREDICTION_ID, self.prediction_id
         yield PREDICTION_RESULTS, self.prediction_results
         yield PREDICTION_ARRAYS, self.prediction_arrays
         yield PREDICTION_SUMMARY, {i_key: dict(self.prediction_summary[i_key])
                                    for i_key in self.prediction_summary.keys()}
         yield LOWER_BOUND, self.lower_bound
         yield UPPER_BOUND, self.upper_bound
 
     def condense_to_arrays(self):
         """
-        This functions reshapes the predictions results to an array and adds
-        them as a member to the EnsemblePrediction objects. It's meant to be
-        used only if all conditions of a prediction have the same observables,
-        as this is often the case for large-scale data sets taken from online
+        Add prediction result to EnsemblePrediction object.
+
+        Reshape the prediction results to an array and add them as a
+        member to the EnsemblePrediction objects. It's meant to be used only
+        if all conditions of a prediction have the same observables, as this
+        is often the case for large-scale data sets taken from online
         databases or similar.
         """
         # prepare for storing results over all predictions
         output = []
         output_sensi = []
         timepoints = []
 
@@ -146,17 +151,19 @@
 
     def compute_summary(self,
                         percentiles_list: Sequence[int] = (5, 20, 80, 95),
                         weighting: bool = False,
                         compute_weighted_sigma: bool = False
                         ) -> Dict:
         """
-        Compute the mean, the median, the standard deviation and possibly
-        percentiles from the ensemble prediction results. Those summary results
-        are added as a data member to the EnsemblePrediction object.
+        Compute summary from the ensemble prediction results.
+
+        Summary includes the mean, the median, the standard deviation and
+        possibly percentiles. Those summary results are added as a data
+        member to the EnsemblePrediction object.
 
         Parameters
         ----------
         percentiles_list:
             List or tuple of percent numbers for the percentiles
         weighting:
             Whether weights should be used for trajectory.
@@ -180,47 +187,53 @@
                 raise ValueError('There are no weights in the '
                                  'prediction results.')
 
         n_conditions = len(self.prediction_results[0].conditions)
 
         def _stack_outputs(ic: int):
             """
+            Stack outputs.
+
             Group outputs for different parameter vectors of one ensemble
             together, if they belong to the same simulation condition, and
-            stacks them in one array
+            stack them in one array.
             """
             # Were outputs computed
             if self.prediction_results[0].conditions[ic].output is None:
                 return None
             # stack predictions
             output_list = [prediction.conditions[ic].output
                            for prediction in self.prediction_results]
             # stack into one numpy array
             return np.stack(output_list, axis=-1)
 
         def _stack_outputs_sensi(ic: int):
             """
+            Stack output sensitivities.
+
             Group output sensitivities for different parameter vectors of one
-            ensemble together, if the belong to the same simulation condition,
-            and stacks them in one array
+            ensemble together, if they belong to the same simulation condition,
+            and stack them in one array.
             """
             # Were output sensitivitiess computed
             if self.prediction_results[0].conditions[ic].output_sensi is None:
                 return None
             # stack predictions
             output_sensi_list = [prediction.conditions[ic].output_sensi
                                  for prediction in self.prediction_results]
             # stack into one numpy array
             return np.stack(output_sensi_list, axis=-1)
 
         def _stack_weights(ic: int) -> np.ndarray:
             """
+            Stack weights.
+
             Group weights for different parameter vectors of one ensemble
             together, if they belong to the same simulation condition, and
-            stacks them in one array
+            stack them in one array
 
             Parameters
             ----------
             ic: the condition number.
 
             Returns
             -------
@@ -233,32 +246,36 @@
             output_weight_list = [prediction.conditions[ic].output_weight
                                   for prediction in self.prediction_results]
             # stack into one numpy array
             return np.stack(output_weight_list, axis=-1)
 
         def _stack_sigmas(ic: int):
             """
+            Stack sigmas.
+
             Group sigmas for different parameter vectors of one ensemble
             together, if they belong to the same simulation condition, and
-            stacks them in one array
+            stack them in one array.
             """
             # Were outputs computed
             if self.prediction_results[0].conditions[ic].output_sigmay is None:
                 return None
             # stack predictions
             output_sigmay_list = [prediction.conditions[ic].output_sigmay
                                   for prediction in self.prediction_results]
             # stack into one numpy array
             return np.stack(output_sigmay_list, axis=-1)
 
         def _compute_summary(tmp_array, percentiles_list, weights,
                              tmp_sigmas=None):
             """
-            Computes means, standard deviation, median, and requested
-            percentiles for a set of stacked simulations
+            Compute summary for a set of stacked simulations.
+
+            Summary includes means, standard deviation, median, and requested
+            percentiles.
             """
             summary = {}
             summary[MEAN] = np.average(tmp_array, axis=-1, weights=weights)
             summary[STANDARD_DEVIATION] = np.sqrt(np.average(
                 (tmp_array.T-summary[MEAN].T).T**2,
                 axis=-1, weights=weights))
             summary[MEDIAN] = np.median(tmp_array, axis=-1)
@@ -377,32 +394,34 @@
                                  'of measurements does not match.')
             chi_2.append(np.nansum(((y_meas-mean_traj)/weighted_sigmas)**2))
         return np.sum(chi_2)
 
 
 class Ensemble:
     """
-    A ensemble is a wrapper around an numpy array. It comes with some
-    convenience functionality: It allows to map parameter values via
-    identifiers to the correct parameters, it allows to compute summaries of
-    the parameter vectors (mean, standard deviation, median, percentiles) more
-    easily, and it can store predictions made by pyPESTO, such that the
-    parameter ensemble and the predictions are linked to each other.
+    An ensemble is a wrapper around a numpy array.
+
+    It comes with some convenience functionality: It allows to map parameter
+    values via identifiers to the correct parameters, it allows to compute
+    summaries of the parameter vectors (mean, standard deviation, median,
+    percentiles) more easily, and it can store predictions made by pyPESTO,
+    such that the parameter ensemble and the predictions are linked to each
+    other.
     """
 
     def __init__(self,
                  x_vectors: np.ndarray,
                  x_names: Sequence[str] = None,
                  vector_tags: Sequence[Tuple[int, int]] = None,
                  ensemble_type: EnsembleType = None,
                  predictions: Sequence[EnsemblePrediction] = None,
                  lower_bound: np.ndarray = None,
                  upper_bound: np.ndarray = None):
         """
-        Constructor.
+        Initialize.
 
         Parameters
         ----------
         x_vectors:
             parameter vectors of the ensemble, in the format
             n_parameter x n_vectors
         x_names:
@@ -467,15 +486,16 @@
             remove_burn_in: bool = True,
             chain_slice: slice = None,
             x_names: Sequence[str] = None,
             lower_bound: np.ndarray = None,
             upper_bound: np.ndarray = None,
             **kwargs,
     ):
-        """Construct an ensemble from a sample.
+        """
+        Construct an ensemble from a sample.
 
         Parameters
         ----------
         result:
             A pyPESTO result that contains a sample result.
         remove_burn_in:
             Exclude parameter vectors from the ensemble if they are in the
@@ -518,15 +538,16 @@
     @staticmethod
     def from_optimization_endpoints(
             result: Result,
             cutoff: float = np.inf,
             max_size: int = np.inf,
             **kwargs,
     ):
-        """Construct an ensemble from an optimization result.
+        """
+        Construct an ensemble from an optimization result.
 
         Parameters
         ----------
         result:
             A pyPESTO result that contains an optimization result.
         cutoff:
             Exclude parameters from the optimization if the
@@ -580,15 +601,16 @@
             result: Result,
             cutoff: float = np.inf,
             max_size: int = np.inf,
             max_per_start: int = np.inf,
             distribute: bool = True,
             **kwargs,
     ):
-        """Construct an ensemble from the history of an optimization.
+        """
+        Construct an ensemble from the history of an optimization.
 
         Parameters
         ----------
         result:
             A pyPESTO result that contains an optimization result
             with history recorded.
         cutoff:
@@ -668,16 +690,17 @@
                         vector_tags=vector_tags,
                         lower_bound=lb,
                         upper_bound=ub,
                         **kwargs)
 
     def __iter__(self):
         """
-        __iter__ makes the instances of the class iterable objects, allowing to
-        apply functions such as __dict__ to them.
+        Make the instances of the class iterable objects.
+
+        Allows to apply functions such as __dict__ to them.
         """
         yield X_VECTOR, self.x_vectors
         yield NX, self.n_x
         yield X_NAMES, self.x_names
         yield NVECTORS, self.n_vectors
         yield VECTOR_TAGS, self.vector_tags
         yield ENSEMBLE_TYPE, self.ensemble_type
@@ -688,16 +711,18 @@
 
     def _map_parameters_by_objective(
             self,
             predictor: Callable,
             default_value: float = None,
     ):
         """
+        Create mapping for parameters from ensebmle to predictor.
+
         The parameters of the ensemble don't need to have the same ordering as
-        in the predictor. This functions maps them onto each other
+        in the predictor.
         """
         # create short hands
         parameter_ids_objective = predictor.amici_objective.x_names
         parameter_ids_ensemble = self.x_names
         # map, and fill with `default_value` if not found and `default_value`
         # is specified.
         mapping = []
@@ -719,15 +744,16 @@
             mode: str = MODE_FUN,
             include_llh_weights: bool = False,
             include_sigmay: bool = False,
             engine: Engine = None,
             progress_bar: bool = True
     ) -> EnsemblePrediction:
         """
-        Convenience function to run predictions for a full ensemble:
+        Run predictions for a full ensemble.
+
         User needs to hand over a predictor function and settings, then all
         results are grouped as EnsemblePrediction for the whole ensemble
 
         Parameters
         ----------
         predictor:
             Prediction function, e.g., an AmiciPredictor
@@ -811,18 +837,19 @@
             prediction_id=prediction_id,
             prediction_results=prediction_results,
         )
 
     def compute_summary(self,
                         percentiles_list: Sequence[int] = (5, 20, 80, 95)):
         """
-        This function computes the mean, the median, the standard deviation
-        and possibly percentiles for the parameters of the ensemble.
-        Those summary results are added as a data member to the
-        EnsemblePrediction object.
+        Compute summary for the parameters of the ensemble.
+
+        Summary includes the mean, the median, the standard deviation and
+        possibly percentiles. Those summary results are added as a data
+        member to the EnsemblePrediction object.
 
         Parameters
         ----------
         percentiles_list:
             List or tuple of percent numbers for the percentiles
 
         Returns
@@ -839,14 +866,16 @@
                 np.percentile(self.x_vectors, perc, axis=1)
         # store and return results
         self.summary = summary
         return summary
 
     def check_identifiability(self) -> pd.DataFrame:
         """
+        Check identifiability of ensemble.
+
         Use ensemble mean and standard deviation to assess (in a rudimentary
         way) whether or not parameters are identifiable. Returns a dataframe
         with tuples, which specify whether or not the lower and the upper
         bounds are violated.
 
         Returns
         -------
@@ -905,16 +934,15 @@
 
 
 def entries_per_start(fval_traces: List['np.ndarray'],
                       cutoff: float,
                       max_size: int,
                       max_per_start: int, ):
     """
-    Creates the indices of each start that will be included
-    in the ensemble.
+    Create the indices of each start that will be included in the ensemble.
 
     Parameters
     ----------
     fval_traces:
         the fval-trace of each start.
     cutoff:
         Exclude parameters from the optimization if the nllh
@@ -925,15 +953,14 @@
         The maximum number of vectors to be included from a
         single optimization start.
 
     Returns
     -------
         A list of number of candidates per start that are to
         be included in the ensemble.
-
     """
     # choose possible candidates
     ens_ind = [np.flatnonzero(fval <= cutoff) for fval in fval_traces]
 
     # count the number of candidates per start
     n_per_start = np.array([len(start) for start in ens_ind])
 
@@ -964,15 +991,15 @@
 
 
 def get_vector_indices(trace_start: np.ndarray,
                        cutoff: float,
                        n_vectors: int,
                        distribute: bool, ):
     """
-    Returns the indices to be taken into an ensemble.
+    Return the indices to be taken into an ensemble.
 
     Parameters
     ----------
     trace_start:
         The fval_trace of a single start.
     cutoff:
         Exclude parameters from the optimization if the nllh
@@ -984,15 +1011,14 @@
         start should be taken or whether the indices should be
         more evenly distributed.
 
     Returns
     -------
         The indices to include in the ensemble.
     """
-
     candidates = np.flatnonzero(trace_start <= cutoff)
 
     if distribute:
         indices = np.round(np.linspace(0, len(candidates) - 1, n_vectors))
         return candidates[indices.astype(int)]
     else:
         return candidates[:n_vectors]
```

### Comparing `pypesto-0.2.8/pypesto/ensemble/task.py` & `pypesto-0.2.9/pypesto/ensemble/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,12 +28,13 @@
     ):
         super().__init__()
         self.method = method
         self.vectors = vectors
         self.id = id
 
     def execute(self) -> List[Any]:
+        """Execute the task."""
         logger.info(f"Executing task {self.id}.")
         results = []
         for index in range(self.vectors.shape[1]):
             results.append(self.method(self.vectors[:, index]))
         return results
```

### Comparing `pypesto-0.2.8/pypesto/ensemble/utils.py` & `pypesto-0.2.9/pypesto/ensemble/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                   sep: str = '\t',
                   index_col: int = 0,
                   headline_parser: Callable = None,
                   ensemble_type: EnsembleType = None,
                   lower_bound: np.ndarray = None,
                   upper_bound: np.ndarray = None):
     """
-    function for creating an ensemble from a csv file
+    Create an ensemble from a csv file.
 
     Parameters
     ----------
     path:
         path to csv file to read in parameter ensemble
     sep:
         separator in csv file
@@ -74,15 +74,15 @@
     ----------
     filename:
         Name or path of the HDF5 file.
     input_type:
         Which type of ensemble to create. From History, from
         Optimization or from Sample.
 
-    Returns:
+    Returns
     -------
     ensemble:
         Ensemble object of parameter vectors
     """
     # TODO: add option HISTORY. Need to fix
     #  reading history from hdf5.
     if input_type == OPTIMIZE:
@@ -106,15 +106,15 @@
 
 def read_from_df(dataframe: pd.DataFrame,
                  headline_parser: Callable = None,
                  ensemble_type: EnsembleType = None,
                  lower_bound: np.ndarray = None,
                  upper_bound: np.ndarray = None):
     """
-    function for creating an ensemble from a csv file
+    Create an ensemble from a csv file.
 
     Parameters
     ----------
     dataframe:
         pandas.DataFrame to read in parameter ensemble
     headline_parser:
         A function which reads in the headline of the csv file and converts it
@@ -146,14 +146,26 @@
                     lower_bound=lower_bound,
                     upper_bound=upper_bound)
 
 
 def write_ensemble_prediction_to_h5(ensemble_prediction: EnsemblePrediction,
                                     output_file: str,
                                     base_path: str = None):
+    """
+    Write an `EnsemblePrediction` to hdf5.
+
+    Parameters
+    ----------
+    ensemble_prediction:
+        The prediciton to be saved.
+    output_file:
+        The filename of the hdf5 file.
+    base_path:
+        An optional filepath where the file should be saved to.
+    """
     # parse base path
     base = Path('')
     if base_path is not None:
         base = Path(base_path)
 
     # open file
     with h5py.File(output_file, 'a') as f:
@@ -208,32 +220,33 @@
                                          f'{PREDICTION_RESULTS}_{i_result}')
             result.write_to_h5(output_file, base_path=tmp_base_path)
 
 
 def get_prediction_dataset(ens: Union[Ensemble, EnsemblePrediction],
                            prediction_index: int = 0) -> np.ndarray:
     """
-    Extract an array of prediction from either an Ensemble object which
-    contains a list of predictions of from an EnsemblePrediction object.
+    Extract an array of prediction.
+
+    Can be done from either an Ensemble object which contains a list of
+    predictions of from an EnsemblePrediction object.
 
     Parameters
-    ==========
+    ----------
     ens:
         Ensemble objects containing a set of parameter vectors and a set of
         predictions or EnsemblePrediction object containing only predictions
 
     prediction_index:
         index telling which prediction from the list should be analyzed
 
     Returns
-    =======
+    -------
     dataset:
         numpy array containing the ensemble predictions
     """
-
     if isinstance(ens, Ensemble):
         dataset = ens.predictions[prediction_index]
     elif isinstance(ens, EnsemblePrediction):
         ens.condense_to_arrays()
         dataset = ens.prediction_arrays[OUTPUT].transpose()
     else:
         raise Exception('Need either an Ensemble object with predictions or '
@@ -241,15 +254,15 @@
 
     return dataset
 
 
 def read_ensemble_prediction_from_h5(
         predictor: Union[Callable[[Sequence], PredictionResult], None],
         input_file: str):
-
+    """Read an ensemble prediction from an HDF5 File."""
     # open file
     with h5py.File(input_file, 'r') as f:
         pred_res_list = []
         bounds = {}
         for key in f.keys():
             if key == PREDICTION_ID:
                 prediction_id = f[key][()].decode()
@@ -284,11 +297,11 @@
         return EnsemblePrediction(predictor=predictor,
                                   prediction_id=prediction_id,
                                   prediction_results=pred_res_list,
                                   )
 
 
 def decode_array(array: np.ndarray) -> np.ndarray:
-    """Decodes array of bytes to string"""
+    """Decode array of bytes to string."""
     for i in range(len(array)):
         array[i] = array[i].decode()
     return array
```

### Comparing `pypesto-0.2.8/pypesto/logging.py` & `pypesto-0.2.9/pypesto/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: D400,D205
 """
 Logging
 =======
 
 Logging convenience functions.
 """
 
@@ -9,28 +10,24 @@
 
 
 def log(name: str = 'pypesto',
         level: int = logging.INFO,
         console: bool = True,
         filename: str = ''):
     """
-    Log messages from a specified name with a specified level to any
-    combination of console and file.
+    Log messages from `name` with `level` to any combination of console/file.
 
     Parameters
     ----------
     name:
         The name of the logger.
-
     level:
         The output level to use.
-
     console:
         If True, messages are logged to console.
-
     filename:
         If specified, messages are logged to a file with this name.
     """
     logger = logging.getLogger(name)
     logger.setLevel(level)
 
     if console:
```

### Comparing `pypesto-0.2.8/pypesto/objective/__init__.py` & `pypesto-0.2.9/pypesto/objective/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.2.8/pypesto/objective/aesara.py` & `pypesto-0.2.9/pypesto/objective/aesara.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
-This adds an interface for the construction of loss functions
+Aesara models interface.
+
+Adds an interface for the construction of loss functions
 incorporating aesara models. This permits computation of derivatives using a
-combination of objective based methods and aeara based backpropagation
+combination of objective based methods and aeara based backpropagation.
 """
 
 import numpy as np
 import copy
 
 from .base import ObjectiveBase, ResultDict
 from .constants import MODE_FUN, FVAL, GRAD, HESS, RDATAS
@@ -19,19 +21,20 @@
     from aesara.graph.op import Op
 except ImportError:
     aesara = aet = Op = TensorVariable = None
 
 
 class AesaraObjective(ObjectiveBase):
     """
-    Wrapper around an ObjectiveBase which computes the gradient at each
-    evaluation, caching it for later calls.
+    Wrapper around an ObjectiveBase.
+
+    Computes the gradient at each evaluation, caching it for later calls.
     Caching is only enabled after the first time the gradient is asked for
-    and disabled whenever the cached gradient is not used,
-    in order not to increase computation time for derivative-free samplers.
+    and disabled whenever the cached gradient is not used, in order not to
+    increase computation time for derivative-free samplers.
 
     Parameters
     ----------
     objective:
         The `pypesto.ObjectiveBase` to wrap.
     aet_x:
         Tensor variables that that define the variables of `aet_fun`
@@ -84,30 +87,37 @@
             [aet_x], aet_fun
         )
 
         # temporary storage for evaluation results of objective
         self.inner_ret: ResultDict = {}
 
     def check_mode(self, mode) -> bool:
+        """See `ObjectiveBase` documentation."""
         return mode == MODE_FUN
 
     def check_sensi_orders(self, sensi_orders, mode) -> bool:
+        """See `ObjectiveBase` documentation."""
         if not self.check_mode(mode):
             return False
         else:
             return self.base_objective.check_sensi_orders(sensi_orders, mode)
 
     def call_unprocessed(
             self,
             x: np.ndarray,
             sensi_orders: Tuple[int, ...],
             mode: str,
             **kwargs
     ) -> ResultDict:
+        """
+        See `ObjectiveBase` for more documentation.
 
+        Main method to overwrite from the base class. It handles and
+        delegates the actual objective evaluation.
+        """
         # hess computation in aesara requires grad
         if 2 in sensi_orders and 1 not in sensi_orders:
             sensi_orders = (1, *sensi_orders)
 
         # this computes all the results from the inner objective, rendering
         # them accessible to aesara compiled functions
 
@@ -162,32 +172,37 @@
 
         # initialize the sensitivity Op
         if obj.has_grad:
             self._log_prob_grad = AesaraObjectiveGradOp(obj, coeff)
         else:
             self._log_prob_grad = None
 
-    def perform(self, node, inputs, outputs, params=None):
+    def perform(self, node, inputs, outputs, params=None):  # noqa
         # note that we use precomputed values from the outer
         # AesaraObjective.call_unprocessed here, which which means we can
         # ignore inputs here
         log_prob = self._coeff * self._objective.inner_ret[FVAL]
         outputs[0][0] = np.array(log_prob)
 
     def grad(self, inputs, g):
-        # the method that calculates the gradients - it actually returns the
-        # vector-Jacobian product - g[0] is a vector of parameter values
+        """
+        Calculate the hessian.
+
+        Actually returns the vector-hessian product - g[0] is a vector of
+        parameter values.
+        """
         theta, = inputs
         log_prob_grad = self._log_prob_grad(theta)
         return [g[0] * log_prob_grad]
 
 
 class AesaraObjectiveGradOp(Op):
     """
     Aesara wrapper around a (non-normalized) log-probability gradient function.
+
     This Op will be called with a vector of values and also return a vector of
     values - the gradients in each dimension.
 
     Parameters
     ----------
     obj:
         Base aseara objective
@@ -205,32 +220,37 @@
         self._coeff: float = coeff
 
         if obj.has_hess:
             self._log_prob_hess = AesaraObjectiveHessOp(obj, coeff)
         else:
             self._log_prob_hess = None
 
-    def perform(self, node, inputs, outputs, params=None):
+    def perform(self, node, inputs, outputs, params=None):  # noqa
         # note that we use precomputed values from the outer
         # AesaraObjective.call_unprocessed here, which which means we can
         # ignore inputs here
         log_prob_grad = self._coeff * self._objective.inner_ret[GRAD]
         outputs[0][0] = log_prob_grad
 
     def grad(self, inputs, g):
-        # the method that calculates the hessian - it actually returns the
-        # vector-hessian product - g[0] is a vector of parameter values
+        """
+        Calculate the hessian.
+
+        Actually returns the vector-hessian product - g[0] is a vector of
+        parameter values.
+        """
         theta, = inputs
         log_prob_hess = self._log_prob_hess(theta)
         return [g[0].dot(log_prob_hess)]
 
 
 class AesaraObjectiveHessOp(Op):
     """
     Aesara wrapper around a (non-normalized) log-probability Hessian function.
+
     This Op will be called with a vector of values and also return a matrix of
     values - the Hessian in each dimension.
 
     Parameters
     ----------
     obj:
         Base aseara objective
@@ -243,13 +263,13 @@
 
     def __init__(self, obj:
                  AesaraObjective,
                  coeff: Optional[float] = 1.):
         self._objective: AesaraObjective = obj
         self._coeff: float = coeff
 
-    def perform(self, node, inputs, outputs, params=None):
+    def perform(self, node, inputs, outputs, params=None):  # noqa
         # note that we use precomputed values from the outer
         # AesaraObjective.call_unprocessed here, which which means we can
         # ignore inputs here
         log_prob_hess = self._coeff * self._objective.inner_ret[HESS]
         outputs[0][0] = log_prob_hess
```

### Comparing `pypesto-0.2.8/pypesto/objective/aggregated.py` & `pypesto-0.2.9/pypesto/objective/aggregated.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,37 +4,33 @@
 from typing import Sequence, Tuple
 from .base import ObjectiveBase, ResultDict
 
 from .constants import RDATAS, FVAL, CHI2, SCHI2, RES, SRES, GRAD, HESS, HESSP
 
 
 class AggregatedObjective(ObjectiveBase):
-    """
-    This class aggregates multiple objectives into one objective.
-    """
+    """Aggregates multiple objectives into one objective."""
 
     def __init__(
         self,
         objectives: Sequence[ObjectiveBase],
         x_names: Sequence[str] = None,
     ):
         """
-        Constructor.
-
+        Initialize objective.
 
         Parameters
         ----------
         objectives:
             Sequence of pypesto.ObjectiveBase instances
         x_names:
             Sequence of names of the (optimized) parameters.
             (Details see documentation of x_names in
             :class:`pypesto.ObjectiveBase`)
         """
-
         # input typechecks
         if not isinstance(objectives, Sequence):
             raise TypeError(f'Objectives must be a Sequence, '
                             f'was {type(objectives)}.')
 
         if not all(
                 isinstance(objective, ObjectiveBase)
@@ -47,73 +43,82 @@
             raise ValueError('Length of objectives must be at least one')
 
         self._objectives = objectives
 
         super().__init__(x_names=x_names)
 
     def __deepcopy__(self, memodict=None):
+        """Create copy of objective."""
         other = AggregatedObjective(
             objectives=[deepcopy(objective) for objective in self._objectives],
             x_names=deepcopy(self.x_names),
         )
         for key in set(self.__dict__.keys()) - {'_objectives', 'x_names'}:
             other.__dict__[key] = deepcopy(self.__dict__[key])
 
         return other
 
     def check_mode(self, mode: str) -> bool:
+        """See `ObjectiveBase` documentation."""
         return all(
             objective.check_mode(mode)
             for objective in self._objectives
         )
 
     def check_sensi_orders(
         self,
         sensi_orders: Tuple[int, ...],
         mode: str,
     ) -> bool:
+        """See `ObjectiveBase` documentation."""
         return all(
             objective.check_sensi_orders(sensi_orders, mode)
             for objective in self._objectives
         )
 
     def call_unprocessed(
         self,
         x: np.ndarray,
         sensi_orders: Tuple[int, ...],
         mode: str,
         **kwargs,
     ) -> ResultDict:
+        """
+        See `ObjectiveBase` for more documentation.
+
+        Main method to overwrite from the base class. It handles and
+        delegates the actual objective evaluation.
+        """
         return aggregate_results([
             objective.call_unprocessed(x, sensi_orders, mode, **kwargs)
             for objective in self._objectives
         ])
 
     def initialize(self):
+        """See `ObjectiveBase` documentation."""
         for objective in self._objectives:
             objective.initialize()
 
     def get_config(self) -> dict:
+        """Return basic information of the objective configuration."""
         info = super().get_config()
         for n_obj, obj in enumerate(self._objectives):
             info[f'objective_{n_obj}'] = obj.get_config()
         return info
 
 
 def aggregate_results(rvals: Sequence[ResultDict]) -> ResultDict:
     """
-    Aggregrate the results from the provided sequence of ResultDicts into a
-    single ResultDict.
+    Aggregrate the results from the provided ResultDicts into a single one.
 
     Parameters
     ----------
     rvals:
         results to aggregate
     """
-
     # rvals are guaranteed to be consistent as _check_sensi_orders checks
     # whether each objective can be called with the respective
     # sensi_orders/mode
 
     # sum over fval/grad/hess
     result = {
         key: sum(rval[key] for rval in rvals)
```

### Comparing `pypesto-0.2.8/pypesto/objective/amici.py` & `pypesto-0.2.9/pypesto/objective/amici.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,17 +42,15 @@
 
     @abc.abstractmethod
     def create_edatas(self, model: AmiciModel) -> Sequence['amici.ExpData']:
         """Create AMICI experimental data."""
 
 
 class AmiciObjective(ObjectiveBase):
-    """
-    This class allows to create an objective directly from an amici model.
-    """
+    """Allows to create an objective directly from an amici model."""
 
     def __init__(
         self,
         amici_model: AmiciModel,
         amici_solver: AmiciSolver,
         edatas: Union[Sequence['amici.ExpData'], 'amici.ExpData'],
         max_sensi_order: Optional[int] = None,
@@ -62,15 +60,15 @@
         guess_steadystate: Optional[Optional[bool]] = None,
         n_threads: Optional[int] = 1,
         fim_for_hess: Optional[bool] = True,
         amici_object_builder: Optional[AmiciObjectBuilder] = None,
         calculator: Optional[AmiciCalculator] = None,
     ):
         """
-        Constructor.
+        Initialize objective.
 
         Parameters
         ----------
         amici_model:
             The amici model.
         amici_solver:
             The solver to use for the numeric integration of the model.
@@ -194,23 +192,25 @@
         super().__init__(x_names=x_names)
 
         # Custom (condition-specific) timepoints. See the
         # `set_custom_timepoints` method for more information.
         self.custom_timepoints = None
 
     def get_config(self) -> dict:
+        """Return basic information of the objective configuration."""
         info = super().get_config()
         info['x_names'] = self.x_names
         info['model_name'] = self.amici_model.getName()
         info['solver'] = str(type(self.amici_solver))
         info['sensi_order'] = self.max_sensi_order
 
         return info
 
     def initialize(self):
+        """See `ObjectiveBase` documentation."""
         super().initialize()
         self.reset_steadystate_guesses()
         self.calculator.initialize()
 
     def __deepcopy__(self, memodict: Dict = None) -> 'AmiciObjective':
         other = self.__class__.__new__(self.__class__)
 
@@ -294,14 +294,15 @@
         self.apply_custom_timepoints()
 
     def check_sensi_orders(
         self,
         sensi_orders: Tuple[int, ...],
         mode: str,
     ) -> bool:
+        """See `ObjectiveBase` documentation."""
         sensi_order = max(sensi_orders)
 
         # dynamically obtain maximum allowed sensitivity order
         max_sensi_order = self.max_sensi_order
         if max_sensi_order is None:
             max_sensi_order = 1
             # check whether it is ok to request 2nd order
@@ -312,24 +313,33 @@
                     sensi_mthd == mthd_fwd and self.fim_for_hess)):
                 max_sensi_order = 2
 
         # evaluate sensitivity order
         return sensi_order <= max_sensi_order
 
     def check_mode(self, mode: str) -> bool:
+        """See `ObjectiveBase` documentation."""
         return mode in [MODE_FUN, MODE_RES]
 
     def call_unprocessed(
         self,
         x: np.ndarray,
         sensi_orders: Tuple[int, ...],
         mode: str,
         edatas: Sequence['amici.ExpData'] = None,
         parameter_mapping: 'ParameterMapping' = None,
     ):
+        """
+        Call objective function without pre- or post-processing and formatting.
+
+        Returns
+        -------
+        result:
+            A dict containing the results.
+        """
         sensi_order = max(sensi_orders)
 
         x_dct = self.par_arr_to_dct(x)
 
         # update steady state
         if self.guess_steadystate and \
                 self.steadystate_guesses['fval'] < np.inf:
@@ -363,15 +373,17 @@
 
     def par_arr_to_dct(self, x: Sequence[float]) -> Dict[str, float]:
         """Create dict from parameter vector."""
         return OrderedDict(zip(self.x_ids, x))
 
     def apply_steadystate_guess(self, condition_ix: int, x_dct: Dict) -> None:
         """
-        Use the stored steadystate as well as the respective  sensitivity (
+        Apply steady state guess to `edatas[condition_ix].x0`.
+
+        Use the stored steadystate as well as the respective sensitivity (
         if available) and parameter value to approximate the steadystate at
         the current parameters using a zeroth or first order taylor
         approximation:
         x_ss(x') = x_ss(x) [+ dx_ss/dx(x)*(x'-x)]
         """
         mapping = self.parameter_mapping[condition_ix].map_sim_var
         x_sim = map_par_opt_to_par_sim(mapping, x_dct, self.amici_model)
@@ -395,17 +407,18 @@
     def store_steadystate_guess(
         self,
         condition_ix: int,
         x_dct: Dict,
         rdata: 'amici.ReturnData',
     ) -> None:
         """
-        Store condition parameter, steadystate and steadystate sensitivity in
-        steadystate_guesses if steadystate guesses are enabled for this
-        condition
+        Store condition parameter, steadystate and steadystate sensitivity.
+
+        Stored in steadystate_guesses if steadystate guesses are enabled for
+        this condition.
         """
         if condition_ix not in self.steadystate_guesses['data']:
             return
         preeq_guesses = self.steadystate_guesses['data'][condition_ix]
 
         # update parameter
         condition_map_sim_var = \
@@ -440,16 +453,15 @@
 
     def set_custom_timepoints(
         self,
         timepoints: Sequence[Sequence[Union[float, int]]] = None,
         timepoints_global: Sequence[Union[float, int]] = None,
     ) -> 'AmiciObjective':
         """
-        Create a copy of this objective that will be evaluated at custom
-        timepoints.
+        Create a copy of this objective that is evaluated at custom timepoints.
 
         The intended use is to aid in predictions at unmeasured timepoints.
 
         Parameters
         ----------
         timepoints:
             The outer sequence should contain a sequence of timepoints for each
@@ -489,15 +501,15 @@
 
     def check_gradients_match_finite_differences(
         self,
         x: np.ndarray = None,
         *args,
         **kwargs
     ) -> bool:
-        """Check if gradients match finite differences (FDs)
+        """Check if gradients match finite differences (FDs).
 
         Parameters
         ----------
         x: The parameters for which to evaluate the gradient.
 
         Returns
         -------
```

### Comparing `pypesto-0.2.8/pypesto/objective/amici_calculator.py` & `pypesto-0.2.9/pypesto/objective/amici_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,15 @@
     pass
 
 AmiciModel = Union['amici.Model', 'amici.ModelPtr']
 AmiciSolver = Union['amici.Solver', 'amici.SolverPtr']
 
 
 class AmiciCalculator:
-    """
-    Class to perform the actual call to AMICI and obtain requested objective
-    function values.
-    """
+    """Class to perform the AMICI call and obtain objective function values."""
 
     def __init__(self):
         self._known_least_squares_safe = False
 
     def initialize(self):
         """Initialize the calculator. Default: Do nothing."""
 
@@ -122,14 +119,15 @@
                               mode: str,
                               amici_model: AmiciModel,
                               amici_solver: AmiciSolver,
                               edatas: List['amici.ExpData'],
                               x_ids: Sequence[str],
                               parameter_mapping: 'ParameterMapping',
                               fim_for_hess: bool):
+    """Calculate the function values from rdatas and return as dict."""
     # full optimization problem dimension (including fixed parameters)
     dim = len(x_ids)
 
     # check if the simulation failed
     if any(rdata['status'] < 0.0 for rdata in rdatas):
         return get_error_output(amici_model, edatas, rdatas,
                                 sensi_order, mode, dim)
```

### Comparing `pypesto-0.2.8/pypesto/objective/amici_util.py` & `pypesto-0.2.9/pypesto/objective/amici_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 def map_par_opt_to_par_sim(
         condition_map_sim_var: Dict[str, Union[float, str]],
         x_dct: Dict[str, float],
         amici_model: AmiciModel
 ) -> np.ndarray:
     """
-    From the optimization vector, create the simulation vector according
-    to the mapping.
+    Create simulation vector from optimization vector using the mapping.
 
     Parameters
     ----------
     condition_map_sim_var:
         Simulation to optimization parameter mapping.
     x_dct:
         The optimization parameters dict.
@@ -57,33 +56,34 @@
             par_sim_vals[ix] = x_dct[val]
 
     # return the created simulation parameter vector
     return np.array(par_sim_vals)
 
 
 def create_plist_from_par_opt_to_par_sim(mapping_par_opt_to_par_sim):
-    warnings.warn("This function will be removed in future releases. ",
-                  DeprecationWarning)
     """
+    Create list of parameter indices for which sensitivity is to be computed.
+
     From the parameter mapping `mapping_par_opt_to_par_sim`, create the
     simulation plist according to the mapping `mapping`.
 
     Parameters
     ----------
-
     mapping_par_opt_to_par_sim: array-like of str
         len == n_par_sim, the entries are either numeric, or
         optimization parameter ids.
 
     Returns
     -------
     plist: array-like of float
         List of parameter indices for which the sensitivity needs to be
         computed
     """
+    warnings.warn("This function will be removed in future releases. ",
+                  DeprecationWarning)
     plist = []
 
     # iterate over simulation parameter indices
     for j_par_sim, val in enumerate(mapping_par_opt_to_par_sim):
         if not isinstance(val, numbers.Number):
             plist.append(j_par_sim)
 
@@ -130,18 +130,17 @@
         The optimization parameter ids. Needed for order.
     par_sim_ids:
         The simulation parameter ids. Needed for order.
     condition_map_sim_var:
         The simulation to optimization parameter mapping.
 
     Returns
-    ----------
+    -------
     par_sim_slice:
         array of simulation parameter indices
-
     par_opt_slice:
         array of optimization parameter indices
     """
     # the sum accounts for subindexing according to plist in edata
     par_sim_slice, par_opt_slice = list(zip(*[
         (sum(isinstance(condition_map_sim_var[par_id], str)
              for par_id in
@@ -157,16 +156,17 @@
         par_opt_ids: Sequence[str],
         par_sim_ids: Sequence[str],
         condition_map_sim_var: Dict[str, Union[float, str]],
         sim_grad: np.ndarray,
         opt_grad: np.ndarray,
         coefficient: float = 1.0):
     """
-    Sum simulation gradients to objective gradient according to the provided
-    mapping `mapping_par_opt_to_par_sim`.
+    Sum simulation gradients to objective gradient.
+
+    Uses the provided mapping `mapping_par_opt_to_par_sim` for summing up.
 
     Parameters
     ----------
     par_opt_ids:
         The optimization parameter ids. Needed for order.
     par_sim_ids:
         The simulation parameter ids. Needed for order.
@@ -176,15 +176,14 @@
         Simulation gradient.
     opt_grad:
         The optimization gradient. To which sim_grad is added.
         Changed in-place.
     coefficient:
         Coefficient for sim_grad when adding to opt_grad.
     """
-
     par_sim_slice, par_opt_slice = par_index_slices(par_opt_ids, par_sim_ids,
                                                     condition_map_sim_var)
 
     par_opt_slice_unique, unique_index = np.unique(par_opt_slice,
                                                    return_index=True)
     opt_grad[par_opt_slice_unique] += \
         coefficient * sim_grad[par_sim_slice[unique_index]]
@@ -200,22 +199,20 @@
         par_opt_ids: Sequence[str],
         par_sim_ids: Sequence[str],
         condition_map_sim_var: Dict[str, Union[float, str]],
         sim_hess: np.ndarray,
         opt_hess: np.ndarray,
         coefficient: float = 1.0):
     """
-    Sum simulation hessians to objective hessian according to the provided
-    mapping `mapping_par_opt_to_par_sim`.
+    Sum simulation hessians to objective hessian.
 
     Parameters
     ----------
     Same as for add_sim_grad_to_opt_grad, replacing the gradients by hessians.
     """
-
     par_sim_slice, par_opt_slice = par_index_slices(par_opt_ids, par_sim_ids,
                                                     condition_map_sim_var)
 
     par_opt_slice_unique, unique_index = np.unique(par_opt_slice,
                                                    return_index=True)
 
     non_unique_indices = [idx for idx in range(len(par_opt_slice))
@@ -241,16 +238,16 @@
 
 def sim_sres_to_opt_sres(par_opt_ids: Sequence[str],
                          par_sim_ids: Sequence[str],
                          condition_map_sim_var: Dict[str, Union[float, str]],
                          sim_sres: np.ndarray,
                          coefficient: float = 1.0):
     """
-    Sum simulation residual sensitivities to objective residual sensitivities
-    according to the provided mapping.
+
+    Sum simulation residual sensitivities to objective residual sensitivities.
 
     Parameters
     ----------
     Mostly the same as for add_sim_grad_to_opt_grad, replacing the gradients by
     residual sensitivities.
     """
     opt_sres = np.zeros((sim_sres.shape[0], len(par_opt_ids)))
@@ -288,15 +285,15 @@
 def get_error_output(
         amici_model: AmiciModel,
         edatas: Sequence['amici.ExpData'],
         rdatas: Sequence['amici.ReturnData'],
         sensi_order: int,
         mode: str,
         dim: int):
-    """Default output upon error.
+    """Get default output upon error.
 
     Returns values indicative of an error, that is with nan entries in all
     vectors, and a function value, i.e. nllh, of `np.inf`.
     """
     if not amici_model.nt():
         nt = sum(data.nt() for data in edatas)
     else:
@@ -320,14 +317,15 @@
         SRES: sres,
         RDATAS: rdatas
     }
     return filter_return_dict(ret)
 
 
 def init_return_values(sensi_order, mode, dim, error=False):
+    """Initialize return values."""
     if error:
         fval = np.inf
         sval = np.nan
     else:
         fval = sval = 0.0
 
     nllh = fval
@@ -347,13 +345,13 @@
         if sensi_order > 0:
             sres = np.zeros([0, dim])
 
     return nllh, snllh, s2nllh, chi2, res, sres
 
 
 def filter_return_dict(ret):
-    """Filters return dict for non-None values"""
+    """Filter return dict for non-None values."""
     return {
         key: val
         for key, val in ret.items()
         if val is not None
     }
```

### Comparing `pypesto-0.2.8/pypesto/objective/base.py` & `pypesto-0.2.9/pypesto/objective/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 ResultDict = Dict[str, Union[float, np.ndarray, Dict]]
 
 logger = logging.getLogger(__name__)
 
 
 class ObjectiveBase(abc.ABC):
     """
+    Abstract objective class.
+
     The objective class is a simple wrapper around the objective function,
     giving a standardized way of calling. Apart from that, it manages several
     things including fixing of parameters and history.
 
     The objective function is assumed to be in the format of a cost function,
     log-likelihood function, or log-posterior function. These functions are
     subject to minimization. For profiling and sampling, the sign is internally
@@ -50,76 +52,87 @@
 
         self._x_names = x_names
 
         self.pre_post_processor = PrePostProcessor()
         self.history = HistoryBase()
 
     def __deepcopy__(self, memodict=None) -> 'ObjectiveBase':
+        """Create deepcopy of objective object."""
         other = type(self)()  # maintain type for derived classes
         for attr, val in self.__dict__.items():
             other.__dict__[attr] = copy.deepcopy(val)
         return other
 
     # The following has_ properties can be used to find out what values
     # the objective supports.
     @property
     def has_fun(self) -> bool:
+        """Check whether function is defined."""
         return self.check_sensi_orders((0,), MODE_FUN)
 
     @property
     def has_grad(self) -> bool:
+        """Check whether gradient is defined."""
         return self.check_sensi_orders((1,), MODE_FUN)
 
     @property
     def has_hess(self) -> bool:
+        """Check whether Hessian is defined."""
         return self.check_sensi_orders((2,), MODE_FUN)
 
     @property
-    def has_hessp(self) -> bool:
+    def has_hessp(self) -> bool: # noqa
         # Not supported yet
         return False
 
     @property
     def has_res(self) -> bool:
+        """Check whether residuals are defined."""
         return self.check_sensi_orders((0,), MODE_RES)
 
     @property
     def has_sres(self) -> bool:
+        """Check whether residual sensitivities are defined."""
         return self.check_sensi_orders((1,), MODE_RES)
 
     @property
     def x_names(self) -> Union[List[str], None]:
+        """Parameter names."""
         if self._x_names is None:
             return self._x_names
 
         # change from numpy array with `str_` dtype to list with `str` dtype
         # to avoid issues when writing to hdf (and correctness of typehint)
         return [
             str(name) for name in
             self.pre_post_processor.reduce(np.asarray(self._x_names))
         ]
 
     def initialize(self):
-        """Initialize the objective function.
+        """
+        Initialize the objective function.
+
         This function is used at the beginning of an analysis, e.g.
         optimization, and can e.g. reset the objective memory.
         By default does nothing.
         """
 
     def __call__(
         self,
         x: np.ndarray,
         sensi_orders: Tuple[int, ...] = (0, ),
         mode: str = MODE_FUN,
         return_dict: bool = False,
         **kwargs,
     ) -> Union[float, np.ndarray, Tuple, ResultDict]:
         """
-        Method to obtain arbitrary sensitivities. This is the central method
-        which is always called, also by the get_* methods.
+        Obtain arbitrary sensitivities.
+
+        This is the central method which is always called, also by the
+        get_* methods.
 
         There are different ways in which an optimizer calls the objective
         function, and in how the objective function provides information
         (e.g. derivatives via separate functions or along with the function
         values). The different calling modes increase efficiency in space
         and time and make the objective flexible.
 
@@ -182,16 +195,15 @@
         self,
         x: np.ndarray,
         sensi_orders: Tuple[int, ...],
         mode: str,
         **kwargs,
     ) -> ResultDict:
         """
-        Call objective function without pre- or post-processing and
-        formatting.
+        Call objective function without pre- or post-processing and formatting.
 
         Parameters
         ----------
         x:
             The parameters for which to evaluate the objective function.
         sensi_orders:
             Specifies which sensitivities to compute, e.g. (0,1) -> fval, grad.
@@ -212,42 +224,43 @@
         Either `check_mode` or the `fun_...` functions
         must be overwritten in derived classes.
 
         Parameters
         ----------
         mode:
             Whether to compute function values or residuals.
+
         Returns
         -------
         flag:
             Boolean indicating whether mode is supported
         """
         if mode == MODE_FUN:
             return self.has_fun
         elif mode == MODE_RES:
             return self.has_res
         else:
             raise ValueError(f"Unknown mode {mode}.")
 
     def get_config(self) -> dict:
         """
-        Get the configuration information of the objective
-        function and return it as a dictonary.
+        Get the configuration information of the objective function.
+
+        Return it as a dictonary.
         """
         info = {'type':  self.__class__.__name__}
         return info
 
     def check_sensi_orders(
         self,
         sensi_orders: Tuple[int, ...],
         mode: str,
     ) -> bool:
         """
-        Check if the objective is able to compute the requested
-        sensitivities.
+        Check if the objective is able to compute the requested sensitivities.
 
         Either `check_sensi_orders` or the `fun_...` functions
         must be overwritten in derived classes.
 
         Parameters
         ----------
         sensi_orders:
@@ -284,17 +297,19 @@
     @staticmethod
     def output_to_tuple(
         sensi_orders: Tuple[int, ...],
         mode: str,
         **kwargs: Union[float, np.ndarray],
     ) -> Tuple:
         """
-        Return values as requested by the caller, since usually only a subset
-        is demanded. One output is returned as-is, more than one output are
-        returned as a tuple in order (fval, grad, hess).
+        Return values as requested by the caller.
+
+        Usually only a subset of outputs is demanded. One output is returned
+        as-is, more than one output are returned as a tuple in order (fval,
+        grad, hess).
         """
         output = ()
         if mode == MODE_FUN:
             if 0 in sensi_orders:
                 output += (kwargs[FVAL],)
             if 1 in sensi_orders:
                 output += (kwargs[GRAD],)
@@ -308,15 +323,14 @@
         if len(output) == 1:
             output = output[0]
         return output
 
     # The following are convenience functions for getting specific outputs.
     def get_fval(self, x: np.ndarray) -> float:
         """Get the function value at x."""
-
         fval = self(x, (0,), MODE_FUN)
         return fval
 
     def get_grad(self, x: np.ndarray) -> np.ndarray:
         """Get the gradient at x."""
         grad = self(x, (1,), MODE_FUN)
         return grad
@@ -340,19 +354,21 @@
         self,
         dim_full: int,
         x_free_indices: Sequence[int],
         x_fixed_indices: Sequence[int],
         x_fixed_vals: Sequence[float],
     ):
         """
-        Handle fixed parameters. Later, the objective will be given parameter
-        vectors x of dimension dim, which have to be filled up with fixed
-        parameter values to form a vector of dimension dim_full >= dim.
-        This vector is then used to compute function value and derivatives.
-        The derivatives must later be reduced again to dimension dim.
+        Handle fixed parameters.
+
+        Later, the objective will be given parameter vectors x of dimension
+        dim, which have to be filled up with fixed parameter values to form
+        a vector of dimension dim_full >= dim. This vector is then used to
+        compute function value and derivatives. The derivatives must later
+        be reduced again to dimension dim.
 
         This is so as to make the fixing of parameters transparent to the
         caller.
 
         The methods preprocess, postprocess are overwritten for the above
         functionality, respectively.
 
@@ -366,15 +382,14 @@
         x_fixed_indices:
             Vector containing the indices (zero-based) of parameter components
             that are not to be optimized.
         x_fixed_vals:
             Vector of the same length as x_fixed_indices, containing the values
             of the fixed parameters.
         """
-
         pre_post_processor = FixedParametersProcessor(
             dim_full=dim_full,
             x_free_indices=x_free_indices,
             x_fixed_indices=x_fixed_indices,
             x_fixed_vals=x_fixed_vals)
 
         self.pre_post_processor = pre_post_processor
@@ -383,14 +398,16 @@
         self,
         *args,
         multi_eps: Optional[Iterable] = None,
         label: str = 'rel_err',
         **kwargs,
     ):
         """
+        Compare gradient evaluation.
+
         Equivalent to the `ObjectiveBase.check_grad` method, except multiple
         finite difference step sizes are tested. The result contains the
         lowest finite difference for each parameter, and the corresponding
         finite difference step size.
 
         Parameters
         ----------
@@ -438,16 +455,18 @@
         eps: float = 1e-5,
         verbosity: int = 1,
         mode: str = MODE_FUN,
         order: int = 0,
         detailed: bool = False,
     ) -> pd.DataFrame:
         """
-        Compare gradient evaluation: Firstly approximate via finite
-        differences, and secondly use the objective gradient.
+        Compare gradient evaluation.
+
+        Firstly approximate via finite differences, and secondly use the
+        objective gradient.
 
         Parameters
         ----------
         x:
             The parameters for which to evaluate the gradient.
         x_indices:
             Indices for which to compute gradients. Default: all.
@@ -466,19 +485,18 @@
         detailed:
             Toggle whether additional values are returned. Additional values
             are function values, and the central difference weighted by the
             difference in output from all methods (standard deviation and
             mean).
 
         Returns
-        ----------
+        -------
         result:
             gradient, finite difference approximations and error estimates.
         """
-
         if x_indices is None:
             x_indices = list(range(len(x)))
 
         # function value and objective gradient
         fval, grad = self(x, (0 + order, 1 + order), mode)
 
         grad_list = []
@@ -609,15 +627,15 @@
         rtol: float = 1e-2,
         atol: float = 1e-3,
         mode: str = None,
         order: int = 0,
         multi_eps=None,
         **kwargs,
     ) -> bool:
-        """Check if gradients match finite differences (FDs)
+        """Check if gradients match finite differences (FDs).
 
         Parameters
         ----------
         rtol: relative error tolerance
         x: The parameters for which to evaluate the gradient
         x_free: Indices for which to compute gradients
         rtol: relative error tolerance
```

### Comparing `pypesto-0.2.8/pypesto/objective/constants.py` & `pypesto-0.2.9/pypesto/objective/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-"""
-This is for (string) constants used in the objective module.
-"""
-
+"""Constants used in the objective module."""
 
 MODE_FUN = 'mode_fun'  # mode for function values
 MODE_RES = 'mode_res'  # mode for residuals
 FVAL = 'fval'  # function value
 FVAL0 = 'fval0'  # function value at start
 GRAD = 'grad'  # gradient
 HESS = 'hess'  # Hessian
```

### Comparing `pypesto-0.2.8/pypesto/objective/finite_difference.py` & `pypesto-0.2.9/pypesto/objective/finite_difference.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,23 +140,23 @@
     def _update(
         self,
         x: np.ndarray,
         fval: Union[float, np.ndarray],
         fun: Callable,
         fd_method: str,
     ) -> None:
-        """Actually update. Wants to be called in `update` explicitly.
+        """
+        Actually update. Wants to be called in `update` explicitly.
 
         Run FDs with various deltas and pick the ones, separately for each
         parameter, with the best stability properties.
 
         The parameters are the same as for
         :func:`pypesto.objective.finite_difference.FDDelta.update`.
         """
-
         # calculate gradients for all deltas for all parameters
         nablas = []
         # iterate over deltas
         for delta in self.test_deltas:
             # calculate Jacobian with step size delta
             delta_vec = delta * np.ones_like(x)
             nabla = fd_nabla_1(
@@ -318,49 +318,58 @@
                 f"Method must be one of {FD.METHODS}.",
             )
 
     def __deepcopy__(
         self,
         memodict: Dict = None,
     ) -> 'FD':
+        """Create deepcopy of Objective."""
         other = self.__class__.__new__(self.__class__)
         for attr, val in self.__dict__.items():
             other.__dict__[attr] = copy.deepcopy(val)
         return other
 
     @property
     def has_fun(self) -> bool:
+        """Check whether function is defined."""
         return self.obj.has_fun
 
     @property
     def has_grad(self) -> bool:
+        """Check whether gradient is defined."""
         return self.grad is not False and self.obj.has_fun
 
     @property
     def has_hess(self) -> bool:
+        """Check whether Hessian is defined."""
         return self.hess is not False and self.obj.has_fun
 
     @property
     def has_res(self) -> bool:
+        """Check whether residuals are defined."""
         return self.obj.has_res
 
     @property
     def has_sres(self) -> bool:
+        """Check whether residual sensitivities are defined."""
         return self.sres is not False and self.obj.has_res
 
     def call_unprocessed(
         self,
         x: np.ndarray,
         sensi_orders: Tuple[int, ...],
         mode: str,
         **kwargs,
     ) -> ResultDict:
-        # This is the main method to overwrite from the base class, it handles
-        #  and delegates the actual objective evaluation.
+        """
+        See `ObjectiveBase` for more documentation.
 
+        Main method to overwrite from the base class. It handles and
+        delegates the actual objective evaluation.
+        """
         if mode == MODE_FUN:
             result = self._call_mode_fun(
                 x=x, sensi_orders=sensi_orders, **kwargs)
         elif mode == MODE_RES:
             result = self._call_mode_res(
                 x=x, sensi_orders=sensi_orders, **kwargs)
         else:
@@ -479,16 +488,18 @@
     def _call_from_obj_fun(
         self,
         x: np.ndarray,
         sensi_orders: Tuple[int, ...],
         **kwargs,
     ) -> Tuple[Tuple[int, ...], ResultDict]:
         """
-        Helper function that calculates from the objective the sensitivities
-        that are supposed to be calculated from the objective and not via FDs.
+        Call objective function for sensitivities.
+
+        Calculate from the objective the sensitivities that are supposed to
+        be calculated from the objective and not via FDs.
         """
         # define objective sensis
         sensi_orders_obj = []
         if 0 in sensi_orders:
             sensi_orders_obj.append(0)
         if 1 in sensi_orders and self.grad is None and self.obj.has_grad:
             sensi_orders_obj.append(1)
@@ -505,16 +516,18 @@
     def _call_from_obj_res(
         self,
         x: np.ndarray,
         sensi_orders: Tuple[int, ...],
         **kwargs,
     ) -> Tuple[Tuple[int, ...], ResultDict]:
         """
-        Helper function that calculates from the objective the sensitivities
-        that are supposed to be calculated from the objective and not via FDs.
+        Call objective function for sensitivities in residual mode.
+
+        Calculate from the objective the sensitivities that are supposed to
+        be calculated from the objective and not via FDs.
         """
         # define objective sensis
         sensi_orders_obj = []
         if 0 in sensi_orders:
             sensi_orders_obj.append(0)
         if 1 in sensi_orders and self.sres is None and self.obj.has_sres:
             sensi_orders_obj.append(1)
@@ -524,15 +537,16 @@
         if sensi_orders_obj:
             result = self.obj.call_unprocessed(
                 x=x, sensi_orders=sensi_orders_obj, mode=MODE_RES, **kwargs)
         return sensi_orders_obj, result
 
 
 def unit_vec(dim: int, ix: int) -> np.ndarray:
-    """Unit vector of dimension `dim` at coordinate `ix`.
+    """
+    Return unit vector of dimension `dim` at coordinate `ix`.
 
     Parameters
     ----------
     dim: Vector dimension.
     ix: Index to contain the unit value.
 
     Returns
```

### Comparing `pypesto-0.2.8/pypesto/objective/function.py` & `pypesto-0.2.9/pypesto/objective/function.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,77 +4,73 @@
 from typing import Callable, Sequence, Tuple, Union
 
 from .constants import MODE_FUN, MODE_RES, FVAL, GRAD, HESS, RES, SRES
 
 
 class Objective(ObjectiveBase):
     """
+    Objective class.
+
     The objective class allows the user explicitly specify functions that
     compute the function value and/or residuals as well as respective
     derivatives.
 
     Denote dimensions `n` = parameters, `m` = residuals.
 
     Parameters
     ----------
-
     fun:
         The objective function to be minimized. If it only computes the
         objective function value, it should be of the form
 
             ``fun(x) -> float``
 
         where x is an 1-D array with shape (n,), and n is the parameter space
         dimension.
-
     grad:
         Method for computing the gradient vector. If it is a callable,
         it should be of the form
 
             ``grad(x) -> array_like, shape (n,).``
 
         If its value is True, then fun should return the gradient as a second
         output.
-
     hess:
         Method for computing the Hessian matrix. If it is a callable,
         it should be of the form
 
             ``hess(x) -> array, shape (n, n).``
 
         If its value is True, then fun should return the gradient as a
         second, and the Hessian as a third output, and grad should be True as
         well.
-
     hessp:
         Method for computing the Hessian vector product, i.e.
 
             ``hessp(x, v) -> array_like, shape (n,)``
 
         computes the product H*v of the Hessian of fun at x with v.
-
     res:
         Method for computing residuals, i.e.
 
             ``res(x) -> array_like, shape(m,).``
-
     sres:
         Method for computing residual sensitivities. If it is a callable,
         it should be of the form
 
             ``sres(x) -> array, shape (m, n).``
 
         If its value is True, then res should return the residual
         sensitivities as a second output.
-
     x_names:
         Parameter names. None if no names provided, otherwise a list of str,
         length dim_full (as in the Problem class). Can be read by the
         problem.
     """
+
     def __init__(
         self,
         fun: Callable = None,
         grad: Union[Callable, bool] = None,
         hess: Callable = None,
         hessp: Callable = None,
         res: Callable = None,
@@ -87,38 +83,44 @@
         self.hessp = hessp
         self.res = res
         self.sres = sres
         super().__init__(x_names)
 
     @property
     def has_fun(self) -> bool:
+        """Check whether function is defined."""
         return callable(self.fun)
 
     @property
     def has_grad(self) -> bool:
+        """Check whether gradient is defined."""
         return callable(self.grad) or self.grad is True
 
     @property
     def has_hess(self) -> bool:
+        """Check whether Hessian is defined."""
         return callable(self.hess) or self.hess is True
 
     @property
-    def has_hessp(self) -> bool:
+    def has_hessp(self) -> bool: # noqa
         # Not supported yet
         return False
 
     @property
     def has_res(self) -> bool:
+        """Check whether residuals are defined."""
         return callable(self.res)
 
     @property
     def has_sres(self) -> bool:
+        """Check whether residual sensitivities are defined."""
         return callable(self.sres) or self.sres is True
 
     def get_config(self) -> dict:
+        """Return basic information of the objective configuration."""
         info = super().get_config()
         info['x_names'] = self.x_names
         sensi_order = 0
         while self.check_sensi_orders(
                 sensi_orders=(sensi_order,), mode=MODE_FUN):
             sensi_order += 1
         info['sensi_order'] = sensi_order - 1
@@ -128,16 +130,15 @@
         self,
         x: np.ndarray,
         sensi_orders: Tuple[int, ...],
         mode: str,
         **kwargs,
     ) -> ResultDict:
         """
-        Call objective function without pre- or post-processing and
-        formatting.
+        Call objective function without pre- or post-processing and formatting.
 
         Returns
         -------
         result:
             A dict containing the results.
         """
         if mode == MODE_FUN:
```

### Comparing `pypesto-0.2.8/pypesto/objective/history.py` & `pypesto-0.2.9/pypesto/objective/history.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 
 ResultDict = Dict[str, Union[float, np.ndarray]]
 MaybeArray = Union[np.ndarray, 'np.nan']
 
 
 def trace_wrap(f):
     """
-    Wrapper around trace getters that transforms input `ix` vectors to a valid
-    index list, and reduces for integer `ix` the output to a single value.
+    Wrap around trace getters.
+
+    Transform input `ix` vectors to a valid index list, and reduces for
+    integer `ix` the output to a single value.
     """
     def wrapped_f(
             self, ix: Union[Sequence[int], int, None] = None,
             trim: bool = False
     ) -> Union[Sequence[Union[float, MaybeArray]], Union[float, MaybeArray]]:
         # whether to reduce the output
         reduce = isinstance(ix, numbers.Integral)
@@ -45,16 +47,15 @@
             trace = trace[0]
         return trace
     return wrapped_f
 
 
 class HistoryOptions(dict):
     """
-    Options for the objective that are used in optimization, profiling
-    and sampling.
+    Options for the objective that are used in optimization.
 
     In addition implements a factory pattern to generate history objects.
 
     Parameters
     ----------
     trace_record:
         Flag indicating whether to record the trace of function calls.
@@ -103,52 +104,52 @@
         self.trace_record_sres = trace_record_sres
         self.trace_record_chi2 = trace_record_chi2
         self.trace_record_schi2 = trace_record_schi2
         self.trace_save_iter = trace_save_iter
         self.storage_file = storage_file
 
     def __getattr__(self, key):
+        """Allow to use keys as attributes."""
         try:
             return self[key]
         except KeyError:
             raise AttributeError(key)
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
     @staticmethod
     def assert_instance(
             maybe_options: Union['HistoryOptions', Dict]
     ) -> 'HistoryOptions':
         """
-        Returns a valid options object.
+        Return a valid options object.
 
         Parameters
         ----------
         maybe_options: HistoryOptions or dict
         """
         if isinstance(maybe_options, HistoryOptions):
             return maybe_options
         options = HistoryOptions(**maybe_options)
         return options
 
     def create_history(
             self, id: str, x_names: Sequence[str]
     ) -> 'History':
-        """Factory method creating a :class:`History` object.
+        """Create a :class:`History` object; Factory method.
 
         Parameters
         ----------
         id:
             Identifier for the history.
         x_names:
             Parameter names.
         """
         # create different history types based on the inputs
-
         if self.storage_file is None:
             if self.trace_record:
                 return MemoryHistory(options=self)
             else:
                 return History(options=self)
 
         storage_file = self.storage_file.replace("{id}", id)
@@ -171,15 +172,15 @@
     """Abstract base class for history objects.
 
     Can be used as a dummy history, but does not implement any history
     functionality.
     """
 
     def __len__(self):
-        """Number of stored entries in the history"""
+        """Define length by number of stored entries in the history."""
         raise NotImplementedError()
 
     def update(
             self,
             x: np.ndarray,
             sensi_orders: Tuple[int, ...],
             mode: str,
@@ -201,152 +202,159 @@
         """
 
     def finalize(self):
         """Finalize history. Called after a run."""
 
     @property
     def n_fval(self) -> int:
-        """Number of function evaluations."""
+        """Return number of function evaluations."""
         raise NotImplementedError()
 
     @property
     def n_grad(self) -> int:
-        """Number of gradient evaluations."""
+        """Return number of gradient evaluations."""
         raise NotImplementedError()
 
     @property
     def n_hess(self) -> int:
-        """Number of Hessian evaluations."""
+        """Return number of Hessian evaluations."""
         raise NotImplementedError()
 
     @property
     def n_res(self) -> int:
-        """Number of residual evaluations."""
+        """Return number of residual evaluations."""
         raise NotImplementedError()
 
     @property
     def n_sres(self) -> int:
-        """Number or residual sensitivity evaluations."""
+        """Return number or residual sensitivity evaluations."""
         raise NotImplementedError()
 
     @property
     def start_time(self) -> float:
-        """Start time."""
+        """Return start time."""
         raise NotImplementedError()
 
     def get_x_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[np.ndarray], np.ndarray]:
-        """Parameters.
+        """
+        Return parameters.
 
         Takes as parameter an index or indices and returns corresponding trace
         values. If only a single value is requested, the list is flattened.
         """
         raise NotImplementedError()
 
     def get_fval_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[float], float]:
-        """Function values.
+        """
+        Return function values.
 
         Takes as parameter an index or indices and returns corresponding trace
         values. If only a single value is requested, the list is flattened.
         """
         raise NotImplementedError()
 
     def get_grad_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
-        """Gradients.
+        """
+        Return gradients.
 
         Takes as parameter an index or indices and returns corresponding trace
         values. If only a single value is requested, the list is flattened.
         """
         raise NotImplementedError()
 
     def get_hess_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
-        """Hessians.
+        """
+        Return hessians.
 
         Takes as parameter an index or indices and returns corresponding trace
         values. If only a single value is requested, the list is flattened.
         """
         raise NotImplementedError()
 
     def get_res_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
-        """Residuals.
+        """
+        Residuals.
 
         Takes as parameter an index or indices and returns corresponding trace
         values. If only a single value is requested, the list is flattened.
         """
         raise NotImplementedError()
 
     def get_sres_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
-        """Residual sensitivities.
+        """
+        Residual sensitivities.
 
         Takes as parameter an index or indices and returns corresponding trace
         values. If only a single value is requested, the list is flattened.
         """
         raise NotImplementedError()
 
     def get_chi2_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[float], float]:
-        """Chi2 values.
+        """
+        Chi2 values.
 
         Takes as parameter an index or indices and returns corresponding trace
         values. If only a single value is requested, the list is flattened.
         """
         raise NotImplementedError()
 
     def get_schi2_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
-        """Chi2 sensitivities.
+        """
+        Chi2 sensitivities.
 
         Takes as parameter an index or indices and returns corresponding trace
         values. If only a single value is requested, the list is flattened.
         """
         raise NotImplementedError()
 
     def get_time_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[float], float]:
-        """Cumulative execution times.
+        """
+        Cumulative execution times.
 
         Takes as parameter an index or indices and returns corresponding trace
         values. If only a single value is requested, the list is flattened.
         """
         raise NotImplementedError()
 
     def get_trimmed_indices(self):
-        """
-        Returns indices of the history to get a monotonically
-        decreasing history.
-        """
+        """Get indices for a monotonically decreasing history."""
         fval_trace = self.get_fval_trace()
         return np.where(fval_trace <= np.fmin.accumulate(fval_trace))[0]
 
 
 class History(HistoryBase):
-    """Tracks numbers of function evaluations only, no trace.
+    """
+    Track number of function evaluations only, no trace.
 
     Parameters
     ----------
     options:
         History options.
     """
 
@@ -387,22 +395,21 @@
         res = result.get(RES, None)
         if res is not None and FVAL not in result:
             # no option trace_record_fval
             result[FVAL] = res_to_fval(res)
         self._update_counts(sensi_orders, mode)
 
     def finalize(self):
+        """See `HistoryBase` docstring."""
         pass
 
     def _update_counts(self,
                        sensi_orders: Tuple[int, ...],
                        mode: str):
-        """
-        Update the counters.
-        """
+        """Update the counters."""
         if mode == MODE_FUN:
             if 0 in sensi_orders:
                 self._n_fval += 1
             if 1 in sensi_orders:
                 self._n_grad += 1
             if 2 in sensi_orders:
                 self._n_hess += 1
@@ -410,62 +417,73 @@
             if 0 in sensi_orders:
                 self._n_res += 1
             if 1 in sensi_orders:
                 self._n_sres += 1
 
     @property
     def n_fval(self) -> int:
+        """See `HistoryBase` docstring."""
         return self._n_fval
 
     @property
     def n_grad(self) -> int:
+        """See `HistoryBase` docstring."""
         return self._n_grad
 
     @property
     def n_hess(self) -> int:
+        """See `HistoryBase` docstring."""
         return self._n_hess
 
     @property
     def n_res(self) -> int:
+        """See `HistoryBase` docstring."""
         return self._n_res
 
     @property
     def n_sres(self) -> int:
+        """See `HistoryBase` docstring."""
         return self._n_sres
 
     @property
     def start_time(self) -> float:
+        """See `HistoryBase` docstring."""
         return self._start_time
 
 
 class MemoryHistory(History):
-    """Tracks numbers of function evaluations and keeps an in-memory
+    """
+    Class for optimization history stored in memory.
+
+    Track number of function evaluations and keeps an in-memory
     trace of function evaluations.
 
     Parameters
     ----------
     options:
         History options.
     """
 
     def __init__(self, options: Union[HistoryOptions, Dict] = None):
         super().__init__(options=options)
         self._trace_keys = {X, FVAL, GRAD, HESS, RES, SRES, CHI2, SCHI2, TIME}
         self._trace: Dict[str, Any] = {key: [] for key in self._trace_keys}
 
     def __len__(self):
+        """Define length of history object."""
         return len(self._trace[TIME])
 
     def update(
             self,
             x: np.ndarray,
             sensi_orders: Tuple[int, ...],
             mode: str,
             result: ResultDict
     ) -> None:
+        """See `History` docstring."""
         super().update(x, sensi_orders, mode, result)
         self._update_trace(x, mode, result)
 
     def _update_trace(self, x, mode, result):
         """Update internal trace representation."""
         ret = extract_values(mode, result, self.options)
         for key in self._trace_keys - {X, TIME}:
@@ -475,70 +493,79 @@
         self._trace[TIME].append(used_time)
 
     @trace_wrap
     def get_x_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[np.ndarray], np.ndarray]:
+        """See `HistoryBase` docstring."""
         return [self._trace[X][i] for i in ix]
 
     @trace_wrap
     def get_fval_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[float], float]:
+        """See `HistoryBase` docstring."""
         return [self._trace[FVAL][i] for i in ix]
 
     @trace_wrap
     def get_grad_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return [self._trace[GRAD][i] for i in ix]
 
     @trace_wrap
     def get_hess_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return [self._trace[HESS][i] for i in ix]
 
     @trace_wrap
     def get_res_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return [self._trace[RES][i] for i in ix]
 
     @trace_wrap
     def get_sres_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return [self._trace[SRES][i] for i in ix]
 
     @trace_wrap
     def get_chi2_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[float], float]:
+        """See `HistoryBase` docstring."""
         return [self._trace[CHI2][i] for i in ix]
 
     @trace_wrap
     def get_schi2_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return [self._trace[SCHI2][i] for i in ix]
 
     @trace_wrap
     def get_time_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[float], float]:
+        """See `HistoryBase` docstring."""
         return [self._trace[TIME][i] for i in ix]
 
 
 class CsvHistory(History):
     """Stores a representation of the history in a CSV file.
 
     Parameters
@@ -581,14 +608,15 @@
                 trace[col] = trace[col].apply(string2ndarray)
 
             self._trace = trace
             self.x_names = trace[X].columns
             self._update_counts_from_trace()
 
     def __len__(self):
+        """Define length of history object."""
         return len(self._trace)
 
     def _update_counts_from_trace(self):
         self._n_fval = self._trace[('n_fval', np.NaN)].max()
         self._n_grad = self._trace[('n_grad', np.NaN)].max()
         self._n_hess = self._trace[('n_hess', np.NaN)].max()
         self._n_res = self._trace[('n_res', np.NaN)].max()
@@ -597,29 +625,28 @@
     def update(
             self,
             x: np.ndarray,
             sensi_orders: Tuple[int, ...],
             mode: str,
             result: ResultDict
     ) -> None:
+        """See `History` docstring."""
         super().update(x, sensi_orders, mode, result)
         self._update_trace(x, mode, result)
 
     def finalize(self):
         """Finalize history. Called after a run."""
         super().finalize()
         self._save_trace(finalize=True)
 
     def _update_trace(self,
                       x: np.ndarray,
                       mode: str,
                       result: ResultDict):
-        """
-        Update and possibly store the trace.
-        """
+        """Update and possibly store the trace."""
         if not self.options.trace_record:
             return
 
         # init trace
         if self._trace is None:
             self._init_trace(x)
 
@@ -658,17 +685,15 @@
 
         self._trace = self._trace.append(row)
 
         # save trace to file
         self._save_trace()
 
     def _init_trace(self, x: np.ndarray):
-        """
-        Initialize the trace.
-        """
+        """Initialize the trace."""
         if self.x_names is None:
             self.x_names = [f'x{i}' for i, _ in enumerate(x)]
 
         columns: List[Tuple] = [
             (c, float('nan')) for c in [
                 TIME, N_FVAL, N_GRAD, N_HESS, N_RES, N_SRES,
                 FVAL, CHI2, RES, SRES, HESS,
@@ -702,16 +727,18 @@
 
         for var, dtype in trace_dtypes.items():
             self._trace[(var, np.NaN)] = \
                 self._trace[(var, np.NaN)].astype(dtype)
 
     def _save_trace(self, finalize: bool = False):
         """
-        Save to file via pd.DataFrame.to_csv() if `self.storage_file` is
-        not None and other conditions apply.
+        Save to file via pd.DataFrame.to_csv().
+
+        Only done, if `self.storage_file` is not None and other conditions.
+        apply.
         """
         if self.file is None:
             return
 
         if finalize \
                 or (len(self._trace) > 0 and len(self._trace) %
                     self.options.trace_save_iter == 0):
@@ -724,75 +751,85 @@
             trace_copy.to_csv(self.file)
 
     @trace_wrap
     def get_x_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[np.ndarray], np.ndarray]:
+        """See `HistoryBase` docstring."""
         return list(self._trace[X].values[ix])
 
     @trace_wrap
     def get_fval_trace(
             self, ix: Union[int, Sequence[int], None],
             trim: bool = False
     ) -> Union[Sequence[float], float]:
+        """See `HistoryBase` docstring."""
         return list(self._trace[(FVAL, np.nan)].values[ix])
 
     @trace_wrap
     def get_grad_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return list(self._trace[GRAD].values[ix])
 
     @trace_wrap
     def get_hess_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return list(self._trace[(HESS, np.nan)].values[ix])
 
     @trace_wrap
     def get_res_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return list(self._trace[(RES, np.nan)].values[ix])
 
     @trace_wrap
     def get_sres_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return list(self._trace[(SRES, np.nan)].values[ix])
 
     @trace_wrap
     def get_chi2_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[float], float]:
+        """See `HistoryBase` docstring."""
         return list(self._trace[(CHI2, np.nan)].values[ix])
 
     @trace_wrap
     def get_schi2_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return list(self._trace[SCHI2].values[ix])
 
     @trace_wrap
     def get_time_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[float], float]:
+        """See `HistoryBase` docstring."""
         return list(self._trace[(TIME, np.nan)].values[ix])
 
 
 class Hdf5History(History):
-    """Stores a representation of the history in an HDF5 file.
+    """
+    Stores a representation of the history in an HDF5 file.
 
     Parameters
     ----------
     id:
         Id of the history
     file:
         HDF5 file name.
@@ -806,46 +843,51 @@
                  options: Union[HistoryOptions, Dict] = None):
         super().__init__(options=options)
         self.id = id
         self.file = file
         self._generate_hdf5_group()
 
     def __len__(self):
+        """Define length of history object."""
         with h5py.File(self.file, 'r') as f:
             return f[f'history/{self.id}/trace/'].attrs[
                         'n_iterations']
 
     def update(
             self,
             x: np.ndarray,
             sensi_orders: Tuple[int, ...],
             mode: str,
             result: ResultDict
     ) -> None:
+        """See `History` docstring."""
         super().update(x, sensi_orders, mode, result)
         self._update_trace(x, sensi_orders, mode, result)
 
     def get_history_directory(self):
+        """Return filepath."""
         return self.file
 
     def finalize(self):
+        """See `History` docstring."""
         super().finalize()
 
     @staticmethod
     def load(id: str,
              file: str):
-        """Loads the History object from memory."""
+        """Load the History object from memory."""
         loaded_h5history = Hdf5History(id, file)
         loaded_h5history._recover_options(file)
         return loaded_h5history
 
     def _recover_options(self, file: str):
         """
-        Recovers options when loading the hdf5 history from memory
-        by testing which entries were recorded.
+        Recover options when loading the hdf5 history from memory.
+
+        Done by testing which entries were recorded.
         """
         trace_record = self._check_for_not_nan_entries(X)
         trace_record_grad = self._check_for_not_nan_entries(GRAD)
         trace_record_hess = self._check_for_not_nan_entries(HESS)
         trace_record_res = self._check_for_not_nan_entries(RES)
         trace_record_sres = self._check_for_not_nan_entries(SRES)
         trace_record_chi2 = self._check_for_not_nan_entries(CHI2)
@@ -862,30 +904,28 @@
                            trace_record_schi2=trace_record_schi2,
                            trace_save_iter=self.trace_save_iter,
                            storage_file=storage_file)
 
         self.options = restored_history_options
 
     def _check_for_not_nan_entries(self, hdf5_group: str) -> bool:
-        """Checks if there exist not-nan entries stored for a given group"""
+        """Check if there exist not-nan entries stored for a given group."""
         group = self._get_hdf5_entries(hdf5_group, ix=None)
 
         for entry in group:
             if not (entry is None or np.all(np.isnan(entry))):
                 return True
 
         return False
 
     # overwrite _update_counts
     def _update_counts(self,
                        sensi_orders: Tuple[int, ...],
                        mode: str):
-        """
-        Update the counters in the hdf5
-        """
+        """Update the counters in the hdf5."""
         with h5py.File(self.file, 'a') as f:
 
             if mode == MODE_FUN:
                 if 0 in sensi_orders:
                     f[f'history/{self.id}/trace/'].attrs[
                         'n_fval'] += 1
                 if 1 in sensi_orders:
@@ -900,52 +940,55 @@
                         'n_res'] += 1
                 if 1 in sensi_orders:
                     f[f'history/{self.id}/trace/'].attrs[
                         'n_sres'] += 1
 
     @property
     def n_fval(self) -> int:
+        """See `HistoryBase` docstring."""
         with h5py.File(self.file, 'r') as f:
             return f[f'history/{self.id}/trace/'].attrs['n_fval']
 
     @property
     def n_grad(self) -> int:
+        """See `HistoryBase` docstring."""
         with h5py.File(self.file, 'r') as f:
             return f[f'history/{self.id}/trace/'].attrs['n_grad']
 
     @property
     def n_hess(self) -> int:
+        """See `HistoryBase` docstring."""
         with h5py.File(self.file, 'r') as f:
             return f[f'history/{self.id}/trace/'].attrs['n_hess']
 
     @property
     def n_res(self) -> int:
+        """See `HistoryBase` docstring."""
         with h5py.File(self.file, 'r') as f:
             return f[f'history/{self.id}/trace/'].attrs['n_res']
 
     @property
     def n_sres(self) -> int:
+        """See `HistoryBase` docstring."""
         with h5py.File(self.file, 'r') as f:
             return f[f'history/{self.id}/trace/'].attrs['n_sres']
 
     @property
     def trace_save_iter(self):
+        """After how many iterations to store the trace."""
         with h5py.File(self.file, 'r') as f:
             return f[f'history/{self.id}/trace/']\
                 .attrs['trace_save_iter']
 
     def _update_trace(self,
                       x: np.ndarray,
                       sensi_orders: Tuple[int],
                       mode: str,
                       result: ResultDict):
-        """
-        Update and possibly store the trace.
-        """
-
+        """Update and possibly store the trace."""
         if not self.options.trace_record:
             return
 
         # extract function values
         ret = extract_values(mode, result, self.options)
 
         used_time = time.time() - self._start_time
@@ -972,17 +1015,15 @@
                     f[f'history/{self.id}/trace/'
                       f'{str(iteration)}/{key}'] = values[key]
 
             f[f'history/{self.id}/trace/'].attrs[
                 'n_iterations'] += 1
 
     def _generate_hdf5_group(self, f: h5py.File = None):
-        """
-        Generates the group in the hdf5 file, if it does not exist yet.
-        """
+        """Generate the group in the hdf5 file, if it does not exist yet."""
         try:
             with h5py.File(self.file, 'a') as f:
                 if f'history/{self.id}/trace/' not in f:
                     grp = f.create_group(f'history/{self.id}/trace/')
                     grp.attrs['n_iterations'] = 0
                     grp.attrs['n_fval'] = 0
                     grp.attrs['n_grad'] = 0
@@ -994,25 +1035,27 @@
             pass
 
     def _get_hdf5_entries(
         self,
         entry_id: str,
         ix: Union[int, Sequence[int], None] = None,
     ) -> Sequence:
-        """Get entries for field `entry_id` from HDF5 file, for indices `ix`.
+        """
+        Get entries for field `entry_id` from HDF5 file, for indices `ix`.
 
         Parameters
-        ------------
+        ----------
         entry_id:
             The key whose trace is returned.
         ix:
             Index or list of indices of the iterations that will produce
             the trace.
+
         Returns
-        --------
+        -------
         The entries ix for the key entry_id.
         """
         if ix is None:
             ix = range(len(self))
         trace_result = []
 
         with h5py.File(self.file, 'r') as f:
@@ -1028,77 +1071,87 @@
         return trace_result
 
     @trace_wrap
     def get_x_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[np.ndarray], np.ndarray]:
+        """See `HistoryBase` docstring."""
         return self._get_hdf5_entries(X, ix)
 
     @trace_wrap
     def get_fval_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[float], float]:
+        """See `HistoryBase` docstring."""
         return self._get_hdf5_entries(FVAL, ix)
 
     @trace_wrap
     def get_grad_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return self._get_hdf5_entries(GRAD, ix)
 
     @trace_wrap
     def get_hess_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return self._get_hdf5_entries(HESS, ix)
 
     @trace_wrap
     def get_res_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return self._get_hdf5_entries(RES, ix)
 
     @trace_wrap
     def get_sres_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return self._get_hdf5_entries(SRES, ix)
 
     @trace_wrap
     def get_chi2_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[float], float]:
+        """See `HistoryBase` docstring."""
         return self._get_hdf5_entries(CHI2, ix)
 
     @trace_wrap
     def get_schi2_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[MaybeArray], MaybeArray]:
+        """See `HistoryBase` docstring."""
         return self._get_hdf5_entries(SCHI2, ix)
 
     @trace_wrap
     def get_time_trace(
             self, ix: Union[int, Sequence[int], None] = None,
             trim: bool = False
     ) -> Union[Sequence[float], float]:
+        """See `HistoryBase` docstring."""
         return self._get_hdf5_entries(TIME, ix)
 
 
 class OptimizerHistory:
     """
-    Objective call history. Container around a History object, which keeps
-    track of optimal values.
+    Objective call history.
+
+    Container around a History object, which keeps track of optimal values.
 
     Attributes
     ----------
     fval0, fval_min:
         Initial and best function value found.
     chi20, chi2_min:
         Initial and best chi2 value found.
@@ -1152,22 +1205,21 @@
                mode: str,
                result: ResultDict) -> None:
         """Update history and best found value."""
         self.history.update(x, sensi_orders, mode, result)
         self._update_vals(x, result)
 
     def finalize(self):
+        """Finalize history."""
         self.history.finalize()
 
     def _update_vals(self,
                      x: np.ndarray,
                      result: ResultDict):
-        """
-        Update initial and best function values.
-        """
+        """Update initial and best function values."""
         # update initial point
         if np.allclose(x, self.x0):
             if self.fval0 is None:
                 self.fval0 = result.get(FVAL, None)
             self.x0 = x
 
         # update best point
@@ -1234,23 +1286,25 @@
                                         self.history.get_x_trace(ix_try)):
                     # gradient/sres typically evaluated on the next call
                     # so we check if x remains the same and if yes try to
                     # extract from the next
                     self.extract_from_history(var, ix_try)
 
     def extract_from_history(self, var, ix):
+        """Get value of `var` at iteration `ix`."""
         val = getattr(self.history, f'get_{var}_trace')(ix)
         if not np.all(np.isnan(val)):
             setattr(self, f'{var}_min', val)
 
 
 def ndarray2string_full(x: Union[np.ndarray, None]) -> Union[str, None]:
     """
-    Helper function that converts numpy arrays to string with 16 digit
-    numerical precision and no truncation for large arrays
+    Convert numpy arrays to string.
+
+    Use 16 digit numerical precision and no truncation for large arrays
 
     Parameters
     ----------
     x:
         array to convert
 
     Returns
@@ -1262,15 +1316,15 @@
         return x
     return np.array2string(x, threshold=x.size, precision=16,
                            max_line_width=np.inf)
 
 
 def string2ndarray(x: Union[str, float]) -> Union[np.ndarray, float]:
     """
-    Helper function that converts string to numpy arrays
+    Convert string to numpy arrays.
 
     Parameters
     ----------
     x:
         array to convert
 
     Returns
```

### Comparing `pypesto-0.2.8/pypesto/objective/pre_post_process.py` & `pypesto-0.2.9/pypesto/objective/pre_post_process.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 from typing import Dict, Sequence
 
 from .constants import GRAD, HESS, RES, SRES
 
 
 class PrePostProcessor:
     """
-    Implements the methods preprocess and postprocess that are called at the
-    beginning and at the end of the objective call, in order to handle the
-    mapping of optimization parameters to simulation parameters.
+    Implements the methods preprocess and postprocess.
+
+    They are called at the beginning and at the end of the objective call,
+    in order to handle the mapping of optimization parameters to simulation
+    parameters.
 
     This class acts as a dummy base implementation, not performing any
     changes on the passed objects.
     """
 
     def __init__(self):
         pass
@@ -35,30 +37,29 @@
         """
         return x
 
     def postprocess(
             self, result: Dict
     ) -> Dict:  # pylint: disable=R0201
         """
-        Convert all arrays into np.ndarrays if necessary, and return them
-        without further modifications.
+        Convert all arrays into np.ndarrays if necessary, and return them.
 
         Parameters
         ----------
         result:
             The result object to finalize.
         """
         result = PrePostProcessor.as_ndarrays(result)
         return result
 
     def reduce(
             self, x: np.ndarray
     ) -> np.ndarray:  # pylint: disable=R0201
         """
-        Just return x without modifications.
+        Return x without modifications.
 
         Parameters
         ----------
         x:
             Parameter vector for simulation.
 
         Returns
@@ -69,58 +70,65 @@
         return x
 
     @staticmethod
     def as_ndarrays(
             result: Dict
     ) -> Dict:
         """
-        Convert all array_like objects to np.ndarrays. This has the advantage
-        of a uniform output datatype which offers various methods to assess
-        the data.
+        Convert all array_like objects to np.ndarrays.
+
+        This has the advantage of a uniform output datatype which offers
+        various methods to assess the data.
         """
         keys = [GRAD, HESS, RES, SRES]
         for key in keys:
             if key in result:
                 value = result[key]
                 if value is not None:
                     result[key] = np.array(value)
         return result
 
 
 class FixedParametersProcessor(PrePostProcessor):
-    """
-    Extends the processor to handle the fixing of parameters.
-    """
+    """Extends the processor to handle the fixing of parameters."""
 
     def __init__(self,
                  dim_full: int,
                  x_free_indices: Sequence[int],
                  x_fixed_indices: Sequence[int],
                  x_fixed_vals: Sequence[float]):
         super().__init__()
         self.dim_full: int = dim_full
         self.x_free_indices: np.ndarray = np.array(x_free_indices, dtype=int)
         self.x_fixed_indices: np.ndarray = np.array(x_fixed_indices, dtype=int)
         self.x_fixed_vals: np.ndarray = np.array(x_fixed_vals, dtype=float)
 
     def preprocess(self, x: np.ndarray) -> np.ndarray:
-        """Embed optimization vector to full vector with all simulation
-        parameters.
-        """
+        """Embed optimization vector to full vector with all parameters."""
         x = super().preprocess(x)
 
         x_full = np.zeros(self.dim_full)
         x_full[self.x_free_indices] = x
         x_full[self.x_fixed_indices] = self.x_fixed_vals
 
         return x_full
 
     def reduce(self, x: np.ndarray) -> np.ndarray:
-        """Embed simulation vector to subsetted vector with optimization
-        parameters.
+        """
+        Return x reduced to free indices.
+
+        Parameters
+        ----------
+        x:
+            Parameter vector for simulation.
+
+        Returns
+        -------
+        x:
+            Parameter vector for optimization.
         """
         x = super().reduce(x)
 
         if x.size:
             return x[self.x_free_indices]
         else:
             return x
```

### Comparing `pypesto-0.2.8/pypesto/objective/priors.py` & `pypesto-0.2.9/pypesto/objective/priors.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,67 +20,71 @@
     Consists basically of a list of individual negative log-priors,
     given in self.objectives.
     """
 
 
 class NegLogParameterPriors(ObjectiveBase):
     """
-    This class implements Negative Log Priors on Parameters.
+    Implements Negative Log Priors on Parameters.
 
     Contains a list of prior dictionaries for the individual parameters
     of the format
 
     {'index': [int],
     'density_fun': [Callable],
     'density_dx': [Callable],
     'density_ddx': [Callable]}
 
     A prior instance can be added to e.g. an objective, that gives the
     likelihood, by an AggregatedObjective.
 
     Notes
     -----
-
     All callables should correspond to log-densities. That is, they return
     log-densities and their corresponding derivatives.
     Internally, values are multiplied by -1, since pyPESTO expects the
     Objective function to be of a negative log-density type.
     """
 
     def __init__(self,
                  prior_list: List[Dict],
                  x_names: Sequence[str] = None):
         """
-        Constructor
+        Initialize.
 
         Parameters
         ----------
-
         prior_list:
             List of dicts containing the individual parameter priors.
             Format see above.
-
         x_names:
             Sequence of parameter names (optional).
         """
-
         self.prior_list = prior_list
         super().__init__(x_names)
 
     def __deepcopy__(self, memodict=None):
+        """Create deepcopy of object."""
         other = NegLogParameterPriors(deepcopy(self.prior_list))
         return other
 
     def call_unprocessed(
             self,
             x: np.ndarray,
             sensi_orders: Tuple[int, ...],
             mode: str
     ) -> ResultDict:
+        """
+        Call objective function without pre- or post-processing and formatting.
 
+        Returns
+        -------
+        result:
+            A dict containing the results.
+        """
         res = {}
 
         res[FVAL] = self.neg_log_density(x)
 
         if mode == MODE_FUN:
             for order in sensi_orders:
                 if order == 0:
@@ -103,14 +107,15 @@
                     raise ValueError(f'Invalid sensi order {order}.')
 
         return res
 
     def check_sensi_orders(self,
                            sensi_orders: Tuple[int, ...],
                            mode: str) -> bool:
+        """See `ObjectiveBase` documentation."""
         if mode == MODE_FUN:
             for order in sensi_orders:
                 if not (0 <= order <= 2):
                     return False
         elif mode == MODE_RES:
             for order in sensi_orders:
                 if order == 0:
@@ -124,120 +129,103 @@
         else:
             raise ValueError(f'Invalid input: Expected mode {MODE_FUN} or'
                              f' {MODE_RES}, received {mode} instead.')
 
         return True
 
     def check_mode(self, mode) -> bool:
+        """See `ObjectiveBase` documentation."""
         if mode == MODE_FUN:
             return True
         elif mode == MODE_RES:
             return all(prior.get('residual', None) is not None
                        for prior in self.prior_list)
         else:
             raise ValueError(f'Invalid input: Expected mode {MODE_FUN} or'
                              f' {MODE_RES}, received {mode} instead.')
 
     def neg_log_density(self, x):
-        """
-        Computes the negative log-density for a parameter
-        vector x.
-        """
+        """Evaluate the negative log-density at x."""
         density_val = 0
         for prior in self.prior_list:
             density_val -= prior['density_fun'](x[prior['index']])
 
         return density_val
 
     def gradient_neg_log_density(self, x):
-        """
-        Computes the gradient of the negative log-density for a parameter
-        vector x.
-        """
+        """Evaluate the gradient of the negative log-density at x."""
         grad = np.zeros_like(x)
 
         for prior in self.prior_list:
             grad[prior['index']] -= prior['density_dx'](x[prior['index']])
 
         return grad
 
     def hessian_neg_log_density(self, x):
-        """
-        Computes the hessian of the negative log-density for a parameter
-        vector x.
-        """
+        """Evaluate the hessian of the negative log-density at x."""
         hessian = np.zeros((len(x), len(x)))
 
         for prior in self.prior_list:
             hessian[prior['index'], prior['index']] -= \
                 prior['density_ddx'](x[prior['index']])
 
         return hessian
 
     def hessian_vp_neg_log_density(self, x, p):
-        """
-        Computes the hessian vector product of the hessian of the
-        negative log-density for a parameter vector x with a vector p.
-        """
+        """Compute vector product of the hessian at x with a vector p."""
         h_dot_p = np.zeros_like(p)
 
         for prior in self.prior_list:
             h_dot_p[prior['index']] -= \
                 prior['density_ddx'](x[prior['index']]) * p[prior['index']]
 
         return h_dot_p
 
     def residual(self, x):
-        """
-        Computes the residual representation of the prior for a parameter
-        vector x, if available.
-        """
+        """Evaluate the residual representation of the prior at x."""
         return np.asarray([prior['residual'](x[prior['index']])
                            for prior in self.prior_list])
 
     def residual_jacobian(self, x):
         """
-        Computes the Jacobian of the residual representation of the prior
+        Evaluate residual Jacobian.
+
+        Evaluate the Jacobian of the residual representation of the prior
         for a parameter vector x w.r.t. x, if available.
         """
         sres = np.zeros((len(self.prior_list), len(x)))
         for iprior, prior in enumerate(self.prior_list):
             sres[iprior, prior['index']] = \
                 prior['residual_dx'](x[prior['index']])
 
         return sres
 
 
 def get_parameter_prior_dict(index: int,
                              prior_type: str,
                              prior_parameters: list,
                              parameter_scale: str = 'lin'):
-
     """
-    Returns the prior dict used to define priors for some default priors.
+    Return the prior dict used to define priors for some default priors.
 
     index:
         index of the parameter in x_full
-
     prior_type:
         Prior is defined in LINEAR=untransformed parameter space,
         unless it starts with "parameterScale". prior_type
         can be any of {"uniform", "normal", "laplace", "logNormal",
         "parameterScaleUniform", "parameterScaleNormal",
         "parameterScaleLaplace"}
-
     prior_parameters:
         Parameters of the priors. Parameters are defined in linear scale.
-
     parameter_scale:
         scale in which the parameter is defined (since a parameter can be
         log-transformed, while the prior is always defined in the linear
         space, unless it starts with "parameterScale")
     """
-
     log_f, d_log_f_dx, dd_log_f_ddx, res, d_res_dx = \
         _prior_densities(prior_type, prior_parameters)
 
     if parameter_scale == 'lin' or prior_type.startswith('parameterScale'):
 
         return {'index': index,
                 'density_fun': log_f,
@@ -245,70 +233,70 @@
                 'density_ddx': dd_log_f_ddx,
                 'residual': res,
                 'residual_dx': d_res_dx}
 
     elif parameter_scale == 'log':
 
         def log_f_log(x_log):
-            """log-prior for log-parameters"""
+            """Log-prior for log-parameters."""
             return log_f(np.exp(x_log))
 
         def d_log_f_log(x_log):
-            """derivative of log-prior w.r.t. log-parameters"""
+            """First derivative of log-prior w.r.t. log-parameters."""
             return d_log_f_dx(np.exp(x_log)) * np.exp(x_log)
 
         def dd_log_f_log(x_log):
-            """second derivative of log-prior w.r.t. log-parameters"""
+            """Second derivative of log-prior w.r.t. log-parameters."""
             return np.exp(x_log) * \
                 (d_log_f_dx(np.exp(x_log)) +
                     np.exp(x_log) * dd_log_f_ddx(np.exp(x_log)))
 
         if res is not None:
             def res_log(x_log):
-                """residual-prior for log-parameters"""
+                """Residual-prior for log-parameters."""
                 return res(np.exp(x_log))
 
         if d_res_dx is not None:
             def d_res_log(x_log):
-                """residual-prior for log-parameters"""
+                """Residual-prior for log-parameters."""
                 return d_res_dx(np.exp(x_log)) * np.exp(x_log)
 
         return {'index': index,
                 'density_fun': log_f_log,
                 'density_dx': d_log_f_log,
                 'density_ddx': dd_log_f_log,
                 'residual': res_log if res is not None else None,
                 'residual_dx': d_res_log if d_res_dx is not None else None}
 
     elif parameter_scale == 'log10':
 
         log10 = np.log(10)
 
         def log_f_log10(x_log10):
-            """log-prior for log10-parameters"""
+            """Log-prior for log10-parameters."""
             return log_f(10**x_log10)
 
         def d_log_f_log10(x_log10):
-            """derivative of log-prior w.r.t. log10-parameters"""
+            """Rerivative of log-prior w.r.t. log10-parameters."""
             return d_log_f_dx(10**x_log10) * log10 * 10**x_log10
 
         def dd_log_f_log10(x_log10):
-            """second derivative of log-prior w.r.t. log10-parameters"""
+            """Second derivative of log-prior w.r.t. log10-parameters."""
             return log10**2 * 10**x_log10 * \
                 (dd_log_f_ddx(10**x_log10) * 10**x_log10
                     + d_log_f_dx(10**x_log10))
 
         if res is not None:
             def res_log(x_log10):
-                """residual-prior for log10-parameters"""
+                """Residual-prior for log10-parameters."""
                 return res(10**x_log10)
 
         if d_res_dx is not None:
             def d_res_log(x_log10):
-                """residual-prior for log10-parameters"""
+                """Residual-prior for log10-parameters."""
                 return d_res_dx(10**x_log10) * log10 * 10**x_log10
 
         return {'index': index,
                 'density_fun': log_f_log10,
                 'density_dx': d_log_f_log10,
                 'density_ddx': dd_log_f_log10,
                 'residual': res_log if res is not None else None,
@@ -320,36 +308,25 @@
 
 
 def _prior_densities(prior_type: str,
                      prior_parameters: np.array) -> [Callable,
                                                      Callable,
                                                      Callable]:
     """
-    Returns a tuple of Callables of the (log-)density (in untransformed =
+    Create prior density functions.
+
+    Return a tuple of Callables of the (log-)density (in untransformed =
     linear scale), unless prior_types starts with "parameterScale",
     together with their first + second derivative (= sensis) w.r.t.
     the parameters. If possible, a residual representation and its first
     derivative w.r.t. the parameters is included as 4th and 5th element of
     the vector. If a reformulation as residual is not possible, the respective
     entries will be `None`.
 
     Currently the following distributions are supported:
-
-    Parameters
-    ----------
-
-    prior_type:
-        string identifier indicating the distribution to be used. Here
-        "transformed" parameter scale refers to the scale in which
-        optimization is performed. For example, for parameters with scale
-        "log", "parameterScaleNormal" will apply a normally distributed prior
-        to logarithmic parameters, while "normal" will apply a normally
-        distributed prior to linear parameters. For parameters with scale
-        "lin", "parameterScaleNormal" and "normal" are equivalent.
-
         * uniform:
             Uniform distribution on transformed parameter scale.
         * parameterScaleUniform:
             Uniform distribution on original parameter scale.
         * normal:
             Normal distribution on transformed parameter scale.
         * parameterScaleNormal:
@@ -363,14 +340,24 @@
 
         Currently not supported, but eventually planned are the
         following distributions:
 
         * logUniform
         * logLaplace
 
+    Parameters
+    ----------
+    prior_type:
+        string identifier indicating the distribution to be used. Here
+        "transformed" parameter scale refers to the scale in which
+        optimization is performed. For example, for parameters with scale
+        "log", "parameterScaleNormal" will apply a normally distributed prior
+        to logarithmic parameters, while "normal" will apply a normally
+        distributed prior to linear parameters. For parameters with scale
+        "lin", "parameterScaleNormal" and "normal" are equivalent.
     prior_parameters:
         parameters for the distribution
 
         * uniform/parameterScaleUniform:
             - prior_parameters[0]: lower bound
             - prior_parameters[1]: upper bound
 
@@ -381,18 +368,15 @@
         * normal/parameterScaleNormal:
             - prior_parameters[0]: mean
             - prior_parameters[1]: standard deviation
 
         * logNormal:
             - prior_parameters[0]: mean of log-parameters
             - prior_parameters[1]: standard deviation of log-parameters
-
-
     """
-
     if prior_type in ['uniform', 'parameterScaleUniform']:
 
         def log_f(x):
             if prior_parameters[0] <= x <= prior_parameters[1]:
                 return - np.log(prior_parameters[1] - prior_parameters[0])
             else:
                 return - np.inf
@@ -486,22 +470,18 @@
     else:
         raise ValueError(f'NegLogPriors of type {prior_type} are currently '
                          'not supported')
 
 
 def _get_linear_function(slope: float,
                          intercept: float = 0):
-    """
-    Returns a linear function
-    """
+    """Return a linear function."""
     def function(x):
         return slope * x + intercept
     return function
 
 
 def _get_constant_function(constant: float):
-    """
-    Defines a callable, that returns the constant, regardless of the input.
-    """
+    """Define a callable returning the constant, regardless of the input."""
     def function(x):
         return constant
     return function
```

### Comparing `pypesto-0.2.8/pypesto/objective/util.py` & `pypesto-0.2.9/pypesto/objective/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from typing import Union
 
 
 def _check_none(fun):
-    """Wrapper: Return None if any input argument is None."""
+    """Return None if any input argument is None; Wrapper function."""
     def checked_fun(*args, **kwargs):
         if any(x is None for x in [*args, *(kwargs.values())]):
             return None
         return fun(*args, **kwargs)
     return checked_fun
 
 
@@ -47,19 +47,20 @@
     See also :func:`chi2_to_fval`.
     """
     return 0.5 * schi2
 
 
 @_check_none
 def sres_to_grad(res: np.ndarray, sres: np.ndarray):
-    """Translate residual sensitivities to function value gradien, assuming
-    `fval = 0.5*sum(res**2)`.
+    """Translate residual sensitivities to function value gradient.
+
+    Assumes `fval = 0.5*sum(res**2)`.
 
     See also :func:`chi2_to_fval`.
-     """
+    """
     return schi2_to_grad(sres_to_schi2(res, sres))
 
 
 @_check_none
 def sres_to_fim(sres: np.ndarray):
     """Translate residual sensitivities to FIM.
```

### Comparing `pypesto-0.2.8/pypesto/optimize/optimize.py` & `pypesto-0.2.9/pypesto/optimize/optimize.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..result import Result
 from ..startpoint import (
     assign_startpoints, uniform, StartpointMethod, to_startpoint_method,
 )
 from .optimizer import Optimizer, ScipyOptimizer
 from .options import OptimizeOptions
 from .task import OptimizerTask
-from .util import check_hdf5_mp, fill_hdf5_file
+from .util import check_hdf5_mp, fill_hdf5_file, autosave
 
 logger = logging.getLogger(__name__)
 
 
 def minimize(
     problem: Problem,
     optimizer: Optimizer = None,
@@ -23,17 +23,18 @@
     ids: Iterable[str] = None,
     startpoint_method: Union[StartpointMethod, bool] = None,
     result: Result = None,
     engine: Engine = None,
     progress_bar: bool = True,
     options: OptimizeOptions = None,
     history_options: HistoryOptions = None,
+    filename: str = "Auto"
 ) -> Result:
     """
-    This is the main function to call to do multistart optimization.
+    Do multistart optimization.
 
     Parameters
     ----------
     problem:
         The problem to be solved.
     optimizer:
         The optimizer to be used n_starts times.
@@ -53,22 +54,26 @@
         SingleCoreEngine.
     progress_bar:
         Whether to display a progress bar.
     options:
         Various options applied to the multistart optimization.
     history_options:
         Optimizer history options.
+    filename:
+        Name of the hdf5 file, where the result will be saved. Default is
+        "Auto", in which case it will automatically generate a file named
+        `year_month_day_optimization_result.hdf5`. Deactivate saving by
+        setting filename to `None`.
 
     Returns
     -------
     result:
         Result object containing the results of all multistarts in
         `result.optimize_result`.
     """
-
     # optimizer
     if optimizer is None:
         optimizer = ScipyOptimizer()
 
     # startpoint method
     if startpoint_method is not None and problem.startpoint_method is not None:
         raise Warning(
@@ -112,37 +117,45 @@
 
     # engine
     if engine is None:
         engine = SingleCoreEngine()
 
     # define tasks
     tasks = []
-    filename = None
+    filename_hist = None
     if history_options.storage_file is not None and \
             history_options.storage_file.endswith(('.h5', '.hdf5')):
-        filename = check_hdf5_mp(history_options, engine)
+        filename_hist = check_hdf5_mp(history_options, engine)
 
     for startpoint, id in zip(startpoints, ids):
         task = OptimizerTask(
             optimizer=optimizer,
             problem=problem,
             x0=startpoint,
             id=id,
             options=options,
             history_options=history_options,
+            report_hess=options.report_hess,
+            report_sres=options.report_sres,
         )
         tasks.append(task)
 
     # do multistart optimization
     ret = engine.execute(tasks, progress_bar=progress_bar)
 
-    if filename is not None:
-        fill_hdf5_file(ret, filename)
+    if filename_hist is not None:
+        fill_hdf5_file(ret, filename_hist)
 
     # aggregate results
     for optimizer_result in ret:
         result.optimize_result.append(optimizer_result)
 
     # sort by best fval
     result.optimize_result.sort()
 
+    if filename == "Auto" and filename_hist is not None:
+        filename = filename_hist
+    autosave(filename=filename,
+             result=result,
+             type="optimization")
+
     return result
```

### Comparing `pypesto-0.2.8/pypesto/optimize/optimizer.py` & `pypesto-0.2.9/pypesto/optimize/optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,16 +54,17 @@
 EXITFLAG_LOADED_FROM_FILE = -99
 
 logger = logging.getLogger(__name__)
 
 
 def history_decorator(minimize):
     """
-    Default decorator for the minimize() method to initialize and extract
-    information stored in the history.
+    Initialize and extract information stored in the history.
+
+    Default decorator for the minimize() method.
     """
 
     def wrapped_minimize(self, problem, x0, id, allow_failed_starts,
                          history_options=None):
         objective = problem.objective
 
         # initialize the objective
@@ -101,14 +102,16 @@
         return result
 
     return wrapped_minimize
 
 
 def time_decorator(minimize):
     """
+    Measure time of optimization.
+
     Default decorator for the minimize() method to take time.
     Currently, the method time.time() is used, which measures
     the wall-clock time.
     """
 
     def wrapped_minimize(self, problem, x0, id, allow_failed_starts,
                          history_options=None):
@@ -120,16 +123,17 @@
         return result
 
     return wrapped_minimize
 
 
 def fix_decorator(minimize):
     """
-    Default decorator for the minimize() method to include also fixed
-    parameters in the result arrays (nans will be inserted in the
+    Include also fixed parameters in the result arrays of minimize().
+
+    Default decorator for the minimize() method (nans will be inserted in the
     derivatives).
     """
 
     def wrapped_minimize(self, problem, x0, id, allow_failed_starts,
                          history_options=None):
         # perform the actual optimization
         result = minimize(self, problem, x0, id, allow_failed_starts,
@@ -146,18 +150,15 @@
 
     return wrapped_minimize
 
 
 def fill_result_from_objective_history(
         result: OptimizerResult,
         optimizer_history: OptimizerHistory):
-    """
-    Overwrite function values in the result object with the values recorded in
-    the history.
-    """
+    """Overwrite values in the result object with values in the history."""
     update_vals = True
     # check history for better values
     # value could be different e.g. if constraints violated
     if optimizer_history.fval_min is not None and result.fval is not None \
             and not np.isclose(optimizer_history.fval_min, result.fval):
         logger.warning(
             "Function values from history and optimizer do not match: "
@@ -239,70 +240,70 @@
     result.update_to_full(problem)
 
     return result
 
 
 class Optimizer(abc.ABC):
     """
-    This is the optimizer base class, not functional on its own.
+    Optimizer base class, not functional on its own.
+
     An optimizer takes a problem, and possibly a start point, and then
     performs an optimization. It returns an OptimizerResult.
     """
 
     def __init__(self):
-        """
-        Default constructor.
-        """
+        """Initialize base class."""
 
     @abc.abstractmethod
     @fix_decorator
     @time_decorator
     @history_decorator
     def minimize(
             self,
             problem: Problem,
             x0: np.ndarray,
             id: str,
             history_options: HistoryOptions = None,
     ) -> OptimizerResult:
-        """"
+        """
         Perform optimization.
+
         Parameters
         ----------
         problem:
             The problem to find optimal parameters for.
         x0:
             The starting parameters.
         id:
             Multistart id.
         history_options:
             Optimizer history options.
         """
 
     @abc.abstractmethod
     def is_least_squares(self):
+        """Check whether optimizer is a least squares optimizer."""
         return False
 
     def get_default_options(self):
-        """
-        Create default options specific for the optimizer.
-        """
+        """Create default options specific for the optimizer."""
         return None
 
 
 def check_finite_bounds(lb, ub):
     """Raise if bounds are not finite."""
     if not np.isfinite(lb).all() or not np.isfinite(ub).all():
         raise ValueError('Selected optimizer cannot work with unconstrained '
                          'optimization problems.')
 
 
 class ScipyOptimizer(Optimizer):
     """
     Use the SciPy optimizers.
+
     Find details on the optimizer and configuration options at:
     https://docs.scipy.org/doc/scipy/reference/generated/scipy.\
         optimize.minimize.html#scipy.optimize.minimize
     """
 
     def __init__(self,
                  method: str = 'L-BFGS-B',
@@ -325,14 +326,15 @@
     def minimize(
         self,
         problem: Problem,
         x0: np.ndarray,
         id: str,
         history_options: HistoryOptions = None,
     ) -> OptimizerResult:
+        """Perform optimization. Parameters: see `Optimizer` documentation."""
         lb = problem.lb
         ub = problem.ub
         objective = problem.objective
 
         if self.is_least_squares():
             # is a residual based least squares method
 
@@ -434,30 +436,34 @@
             exitflag=res.status,
             message=res.message
         )
 
         return optimizer_result
 
     def is_least_squares(self):
+        """Check whether optimizer is a least squares optimizer."""
         return re.match(r'(?i)^(ls_)', self.method)
 
     def get_default_options(self):
+        """Create default options specific for the optimizer."""
         if self.is_least_squares():
             options = {'max_nfev': 1000, 'disp': False}
         else:
             options = {'maxiter': 1000, 'disp': False}
         return options
 
 
 class IpoptOptimizer(Optimizer):
     """Use IpOpt (https://pypi.org/project/ipopt/) for optimization."""
 
     def __init__(
             self, options: Dict = None):
         """
+        Initialize.
+
         Parameters
         ----------
         options:
             Options are directly passed on to `cyipopt.minimize_ipopt`.
         """
         super().__init__()
         self.options = options
@@ -468,15 +474,15 @@
     def minimize(
             self,
             problem: Problem,
             x0: np.ndarray,
             id: str,
             history_options: HistoryOptions = None,
     ) -> OptimizerResult:
-
+        """Perform optimization. Parameters: see `Optimizer` documentation."""
         if cyipopt is None:
             raise ImportError(
                 "This optimizer requires an installation of ipopt. You can "
                 "install ipopt via `pip install ipopt`."
             )
 
         objective = problem.objective
@@ -499,21 +505,20 @@
         return OptimizerResult(
             x=ret.x,
             exitflag=ret.status,
             message=ret.message
         )
 
     def is_least_squares(self):
+        """Check whether optimizer is a least squares optimizer."""
         return False
 
 
 class DlibOptimizer(Optimizer):
-    """
-    Use the Dlib toolbox for optimization.
-    """
+    """Use the Dlib toolbox for optimization."""
 
     def __init__(self,
                  options: Dict = None):
         super().__init__()
 
         self.options = options
         if self.options is None:
@@ -528,15 +533,15 @@
     def minimize(
             self,
             problem: Problem,
             x0: np.ndarray,
             id: str,
             history_options: HistoryOptions = None,
     ) -> OptimizerResult:
-
+        """Perform optimization. Parameters: see `Optimizer` documentation."""
         lb = problem.lb
         ub = problem.ub
         check_finite_bounds(lb, ub)
         objective = problem.objective
 
         if dlib is None:
             raise ImportError(
@@ -561,24 +566,24 @@
         )
 
         optimizer_result = OptimizerResult()
 
         return optimizer_result
 
     def is_least_squares(self):
+        """Check whether optimizer is a least squares optimizer."""
         return False
 
     def get_default_options(self):
+        """Create default options specific for the optimizer."""
         return {'maxiter': 10000}
 
 
 class PyswarmOptimizer(Optimizer):
-    """
-    Global optimization using pyswarm.
-    """
+    """Global optimization using pyswarm."""
 
     def __init__(self, options: Dict = None):
         super().__init__()
 
         if options is None:
             options = {'maxiter': 200}
         self.options = options
@@ -589,14 +594,15 @@
     def minimize(
             self,
             problem: Problem,
             x0: np.ndarray,
             id: str,
             history_options: HistoryOptions = None,
     ) -> OptimizerResult:
+        """Perform optimization. Parameters: see `Optimizer` documentation."""
         lb = problem.lb
         ub = problem.ub
         if pyswarm is None:
             raise ImportError(
                 "This optimizer requires an installation of pyswarm. You can "
                 "install pyswarm via `pip install pyswarm."
             )
@@ -610,35 +616,38 @@
             x=np.array(xopt),
             fval=fopt
         )
 
         return optimizer_result
 
     def is_least_squares(self):
+        """Check whether optimizer is a least squares optimizer."""
         return False
 
 
 class CmaesOptimizer(Optimizer):
     """
     Global optimization using cma-es.
+
     Package homepage: https://pypi.org/project/cma-es/
     """
 
     def __init__(self, par_sigma0: float = 0.25, options: Dict = None):
         """
+        Initialize.
+
         Parameters
         ----------
         par_sigma0:
             scalar, initial standard deviation in each coordinate.
             par_sigma0 should be about 1/4th of the search domain width
             (where the optimum is to be expected)
         options:
             Optimizer options that are directly passed on to cma.
         """
-
         super().__init__()
 
         if options is None:
             options = {'maxiter': 10000}
         self.options = options
         self.par_sigma0 = par_sigma0
 
@@ -648,15 +657,15 @@
     def minimize(
             self,
             problem: Problem,
             x0: np.ndarray,
             id: str,
             history_options: HistoryOptions = None,
     ) -> OptimizerResult:
-
+        """Perform optimization. Parameters: see `Optimizer` documentation."""
         lb = problem.lb
         ub = problem.ub
 
         check_finite_bounds(lb, ub)
 
         sigma0 = self.par_sigma0 * np.median(ub - lb)
         self.options['bounds'] = [lb, ub]
@@ -673,20 +682,22 @@
 
         optimizer_result = OptimizerResult(x=np.array(result[0]),
                                            fval=result[1])
 
         return optimizer_result
 
     def is_least_squares(self):
+        """Check whether optimizer is a least squares optimizer."""
         return False
 
 
 class ScipyDifferentialEvolutionOptimizer(Optimizer):
     """
     Global optimization using scipy's differential evolution optimizer.
+
     Package homepage: https://docs.scipy.org/doc/scipy/reference/generated\
         /scipy.optimize.differential_evolution.html
 
     Parameters
     ----------
     options:
         Optimizer options that are directly passed on to scipy's optimizer.
@@ -717,32 +728,35 @@
     def minimize(
             self,
             problem: Problem,
             x0: np.ndarray,
             id: str,
             history_options: HistoryOptions = None,
     ) -> OptimizerResult:
+        """Perform optimization. Parameters: see `Optimizer` documentation."""
         bounds = list(zip(problem.lb, problem.ub))
 
         result = scipy.optimize.differential_evolution(
             problem.objective.get_fval, bounds, **self.options
         )
 
         optimizer_result = OptimizerResult(x=np.array(result.x),
                                            fval=result.fun)
 
         return optimizer_result
 
     def is_least_squares(self):
+        """Check whether optimizer is a least squares optimizer."""
         return False
 
 
 class PyswarmsOptimizer(Optimizer):
     """
     Global optimization using pyswarms.
+
     Package homepage: https://pyswarms.readthedocs.io/en/latest/index.html
 
     Parameters
     ----------
     par_popsize:
         number of particles in the swarm, default value 10
 
@@ -778,14 +792,15 @@
     def minimize(
             self,
             problem: Problem,
             x0: np.ndarray,
             id: str,
             history_options: HistoryOptions = None,
     ) -> OptimizerResult:
+        """Perform optimization. Parameters: see `Optimizer` documentation."""
         lb = problem.lb
         ub = problem.ub
 
         if pyswarms is None:
             raise ImportError(
                 "This optimizer requires an installation of pyswarms.")
 
@@ -800,23 +815,22 @@
         optimizer = pyswarms.single.global_best.GlobalBestPSO(
             n_particles=self.par_popsize, dimensions=len(x0),
             options=self.options, bounds=(lb, ub))
 
         def successively_working_fval(swarm: np.ndarray) -> np.ndarray:
             """Evaluate the function for all parameters in the swarm object.
 
-            Parameters:
-            -----------
+            Parameters
+            ----------
             swarm: np.ndarray, shape (n_particales_in_swarm, n_parameters)
 
-            Returns:
-            --------
+            Returns
+            -------
             result: np.ndarray, shape (n_particles_in_swarm)
             """
-
             n_particles = swarm.shape[0]
             result = np.zeros(n_particles)
             # iterate over the particles in the swarm
             for i_particle, par in enumerate(swarm):
                 result[i_particle] = problem.objective.get_fval(par)
 
             return result
@@ -828,41 +842,44 @@
             x=pos,
             fval=np.array(cost)
         )
 
         return optimizer_result
 
     def is_least_squares(self):
+        """Check whether optimizer is a least squares optimizer."""
         return False
 
 
 class NLoptOptimizer(Optimizer):
     """
     Global/Local optimization using NLopt.
+
     Package homepage: https://nlopt.readthedocs.io/en/latest/
     """
 
     def __init__(self, method=None, local_method=None, options: Dict = None,
                  local_options: Dict = None):
         """
+        Initialize.
+
         Parameters
         ----------
         method:
             Local or global Optimizer to use for minimization.
         local_method:
             Local method to use in combination with the global optimizer (
             for the MLSL family of solvers) or to solve a subproblem (for the
             AUGLAG family of solvers)
         options:
             Optimizer options. scipy option `maxiter` is automatically
             transformed into `maxeval` and takes precedence.
         local_options:
             Optimizer options for the local method
         """
-
         super().__init__()
 
         if options is None:
             options = {}
         elif 'maxiter' in options:
             options['maxeval'] = options.pop('maxiter')
         if local_options is None:
@@ -930,15 +947,15 @@
     def minimize(
             self,
             problem: Problem,
             x0: np.ndarray,
             id: str,
             history_options: HistoryOptions = None,
     ) -> OptimizerResult:
-
+        """Perform optimization. Parameters: see `Optimizer` documentation."""
         opt = nlopt.opt(self.method, problem.dim)
 
         valid_options = ['ftol_abs', 'ftol_rel', 'xtol_abs', 'xtol_rel',
                          'stopval', 'x_weights', 'maxeval', 'maxtime',
                          'initial_step']
 
         def set_options(o, options):
@@ -984,40 +1001,43 @@
                                            fval=opt.last_optimum_value(),
                                            message=msg,
                                            exitflag=opt.last_optimize_result())
 
         return optimizer_result
 
     def is_least_squares(self):
+        """Check whether optimizer is a least squares optimizer."""
         return False
 
 
 class FidesOptimizer(Optimizer):
     """
     Global/Local optimization using the trust region optimizer fides.
+
     Package Homepage: https://fides-optimizer.readthedocs.io/en/latest
     """
 
     def __init__(
             self,
             hessian_update: Optional['HessianApproximation'] = 'Hybrid',
             options: Optional[Dict] = None,
             verbose: Optional[int] = logging.INFO
     ):
         """
+        Initialize.
+
         Parameters
         ----------
         options:
             Optimizer options.
         hessian_update:
             Hessian update strategy. If this is None, a hybrid approximation
             that switches from the problem.objective provided Hessian (
             approximation) to a BFGS approximation will be used.
         """
-
         super().__init__()
 
         if hessian_update == 'Hybrid':
             hessian_update = fides.HybridFixed()
 
         if hessian_update is not None and \
                 not isinstance(hessian_update, HessianApproximation):
@@ -1038,15 +1058,15 @@
     def minimize(
             self,
             problem: Problem,
             x0: np.ndarray,
             id: str,
             history_options: HistoryOptions = None,
     ) -> OptimizerResult:
-
+        """Perform optimization. Parameters: see `Optimizer` documentation."""
         if fides is None:
             raise ImportError(
                 "This optimizer requires an installation of fides. You can "
                 "install fides via `pip install fides`."
             )
 
         resfun = self.hessian_update.requires_resfun if self.hessian_update \
@@ -1090,8 +1110,9 @@
             grad=opt.grad_min, hess=opt.hess, message=msg,
             exitflag=opt.exitflag
         )
 
         return optimizer_result
 
     def is_least_squares(self):
+        """Check whether optimizer is a least squares optimizer."""
         return False
```

### Comparing `pypesto-0.2.8/pypesto/optimize/result.py` & `pypesto-0.2.9/pypesto/optimize/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 from ..objective import History
 from ..problem import Problem
 
 
 class OptimizerResult(dict):
     """
-    The result of an optimizer run. Used as a standardized return value to
-    map from the individual result objects returned by the employed
-    optimizers to the format understood by pypesto.
+    The result of an optimizer run.
+
+    Used as a standardized return value to map from the individual result
+    objects returned by the employed optimizers to the format understood by
+    pypesto.
 
     Can be used like a dict.
 
     Attributes
     ----------
     id:
         Id of the optimizer run. Usually the start index.
@@ -49,15 +51,14 @@
     time:
         Execution time.
     message: str
         Textual comment on the optimization result.
 
     Notes
     -----
-
     Any field not supported by the optimizer is filled with None.
     """
 
     def __init__(self,
                  id: str = None,
                  x: np.ndarray = None,
                  fval: float = None,
@@ -103,15 +104,15 @@
             raise AttributeError(key)
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
     def update_to_full(self, problem: Problem) -> None:
         """
-        Updates values to full vectors/matrices
+        Update values to full vectors/matrices.
 
         Parameters
         ----------
         problem:
             problem which contains info about how to convert to full vectors
             or matrices
         """
```

### Comparing `pypesto-0.2.8/pypesto/optimize/util.py` & `pypesto-0.2.9/pypesto/optimize/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,30 @@
+"""Utility functions for :py:func:`pypesto.optimize.minimize`."""
+import datetime
+
 from ..engine import Engine, SingleCoreEngine
 from ..objective import HistoryOptions
 from ..store.save_to_hdf5 import get_or_create_group
+from ..store import write_result
+from ..result import Result
 from pathlib import Path
 from typing import Union
 
 
 import h5py
 
 
 def check_hdf5_mp(
     history_options: HistoryOptions,
     engine: Engine,
 ) -> Union[str, None]:
     """
-    Create a folder for partial HDF5 files,
-    if a parallelization engine will be used.
+    Create a folder for partial HDF5 files.
+
+    If no parallelization engine is used, do nothing.
 
     Parameters
     ----------
     engine:
         The Engine which is used in the optimization
     history_options:
         The HistoryOptions used in the optimization
@@ -48,14 +54,16 @@
 
 
 def fill_hdf5_file(
     ret: list,
     filename: str
 ) -> None:
     """
+    Create single history file pointing to files of multiple starts.
+
     Create links in `filename` to the
     history of each start contained in ret, the results
     of the optimization.
 
     Parameters
     ----------
     ret:
@@ -67,7 +75,33 @@
     with h5py.File(filename, mode='a') as f:
         for result in ret:
             id = result['id']
             f[f'history/{id}'] = h5py.ExternalLink(
                 result['history'].file,
                 f'history/{id}'
             )
+
+
+def autosave(filename: str, result: Result,
+             type: str):
+    """
+    Save the result of optimization, profiling or sampling automatically.
+
+    Parameters
+    ----------
+    filename:
+        Either the filename to save to or "Auto", in which case it will
+        automatically generate a file named
+        `year_month_day_{type}_result.hdf5`.
+    result:
+        The result to be saved.
+    type:
+        Either `optimization`, `sampling` or `profiling`. Depending on the
+        method the function is called in.
+    """
+    if filename is None:
+        return None
+    if filename == "Auto":
+        time = datetime.datetime.now().strftime("%Y_%d_%m_%H_%M_%S")
+        filename = time+f"_{type}_result.hdf5"
+    write_result(result=result, overwrite=True,
+                 optimize=True, filename=filename)
```

### Comparing `pypesto-0.2.8/pypesto/petab/__init__.py` & `pypesto-0.2.9/pypesto/petab/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.2.8/pypesto/petab/importer.py` & `pypesto-0.2.9/pypesto/petab/importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+"""Contains the PetabImporter class."""
 import pandas as pd
 import numpy as np
 import os
 import sys
 import importlib
 import shutil
 import logging
 import tempfile
-from typing import Iterable, List, Literal, Optional, Sequence, Union, Callable
+from typing import Iterable, List, Optional, Sequence, Union, Callable
 
 from ..problem import Problem
 from ..objective import AmiciObjective, AmiciObjectBuilder, AggregatedObjective
 from ..predict import AmiciPredictor, PredictionResult
 from ..predict.constants import CONDITION_SEP
 from ..objective.priors import NegLogParameterPriors, \
     get_parameter_prior_dict
@@ -27,22 +28,33 @@
 except ImportError:
     pass
 
 logger = logging.getLogger(__name__)
 
 
 class PetabImporter(AmiciObjectBuilder):
+    """
+    Importer for Petab files.
+
+    Create an `amici.Model`, an `objective.AmiciObjective` or a
+    `pypesto.Problem` from Petab files.
+    """
+
     MODEL_BASE_DIR = "amici_models"
 
     def __init__(self,
                  petab_problem: 'petab.Problem',
                  output_folder: str = None,
                  model_name: str = None,
                  validate_petab: bool = True):
         """
+        Initialize importer.
+
+        Parameters
+        ----------
         petab_problem:
             Managing access to the model and data.
         output_folder:
             Folder to contain the amici model. Defaults to
             './amici_models/{model_name}'.
         model_name:
             Name of the model, which will in particular be the name of the
@@ -67,34 +79,33 @@
             model_name = _find_model_name(self.output_folder)
         self.model_name = model_name
 
     @staticmethod
     def from_yaml(yaml_config: Union[dict, str],
                   output_folder: str = None,
                   model_name: str = None) -> 'PetabImporter':
-        """
-        Simplified constructor using a petab yaml file.
-        """
+        """Simplified constructor using a petab yaml file."""
         petab_problem = petab.Problem.from_yaml(yaml_config)
 
         return PetabImporter(
             petab_problem=petab_problem,
             output_folder=output_folder,
             model_name=model_name)
 
     def check_gradients(
         self,
         *args,
         rtol: float = 1e-2,
         atol: float = 1e-3,
-        mode: Literal = None,
+        mode: Union[str, List[str]] = None,
         multi_eps=None,
         **kwargs,
     ) -> bool:
-        """Check if gradients match finite differences (FDs)
+        """
+        Check if gradients match finite differences (FDs).
 
         Parameters
         ----------
         rtol: relative error tolerance
         atol: absolute error tolerance
         mode: function values or residuals
         objAbsoluteTolerance: absolute tolerance in sensitivity calculation
@@ -139,16 +150,15 @@
             for mode_df in dfs
         ])
 
     def create_model(self,
                      force_compile: bool = False,
                      **kwargs) -> 'amici.Model':
         """
-        Import amici model. If necessary or force_compile is True, compile
-        first.
+        Import amici model.
 
         Parameters
         ----------
         force_compile:
             If False, the model is compiled only if the output folder does not
             exist yet. If True, the output folder is deleted and the model
             (re-)compiled in either case.
@@ -178,29 +188,24 @@
         else:
             logger.info(f"Using existing amici model in folder "
                         f"{self.output_folder}.")
 
         return self._create_model()
 
     def _create_model(self) -> 'amici.Model':
-        """
-        No checks, no compilation, just load the model module and return
-        the model.
-        """
+        """Load model module and return the model, no checks/compilation."""
         # load moduĺe
         module = amici.import_model_module(module_name=self.model_name,
                                            module_path=self.output_folder)
         model = module.getModel()
 
         return model
 
     def _must_compile(self, force_compile: bool):
-        """
-        Check whether the model needs to be compiled first.
-        """
+        """Check whether the model needs to be compiled first."""
         # asked by user
         if force_compile:
             return True
 
         # folder does not exist
         if not os.path.exists(self.output_folder) or \
                 not os.listdir(self.output_folder):
@@ -214,54 +219,50 @@
             return True
 
         # no need to (re-)compile
         return False
 
     def compile_model(self, **kwargs):
         """
-        Compile the model. If the output folder exists already, it is first
-        deleted.
+        Compile the model.
+
+        If the output folder exists already, it is first deleted.
 
         Parameters
         ----------
         kwargs: Extra arguments passed to `amici.SbmlImporter.sbml2amici`.
 
         """
-
         # delete output directory
         if os.path.exists(self.output_folder):
             shutil.rmtree(self.output_folder)
 
         amici.petab_import.import_model(
             sbml_model=self.petab_problem.sbml_model,
             condition_table=self.petab_problem.condition_df,
             observable_table=self.petab_problem.observable_df,
             model_name=self.model_name,
             model_output_dir=self.output_folder,
             **kwargs)
 
     def create_solver(self, model: 'amici.Model' = None) -> 'amici.Solver':
-        """
-        Return model solver.
-        """
+        """Return model solver."""
         # create model
         if model is None:
             model = self.create_model()
 
         solver = model.getSolver()
         return solver
 
     def create_edatas(
             self,
             model: 'amici.Model' = None,
             simulation_conditions=None
     ) -> List['amici.ExpData']:
-        """
-        Create list of amici.ExpData objects.
-        """
+        """Create list of amici.ExpData objects."""
         # create model
         if model is None:
             model = self.create_model()
 
         return amici.petab_objective.create_edatas(
             amici_model=model,
             petab_problem=self.petab_problem,
@@ -432,18 +433,18 @@
             output_ids=output_ids,
             condition_ids=condition_ids)
 
         return predictor
 
     def create_prior(self) -> NegLogParameterPriors:
         """
-        Creates a prior from the parameter table. Returns None, if no priors
-        are defined.
-        """
+        Create a prior from the parameter table.
 
+        Returns None, if no priors are defined.
+        """
         prior_list = []
 
         if petab.OBJECTIVE_PRIOR_TYPE in self.petab_problem.parameter_df:
 
             for i, x_id in enumerate(self.petab_problem.x_ids):
 
                 prior_type_entry = self.petab_problem.\
@@ -469,17 +470,18 @@
         if len(prior_list):
             return NegLogParameterPriors(prior_list)
         else:
             return None
 
     def create_startpoint_method(self):
         """
-        Creates a startpoint method, if the PEtab problem specifies an
-        initializationPrior. Returns None, if no initializationPrior
-        is specified.
+        Create a startpoint method.
+
+        If the PEtab problem specifies an initializationPrior. Returns None,
+        if no initializationPrior is specified.
         """
         if petab.INITIALIZATION_PRIOR_TYPE \
                 not in self.petab_problem.parameter_df:
             return None
 
         def startpoint_method(n_starts: int, **kwargs):
             return petab.sample_parameter_startpoints(
@@ -538,16 +540,15 @@
         return problem
 
     def rdatas_to_measurement_df(
             self, rdatas: Sequence['amici.ReturnData'],
             model: 'amici.Model' = None
     ) -> pd.DataFrame:
         """
-        Create a measurement dataframe in the petab format from
-        the passed `rdatas` and own information.
+        Create a measurement dataframe in the petab format.
 
         Parameters
         ----------
         rdatas:
             A list of rdatas as produced by
             pypesto.AmiciObjective.__call__(x, return_dict=True)['rdatas'].
         model:
@@ -568,26 +569,31 @@
         return amici.petab_objective.rdatas_to_measurement_df(
             rdatas, model, measurement_df)
 
     def rdatas_to_simulation_df(
             self, rdatas: Sequence['amici.ReturnData'],
             model: 'amici.Model' = None
     ) -> pd.DataFrame:
-        """Same as `rdatas_to_measurement_df`, execpt a petab simulation
-        dataframe is created, i.e. the measurement column label is adjusted.
+        """
+        See `rdatas_to_measurement_df`.
+
+        Execpt a petab simulation dataframe is created, i.e. the measurement
+        column label is adjusted.
         """
         return self.rdatas_to_measurement_df(rdatas, model).rename(
             columns={petab.MEASUREMENT: petab.SIMULATION})
 
     def prediction_to_petab_measurement_df(
             self,
             prediction: PredictionResult,
             predictor: AmiciPredictor = None
     ) -> pd.DataFrame:
         """
+        Cast prediction into a dataframe.
+
         If a PEtab problem is simulated without post-processing, then the
         result can be cast into a PEtab measurement or simulation dataframe
 
         Parameters
         ----------
         prediction:
             A prediction result as produced by an AmiciPredictor
@@ -614,33 +620,36 @@
         return self.rdatas_to_measurement_df(rdatas, model)
 
     def prediction_to_petab_simulation_df(
             self,
             prediction: PredictionResult,
             predictor: AmiciPredictor = None
     ) -> pd.DataFrame:
-        """Same as `prediction_to_petab_measurement_df`, except a PEtab
-        simulation dataframe is created, i.e. the measurement column label is
-        adjusted.
+        """
+        See `prediction_to_petab_measurement_df`.
+
+        Except a PEtab simulation dataframe is created, i.e. the measurement
+        column label is adjusted.
         """
         return self.prediction_to_petab_measurement_df(
             prediction, predictor).rename(
             columns={petab.MEASUREMENT: petab.SIMULATION})
 
 
 def _find_output_folder_name(
         petab_problem: 'petab.Problem',
         model_name: str,
 ) -> str:
     """
-    Find a name for storing the compiled amici model in. If available,
-    use the sbml model name from the `petab_problem` or the provided
-    `model_name` (latter is given priority), otherwise create a unique name.
-    The folder will be located in the `PetabImporter.MODEL_BASE_DIR`
-    subdirectory of the current directory.
+    Find a name for storing the compiled amici model in.
+
+    If available, use the sbml model name from the `petab_problem` or the
+    provided `model_name` (latter is given priority), otherwise create a
+    unique name. The folder will be located in the
+    `PetabImporter.MODEL_BASE_DIR` subdirectory of the current directory.
     """
     # check whether location for amici model is a file
     if os.path.exists(PetabImporter.MODEL_BASE_DIR) and \
             not os.path.isdir(PetabImporter.MODEL_BASE_DIR):
         raise AssertionError(
             f"{PetabImporter.MODEL_BASE_DIR} exists and is not a directory, "
             f"thus cannot create a directory for the compiled amici model.")
@@ -661,11 +670,9 @@
         # create random folder name
         output_folder = os.path.abspath(
             tempfile.mkdtemp(dir=PetabImporter.MODEL_BASE_DIR))
     return output_folder
 
 
 def _find_model_name(output_folder: str) -> str:
-    """
-    Just re-use the last part of the output folder.
-    """
+    """Just re-use the last part of the output folder."""
     return os.path.split(os.path.normpath(output_folder))[-1]
```

### Comparing `pypesto-0.2.8/pypesto/petab/pysb_importer.py` & `pypesto-0.2.9/pypesto/petab/pysb_importer.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,42 +6,45 @@
     import amici
     import amici.petab_import_pysb
 except ImportError:
     pass
 
 
 class PetabImporterPysb(PetabImporter):
-    """Import for experimental PySB-based PEtab problems"""
+    """Import for experimental PySB-based PEtab problems."""
 
     def __init__(self,
                  petab_problem: 'amici.petab_import_pysb.PysbPetabProblem',
                  output_folder: str = None):
         """
+        Initialize importer.
+
+        Parameters
+        ----------
         petab_problem:
             Managing access to the model and data.
         output_folder:
             Folder to contain the amici model.
         """
-
         super().__init__(petab_problem,
                          model_name=petab_problem.pysb_model.name,
                          output_folder=output_folder,
                          validate_petab=False)
 
     def compile_model(self, **kwargs):
         """
-        Compile the model. If the output folder exists already, it is first
-        deleted.
+        Compile the model.
+
+        If the output folder exists already, it is first deleted.
 
         Parameters
         ----------
         kwargs: Extra arguments passed to `amici.SbmlImporter.sbml2amici`.
 
         """
-
         # delete output directory
         if os.path.exists(self.output_folder):
             shutil.rmtree(self.output_folder)
 
         amici.petab_import_pysb.import_model_pysb(
             petab_problem=self.petab_problem,
             model_output_dir=self.output_folder,
```

### Comparing `pypesto-0.2.8/pypesto/predict/amici_predictor.py` & `pypesto-0.2.9/pypesto/predict/amici_predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,39 +9,41 @@
                         AMICI_X, AMICI_SX)
 from .result import PredictionResult
 from ..objective import AmiciObjective
 
 
 class AmiciPredictor:
     """
-    Do forward simulations (predictions) with parameter vectors,
-    for an AMICI model. The user may supply post-processing methods.
+    Do forward simulations/predictions for an AMICI model.
+
+    The user may supply post-processing methods.
     If post-processing methods are supplied, and a gradient of the prediction
     is requested, then the sensitivities of the AMICI model must also be
     post-processed. There are no checks here to ensure that the sensitivities
     are correctly post-processed, this is explicitly left to the user.
     There are also no safeguards if the postprocessor routines fail. This may
     happen if, e.g., a call to Amici fails, and no timepoints, states or
     observables are returned. As the AmiciPredictor is agnostic about the
     dimension of the postprocessor and also the dimension of the postprocessed
     output, these checks are also left to the user. An example for such a check
     is provided in the default output (see _default_output()).
     """
+
     def __init__(self,
                  amici_objective: AmiciObjective,
                  amici_output_fields: Union[Sequence[str], None] = None,
                  post_processor: Union[Callable, None] = None,
                  post_processor_sensi: Union[Callable, None] = None,
                  post_processor_time: Union[Callable, None] = None,
                  max_chunk_size: Union[int, None] = None,
                  output_ids: Union[Sequence[str], None] = None,
                  condition_ids: Union[Sequence[str], None] = None,
                  ):
         """
-        Constructor.
+        Initialize predictor.
 
         Parameters
         ----------
         amici_objective:
             An objective object, which will be used to get model simulations
         amici_output_fields:
             keys that exist in the return data object from AMICI, which should
@@ -122,14 +124,16 @@
             mode: str = MODE_FUN,
             output_file: str = '',
             output_format: str = CSV,
             include_llh_weights: bool = False,
             include_sigmay: bool = False
     ) -> PredictionResult:
         """
+        Call the predictor.
+
         Simulate a model for a certain prediction function.
         This method relies on the AmiciObjective, which is underlying, but
         allows the user to apply any post-processing of the results, the
         sensitivities, and the timepoints.
 
         Parameters
         ----------
@@ -218,29 +222,30 @@
                      x: np.ndarray,
                      sensi_orders: Tuple[int, ...],
                      mode: str = MODE_FUN,
                      include_llh_weights: bool = False,
                      include_sigmay: bool = False
                      ) -> Tuple[List, List, List]:
         """
-        This function splits the calls to amici into smaller chunks, as too
-        large ReturnData objects from amici including many simulations can be
-        problematic in terms of memory
+        Split the calls to amici into smaller chunks.
+
+        Too large ReturnData objects from amici including many simulations
+        can be problematic in terms of memory.
 
         Parameters
         ----------
         x:
             The parameters for which to evaluate the prediction function.
         sensi_orders:
             Specifies which sensitivities to compute, e.g. (0,1) -> fval, grad.
         mode:
             Whether to compute function values or residuals.
 
-        Returns:
-        --------
+        Returns
+        -------
         timepoints:
             List of np.ndarrays, every entry includes the output timepoints of
             the respective condition
         outputs:
             List of np.ndarrays, every entry includes the postprocessed outputs
             of the respective condition
         outputs_sensi:
@@ -250,15 +255,14 @@
             Boolean whether weights should be included in the prediction.
             Necessary for weighted means of Ensembles.
         include_sigmay:
             Boolean whether standard deviations should be included in the
             prediction output. Necessary for evaluation of weighted means
             of Ensembles.
         """
-
         # Do we have a maximum number of simulations allowed?
         n_edatas = len(self.amici_objective.edatas)
         if self.max_chunk_size is None:
             # simulate all conditions at once
             n_simulations = 1
         else:
             # simulate only a subset of conditions
@@ -279,17 +283,18 @@
             self._wrap_call_to_amici(
                 amici_outputs=amici_outputs, x=x, sensi_orders=sensi_orders,
                 parameter_mapping=self.amici_objective.parameter_mapping[ids],
                 edatas=self.amici_objective.edatas[ids], mode=mode)
 
         def _default_output(amici_outputs):
             """
-            Default output of prediction, equals to observables of AMICI model.
-            We need to check that call to AMICI was successful (status == 0),
-            before writing the output
+            Create default output of prediction.
+
+            Equals to observables of AMICI model. We need to check that call
+            to AMICI was successful (status == 0), before writing the output.
             """
             amici_nt = [len(edata.getTimepoints())
                         for edata in self.amici_objective.edatas]
             amici_ny = len(self.output_ids)
             amici_np = len(self.amici_objective.x_names)
 
             outputs = []
@@ -351,15 +356,16 @@
 
         return (timepoints, outputs, outputs_sensi, outputs_weights,
                 outputs_sigmay)
 
     def _wrap_call_to_amici(self, amici_outputs, x, sensi_orders, mode,
                             parameter_mapping, edatas):
         """
-        The only purpose of this function is to encapsulate the call to amici:
+        Encapsulate the call to amici.
+
         This allows to use variable scoping as a mean to clean up the memory
         after calling amici, which is beneficial if large models with large
         datasets are used.
         """
         chunk = self.amici_objective(x=x, sensi_orders=sensi_orders, mode=mode,
                                      parameter_mapping=parameter_mapping,
                                      edatas=edatas,  return_dict=True)
```

### Comparing `pypesto-0.2.8/pypesto/predict/constants.py` & `pypesto-0.2.9/pypesto/predict/constants.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.2.8/pypesto/predict/result.py` & `pypesto-0.2.9/pypesto/predict/result.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""PredictionResult and PredictionConditionResult."""
 import numpy as np
 import pandas as pd
 import h5py
 from warnings import warn
 from time import time
 from typing import Sequence, Union, Dict
 from pathlib import Path
@@ -18,29 +19,30 @@
     TIME,
     TIMEPOINTS,
 )
 
 
 class PredictionConditionResult:
     """
-    This class is a light-weight wrapper for the prediction of one simulation
-    condition of an amici model. It should provide a common api how amici
-    predictions should look like in pyPESTO.
+    Light-weight wrapper for the prediction of one simulation condition.
+
+    It should provide a common api how amici predictions should look like in
+    pyPESTO.
     """
 
     def __init__(self,
                  timepoints: np.ndarray,
                  output_ids: Sequence[str],
                  output: np.ndarray = None,
                  output_sensi: np.ndarray = None,
                  output_weight: float = None,
                  output_sigmay: np.ndarray = None,
                  x_names: Sequence[str] = None):
         """
-        Constructor.
+        Initialize PredictionConditionResult.
 
         Parameters
         ----------
         timepoints:
             Output timepoints for this simulation condition
         output_ids:
             IDs of outputs for this simulation condition
@@ -63,23 +65,25 @@
         self.output_sigmay = output_sigmay
         self.x_names = x_names
         if x_names is None and output_sensi is not None:
             self.x_names = [f'parameter_{i_par}' for i_par in
                             range(output_sensi.shape[1])]
 
     def __iter__(self):
+        """Allow usage like a dict."""
         yield 'timepoints', self.timepoints
         yield 'output_ids', self.output_ids
         yield 'x_names', self.x_names
         yield 'output', self.output
         yield 'output_sensi', self.output_sensi
         yield 'output_weight', self.output_weight
         yield 'output_sigmay', self.output_sigmay
 
     def __eq__(self, other):
+        """Check equality of two PredictionConditionResults."""
         def to_bool(expr):
             if isinstance(expr, bool):
                 return expr
             return expr.any()
 
         if to_bool(self.timepoints != other.timepoints):
             return False
@@ -96,27 +100,28 @@
         if to_bool(self.output_sigmay != other.output_sigmay):
             return False
         return True
 
 
 class PredictionResult:
     """
-    This class is a light-weight wrapper around predictions from pyPESTO made
-    via an amici model. It's only purpose is to have fixed format/api, how
-    prediction results should be stored, read, and handled: as predictions are
-    a very flexible format anyway, they should at least have a common
-    definition, which allows to work with them in a reasonable way.
+    Light-weight wrapper around prediction from pyPESTO made by an AMICI model.
+
+    Its only purpose is to have fixed format/api, how prediction results
+    should be stored, read, and handled: as predictions are a very flexible
+    format anyway, they should at least have a common definition,
+    which allows to work with them in a reasonable way.
     """
 
     def __init__(self,
                  conditions: Sequence[Union[PredictionConditionResult, Dict]],
                  condition_ids: Sequence[str] = None,
                  comment: str = None):
         """
-        Constructor.
+        Initialize PredictionResult.
 
         Parameters
         ----------
         conditions:
             A list of PredictionConditionResult objects or dicts
         condition_ids:
             IDs or names of the simulation conditions, which belong to this
@@ -135,47 +140,51 @@
             self.condition_ids = [get_condition_label(i_cond)
                                   for i_cond in range(len(conditions))]
 
         # add a comment to this prediction if available
         self.comment = comment
 
     def __iter__(self):
+        """Allow usage like an iterator."""
         parameter_ids = None
         if self.conditions:
             parameter_ids = self.conditions[0].x_names
 
         yield 'conditions', [dict(cond) for cond in self.conditions]
         yield 'condition_ids', self.condition_ids
         yield 'comment', self.comment
         yield 'parameter_ids', parameter_ids
 
     def __eq__(self, other):
+        """Check equality of two PredictionResults."""
         if not isinstance(other, PredictionResult):
             return False
         if self.comment != other.comment:
             return False
         if self.condition_ids != other.condition_ids:
             return False
         for i_cond, _ in enumerate(self.conditions):
             if self.conditions[i_cond] != other.conditions[i_cond]:
                 return False
         return True
 
     def write_to_csv(self, output_file: str):
         """
-        This method saves predictions to a csv file.
+        Save predictions to a csv file.
 
         Parameters
         ----------
         output_file:
             path to file/folder to which results will be written
         """
 
         def _prepare_csv_output(output_file):
             """
+            Prepare a folder for output.
+
             If a csv is requested, this routine will create a folder for it,
             with a suiting name: csv's are by default 2-dimensional, but the
             output will have the format n_conditions x n_timepoints x n_outputs
             For sensitivities, we even have x n_parameters. This makes it
             necessary to create multiple files and hence, a folder of its own
             makes sense. Returns a pathlib.Path object of the output.
             """
@@ -230,22 +239,22 @@
                                           data=cond.output_sensi[:, i_par, :])
                     result.to_csv(filename, sep='\t')
 
     def write_to_h5(self,
                     output_file: str,
                     base_path: str = None):
         """
-        This method saves predictions to an h5 file. It appends to the file if
-        the file already exists.
+        Save predictions to an h5 file.
+
+        It appends to the file if the file already exists.
 
         Parameters
         ----------
         output_file:
             path to file/folder to which results will be written
-
         base_path:
             base path in the h5 file
         """
         # check if the file exists and append to it in case it does
         output_path = Path(output_file)
         filemode = 'w'
         if os.path.exists(output_path):
@@ -280,16 +289,17 @@
                     f.create_dataset(os.path.join(base, str(i_cond),
                                                   OUTPUT_SENSI),
                                      data=cond.output_sensi)
 
     @staticmethod
     def _check_existence(output_path):
         """
-        Checks whether a file or a folder already exists and appends a
-        timestamp if this is the case
+        Check whether a file or a folder already exists.
+
+        Append a timestamp if this is the case.
         """
         output_path_out = output_path
         while output_path_out.exists():
             output_path_out = output_path_out.with_name(
                 output_path_out.stem + f'_{round(time() * 1000)}')
             warn('Output name already existed! Changed the name of the output '
                  'by appending the unix timestampp to make it unique!')
```

### Comparing `pypesto-0.2.8/pypesto/predict/task.py` & `pypesto-0.2.9/pypesto/predict/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,10 +37,11 @@
         self.predictor = predictor
         self.x = x
         self.sensi_orders = sensi_orders
         self.mode = mode
         self.id = id
 
     def execute(self) -> 'pypesto.predict.PredictionResult':  # noqa: F821
+        """Execute and return the prediction."""
         logger.info(f"Executing task {self.id}.")
         prediction = self.predictor(self.x, self.sensi_orders, self.mode)
         return prediction
```

### Comparing `pypesto-0.2.8/pypesto/problem.py` & `pypesto-0.2.9/pypesto/problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: D400,D205
 """
 Problem
 =======
 
 A problem contains the objective as well as all information like prior
 describing the problem to be solved.
 
@@ -19,17 +20,18 @@
 
 SupportsFloatIterableOrValue = Union[Iterable[SupportsFloat], SupportsFloat]
 SupportsIntIterableOrValue = Union[Iterable[SupportsInt], SupportsInt]
 
 
 class Problem:
     """
-    The problem formulation. A problem specifies the objective function,
-    boundaries and constraints, parameter guesses as well as the parameters
-    which are to be optimized.
+    The problem formulation.
+
+    A problem specifies the objective function, boundaries and constraints,
+    parameter guesses as well as the parameters which are to be optimized.
 
     Parameters
     ----------
     objective:
         The objective function for minimization. Note that a shallow copy
         is created.
     lb, ub:
@@ -68,15 +70,14 @@
         required and optional parameters, are described in the `Prior` class.
     copy_objective:
         Whethter to generate a deep copy of the objective function before
         potential modification the problem class performs on it.
 
     Notes
     -----
-
     On the fixing of parameter values:
 
     The number of parameters dim_full the objective takes as input must
     be known, so it must be either lb a vector of that size, or dim_full
     specified as a parameter.
 
     All vectors are mapped to the reduced space of dimension dim in __init__,
@@ -156,46 +157,54 @@
 
         self.x_priors = x_priors_defs
 
         self.normalize()
 
     @property
     def lb(self) -> np.ndarray:
+        """Return lower bounds of free parameters."""
         return self.lb_full[self.x_free_indices]
 
     @property
     def ub(self) -> np.ndarray:
+        """Return upper bounds of free parameters."""
         return self.ub_full[self.x_free_indices]
 
     @property
     def lb_init(self) -> np.ndarray:
+        """Return initial lower bounds of free parameters."""
         return self.lb_init_full[self.x_free_indices]
 
     @property
     def ub_init(self) -> np.ndarray:
+        """Return initial upper bounds of free parameters."""
         return self.ub_init_full[self.x_free_indices]
 
     @property
     def x_guesses(self) -> np.ndarray:
+        """Return guesses of the free parameter values."""
         return self.x_guesses_full[:, self.x_free_indices]
 
     @property
     def dim(self) -> int:
+        """Return dimension only considering non fixed parameters."""
         return self.dim_full - len(self.x_fixed_indices)
 
     @property
     def x_free_indices(self) -> List[int]:
+        """Return non fixed parameters."""
         return sorted(set(range(0, self.dim_full)) - set(self.x_fixed_indices))
 
     def normalize(self) -> None:
         """
+        Process vectors.
+
         Reduce all vectors to dimension dim and have the objective accept
         vectors of dimension dim.
         """
-
         for attr in ['lb_full', 'lb_init_full', 'ub_full', 'ub_init_full']:
             value = self.__getattribute__(attr)
             if value.size == 1:
                 self.__setattr__(attr, value * np.ones(self.dim_full))
             elif value.size == self.dim:
                 # in this case the bounds only holds the values of the
                 # reduced bounds.
@@ -234,32 +243,30 @@
             raise ValueError('ub must not contain nan values')
         if np.any(self.lb >= self.ub):
             raise ValueError('lb<ub not fulfilled.')
 
     def set_x_guesses(self,
                       x_guesses: Iterable[float]):
         """
-        Sets the x_guesses of a problem.
+        Set the x_guesses of a problem.
 
         Parameters
         ----------
         x_guesses:
         """
         x_guesses_full = np.array(x_guesses)
         if x_guesses_full.shape[1] != self.dim_full:
             raise ValueError('The dimension of individual x_guesses must be '
                              'dim_full.')
         self.x_guesses_full = x_guesses_full
 
     def fix_parameters(self,
                        parameter_indices: SupportsIntIterableOrValue,
                        parameter_vals: SupportsFloatIterableOrValue) -> None:
-        """
-        Fix specified parameters to specified values
-        """
+        """Fix specified parameters to specified values."""
         parameter_indices = _make_iterable_if_value(parameter_indices, 'int')
         parameter_vals = _make_iterable_if_value(parameter_vals, 'float')
 
         # first clean to-be-fixed indices to avoid redundancies
         for iter_index, (x_index, x_value) in enumerate(
                 zip(parameter_indices, parameter_vals)
         ):
@@ -276,18 +283,15 @@
                 self.x_fixed_indices.append(index)
                 self.x_fixed_vals.append(val)
 
         self.normalize()
 
     def unfix_parameters(self, parameter_indices: SupportsIntIterableOrValue
                          ) -> None:
-        """
-        Free specified parameters
-        """
-
+        """Free specified parameters."""
         # check and adapt input
         parameter_indices = _make_iterable_if_value(parameter_indices, 'int')
 
         # first clean to-be-freed indices
         for iter_index, x_index in enumerate(parameter_indices):
             index = _type_conversion_with_check(iter_index, x_index,
                                                 'indices', 'int')
@@ -360,15 +364,16 @@
         return x_full
 
     def get_reduced_vector(
             self, x_full: Union[np.ndarray, None],
             x_indices: Optional[List[int]] = None
     ) -> Union[np.ndarray, None]:
         """
-        Keep only those elements, which indices are specified in x_indices
+        Keep only those elements, which indices are specified in x_indices.
+
         If x_indices is not provided, delete fixed indices.
 
         Parameters
         ----------
         x_full: array_like, ndim=1
             The vector in dimension dim_full.
         x_indices:
@@ -404,15 +409,16 @@
             return x_full
 
         x = x_full[np.ix_(self.x_free_indices, self.x_free_indices)]
 
         return x
 
     def full_index_to_free_index(self, full_index: int):
-        """Calculate index in reduced vector from index in full vector.
+        """
+        Calculate index in reduced vector from index in full vector.
 
         Parameters
         ----------
         full_index: The index in the full vector.
 
         Returns
         -------
@@ -422,16 +428,17 @@
         if full_index in fixed_indices:
             raise ValueError(
                 "Cannot compute index in free vector: Index is fixed.")
         return full_index - sum(fixed_indices < full_index)
 
     def print_parameter_summary(self) -> None:
         """
-        Prints a summary of what parameters are being optimized and
-        parameter boundaries.
+        Print a summary of parameters.
+
+        Include what parameters are being optimized and parameter boundaries.
         """
         print(  # noqa: T001 (print)
             pd.DataFrame(
                 index=self.x_names,
                 data={
                     'free': [idx in self.x_free_indices
                              for idx in range(self.dim_full)],
@@ -455,18 +462,18 @@
 
 
 def _type_conversion_with_check(index: int,
                                 value: Union[SupportsFloat, SupportsInt],
                                 valuename: str,
                                 convtype: str) -> Union[float, int]:
     """
-    Converts values to the requested type, raises and appropriate error if
-    not possible.
-    """
+    Convert values to the requested type.
 
+    Raises and appropriate error if not possible.
+    """
     if convtype not in _convtypes:
         raise ValueError(f'Unsupported type {convtype}')
 
     can_convert = hasattr(value, _convtypes[convtype]['attr'])
     # this may fail for weird custom ypes that can be converted to int but
     # not float, but we probably don't want those as indiced anyways
     lossless_conversion = not convtype == 'int' \
@@ -483,18 +490,15 @@
     return _convtypes[convtype]['conv'](value)
 
 
 def _make_iterable_if_value(value: Union[SupportsFloatIterableOrValue,
                                          SupportsIntIterableOrValue],
                             convtype: str) -> Union[Iterable[SupportsFloat],
                                                     Iterable[SupportsInt]]:
-    """
-    Converts scalar values to iterables if input is scalar, may update type
-    """
-
+    """Convert scalar values to iterables for scalar input, may update type."""
     if convtype not in _convtypes:
         raise ValueError(f'Unsupported type {convtype}')
 
     if not hasattr(value, '__iter__'):
         return [_type_conversion_with_check(0, value, 'values', convtype)]
     else:
         return value
```

### Comparing `pypesto-0.2.8/pypesto/profile/approximate.py` & `pypesto-0.2.9/pypesto/profile/approximate.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,19 @@
         result: Result,
         profile_index: Iterable[int] = None,
         profile_list: int = None,
         result_index: int = 0,
         n_steps: int = 100,
 ) -> Result:
     """
-    Calculate profiles based on an approximation via a normal likelihood
-    centered at the chosen optimal parameter value, with the covariance matrix
-    being the Hessian or FIM.
+    Calculate profile approximation.
+
+    Based on an approximation via a normal likelihood centered at the chosen
+    optimal parameter value, with the covariance matrix being the Hessian or
+    FIM.
 
     Parameters
     ----------
     problem:
         The problem to be solved.
     result:
         A result object to initialize profiling and to append the profiling
```

### Comparing `pypesto-0.2.8/pypesto/profile/options.py` & `pypesto-0.2.9/pypesto/profile/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,28 +56,29 @@
         self.step_size_factor = step_size_factor
         self.delta_ratio_max = delta_ratio_max
         self.reg_points = reg_points
         self.reg_order = reg_order
         self.magic_factor_obj_value = magic_factor_obj_value
 
     def __getattr__(self, key):
+        """Allow usage of keys like attributes."""
         try:
             return self[key]
         except KeyError:
             raise AttributeError(key)
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
     @staticmethod
     def create_instance(
             maybe_options: Union['ProfileOptions', Dict]
     ) -> 'ProfileOptions':
         """
-        Returns a valid options object.
+        Return a valid options object.
 
         Parameters
         ----------
         maybe_options: ProfileOptions or dict
         """
         if isinstance(maybe_options, ProfileOptions):
             return maybe_options
```

### Comparing `pypesto-0.2.8/pypesto/profile/profile.py` & `pypesto-0.2.9/pypesto/profile/profile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import Callable, Union, Iterable
 
 from ..engine import Engine, SingleCoreEngine
 from ..optimize import Optimizer
 from ..problem import Problem
 from ..result import Result
+from ..optimize.util import autosave
 from .profile_next_guess import next_guess
 from .options import ProfileOptions
 from .util import initialize_profile
 from .task import ProfilerTask
 
 logger = logging.getLogger(__name__)
 
@@ -19,18 +20,19 @@
         optimizer: Optimizer,
         engine: Engine = None,
         profile_index: Iterable[int] = None,
         profile_list: int = None,
         result_index: int = 0,
         next_guess_method: Union[Callable, str] = 'adaptive_step_regression',
         profile_options: ProfileOptions = None,
-        progress_bar: bool = True
+        progress_bar: bool = True,
+        filename: str = "Auto"
 ) -> Result:
     """
-    This is the main function to call to do parameter profiling.
+    Call to do parameter profiling.
 
     Parameters
     ----------
     problem:
         The problem to be solved.
     result:
         A result object to initialize profiling and to append the profiling
@@ -54,14 +56,19 @@
     next_guess_method:
         Function handle to a method that creates the next starting point for
         optimization in profiling.
     profile_options:
         Various options applied to the profile optimization.
     progress_bar:
         Whether to display a progress bar.
+    filename:
+        Name of the hdf5 file, where the result will be saved. Default is
+        "Auto", in which case it will automatically generate a file named
+        `year_month_day_profiling_result.hdf5`. Deactivate saving by
+        setting filename to `None`.
 
     Returns
     -------
     result:
         The profile results are filled into `result.profile_result`.
     """
     # Handling defaults
@@ -121,8 +128,12 @@
     indexed_profiles = engine.execute(tasks, progress_bar=progress_bar)
 
     # fill in the ProfilerResults at the right index
     for indexed_profile in indexed_profiles:
         result.profile_result.list[-1][indexed_profile['index']] = \
             indexed_profile['profile']
 
+    autosave(filename=filename,
+             result=result,
+             type="profiling")
+
     return result
```

### Comparing `pypesto-0.2.8/pypesto/profile/profile_next_guess.py` & `pypesto-0.2.9/pypesto/profile/profile_next_guess.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,17 @@
         profile_options: ProfileOptions,
         update_type: str,
         current_profile: ProfilerResult,
         problem: Problem,
         global_opt: float
 ) -> np.ndarray:
     """
-    This function creates the next initial guess for the optimizer in
-    order to compute the next profile point. Different proposal methods
+    Create the next initial guess for the optimizer.
+
+    Used in order to compute the next profile point. Different proposal methods
     are available.
 
     Parameters
     ----------
     x:
         The current position of the profiler.
     par_index:
@@ -42,15 +43,14 @@
         Log-posterior value of the global optimum.
 
     Returns
     -------
     next_guess:
         The next initial guess as base for the next profile point.
     """
-
     if update_type == 'fixed_step':
         return fixed_step(x, par_index, par_direction, profile_options,
                           problem)
     elif update_type == 'adaptive_step_order_0':
         order = 0
     elif update_type == 'adaptive_step_order_1':
         order = 1
@@ -113,16 +113,18 @@
         options: ProfileOptions,
         current_profile: ProfilerResult,
         problem: Problem,
         global_opt: float,
         order: int = 1
 ) -> np.ndarray:
     """
-    group of more complex methods for point proposal, step size is
-    automatically computed by a line search algorithm (hence: adaptive)
+    Group of more complex methods for point proposal.
+
+    Step size is automatically computed by a line search algorithm (hence:
+    adaptive).
 
     Parameters
     ----------
     x:
         The current position of the profiler, size `dim_full`.
     par_index:
         The index of the parameter of the current profile
@@ -243,19 +245,19 @@
         global_opt: float,
         order: int,
         current_profile: ProfilerResult,
         problem: Problem,
         options: ProfileOptions
 ) -> Tuple:
     """
-    Computes the very first step direction update guesses, check whether
-    enough steps have been taken for applying regression, computes
-    regression or simple extrapolation.
-    """
+    Compute the very first step direction update guesses.
 
+    Check whether enough steps have been taken for applying regression,
+    computes regression or simple extrapolation.
+    """
     # set the update direction
     delta_x_dir = np.zeros(len(x))
     delta_x_dir[par_index] = par_direction
     reg_par = None
 
     # Is this the first step along this profile? If so, try a simple step
     if n_profile_points == 1:
@@ -290,18 +292,18 @@
         n_profile_points: int,
         par_index: int,
         current_profile: ProfilerResult,
         problem: Problem,
         options: ProfileOptions
 ) -> List[float]:
     """
-    Computes the regression polynomial which is used to step proposal
-    extrapolation from the last profile points
-    """
+    Compute the regression polynomial.
 
+    Used to step proposal extrapolation from the last profile points
+    """
     # determine interpolation order
     reg_max_order = np.floor(n_profile_points / 2)
     reg_order = np.min([reg_max_order, options.reg_order])
     reg_points = np.min([n_profile_points, options.reg_points])
 
     # set up matrix of regression parameters
     reg_par = []
@@ -342,17 +344,18 @@
         clip_to_minmax: Callable,
         clip_to_bounds: Callable,
         par_index: int,
         problem: Problem,
         options: ProfileOptions
 ) -> np.ndarray:
     """
-    Performs the line search based on the objective function we want to
-    reach, based on the current position in parameter space and on the
-    first guess for the proposal.
+    Perform the line search.
+
+    Based on the objective function we want to reach, based on the current
+    position in parameter space and on the first guess for the proposal.
     """
     # Was the initial step too big or too small?
     if direction == 'increase':
         adapt_factor = options.step_size_factor
     else:
         adapt_factor = 1 / options.step_size_factor
 
@@ -390,33 +393,29 @@
 def next_x_interpolate(
         next_obj: float,
         last_obj: float,
         next_x: np.ndarray,
         last_x: np.ndarray,
         next_obj_target: float
 ) -> np.ndarray:
-    """
-    Interpolate between the last two steps-
-    """
+    """Interpolate between the last two steps."""
     delta_obj = np.abs(next_obj - last_obj)
     add_x = np.abs(last_obj - next_obj_target) * (
             next_x - last_x) / delta_obj
 
     # fix final guess and return
     return last_x + add_x
 
 
 def clip(
         vector_guess: Union[float, np.ndarray],
         lower: Union[float, np.ndarray],
         upper: Union[float, np.ndarray]
 ) -> Union[float, np.ndarray]:
-    """
-    Restrict a scalar or a vector to given bounds.
-    """
+    """Restrict a scalar or a vector to given bounds."""
     if isinstance(vector_guess, float):
         vector_guess = np.max([np.min([vector_guess, upper]), lower])
     else:
         for i_par, i_guess in enumerate(vector_guess):
             vector_guess[i_par] = np.max([np.min([i_guess, upper[i_par]]),
                                           lower[i_par]])
     return vector_guess
```

### Comparing `pypesto-0.2.8/pypesto/profile/result.py` & `pypesto-0.2.9/pypesto/profile/result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import numpy as np
 
 
 class ProfilerResult(dict):
     """
-    The result of a profiler run. The standardized return return value from
-    pypesto.profile, which can either be initialized from an OptimizerResult
-    or from an existing ProfilerResult (in order to extend the computation).
+    The result of a profiler run.
+
+    The standardized return value from pypesto.profile, which can
+    either be initialized from an OptimizerResult or from an existing
+    ProfilerResult (in order to extend the computation).
 
     Can be used like a dict.
 
     Attributes
     ----------
     x_path:
         The path of the best found parameters along the profile
@@ -33,15 +35,14 @@
     n_hess:
         Number of Hessian evaluations.
     message:
         Textual comment on the profile result.
 
     Notes
     -----
-
     Any field not supported by the profiler or the profiling optimizer is
     filled with None. Some fields are filled by pypesto itself.
     """
 
     def __init__(self,
                  x_path: np.ndarray,
                  fval_path: np.ndarray,
@@ -74,14 +75,15 @@
         self.time_total = time_total
         self.n_fval = n_fval
         self.n_grad = n_grad
         self.n_hess = n_hess
         self.message = message
 
     def __getattr__(self, key):
+        """Allow usage of keys like attributes."""
         try:
             return self[key]
         except KeyError:
             raise AttributeError(key)
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
@@ -93,15 +95,15 @@
                              gradnorm: float = np.nan,
                              time: float = np.nan,
                              exitflag: float = np.nan,
                              n_fval: int = 0,
                              n_grad: int = 0,
                              n_hess: int = 0) -> None:
         """
-        This function appends a new point to the profile path.
+        Append a new point to the profile path.
 
         Parameters
         ----------
         x:
             The parameter values.
         fval:
             The function value at `x`.
@@ -118,15 +120,14 @@
         n_fval:
             Number of function evaluations performed to find `x`.
         n_grad:
             Number of gradient evaluations performed to find `x`.
         n_hess:
             Number of Hessian evaluations performed to find `x`.
         """
-
         # short function to append to numpy vectors
         def append_to_vector(field_name, val):
             field_new = np.zeros(self[field_name].size + 1)
             field_new[0:-1] = self[field_name]
             field_new[-1] = val
             self[field_name] = field_new
 
@@ -147,20 +148,19 @@
         self.time_total += time
         self.n_fval += n_fval
         self.n_grad += n_grad
         self.n_hess += n_hess
 
     def flip_profile(self) -> None:
         """
-        This function flips the profiling direction (left-right)
-        Profiling direction needs to be changed once (if the profile is new),
-        or twice if we append to an existing profile.
+        Flip the profiling direction (left-right).
 
-        All profiling paths are flipped in-place.
+        Profiling direction needs to be changed once (if the profile is new),
+        or twice if we append to an existing profile. All profiling paths
+        are flipped in-place.
         """
-
         self.x_path = np.fliplr(self.x_path)
         self.fval_path = np.flip(self.fval_path)
         self.ratio_path = np.flip(self.ratio_path)
         self.gradnorm_path = np.flip(self.gradnorm_path)
         self.exitflag_path = np.flip(self.exitflag_path)
         self.time_path = np.flip(self.time_path)
```

### Comparing `pypesto-0.2.8/pypesto/profile/task.py` & `pypesto-0.2.9/pypesto/profile/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,16 @@
         self.current_profile = current_profile
         self.global_opt = global_opt
         self.create_next_guess = create_next_guess
         self.i_par = i_par
         self.options = options
 
     def execute(self) -> 'pypesto.profile.ProfilerResult':
+        """Compute profile in descending and ascending direction."""
         logger.info(f"Executing task {self.i_par}.")
-        # compute profile in descending and ascending direction
         for par_direction in [-1, 1]:
             # flip profile
             self.current_profile.flip_profile()
 
             # compute the current profile
             self.current_profile = walk_along_profile(
                 current_profile=self.current_profile,
```

### Comparing `pypesto-0.2.8/pypesto/profile/util.py` & `pypesto-0.2.9/pypesto/profile/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+"""Utility function for profile module."""
 import numpy as np
 import scipy.stats
 from typing import Any, Dict, Tuple, Iterable
 
 from ..objective.constants import GRAD
 from ..problem import Problem
 from ..result import Result, ProfileResult
 from .result import ProfilerResult
 
 
 def chi2_quantile_to_ratio(alpha: float = 0.95, df: int = 1):
     """
+    Compute profile likelihood threshold.
+
     Transform lower tail probability `alpha` for a chi2 distribution with `df`
     degrees of freedom to a profile likelihood ratio threshold.
 
     Parameters
     ----------
     alpha:
         Lower tail probability, defaults to 95% interval.
@@ -30,16 +33,17 @@
     return ratio
 
 
 def calculate_approximate_ci(
         xs: np.ndarray, ratios: np.ndarray, confidence_ratio: float
 ) -> Tuple[float, float]:
     """
-    Calculate approximate confidence interval based on profile. Interval
-    bounds are linerly interpolated.
+    Calculate approximate confidence interval based on profile.
+
+    Interval bounds are linerly interpolated.
 
     Parameters
     ----------
     xs:
         The ordered parameter values along the profile for the coordinate of
         interest.
     ratios:
@@ -80,15 +84,15 @@
         problem: Problem,
         result: Result,
         result_index: int,
         profile_index: Iterable[int],
         profile_list: int
 ) -> float:
     """
-    This function initializes profiling based on a previous optimization.
+    Initialize profiling based on a previous optimization.
 
     Parameters
     ----------
     problem:
         The problem to be solved.
     result:
         A result object to initialize profiling and to append the profiling
@@ -144,15 +148,17 @@
         optimizer_result: Dict[str, Any],
         profile_index: Iterable[int],
         profile_list: int,
         problem_dimension: int,
         global_opt: float
 ) -> None:
     """
-    This is a helper function for initialize_profile
+    Fill a ProfileResult.
+
+    Helper function for `initialize_profile`.
 
     Parameters
     ----------
     profile_result:
         A list of profiler result objects.
     optimizer_result:
         A local optimization result.
@@ -165,15 +171,14 @@
         create a new list of profiles (default) or should be added to a
         specific profile list.
     problem_dimension:
         number of parameters in the unreduced problem.
     global_opt:
         log-posterior at global optimum.
     """
-
     if optimizer_result[GRAD] is not None:
         gradnorm = np.linalg.norm(optimizer_result[GRAD])
     else:
         gradnorm = None
 
     # create blank profile
     new_profile = ProfilerResult(
```

### Comparing `pypesto-0.2.8/pypesto/profile/validation_intervals.py` & `pypesto-0.2.9/pypesto/profile/validation_intervals.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,20 @@
         result_full_data: Optional[Result] = None,
         n_starts: Optional[int] = 1,
         optimizer: Optional[Optimizer] = None,
         engine: Optional[Engine] = None,
         lsq_objective: bool = False,
         return_significance: bool = True,
 ) -> float:
-    """
-    A Validation Interval for significance alpha is a confidence region/
-    interval for a new validation experiment. [#Kreutz]_ et al.
-    (This method per default returns the significance = 1-alpha!)
+    r"""
+    Compute significance of Validation Interval.
+
+    It is a confidence region/interval for a new validation experiment.
+    [#Kreutz]_ et al. (This method per default returns the significance =
+    1-alpha!)
 
     The reasoning behind their approach is, that a validation data set
     is outside the validation interval, if fitting the full data set
     would lead to a fit $\theta_{new}$, that does not contain the old
     fit $\theta_{train}$ in their (Profile-Likelihood) based
     parameter-confidence intervals. (I.e. the old fit would be rejected by
     the fit of the full data.)
@@ -74,22 +76,19 @@
         indicates, if the function should return the significance (True) (i.e.
         the  probability, that the new data set lies outside the Confidence
         Interval for the validation experiment, as given by the method), or
         the largest alpha, such that the validation experiment still lies
         within the Confidence Interval (False). I.e. alpha = 1-significance.
 
 
-        .. [#Kreutz] Kreutz, Clemens, Raue, Andreas and Timmer, Jens.
-                  “Likelihood based observability analysis and
-                  confidence intervals for predictions of dynamic models”.
-                  BMC Systems Biology 2012/12.
-                  doi:10.1186/1752-0509-6-120
-
-     """
-
+    .. [#Kreutz] Kreutz, Clemens, Raue, Andreas and Timmer, Jens.
+        “Likelihood based observability analysis and
+        confidence intervals for predictions of dynamic models”.
+        BMC Systems Biology 2012/12. doi:10.1186/1752-0509-6-120
+    """
     if (result_full_data is not None) and (optimizer is not None):
         raise UserWarning("optimizer will not be used, as a result object "
                           "for the full data set is provided.")
 
     # if result for full data is not provided: minimize
     if result_full_data is None:
```

### Comparing `pypesto-0.2.8/pypesto/profile/walk_along_profile.py` & `pypesto-0.2.9/pypesto/profile/walk_along_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,19 @@
         optimizer: Optimizer,
         options: ProfileOptions,
         create_next_guess: Callable,
         global_opt: float,
         i_par: int
 ) -> ProfilerResult:
     """
-    This function computes half a profile, by walking ahead in positive
-    direction until some stopping criterion is fulfilled. A two-sided profile
-    is obtained by flipping the profile direction.
+    Compute half a profile.
+
+    Walk ahead in positive direction until some stopping criterion is
+    fulfilled. A two-sided profile is obtained by flipping the profile
+    direction.
 
     Parameters
     ----------
     current_profile:
         The profile which should be computed
     problem:
         The problem to be solved.
@@ -46,15 +48,14 @@
         index for the current parameter
 
     Returns
     -------
     current_profile:
         The current profile, modified in-place.
     """
-
     # create variables which are needed during iteration
     stop_profile = False
 
     # while loop for profiling (will be exited by break command)
     while True:
         # get current position on the profile path
         x_now = current_profile.x_path[:, -1]
```

### Comparing `pypesto-0.2.8/pypesto/result.py` & `pypesto-0.2.9/pypesto/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: D400,D205
 """
 Result
 ======
 
 The pypesto.Result object contains all results generated by
 the pypesto components. It contains sub-results for
 optimization, profiling, sampling.
@@ -14,17 +15,15 @@
 
 if TYPE_CHECKING:
     import pypesto.optimize as optimize
     import pypesto.profile as profile
 
 
 class OptimizeResult:
-    """
-    Result of the minimize() function.
-    """
+    """Result of the :py:func:`pypesto.optimize.minimize` function."""
 
     def __init__(self):
         self.list = []
 
     def append(
             self,
             optimizer_result: 'optimize.OptimizerResult',
@@ -33,62 +32,56 @@
         Append an optimizer result to the result object.
 
         Parameters
         ----------
         optimizer_result:
             The result of one (local) optimizer run.
         """
-
         self.list.append(optimizer_result)
         self.sort()
 
     def sort(self):
-        """
-        Sort the optimizer results by function value fval (ascending).
-        """
+        """Sort the optimizer results by function value fval (ascending)."""
         def get_fval(res):
             return res.fval if not np.isnan(res.fval) else np.inf
 
         self.list = sorted(self.list, key=get_fval)
 
     def as_dataframe(self, keys=None) -> pd.DataFrame:
         """
-        Get as pandas DataFrame. If keys is a list,
-        return only the specified values.
-        """
+        Get as pandas DataFrame.
 
+        If keys is a list, return only the specified values, otherwise all.
+        """
         lst = self.as_list(keys)
 
         df = pd.DataFrame(lst)
 
         return df
 
     def as_list(self, keys=None) -> Sequence:
         """
-        Get as list. If keys is a list,
-        return only the specified values.
+        Get as list.
+
+        If keys is a list, return only the specified values.
 
         Parameters
         ----------
         keys: list(str), optional
             Labels of the field to extract.
         """
-
         lst = self.list
 
         if keys is not None:
             lst = [{key: res[key] for key in keys} for res in lst]
 
         return lst
 
     def get_for_key(self, key) -> list:
-        """
-        Extract the list of values for the specified key as a list.
-        """
-
+        """Extract the list of values for the specified key as a list."""
         return [res[key] for res in self.list]
 
 
 class ProfileResult:
     """
     Result of the profile() function.
 
@@ -131,79 +124,73 @@
         self.list[profile_list].append(profiler_result)
 
     def set_profiler_result(
             self,
             profiler_result: 'profile.ProfilerResult',
             i_par: int,
             profile_list: int = None) -> None:
-        """Write a profiler result to the result object at `i_par` of profile
-        list `profile_list`.
+        """
+        Write a profiler result to the result object.
 
         Parameters
         ----------
         profiler_result:
             The result of one (local) profiler run.
         i_par:
-            Integer specifying the parameter index.
+            Integer specifying the parameter index where to put
+            profiler_result.
         profile_list:
             Index specifying the profile list. Defaults to the last list.
         """
         if profile_list is None:
             profile_list = -1  # last
         self.list[profile_list][i_par] = copy.deepcopy(profiler_result)
 
     def get_profiler_result(
             self, i_par: int, profile_list: int = None
     ):
         """
-        Get theprofiler result at parameter index `i_par` of profile list
-        `profile_list`.
+        Get the profiler result at parameter index `i_par` of `profile_list`.
 
         Parameters
         ----------
         i_par:
             Integer specifying the profile index.
         profile_list:
             Index specifying the profile list. Defaults to the last list.
         """
         if profile_list is None:
             profile_list = -1  # last
         return self.list[profile_list][i_par]
 
 
 class SampleResult:
-    """
-    Result of the sample() function.
-    """
+    """Result of the sample() function."""
 
     def __init__(self):
         pass
 
 
 class Result:
     """
     Universal result object for pypesto.
+
     The algorithms like optimize, profile,
     sample fill different parts of it.
 
     Attributes
     ----------
-
     problem: pypesto.Problem
         The problem underlying the results.
-
     optimize_result:
         The results of the optimizer runs.
-
     profile_result:
         The results of the profiler run.
-
     sample_result:
         The results of the sampler run.
-
     """
 
     def __init__(self, problem=None):
         self.problem = problem
         self.optimize_result = OptimizeResult()
         self.profile_result = ProfileResult()
         self.sample_result = SampleResult()
```

### Comparing `pypesto-0.2.8/pypesto/sample/__init__.py` & `pypesto-0.2.9/pypesto/sample/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: D400,D205
 """
 Sample
 ======
 
 Draw samples from the distribution, with support for various samplers.
 """
```

### Comparing `pypesto-0.2.8/pypesto/sample/adaptive_metropolis.py` & `pypesto-0.2.9/pypesto/sample/adaptive_metropolis.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 import numbers
 
 from ..problem import Problem
 from .metropolis import MetropolisSampler
 
 
 class AdaptiveMetropolisSampler(MetropolisSampler):
-    """
-    Metropolis-Hastings sampler with adaptive proposal covariance.
-    """
+    """Metropolis-Hastings sampler with adaptive proposal covariance."""
 
     def __init__(self, options: Dict = None):
         super().__init__(options)
         self._cov = None
         self._mean_hist = None
         self._cov_hist = None
         self._cov_scale = None
 
     @classmethod
     def default_options(cls):
+        """Return the default options for the sampler."""
         return {
             # controls adaptation degeneration velocity of the proposals
             # in [0, 1], with 0 -> no adaptation, i.e. classical
             # Metropolis-Hastings
             'decay_constant': 0.51,
             # number of samples before adaptation decreases significantly.
             # a higher value reduces the impact of early adaptation
@@ -39,14 +38,15 @@
             # target acceptance rate
             'target_acceptance_rate': 0.234,
             # show progress
             'show_progress': True,
         }
 
     def initialize(self, problem: Problem, x0: np.ndarray):
+        """Initialize the sampler."""
         super().initialize(problem, x0)
 
         if self.options['cov0'] is not None:
             cov0 = self.options['cov0']
             if isinstance(cov0, numbers.Real):
                 cov0 = float(cov0) * np.eye(len(x0))
         else:
@@ -129,16 +129,17 @@
         update_rate * dx.reshape((-1, 1)) @ dx.reshape((1, -1))
 
     return mean, cov
 
 
 def regularize_covariance(cov: np.ndarray, reg_factor: float) -> np.ndarray:
     """
-    Regularize the estimated covariance matrix of the sample. Useful if the
-    estimated covariance matrix is ill-conditioned.
+    Regularize the estimated covariance matrix of the sample.
+
+    Useful if the estimated covariance matrix is ill-conditioned.
     Increments the diagonal a little to ensure positivity.
 
     Parameters
     ----------
     cov:
         Estimate of the covariance matrix of the sample.
     reg_factor:
```

### Comparing `pypesto-0.2.8/pypesto/sample/auto_correlation.py` & `pypesto-0.2.9/pypesto/sample/auto_correlation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import numpy as np
 
 
 def autocorrelation_sokal(chain: np.ndarray) -> np.ndarray:
     """
-    Estimate the integrated autocorrelation time of a MCMC chain
-    using Sokal's adaptive truncated periodogram estimator.
+    Estimate the integrated autocorrelation time of a MCMC chain.
+
+    Uses Sokal's adaptive truncated periodogram estimator.
 
     - Haario, H., Laine, M., Mira, A. et al. DRAM: Efficient
     adaptive MCMC. Stat Comput 16, 339–354 (2006).
     https://doi.org/10.1007/s11222-006-9438-0
 
     - Sokal A. (1997) Monte Carlo Methods in Statistical Mechanics:
     Foundations and New Algorithms. In: DeWitt-Morette C.,
     Cartier P., Folacci A. (eds) Functional Integration.
     NATO ASI Series (Series B: Physics), vol 361. Springer, Boston, MA
 
     Parameters
     ----------
         chain: The MCMC chain.
+
     Returns
     -------
         tau_est: An estimate of the integrated autocorrelation time of
         the MCMC chain.
     """
-
     nsamples, npar = chain.shape
     tau_est = np.zeros((npar))
 
     # Calculate the fast Fourier transform
     x = np.fft.fft(chain, axis=0)
     # Get the real part
     xr = np.real(x)
```

### Comparing `pypesto-0.2.8/pypesto/sample/diagnostics.py` & `pypesto-0.2.9/pypesto/sample/diagnostics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+"""Calculate different diagnostics of the sampling result."""
 import numpy as np
 import logging
 
 from ..result import Result
 from .geweke_test import burn_in_by_sequential_geweke
 from .auto_correlation import autocorrelation_sokal
 
 logger = logging.getLogger(__name__)
 
 
 def geweke_test(result: Result, zscore: float = 2.) -> int:
     """
-    Calculates the burn-in of MCMC chains.
+    Calculate the burn-in of MCMC chains.
 
     Parameters
     ----------
     result:
         The pyPESTO result object with filled sample result.
     zscore:
         The Geweke test threshold.
@@ -40,15 +41,15 @@
     result.sample_result.burn_in = burn_in
 
     return burn_in
 
 
 def auto_correlation(result: Result) -> float:
     """
-    Calculates the autocorrelation of the MCMC chains.
+    Calculate the autocorrelation of the MCMC chains.
 
     Parameters
     ----------
     result:
         The pyPESTO result object with filled sample result.
 
     Returns
@@ -104,15 +105,14 @@
 
     Returns
     -------
     ess:
         Estimate of the effective sample size of
         the MCMC chains.
     """
-
     # Check if autocorrelation is available
     if result.sample_result.auto_correlation is None:
         # Calculate autocorrelation
         auto_correlation(result)
 
     # Get burn in index
     burn_in = result.sample_result.burn_in
```

### Comparing `pypesto-0.2.8/pypesto/sample/emcee.py` & `pypesto-0.2.9/pypesto/sample/emcee.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     def __init__(
         self,
         nwalkers: int = 1,
         sampler_args: dict = None,
         run_args: dict = None,
     ):
         """
+        Initialize sampler.
+
         Parameters
         ----------
         nwalkers: The number of walkers in the ensemble.
         sampler_args:
             Further keyword arguments that are passed on to
             ``emcee.EnsembleSampler.__init__``.
         run_args:
@@ -59,14 +61,15 @@
         self.state: Union[emcee.State, None] = None
 
     def initialize(
         self,
         problem: Problem,
         x0: Union[np.ndarray, List[np.ndarray]],
     ) -> None:
+        """Initialize the sampler."""
         self.problem = problem
 
         # extract for pickling efficiency
         objective = self.problem.objective
         lb = self.problem.lb
         ub = self.problem.ub
 
@@ -104,19 +107,20 @@
                 n_starts=self.nwalkers, startpoint_method=uniform,
                 problem=problem, startpoint_resample=True)
 
             #  restore original guesses
             problem.x_guesses_full = problem.x_guesses_full[x0.shape[0]:]
 
     def sample(self, n_samples: int, beta: float = 1.) -> None:
-        # the method returns the most recent sample state
+        """Return the most recent sample state."""
         self.state = self.sampler.run_mcmc(
             self.state, n_samples, **self.run_args)
 
     def get_samples(self) -> McmcPtResult:
+        """Get the samples into the fitting pypesto format."""
         # all walkers are concatenated, yielding a flat array
         trace_x = np.array([self.sampler.get_chain(flat=True)])
         trace_neglogpost = np.array([- self.sampler.get_log_prob(flat=True)])
         # the sampler does not know priors
         trace_neglogprior = np.full(trace_neglogpost.shape, np.nan)
         # the walkers all run on temperature 1
         betas = np.array([1.])
```

### Comparing `pypesto-0.2.8/pypesto/sample/geweke_test.py` & `pypesto-0.2.9/pypesto/sample/geweke_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Helper function for `geweke_test`."""
 import logging
 import warnings
 from typing import Tuple
 import numpy as np
 from scipy.stats import norm
 
 logger = logging.getLogger(__name__)
@@ -24,15 +25,14 @@
         Number of windows.
 
     Returns
     -------
     spectral_density:
         The spectral density.
     """
-
     if nfft is None:
         nfft = np.min(len(x), 256)
 
     if nw is None:
         nw = np.floor(nfft / 4).astype(int)
 
     n_overlap = np.floor(nw / 2).astype(int)
@@ -67,45 +67,45 @@
     spectral_density = spectral_density[0:n2]
 
     return spectral_density
 
 
 def spectrum0(x: np.ndarray) -> np.ndarray:
     """
-    Calculates the spectral density at frequency zero.
+    Calculate the spectral density at frequency zero.
 
     Parameters
     ----------
     x:
         Fraction/fragment of the MCMC chain.
 
     Returns
     -------
     spectral_density_zero:
         Spectral density at zero.
     """
-
     n_samples, n_par = x.shape
     spectral_density_zero = np.zeros((1, n_par))
 
     for i in range(n_par):
         _spectral_density_zero = spectrum(x[:, i], n_samples)
         if len(_spectral_density_zero) > 0:
             spectral_density_zero[:, i] = _spectral_density_zero[0]
     return spectral_density_zero
 
 
 def calculate_zscore(chain: np.ndarray,
                      a: float = 0.1,
                      b: float = 0.5) -> Tuple[float, float]:
     """
-    Performs a Geweke test on a chain using the first
-    "a" fraction and the last "b" fraction of it for
-    comparison. Test for equality of the means of the
-    first a% and last b% of a Markov chain.
+    Perform a Geweke test on a chain.
+
+    Use the first "a" fraction and the last "b" fraction of it for
+    comparison. Test for equality of the means of the first a% and last b%
+    of a Markov chain.
 
     See:
     Stephen P. Brooks and Gareth O. Roberts.
     Assessing convergence of Markov chain Monte Carlo
     algorithms. Statistics and Computing, 8:319--335, 1998.
 
     Parameters
@@ -119,15 +119,14 @@
     Returns
     -------
     z_score:
         Z-score of the Geweke test.
     p:
         Significance level of the Geweke test.
     """
-
     nsamples, _ = chain.shape
 
     # Define First fraction
     index_a = np.floor(a * nsamples).astype(int)
     # Define Second fraction
     index_b = nsamples - np.floor(b * nsamples).astype(int) + 1
 
@@ -159,15 +158,15 @@
 
     return z_score, p
 
 
 def burn_in_by_sequential_geweke(chain: np.ndarray,
                                  zscore: float = 2.) -> int:
     """
-    Calculates the burn-in of MCMC chains.
+    Calculate the burn-in of MCMC chains.
 
     Parameters
     ----------
     chain:
         The MCMC chain after removing warm up phase.
     zscore:
         The Geweke test threshold.
@@ -175,15 +174,14 @@
     Returns
     -------
     burn_in:
         Iteration where the first and the last fraction
         of the chain do not differ significantly
         regarding Geweke test.
     """
-
     nsamples, npar = chain.shape
     # number of fragments
     n = 20
     # round each element to the nearest integer
     # toward zero
     step = np.floor(nsamples / n).astype(int)
     fragments = np.arange(0, nsamples-1, step)
```

### Comparing `pypesto-0.2.8/pypesto/sample/metropolis.py` & `pypesto-0.2.9/pypesto/sample/metropolis.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,49 +5,49 @@
 from ..objective import History, ObjectiveBase, NegLogPriors
 from ..problem import Problem
 from .sampler import InternalSample, InternalSampler
 from .result import McmcPtResult
 
 
 class MetropolisSampler(InternalSampler):
-    """
-    Simple Metropolis-Hastings sampler with fixed proposal variance.
-    """
+    """Simple Metropolis-Hastings sampler with fixed proposal variance."""
 
     def __init__(self, options: Dict = None):
         super().__init__(options)
         self.problem: Union[Problem, None] = None
         self.neglogpost: Union[ObjectiveBase, None] = None
         self.neglogprior: Union[NegLogPriors, None] = None
         self.trace_x: Union[Sequence[np.ndarray], None] = None
         self.trace_neglogpost: Union[Sequence[float], None] = None
         self.trace_neglogprior: Union[Sequence[float], None] = None
         self.temper_lpost: bool = False
 
     @classmethod
     def default_options(cls):
+        """Return the default options for the sampler."""
         return {
             'std': 1.,  # the proposal standard deviation
             'show_progress': True,  # whether to show the progress
         }
 
     def initialize(self, problem: Problem, x0: np.ndarray):
+        """Initialize the sampler."""
         self.problem = problem
         self.neglogpost = problem.objective
         self.neglogpost.history = History()
         if problem.x_priors is None:
             self.neglogprior = lambda x: -0.
         else:
             self.neglogprior = problem.x_priors
         self.trace_x = [x0]
         self.trace_neglogpost = [self.neglogpost(x0)]
         self.trace_neglogprior = [self.neglogprior(x0)]
 
     def sample(self, n_samples: int, beta: float = 1.):
-        # load last recorded particle
+        """Load last recorded particle."""
         x = self.trace_x[-1]
         lpost = - self.trace_neglogpost[-1]
         lprior = - self.trace_neglogprior[-1]
 
         show_progress = self.options['show_progress']
 
         # loop over iterations
@@ -57,24 +57,35 @@
                 x=x, lpost=lpost, lprior=lprior, beta=beta)
             # record step
             self.trace_x.append(x)
             self.trace_neglogpost.append(-lpost)
             self.trace_neglogprior.append(-lprior)
 
     def make_internal(self, temper_lpost: bool):
+        """
+        Allow the inner samplers to be used as inner samplers.
+
+        Can be called by parallel tempering samplers during initialization.
+        Default: Do nothing.
+
+        Parameters
+        ----------
+        temper_lpost:
+            Whether to temperate the posterior or only the likelihood.
+        """
         self.options['show_progress'] = False
         self.temper_lpost = temper_lpost
 
     def _perform_step(self, x: np.ndarray, lpost: np.ndarray,
                       lprior: np.ndarray, beta: float):
         """
-        Perform a step: Propose new parameter, evaluate and check whether to
-        accept.
-        """
+        Perform a step.
 
+        Propose new parameter, evaluate and check whether to accept.
+        """
         # propose step
         x_new: np.ndarray = self._propose_parameter(x)
 
         # check if step lies within bounds
         if any(x_new < self.problem.lb) or any(x_new > self.problem.ub):
             # will not be accepted
             lpost_new = - np.inf
@@ -123,26 +134,42 @@
         return x_new
 
     def _update_proposal(self, x: np.ndarray, lpost: float,
                          log_p_acc: float, n_sample_cur: int):
         """Update the proposal density. Default: Do nothing."""
 
     def get_last_sample(self) -> InternalSample:
+        """Get the last sample in the chain.
+
+        Returns
+        -------
+        internal_sample:
+            The last sample in the chain in the exchange format.
+        """
         return InternalSample(
             x=self.trace_x[-1],
             lpost=- self.trace_neglogpost[-1],
             lprior=- self.trace_neglogprior[-1]
         )
 
     def set_last_sample(self, sample: InternalSample):
+        """
+        Set the last sample in the chain to the passed value.
+
+        Parameters
+        ----------
+        sample:
+            The sample that will replace the last sample in the chain.
+        """
         self.trace_x[-1] = sample.x
         self.trace_neglogpost[-1] = - sample.lpost
         self.trace_neglogprior[-1] = - sample.lprior
 
     def get_samples(self) -> McmcPtResult:
+        """Get the samples into the fitting pypesto format."""
         result = McmcPtResult(
             trace_x=np.array([self.trace_x]),
             trace_neglogpost=np.array([self.trace_neglogpost]),
             trace_neglogprior=np.array([self.trace_neglogprior]),
             betas=np.array([1.]),
         )
         return result
```

### Comparing `pypesto-0.2.8/pypesto/sample/parallel_tempering.py` & `pypesto-0.2.9/pypesto/sample/parallel_tempering.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,36 +37,38 @@
                          for _ in range(len(self.betas0))]
         # configure internal samplers
         for sampler in self.samplers:
             sampler.make_internal(temper_lpost=self.temper_lpost)
 
     @classmethod
     def default_options(cls) -> Dict:
+        """Return the default options for the sampler."""
         return {
             'max_temp': 5e4,
             'exponent': 4,
             'temper_log_posterior': False,
         }
 
     def initialize(self,
                    problem: Problem,
                    x0: Union[np.ndarray, List[np.ndarray]]):
-        # initialize all samplers
+        """Initialize all samplers."""
         n_chains = len(self.samplers)
         if isinstance(x0, list):
             x0s = x0
         else:
             x0s = [x0 for _ in range(n_chains)]
         for sampler, x0 in zip(self.samplers, x0s):
             _problem = copy.deepcopy(problem)
             sampler.initialize(_problem, x0)
         self.betas = self.betas0
 
     def sample(
             self, n_samples: int, beta: float = 1.):
+        """Sample and swap in between samplers."""
         # loop over iterations
         for i_sample in tqdm(range(int(n_samples))):  # TODO test
             # sample
             for sampler, beta in zip(self.samplers, self.betas):
                 sampler.sample(n_samples=1, beta=beta)
 
             # swap samples
```

### Comparing `pypesto-0.2.8/pypesto/sample/result.py` & `pypesto-0.2.9/pypesto/sample/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 from typing import Iterable
 
 
 class McmcPtResult(dict):
-    """The result of a sampler run using Markov-chain Monte Carlo, and
-    optionally parallel tempering.
+    """
+    The result of a sampler run using Markov-chain Monte Carlo.
 
-    Can be used like a dict.
+    Currently result object of all supported samplers. Can be used like a dict.
 
     Parameters
     ----------
     trace_x: [n_chain, n_iter, n_par]
         Parameters.
     trace_neglogpost: [n_chain, n_iter]
         Negative log posterior values.
@@ -76,14 +76,15 @@
         if trace_neglogpost.shape[0] != trace_neglogprior.shape[0] \
                 or trace_neglogpost.shape[1] != trace_neglogprior.shape[1]:
             raise ValueError("Trace dimensions do not match:"
                              f"trace_neglogpost.shape={trace_neglogpost.shape}," # noqa
                              f"trace_neglogprior.shape={trace_neglogprior.shape}") # noqa
 
     def __getattr__(self, key):
+        """Allow usage of keys like attributes."""
         try:
             return self[key]
         except KeyError:
             raise AttributeError(key)
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
```

### Comparing `pypesto-0.2.8/pypesto/sample/sample.py` & `pypesto-0.2.9/pypesto/sample/sample.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import logging
 import numpy as np
 from typing import List, Union
 from time import process_time
 
 from ..problem import Problem
 from ..result import Result
+from ..optimize.util import autosave
 from .sampler import Sampler
 from .adaptive_metropolis import AdaptiveMetropolisSampler
 
 logger = logging.getLogger(__name__)
 
 
 def sample(
         problem: Problem,
         n_samples: int,
         sampler: Sampler = None,
         x0: Union[np.ndarray, List[np.ndarray]] = None,
-        result: Result = None
+        result: Result = None,
+        filename: str = "Auto"
 ) -> Result:
     """
-    This is the main function to call to do parameter sampling.
+    Call to do parameter sampling.
 
     Parameters
     ----------
     problem:
         The problem to be solved. If None is provided, a
         :class:`pypesto.AdaptiveMetropolisSampler` is used.
     n_samples:
@@ -34,14 +36,19 @@
         Initial parameter for the Markov chain. If None, the best parameter
         found in optimization is used. Note that some samplers require an
         initial parameter, some may ignore it. x0 can also be a list,
         to have separate starting points for parallel tempering chains.
     result:
         A result to write to. If None provided, one is created from the
         problem.
+    filename:
+        Name of the hdf5 file, where the result will be saved. Default is
+        "Auto", in which case it will automatically generate a file named
+        `year_month_day_sampling_result.hdf5`. Deactivate saving by
+        setting filename to `None`.
 
     Returns
     -------
     result:
         A result with filled in sample_options part.
     """
     # prepare result object
@@ -74,8 +81,12 @@
 
     # record time
     sampler_result.time = t_elapsed
 
     # record results
     result.sample_result = sampler_result
 
+    autosave(filename=filename,
+             result=result,
+             type="sampling")
+
     return result
```

### Comparing `pypesto-0.2.8/pypesto/sample/sampler.py` & `pypesto-0.2.9/pypesto/sample/sampler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Various Sampler classes."""
 import abc
 import numpy as np
 from typing import Dict, List, Union
 
 from ..problem import Problem
 from .result import McmcPtResult
 
@@ -46,26 +47,28 @@
 
     @abc.abstractmethod
     def get_samples(self) -> McmcPtResult:
         """Get the generated samples."""
 
     @classmethod
     def default_options(cls) -> Dict:
-        """Convenience method to set/get default options.
+        """
+        Set/Get default options.
 
         Returns
         -------
         default_options:
             Default sampler options.
         """
         return {}
 
     @classmethod
     def translate_options(cls, options):
-        """Convenience method to translate options and fill in defaults.
+        """
+        Translate options and fill in defaults.
 
         Parameters
         ----------
         options:
             Options configuring the sampler.
         """
         used_options = cls.default_options()
@@ -76,15 +79,17 @@
                 raise KeyError(f"Cannot handle key {key}.")
             used_options[key] = val
         return used_options
 
 
 class InternalSample:
     """
-    This is the exchange object provided and accepted by
+    Internal sample class.
+
+    Exchange object provided and accepted by
     `InternalSampler.get_last_sample()`, `InternalSampler.set_last_sample()`.
     It carries all information needed to check whether to swap between chains,
     and to continue the chain from the updated sample.
 
     Attributes
     ----------
     x:
@@ -127,16 +132,17 @@
         ----------
         sample:
             The sample that will replace the last sample in the chain.
         """
 
     def make_internal(self, temper_lpost: bool):
         """
-        This function can be called by parallel tempering samplers during
-        initialization to allow the inner samplers to adjust to them
-        being used as inner samplers. Default: Do nothing.
+        Allow the inner samplers to be used as inner samplers.
+
+        Can be called by parallel tempering samplers during initialization.
+        Default: Do nothing.
 
         Parameters
         ----------
         temper_lpost:
             Whether to temperate the posterior or only the likelihood.
         """
```

### Comparing `pypesto-0.2.8/pypesto/sample/theano.py` & `pypesto-0.2.9/pypesto/sample/theano.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,32 +39,38 @@
         # initialize the sensitivity Op
         if problem.objective.has_grad:
             self._log_prob_grad = TheanoLogProbabilityGradient(problem, beta)
         else:
             self._log_prob_grad = None
 
     def perform(self, node, inputs, outputs, params=None):
+        """Calculate the gradients of the objective function at the inputs."""
         theta, = inputs
         log_prob = self._log_prob(theta)
         outputs[0][0] = np.array(log_prob)
 
     def grad(self, inputs, g):
-        # the method that calculates the gradients - it actually returns the
-        # vector-Jacobian product - g[0] is a vector of parameter values
+        """
+        Calculate the gradients.
+
+        Actually returns the vector-Jacobian product - g[0] is a vector of
+        parameter values.
+        """
         if self._log_prob_grad is None:
             # indicates gradient not available
             return [NullType]
         theta, = inputs
         log_prob_grad = self._log_prob_grad(theta)
         return [g[0] * log_prob_grad]
 
 
 class TheanoLogProbabilityGradient(tt.Op):
     """
     Theano wrapper around a (non-normalized) log-probability gradient function.
+
     This Op will be called with a vector of values and also return a vector of
     values - the gradients in each dimension.
 
     Parameters
     ----------
     problem:
         The `pypesto.Problem` to analyze.
@@ -77,11 +83,12 @@
 
     def __init__(self, problem: Problem, beta: float = 1.):
         self._objective: Objective = problem.objective
         self._log_prob_grad = \
             lambda x: - beta * self._objective(x, sensi_orders=(1,))
 
     def perform(self, node, inputs, outputs, params=None):
+        """Calculate the gradients of the objective function at the inputs."""
         theta, = inputs
         # calculate gradients
         log_prob_grad = self._log_prob_grad(theta)
         outputs[0][0] = log_prob_grad
```

### Comparing `pypesto-0.2.8/pypesto/sample/util.py` & `pypesto-0.2.9/pypesto/sample/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""A set of helper functions"""
+"""A set of helper functions."""
 import numpy as np
 import logging
 from typing import Tuple
 
 from ..result import Result
 from .diagnostics import geweke_test
```

### Comparing `pypesto-0.2.8/pypesto/startpoint/__init__.py` & `pypesto-0.2.9/pypesto/startpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.2.8/pypesto/startpoint/assign.py` & `pypesto-0.2.9/pypesto/startpoint/assign.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,16 @@
     startpoints: np.ndarray,
     lb: np.ndarray,
     ub: np.ndarray,
     objective: ObjectiveBase,
     x_guesses: np.ndarray,
     startpoint_method: StartpointMethod,
 ):
-    """Resample startpoints having non-finite value.
+    """
+    Resample startpoints having non-finite value.
 
     Check all proposed startpoints and resample ones with non-finite value
     via the startpoint_method.
 
     Also order startpoints by function value, ascending.
 
     Parameters
@@ -112,15 +113,14 @@
         Startpoint generation method to use.
 
     Returns
     -------
     startpoints:
         Startpoints with all finite function values, shape (n_starts, n_par).
     """
-
     n_starts = startpoints.shape[0]
     resampled_startpoints = np.zeros_like(startpoints)
 
     fvals = np.empty((n_starts,))
     # iterate over startpoints
     for j in range(0, n_starts):
         startpoint = startpoints[j, :]
```

### Comparing `pypesto-0.2.8/pypesto/startpoint/base.py` & `pypesto-0.2.9/pypesto/startpoint/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,27 +49,30 @@
     """
 
     def __init__(
         self,
         function: Callable,
     ):
         """
+        Initialize.
+
         Parameters
         ----------
         function: The callable sampling startpoints.
         """
         self.function = function
 
     def __call__(
             self,
             n_starts: int,
             lb: np.ndarray,
             ub: np.ndarray,
             objective: ObjectiveBase,
     ) -> np.ndarray:
+        """Call function."""
         return self.function(
             n_starts=n_starts, lb=lb, ub=ub, objective=objective,
         )
 
 
 def to_startpoint_method(
     maybe_startpoint_method: Union[StartpointMethod, Callable],
```

### Comparing `pypesto-0.2.8/pypesto/startpoint/latin_hypercube.py` & `pypesto-0.2.9/pypesto/startpoint/latin_hypercube.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,21 +80,24 @@
 
     return xs
 
 
 class LatinHypercubeStartpoints(StartpointMethod):
     """Generate latin hypercube-sampled startpoints.
 
-    See e.g. https://en.wikipedia.org/wiki/Latin_hypercube_sampling."""
+    See e.g. https://en.wikipedia.org/wiki/Latin_hypercube_sampling.
+    """
 
     def __init__(
         self,
         smooth: bool = True,
     ):
         """
+        Initialize.
+
         Parameters
         ----------
         smooth:
             Whether a (uniformly chosen) random starting point within the
             hypercube [i/n_starts, (i+1)/n_starts] should be chosen (True) or
             the midpoint of the interval (False).
         """
@@ -103,14 +106,15 @@
     def __call__(
         self,
         n_starts: int,
         lb: np.ndarray,
         ub: np.ndarray,
         objective: ObjectiveBase = None,
     ) -> np.ndarray:
+        """Call function."""
         return _latin_hypercube(
             n_starts=n_starts,
             lb=lb,
             ub=ub,
             smooth=self.smooth,
         )
```

### Comparing `pypesto-0.2.8/pypesto/startpoint/uniform.py` & `pypesto-0.2.9/pypesto/startpoint/uniform.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,12 +49,13 @@
     def __call__(
         self,
         n_starts: int,
         lb: np.ndarray,
         ub: np.ndarray,
         objective: ObjectiveBase = None,
     ) -> np.ndarray:
+        """Call function."""
         return _uniform(n_starts=n_starts, lb=lb, ub=ub)
 
 
 # convenience and legacy
 uniform = UniformStartpoints()
```

### Comparing `pypesto-0.2.8/pypesto/store/__init__.py` & `pypesto-0.2.9/pypesto/store/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.2.8/pypesto/store/hdf5.py` & `pypesto-0.2.9/pypesto/store/hdf5.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-"""Convenience functions for working with HDF5 files"""
+"""Convenience functions for working with HDF5 files."""
 import h5py
 import numpy as np
 
 from typing import Collection
 from numbers import Number, Integral, Real
 
 
 def write_array(f: h5py.Group,
                 path: str,
                 values: Collection) -> None:
     """
-    Write array to hdf5
+    Write array to hdf5.
 
     Parameters
-    -------------
+    ----------
     f:
         h5py.Group  where dataset should be created
     path:
         path of the dataset to create
     values:
         array to write
     """
-
     if all(isinstance(x, Integral) for x in values):
         write_int_array(f, path, values)
     elif all(isinstance(x, Real) for x in values):
         write_float_array(f, path, values)
     elif all(isinstance(x, str) for x in values):
         write_string_array(f, path,
                            values)
@@ -33,18 +32,18 @@
         f[path] = values
 
 
 def write_string_array(f: h5py.Group,
                        path: str,
                        strings: Collection) -> None:
     """
-    Write string array to hdf5
+    Write string array to hdf5.
 
     Parameters
-    -------------
+    ----------
     f:
         h5py.Group where dataset should be created
     path:
         path of the dataset to create
     strings:
         list of strings to be written to f
     """
@@ -54,18 +53,18 @@
 
 
 def write_float_array(f: h5py.Group,
                       path: str,
                       values: Collection[Number],
                       dtype='f8') -> None:
     """
-    Write float array to hdf5
+    Write float array to hdf5.
 
     Parameters
-    -------------
+    ----------
     f:
         h5py.Group where dataset should be created
     path:
         path of the dataset to create
     values:
         array to write
     dtype:
@@ -79,18 +78,18 @@
 
 
 def write_int_array(f: h5py.Group,
                     path: str,
                     values: Collection[int],
                     dtype='<i4'):
     """
-    Write integer array to hdf5
+    Write integer array to hdf5.
 
     Parameters
-    -------------
+    ----------
     f:
         h5py.Group where dataset should be created
     path:
         path of the dataset to create
     values:
         array to write
     dtype:
```

### Comparing `pypesto-0.2.8/pypesto/store/read_from_hdf5.py` & `pypesto-0.2.9/pypesto/store/read_from_hdf5.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Include various function to read results from hdf5 Files."""
 import h5py
 from ..result import Result
 from ..optimize.result import OptimizerResult
 from ..optimize.optimizer import fill_result_from_objective_history
 from ..profile.result import ProfilerResult
 from ..sample.result import McmcPtResult
 from ..problem import Problem
@@ -17,25 +18,24 @@
 def read_hdf5_profile(f: h5py.File,
                       profile_id: str,
                       parameter_id: str) -> 'ProfilerResult':
     """
     Read HDF5 results per start.
 
     Parameters
-    -------------
+    ----------
     f:
         The HDF5 result file
     profile_id:
         specifies the profile start that is read
         from the HDF5 file
     parameter_id:
         specifies the profile index that is read
         from the HDF5 file
     """
-
     result = ProfilerResult(np.array([]), np.array([]), np.array([]))
 
     for profile_key in result.keys():
         if profile_key in f[f'/profiling/{profile_id}/{parameter_id}']:
             result[profile_key] = \
                 f[f'/profiling/{profile_id}/{parameter_id}/{profile_key}'][:]
         elif profile_key in \
@@ -48,23 +48,22 @@
 def read_hdf5_optimization(f: h5py.File,
                            file_name: str,
                            opt_id: str) -> 'OptimizerResult':
     """
     Read HDF5 results per start.
 
     Parameters
-    -------------
+    ----------
     f:
         The HDF5 result file
     file_name:
         The name of the HDF5 file, needed to create HDF5History
     opt_id:
         Specifies the start that is read from the HDF5 file
     """
-
     result = OptimizerResult()
 
     for optimization_key in result.keys():
         if optimization_key == 'history':
             if optimization_key in f:
                 result['history'] = Hdf5History(id=opt_id,
                                                 file=file_name)
@@ -78,46 +77,47 @@
             result[optimization_key] = \
                 f[f'/optimization/results/{opt_id}'].attrs[optimization_key]
     return result
 
 
 class ProblemHDF5Reader:
     """
-    Reader of the HDF5 problem files written
-    by class ProblemHDF5Writer.
+    Reader of the HDF5 problem files written by ProblemHDF5Writer.
 
     Attributes
-    -------------
+    ----------
     storage_filename:
         HDF5 problem file name
     """
+
     def __init__(self, storage_filename: str):
         """
+        Initialize reader.
+
         Parameters
         ----------
-
         storage_filename: str
             HDF5 problem file name
         """
         self.storage_filename = storage_filename
 
     def read(self, objective: ObjectiveBase = None) -> Problem:
         """
         Read HDF5 problem file and return pyPESTO problem object.
 
         Parameters
         ----------
         objective:
             Objective function which is currently not saved to storage.
+
         Returns
         -------
         problem:
             A problem instance with all attributes read in.
         """
-
         # create empty problem
         if objective is None:
             objective = Objective()
             # raise warning that objective is not loaded.
             logger.info('WARNING: You are loading a problem.\nThis problem'
                         ' is not to be used without a separately created'
                         ' objective.')
@@ -139,37 +139,36 @@
         problem.x_names = [name.decode() for name in problem.x_names]
 
         return problem
 
 
 class OptimizationResultHDF5Reader:
     """
-    Reader of the HDF5 result files written
-    by class OptimizationResultHDF5Writer.
+    Reader of the HDF5 result files written by OptimizationResultHDF5Writer.
 
     Attributes
-    -------------
+    ----------
     storage_filename:
         HDF5 result file name
     """
+
     def __init__(self, storage_filename: str):
         """
+        Initialize reader.
+
         Parameters
         ----------
-
         storage_filename: str
             HDF5 result file name
         """
         self.storage_filename = storage_filename
         self.results = Result()
 
     def read(self) -> Result:
-        """
-        Read HDF5 result file and return pyPESTO result object.
-        """
+        """Read HDF5 result file and return pyPESTO result object."""
         with h5py.File(self.storage_filename, "r") as f:
             if '/problem' in f['/']:
                 problem_reader = ProblemHDF5Reader(self.storage_filename)
                 self.results.problem = problem_reader.read()
 
             for opt_id in f['/optimization/results']:
                 result = read_hdf5_optimization(f,
@@ -178,37 +177,36 @@
                 self.results.optimize_result.append(result)
             self.results.optimize_result.sort()
         return self.results
 
 
 class SamplingResultHDF5Reader:
     """
-    Reader of the HDF5 result files written
-    by class SamplingResultHDF5Writer.
+    Reader of the HDF5 result files written by SamplingResultHDF5Writer.
 
     Attributes
-    -------------
+    ----------
     storage_filename:
         HDF5 result file name
     """
+
     def __init__(self, storage_filename: str):
         """
+        Initialize reader.
+
         Parameters
         ----------
-
         storage_filename: str
             HDF5 result file name
         """
         self.storage_filename = storage_filename
         self.results = Result()
 
     def read(self) -> Result:
-        """
-        Read HDF5 result file and return pyPESTO result object.
-        """
+        """Read HDF5 result file and return pyPESTO result object."""
         sample_result = {}
         with h5py.File(self.storage_filename, "r") as f:
             if '/problem' in f['/']:
                 problem_reader = ProblemHDF5Reader(self.storage_filename)
                 self.results.problem = problem_reader.read()
             for key in f['/sampling/results']:
                 sample_result[key] = \
@@ -223,37 +221,36 @@
                            "sampling result.")
 
         return self.results
 
 
 class ProfileResultHDF5Reader:
     """
-    Reader of the HDF5 result files written
-    by class OptimizationResultHDF5Writer.
+    Reader of the HDF5 result files written by OptimizationResultHDF5Writer.
 
     Attributes
-    -------------
+    ----------
     storage_filename:
         HDF5 result file name
     """
+
     def __init__(self, storage_filename: str):
         """
+        Initialize reader.
+
         Parameters
         ----------
-
-        storage_filename: str
+        storage_filename:
             HDF5 result file name
         """
         self.storage_filename = storage_filename
         self.results = Result()
 
     def read(self) -> Result:
-        """
-        Read HDF5 result file and return pyPESTO result object.
-        """
+        """Read HDF5 result file and return pyPESTO result object."""
         profiling_list = []
         with h5py.File(self.storage_filename, "r") as f:
             if '/problem' in f['/']:
                 problem_reader = ProblemHDF5Reader(self.storage_filename)
                 self.results.problem = problem_reader.read()
             for profile_id in f['/profiling']:
                 profiling_list.append([
@@ -274,16 +271,15 @@
 def read_result(filename: str,
                 problem: bool = True,
                 optimize: bool = False,
                 profile: bool = False,
                 sample: bool = False,
                 ) -> Result:
     """
-    This is a function that saves the whole pypesto.Result object in an
-    HDF5 file. With booleans one can choose more detailed what to save.
+    Save the whole pypesto.Result object in an HDF5 file.
 
     Parameters
     ----------
     filename:
         The HDF5 filename.
     problem:
         Read the problem.
@@ -340,47 +336,48 @@
                            f'within {filename}.')
 
     return result
 
 
 def load_objective_config(filename: str):
     """
-    Load the objective information stored in f
+    Load the objective information stored in f.
 
     Parameters
     ----------
     filename:
         The name of the file in which the information are stored.
 
-    Returns:
+    Returns
+    -------
         A dictionary of the information, stored instead of the
         actual objective in problem.objective.
     """
-
     with h5py.File(filename, 'r') as f:
         info_str = f['problem/config'][()].decode()
         info = ast.literal_eval(info_str)
         return info
 
 
-def optimization_result_from_history(filename: str):
+def optimization_result_from_history(filename: str) -> Result:
     """
-    Converts a saved hdf5 History to an optimization result.
+    Convert a saved hdf5 History to an optimization result.
+
     Used for interrupted optimization runs.
 
     Parameters
     ----------
     filename:
         The name of the file in which the information are stored.
 
-    Returns:
+    Returns
+    -------
         A result object in which the optimization result is constructed from
         history. But missing "Time, Message and Exitflag" keys.
     """
-
     result = Result()
     with h5py.File(filename, 'r') as f:
         for id_name in f['history'].keys():
             history = Hdf5History(id=id_name, file=filename)
             history._recover_options(filename)
             optimizer_history = OptimizerHistory(
                 history,
```

### Comparing `pypesto-0.2.8/pypesto/store/save_to_hdf5.py` & `pypesto-0.2.9/pypesto/store/save_to_hdf5.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Include functions for saving various results to hdf5."""
 import os
 import logging
 from typing import Union
 from numbers import Integral
 
 import h5py
 import numpy as np
@@ -12,19 +13,20 @@
 logger = logging.getLogger(__name__)
 
 
 def check_overwrite(f: Union[h5py.File, h5py.Group],
                     overwrite: bool,
                     target: str):
     """
-    Checks whether target already exists. Sends a warning if
-    overwrite=False, deletes the target if overwrite=True.
+    Check whether target already exists.
+
+    Sends a warning if overwrite=False, deletes the target if overwrite=True.
 
     Attributes
-    -------------
+    ----------
     f: file or group where existence of a group with the path group_path
        should be checked
     target: name of the group, whose existence is checked
     overwrite: if overwrite is true, it deltes the target in f
     """
     if target in f:
         if overwrite:
@@ -37,34 +39,32 @@
 
 
 class ProblemHDF5Writer:
     """
     Writer of the HDF5 problem files.
 
     Attributes
-    -------------
+    ----------
     storage_filename:
         HDF5 result file name
     """
 
     def __init__(self, storage_filename: str):
         """
+        Initialize writer.
+
         Parameters
         ----------
-
         storage_filename: str
             HDF5 problem file name
         """
         self.storage_filename = storage_filename
 
     def write(self, problem, overwrite: bool = False):
-        """
-        Write HDF5 problem file from pyPESTO problem object.
-        """
-
+        """Write HDF5 problem file from pyPESTO problem object."""
         # Create destination directory
         if isinstance(self.storage_filename, str):
             basedir = os.path.dirname(self.storage_filename)
             if basedir:
                 os.makedirs(basedir, exist_ok=True)
 
         with h5py.File(self.storage_filename, "a") as f:
@@ -86,60 +86,57 @@
                 elif isinstance(value, Integral):
                     problem_grp.attrs[problem_attr] = value
 
 
 def get_or_create_group(f: Union[h5py.File, h5py.Group],
                         group_path: str) -> h5py.Group:
     """
-    Helper function that returns a group object for the group with group_path
-    relative to f. Creates it if it doesn't exist.
+    Return/create a group object for the group with group_path relative to f.
 
     Attributes
-    -------------
+    ----------
     f: file or group where existence of a group with the path group_path
        should be checked
     group_path: the path or simply the name of the group that should exist in f
 
     Returns
     -------
     grp:
-        hdf5 group object with specified path.
+        hdf5 group object with specified path relative to f.
     """
     if group_path in f:
         grp = f[group_path]
     else:
         grp = f.create_group(group_path)
     return grp
 
 
 class OptimizationResultHDF5Writer:
     """
     Writer of the HDF5 result files.
 
     Attributes
-    -------------
+    ----------
     storage_filename:
         HDF5 result file name
     """
 
     def __init__(self, storage_filename: str):
         """
+        Initialize Writer.
+
         Parameters
         ----------
-
         storage_filename: str
             HDF5 result file name
         """
         self.storage_filename = storage_filename
 
     def write(self, result: Result, overwrite=False):
-        """
-        Write HDF5 result file from pyPESTO result object.
-        """
-
+        """Write HDF5 result file from pyPESTO result object."""
         # Create destination directory
         if isinstance(self.storage_filename, str):
             basedir = os.path.dirname(self.storage_filename)
             if basedir:
                 os.makedirs(basedir, exist_ok=True)
 
         with h5py.File(self.storage_filename, "a") as f:
@@ -163,33 +160,32 @@
 
 
 class SamplingResultHDF5Writer:
     """
     Writer of the HDF5 sampling files.
 
     Attributes
-    -------------
+    ----------
     storage_filename:
         HDF5 result file name
     """
 
     def __init__(self, storage_filename: str):
         """
+        Initialize Writer.
+
         Parameters
         ----------
-
         storage_filename: str
             HDF5 result file name
         """
         self.storage_filename = storage_filename
 
     def write(self, result: Result, overwrite: bool = False):
-        """
-        Write HDF5 sampling file from pyPESTO result object.
-        """
+        """Write HDF5 sampling file from pyPESTO result object."""
         # if there is no sample available, log a warning and return
         # SampleResult is only a dummy class created by the Result class
         # and always indicates the lack of a sampling result.
         if(isinstance(result.sample_result, SampleResult)):
             logger.warning("Warning: There is no sampling_result, "
                            "which you tried to save to hdf5.")
             return
@@ -216,34 +212,32 @@
 
 
 class ProfileResultHDF5Writer:
     """
     Writer of the HDF5 result files.
 
     Attributes
-    -------------
+    ----------
     storage_filename:
         HDF5 result file name
     """
 
     def __init__(self, storage_filename: str):
         """
+        Initialize Writer.
+
         Parameters
         ----------
-
         storage_filename: str
             HDF5 result file name
         """
         self.storage_filename = storage_filename
 
     def write(self, result: Result, overwrite: bool = False):
-        """
-        Write HDF5 result file from pyPESTO result object.
-        """
-
+        """Write HDF5 result file from pyPESTO result object."""
         # Create destination directory
         if isinstance(self.storage_filename, str):
             basedir = os.path.dirname(self.storage_filename)
             if basedir:
                 os.makedirs(basedir, exist_ok=True)
 
         with h5py.File(self.storage_filename, "a") as f:
@@ -271,19 +265,20 @@
             f.flush()
 
 
 def write_result(result: Result,
                  filename: str,
                  overwrite: bool = False,
                  problem: bool = True,
-                 optimize: bool = True,
-                 profile: bool = True,
-                 sample: bool = True,
+                 optimize: bool = False,
+                 profile: bool = False,
+                 sample: bool = False,
                  ):
-    """Save whole pypesto.Result to hdf5 file.
+    """
+    Save whole pypesto.Result to hdf5 file.
 
     Boolean indicators allow specifying what to save.
 
     Parameters
     ----------
     result:
         The :class:`pypesto.Result` object to be saved.
@@ -296,14 +291,18 @@
     optimize:
         Read the optimize result.
     profile:
         Read the profile result.
     sample:
         Read the sample result.
     """
+    if not any([optimize, profile, sample]):
+        optimize = True
+        profile = True
+        sample = True
 
     if problem:
         pypesto_problem_writer = ProblemHDF5Writer(filename)
         pypesto_problem_writer.write(result.problem, overwrite=overwrite)
 
     if optimize:
         pypesto_opt_writer = OptimizationResultHDF5Writer(filename)
```

### Comparing `pypesto-0.2.8/pypesto/visualize/__init__.py` & `pypesto-0.2.9/pypesto/visualize/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: D400,D205
 """
 Visualize
 =========
 
 pypesto comes with various visualization routines. To use these,
 import pypesto.visualize.
 """
```

### Comparing `pypesto-0.2.8/pypesto/visualize/clust_color.py` & `pypesto-0.2.9/pypesto/visualize/clust_color.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,25 @@
 
 def assign_clusters(vals):
     """
     Find clustering.
 
     Parameters
     ----------
-
     vals: numeric list or array
         List to be clustered.
 
     Returns
     -------
-
     clust: numeric list
-         Indicating the corresponding cluster of each element from
-         'vals'.
-
+        Indicating the corresponding cluster of each element from
+        'vals'.
     clustsize: numeric list
         Size of clusters, length equals number of clusters.
     """
-
     # sanity checks
     if vals is None or len(vals) == 0:
         return [], []
     elif len(vals) == 1:
         return np.array([0]), np.array([1.])
 
     # linkage requires (n, 1) data array
@@ -61,32 +57,27 @@
 
 def assign_clustered_colors(vals, balance_alpha=True, highlight_global=True):
     """
     Cluster and assign colors.
 
     Parameters
     ----------
-
     vals: numeric list or array
         List to be clustered and assigned colors.
-
     balance_alpha: bool (optional)
         Flag indicating whether alpha for large clusters should be reduced to
         avoid overplotting (default: True)
-
     highlight_global: bool (optional)
         flag indicating whether global optimum should be highlighted
 
     Returns
     -------
-
     colors: list of RGBA
         One for each element in 'vals'.
     """
-
     # sanity checks
     if vals is None or len(vals) == 0:
         return []
 
     # assign clusters
     clusters, cluster_size = assign_clusters(vals)
 
@@ -146,15 +137,14 @@
 def assign_colors(vals, colors=None, balance_alpha=True,
                   highlight_global=True):
     """
     Assign colors or format user specified colors.
 
     Parameters
     ----------
-
     vals: numeric list or array
         List to be clustered and assigned colors.
 
     colors: list, or RGBA, optional
         list of colors, or single color
 
     balance_alpha: bool (optional)
@@ -162,19 +152,17 @@
         avoid overplotting (default: True)
 
     highlight_global: bool (optional)
         flag indicating whether global optimum should be highlighted
 
     Returns
     -------
-
     colors: list of RGBA
         One for each element in 'vals'.
     """
-
     # sanity checks
     if vals is None or len(vals) == 0:
         return np.array([])
 
     # if the user did not specify any colors:
     if colors is None:
         return assign_clustered_colors(vals, balance_alpha=balance_alpha,
@@ -213,33 +201,31 @@
 
 
 def assign_colors_for_list(
         num_entries: int,
         colors: Optional[Union[RGBA, List[RGBA], np.ndarray]] = None
 ) -> Union[List[List[float]], np.ndarray]:
     """
-    Creates a list of colors for a list of items or checks
-    a user-provided list of colors and uses this if everything is ok
+    Create a list of colors for a list of items.
+
+    Can also check a user-provided list of colors and use this if
+    everything is ok.
 
     Parameters
     ----------
-
     num_entries:
         number of results in list
-
     colors:
         list of colors, or single color
 
     Returns
     -------
-
     colors:
         List of RGBA, one for each element in 'vals'.
     """
-
     # if the user did not specify any colors:
     if colors is None:
         # default colors will be used, on for each entry in the result list.
         # Colors are created from assign_colors, which needs a dummy list
         dummy_clusters = np.array(list(range(num_entries)) * 2)
 
         # we don't want alpha levels for all plotting routines in this case...
@@ -260,35 +246,31 @@
     return colors
 
 
 def delete_nan_inf(fvals: np.ndarray,
                    x: Optional[np.ndarray] = None,
                    xdim: Optional[int] = 1) -> Tuple[np.ndarray, np.ndarray]:
     """
-    Delete nan and inf values in fvals. If parameters 'x' are passed, also
-    the corresponding entries are deleted.
+    Delete nan and inf values in fvals.
+
+    If parameters 'x' are passed, also the corresponding entries are deleted.
 
     Parameters
     ----------
-
     x:
         array of parameters
-
     fvals:
         array of fval
-
     xdim:
         dimension of x, in case x dimension cannot be inferred
 
     Returns
     -------
-
     x:
         array of parameters without nan or inf
-
     fvals:
         array of fval without nan or inf
     """
     fvals = np.asarray(fvals)
     if x is not None:
         # if we start out with a list of x, the x corresponding to
         # to finite fvals may be None, so we cannot stack the x before taking
```

### Comparing `pypesto-0.2.8/pypesto/visualize/constants.py` & `pypesto-0.2.9/pypesto/visualize/constants.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.2.8/pypesto/visualize/dimension_reduction.py` & `pypesto-0.2.9/pypesto/visualize/dimension_reduction.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,16 +12,18 @@
     UmapTypeObject = None
 
 
 def projection_scatter_umap(umap_coordinates: np.ndarray,
                             components: Sequence[int] = (0, 1),
                             **kwargs):
     """
-    Plot a scatter plots for UMAP coordinates. Creates either one or multiple
-    scatter plots, depending on the number of coordinates passed to it.
+    Plot a scatter plots for UMAP coordinates.
+
+    Creates either one or multiple scatter plots, depending on the number of
+    coordinates passed to it.
 
     Parameters
     ----------
     umap_coordinates:
         array of umap coordinates (returned as first output by the routine
         get_umap_representation) to be shown as scatter plot
 
@@ -60,55 +62,55 @@
 
 
 def projection_scatter_umap_original(umap_object: UmapTypeObject,
                                      color_by: Sequence[float] = None,
                                      components: Sequence[int] = (0, 1),
                                      **kwargs):
     """
-    Wrapper around umap.plot.points. Similar to projection_scatter_umap, but
+    See `projection_scatter_umap` for more documentation.
+
+    Wrapper around umap.plot.points. Similar to `projection_scatter_umap`, but
     uses the original plotting routine from umap.plot.
 
     Parameters
     ----------
     umap_object:
         umap object (returned as second output by get_umap_representation)
         to be shown as scatter plot
-
     color_by:
         A sequence/list of floats, which specify the color in the colormap
-
     components:
         Components to be plotted (corresponds to columns of umap_coordinates)
 
     Returns
     -------
     ax: matplotlib.Axes
         The plot axes.
     """
-
     # reduce, if necessary
     umap_object.embedding_ = umap_object.embedding_[:, components]
 
     # use umap's original plotting routine to visualize
     umap.plot.points(umap_object, values=color_by, theme='viridis', **kwargs)
 
 
 def projection_scatter_pca(pca_coordinates: np.ndarray,
                            components: Sequence[int] = (0, 1),
                            **kwargs):
     """
-    Plot a scatter plots for PCA coordinates. Creates either one or multiple
-    scatter plots, depending on the number of coordinates passed to it.
+    Plot a scatter plot for PCA coordinates.
+
+    Creates either one or multiple scatter plots, depending on the number of
+    coordinates passed to it.
 
     Parameters
     ----------
     pca_coordinates:
         array of pca coordinates (returned as first output by the routine
         get_pca_representation) to be shown as scatter plot
-
     components:
         Components to be plotted (corresponds to columns of pca_coordinates)
 
     Returns
     -------
     axs:
         Either one axes object, or a dictionary of plot axes (depending on the
@@ -141,31 +143,30 @@
 
 
 def ensemble_crosstab_scatter_lowlevel(dataset: np.ndarray,
                                        component_labels: Sequence[str] = None,
                                        **kwargs):
     """
     Plot cross-classification table of scatter plots for different coordinates.
+
     Lowlevel routine for multiple UMAP and PCA plots, but can also be used to
-    visualize, e.g., parameter traces across optimizer runs
+    visualize, e.g., parameter traces across optimizer runs.
 
     Parameters
     ----------
     dataset:
         array of data points to be shown as scatter plot
-
     component_labels:
         labels for the x-axes and the y-axes
 
     Returns
     -------
     axs:
         A dictionary of plot axes.
     """
-
     # We got more than two components. Create a cross-classification table
     n_components = dataset.shape[1]
     axs = _create_crosstab_axes(n_components)
 
     # wo don't even try to plot this into an existing axes object.
     # Overplotting a multi-axes figure is asking for trouble...
     if 'ax' in kwargs.keys():
@@ -202,59 +203,48 @@
                               color_by: Sequence[float] = None,
                               color_map: str = 'viridis',
                               background_color: RGBA = (0., 0., 0., 1.),
                               marker_type: str = '.',
                               scatter_size: float = 0.5,
                               invert_scatter_order: bool = False):
     """
-    Create a scatter plot
+    Create a scatter plot.
 
     Parameters
     ----------
     dataset:
         array of data points in reduced dimension
-
     ax:
         Axes object to use.
-
     size:
         Figure size (width, height) in inches. Is only applied when no ax
         object is specified
-
     x_label:
         The x-axis label
-
     y_label:
         The y-axis label
-
     color_by:
         A sequence/list of floats, which specify the color in the colormap
-
     color_map:
         A colormap name known to pyplot
-
     background_color:
         Background color of the axes object (defaults to black)
-
     marker_type:
         Type of plotted markers
-
     scatter_size:
         Size of plotted markers
-
     invert_scatter_order:
         Specifies the order of plotting the scatter points, can be important
         in case of overplotting
 
     Returns
     -------
     ax: matplotlib.Axes
         The plot axes.
     """
-
     # first get the data to check identifiability
     # axes
     if ax is None:
         fig, ax = plt.subplots()
         fig.set_size_inches(*size)
     plt.sca(ax)
 
@@ -278,15 +268,15 @@
     plt.tight_layout()
 
     return ax
 
 
 def _create_crosstab_axes(n_comp: int):
     """
-    Create a figure with cross-classification table of axes
+    Create a figure with cross-classification table of axes.
 
     Parameters
     ----------
     n_comp:
         number of component to be mutually compared
 
     Returns
```

### Comparing `pypesto-0.2.8/pypesto/visualize/ensemble.py` & `pypesto-0.2.9/pypesto/visualize/ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,39 +11,36 @@
     COLOR_HIT_BOTH_BOUNDS, COLOR_HIT_ONE_BOUND, COLOR_HIT_NO_BOUNDS)
 
 
 def ensemble_identifiability(ensemble: Ensemble,
                              ax: Optional[plt.Axes] = None,
                              size: Optional[Tuple[float]] = (12, 6)):
     """
-    Plots an overview about how many parameters hit the parameter bounds based
+    Visualize identifiablity of parameter ensemble.
+
+    Plot an overview about how many parameters hit the parameter bounds based
     on a ensemble of parameters. confidence intervals/credible ranges are
     computed via the ensemble mean plus/minus 1 standard deviation.
     This highlevel routine expects a ensemble object as input.
 
     Parameters
     ----------
-
     ensemble:
         ensemble of parameter vectors (from pypesto.ensemble)
-
     ax:
         Axes object to use.
-
     size:
         Figure size (width, height) in inches. Is only applied when no ax
         object is specified
 
     Returns
     -------
-
     ax: matplotlib.Axes
         The plot axes.
     """
-
     # first get the data to check identifiability
     id_df = ensemble.check_identifiability()
 
     # check how many bounds are actually hit and which ones
     none_hit, lb_hit, ub_hit, both_hit = _prepare_identifiability_plot(id_df)
 
     # call lowlevel routine whick works with np arrays only
@@ -56,53 +53,47 @@
 def ensemble_identifiability_lowlevel(none_hit: np.ndarray,
                                       lb_hit: np.ndarray,
                                       ub_hit: np.ndarray,
                                       both_hit: np.ndarray,
                                       ax: Optional[plt.Axes] = None,
                                       size: Optional[Tuple[float]] = (16, 10)):
     """
-    Plots an overview about how many parameters hit the parameter bounds based
+    Low-level identifiablity routine.
+
+    Plot an overview about how many parameters hit the parameter bounds based
     on a ensemble of parameters. Confidence intervals/credible ranges are
     computed via the ensemble mean plus/minus 1 standard deviation.
     This lowlevel routine works with numpy arrays which define the confidence
     intervals/credible ranges of each parameter.
 
     Parameters
     ----------
-
     none_hit:
         2-dimensional array of confidence interval/credible ranges for
         identifiable parameters
-
     lb_hit:
         2-dimensional array of confidence interval/credible ranges for
         parameters which hit the lower parameter bound
-
     ub_hit:
         2-dimensional array of confidence interval/credible ranges for
         parameters which hit the upper parameter bound
-
     both_hit:
         2-dimensional array of confidence interval/credible ranges for
         parameters which hit both parameter bounds
-
     ax:
         Axes object to use.
-
     size:
         Figure size (width, height) in inches. Is only applied when no ax
         object is specified
 
     Returns
     -------
-
     ax: matplotlib.Axes
         The plot axes.
     """
-
     # define some short hands for later plotting
     n_par = sum([none_hit.shape[0], lb_hit.shape[0],
                  ub_hit.shape[0], both_hit.shape[0]])
     x_both = len(both_hit) / n_par
     x_lb = len(lb_hit) / n_par
     x_ub = len(ub_hit) / n_par
     x_none = 1. - x_both - x_ub - x_lb
@@ -171,20 +162,21 @@
     ax.spines['top'].set_visible(False)
 
     return ax
 
 
 def _prepare_identifiability_plot(id_df: pd.DataFrame):
     """
-    This routine groups model parameters based on a ensemble object into
-    four categories, based on the mean of the parameter ensemble plus/minus
-    1 standard deviation: Parameters that hit both bounds, parameters that hit
-    only the lower [or upper] bound, and parameters that hit no bounds.
-    It returns them as four numpy arrays, together with their confidence
-    intervals/credible ranges.
+    Group model parameters based on an ensemble object .
+
+    Can group into four categories, based on the mean of the parameter
+    ensemble plus/minus 1 standard deviation: Parameters that hit both
+    bounds, parameters that hit only the lower [or upper] bound,
+    and parameters that hit no bounds. It returns them as four numpy arrays,
+    together with their confidence intervals/credible ranges.
 
     Parameters
     ----------
     id_df:
         Pandas dataframe with information about parameter identifiability,
         as created by pypesto.ensemble.check_identifiability()
 
@@ -202,15 +194,14 @@
         2-dimensional array of confidence interval/credible ranges for
         parameters which hit the upper parameter bound
 
     both_hit:
         2-dimensional array of confidence interval/credible ranges for
         parameters which hit both parameter bounds
     """
-
     # prepare
     both_hit = []
     lb_hit = []
     ub_hit = []
     none_hit = []
 
     def _affine_transform(par_info):
@@ -248,15 +239,17 @@
 
 
 def _create_patches(none_hit: np.ndarray,
                     lb_hit: np.ndarray,
                     ub_hit: np.ndarray,
                     both_hit: np.ndarray):
     """
-    Creates matplotlib.patches.PatchCollection objects from numpy arrays with
+    Create patches for identifiability analysis.
+
+    Create matplotlib.patches.PatchCollection objects from numpy arrays with
     confidence intervals/credible ranges, which visualize identifiability
     properties of the model parameters.
 
     Parameters
     ----------
     none_hit:
         2-dimensional array of confidence interval/credible ranges for
```

### Comparing `pypesto-0.2.8/pypesto/visualize/misc.py` & `pypesto-0.2.9/pypesto/visualize/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,41 +16,34 @@
     RGBA_ALPHA,
     RGBA_WHITE,
 )
 
 
 def process_result_list(results, colors=None, legends=None):
     """
-    assigns colors and legends to a list of results, check user provided lists
+    Assign colors and legends to a list of results, check user provided lists.
 
     Parameters
     ----------
-
     results: list or pypesto.Result
         list of pypesto.Result objects or a single pypesto.Result
-
     colors: list, optional
         list of RGBA colors
-
     legends: str or list
         labels for line plots
 
     Returns
     -------
-
     results: list of pypesto.Result
        list of pypesto.Result objects
-
     colors: list of RGBA
         One for each element in 'results'.
-
     legends: list of str
         labels for line plots
     """
-
     # check how many results were passed
     single_result = False
     legend_error = False
     if isinstance(results, list):
         if len(results) == 1:
             single_result = True
     else:
@@ -93,38 +86,33 @@
     return results, colors, legends
 
 
 def process_offset_y(offset_y: Optional[float],
                      scale_y: str,
                      min_val: float) -> float:
     """
-    compute offset for y-axis, depend on user settings
+    Compute offset for y-axis, depend on user settings.
 
     Parameters
     ----------
-
     offset_y:
        value for offsetting the later plotted values, in order to ensure
        positivity if a semilog-plot is used
-
     scale_y:
        Can be 'lin' or 'log10', specifying whether values should be plotted
        on linear or on log10-scale
-
     min_val:
         Smallest value to be plotted
 
     Returns
     -------
-
     offset_y: float
        value for offsetting the later plotted values, in order to ensure
        positivity if a semilog-plot is used
     """
-
     # check whether the offset specified by the user is sufficient
     if offset_y is not None:
         if (scale_y == 'log10') and (min_val + offset_y <= 0.):
             warnings.warn("Offset specified by user is insufficient. "
                           "Ignoring specified offset and using " +
                           str(np.abs(min_val) + 1.) + " instead.")
         else:
@@ -136,32 +124,28 @@
             return 0.
 
     return 1. - min_val
 
 
 def process_y_limits(ax, y_limits):
     """
-    apply user specified limits of y-axis
+    Apply user specified limits of y-axis.
 
     Parameters
     ----------
-
     ax: matplotlib.Axes, optional
         Axes object to use.
-
     y_limits: ndarray
        y_limits, minimum and maximum, for current axes object
 
     Returns
     -------
-
     ax: matplotlib.Axes, optional
         Axes object to use.
     """
-
     # apply y-limits, if they were specified by the user
     if y_limits is not None:
         y_limits = np.array(y_limits)
 
         # check validity of bounds
         if y_limits.size == 0:
             y_limits = np.array(ax.get_ylim())
@@ -210,27 +194,27 @@
 
     return ax
 
 
 def process_start_indices(start_indices: Union[int, Iterable[int]],
                           max_length: int) -> List[int]:
     """
-    helper function that processes the start_indices and
-    creates an array of indices if a number was provided and checks that the
-    indices do not exceed the max_index
+    Process the start_indices.
+
+    Create an array of indices if a number was provided and checks that the
+    indices do not exceed the max_index.
 
     Parameters
     ----------
     start_indices:
         list of indices or int specifying an endpoint of the sequence of
         indices
     max_length:
         maximum possible index for the start_indices
     """
-
     if isinstance(start_indices, Number):
         start_indices = range(int(start_indices))
 
     start_indices = np.array(start_indices, dtype=int)
 
     # check, whether index set is not too big
     start_indices = [start_index for start_index in start_indices if
@@ -277,16 +261,15 @@
     def apparent_composite_color_component(
             fg_component: float,
             bg_component: float,
             fg_alpha: float = fg[RGBA_ALPHA],
             bg_alpha: float = bg[RGBA_ALPHA],
     ) -> float:
         """
-        Composite a foreground color component over a background color
-        component.
+        Composite a foreground over a background color component.
 
         Porter and Duff equations are used for alpha compositing.
 
         Parameters
         ----------
         fg_component:
             The foreground color component.
```

### Comparing `pypesto-0.2.8/pypesto/visualize/model_fit.py` & `pypesto-0.2.9/pypesto/visualize/model_fit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Visualization of the model fit after optimization.
 
 Currently only for PEtab problems.
 """
+import matplotlib.axes
 import numpy as np
 import matplotlib.pyplot as plt
 import amici.petab_import as petab_import
 import petab
 import amici.plotting
 from ..problem import Problem
 from amici.petab_simulate import simulate_petab
@@ -16,43 +17,47 @@
 from amici.petab_objective import rdatas_to_simulation_df
 
 AmiciModel = Union['amici.Model', 'amici.ModelPtr']
 
 
 def visualize_optimized_model_fit(petab_problem: petab.Problem,
                                   result: Union[Result, Sequence[Result]],
+                                  start_index: int = 0,
                                   **kwargs
-                                  ):
+                                  ) -> Union[matplotlib.axes.Axes, None]:
     """
     Visualize the optimized model fit of a PEtab problem.
+
     Function calls the PEtab visualization file of the petab_problem and
     visualizes the fit of the optimized parameter. Common additional
     argument is `subplot_dir` to specify the directory each subplot is
     saved to. Further keyword arguments are delegated to
     petab.visualize.plot_with_vis_spec, see there for more information.
 
     Parameters
     ----------
     petab_problem:
         The :py:class:`petab.Problem` that was optimized.
     result:
         The result object from optimization.
+    start_index:
+        The index of the optimization run in `result.optimize_result.list`.
 
     Returns
     -------
-    ax: Axis object of the created plot.
+    axes: `matplotlib.axes.Axes` object of the created plot.
     None: In case subplots are saved to file
     """
     if petab_problem is not None:
         if petab is None:
             raise
 
     problem_parameters = \
         dict(zip(petab_problem.parameter_df.index,
-                 result.optimize_result.list[0]['x']))
+                 result.optimize_result.list[start_index]['x']))
 
     amici_model = petab_import.import_petab_problem(
         petab_problem,
         model_output_dir=kwargs.pop('model_output_dir', None),
         force_compile=kwargs.pop('force_compile', False))
 
     res = simulate_petab(petab_problem, amici_model=amici_model,
@@ -61,33 +66,35 @@
                          solver=kwargs.pop('amici_solver', None))
 
     sim_df = rdatas_to_simulation_df(res["rdatas"],
                                      amici_model,
                                      petab_problem.measurement_df)
 
     # function to call, to plot data and simulations
-    ax = plot_problem(petab_problem=petab_problem,
-                      simulations_df=sim_df,
-                      **kwargs
-                      )
-    return ax
+    axes = plot_problem(petab_problem=petab_problem,
+                        simulations_df=sim_df,
+                        **kwargs
+                        )
+    return axes
 
 
 def time_trajectory_model(
         result: Union[Result, Sequence[Result]],
         problem: Problem = None,
         # TODO: conditions: Union[str, Sequence[str]] = None,
         timepoints: Union[np.ndarray, Sequence[np.ndarray]] = None,
         n_timepoints: int = 1000,
         start_index: int = 0,
         state_ids: Union[str, Sequence[str]] = None,
         state_names: Union[str, Sequence[str]] = None,
-        observable_ids: Union[str, Sequence[str]] = None,):
+        observable_ids: Union[str, Sequence[str]] = None,
+) -> Union[matplotlib.axes.Axes, None]:
     """
     Visualize the time trajectory of the model with given timepoints.
+
     It does this by calling the amici plotting routines.
 
     Parameters
     ----------
     result:
         The result object from optimization.
     problem:
@@ -105,17 +112,17 @@
     state_names:
         Names of the states to be plotted.
     observable_ids:
         Ids of the observables to be plotted.
 
     Returns
     -------
-    axes: `matplotlib.axes.Axes` object of the plot.
+    axes:
+        `matplotlib.axes.Axes` object of the plot.
     """
-
     if problem is None:
         problem = result.problem
     # add timepoints as needed
     if timepoints is None:
         end_time = max(problem.objective.edatas[0].getTimepoints())
         timepoints = np.linspace(start=0,
                                  stop=end_time,
@@ -151,16 +158,17 @@
 def _time_trajectory_model_with_states(
         model: AmiciModel,
         rdatas: Union['amici.ReturnData', Sequence['amici.ReturnData']],
         state_ids: Sequence[str],
         state_names: Sequence[str],
         observable_ids: Union[str, Sequence[str]]):
     """
-    Helper function for time_trajectory_model. Visualizes both states and
-    observables.
+    Visualizes both, states and observables.
+
+    Helper function for time_trajectory_model.
 
     Parameters
     ----------
     model:
         The amici.Model from the model of interest. Used to annotate the plot.
     rdatas:
         The data to be plotted. Each entry in the Sequence corresponds to a
@@ -170,15 +178,16 @@
     state_names:
         Names of the states to be plotted.
     observable_ids:
         Ids of the observable Ids to be plotted.
 
     Returns
     -------
-    axes: `matplotlib.axes.Axes` object of the plot.
+    axes:
+        `matplotlib.axes.Axes` object of the plot.
     """
     # if state_name, state_id or observable_id is not None, get indices
     # for these the AMICI plotting functions default to all indices if
     # `None` is specified.
     state_indices_by_id = []
     state_indices_by_name = []
     if state_ids is not None:
@@ -218,30 +227,32 @@
 
 
 def _time_trajectory_model_without_states(
         model: AmiciModel,
         rdatas: Union['amici.ReturnData', Sequence['amici.ReturnData']],
         observable_ids: Union[str, Sequence[str]]):
     """
-    Helper function for time_trajectory_model. Visualizes both states and
-    observables.
+    Visualize both, states and observables.
+
+    Helper function for time_trajectory_model.
 
     Parameters
     ----------
     model:
         The amici.Model from the model of interest. Used to annotate the plot.
     rdatas:
         The data to be plotted. Each entry in the Sequence corresponds to a
         condition.
     observable_ids:
         Ids of the observables to be plotted.
 
     Returns
     -------
-    axes: `matplotlib.axes.Axes` object of the plot.
+    axes:
+        `matplotlib.axes.Axes` object of the plot.
     """
     # if observable_id's is not None, get indices for these
     # the AMICI plotting functions default to all indices if `None` is
     # specified.
     observable_indices = None
     if observable_ids is not None:
         observable_indices = [
```

### Comparing `pypesto-0.2.8/pypesto/visualize/optimization_stats.py` & `pypesto-0.2.9/pypesto/visualize/optimization_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,15 @@
     size: Tuple[float, float] = (18.5, 10.5),
     start_indices: Optional[Union[int, Iterable[int]]] = None,
     colors: Optional[Union[List[float], List[List[float]]]] = None,
     legends: Optional[Union[str, List[str]]] = None,
     plot_type: str = 'line'
 ) -> matplotlib.axes.Axes:
     """
-    Plot stats for all optimization properties specified  in properties_to_plot
-    on one plot.
+    Plot stats for allproperties specified in properties_to_plot on one plot.
 
     Parameters
     ----------
     results:
         Optimization result obtained by 'optimize.py' or list of those
     properties_to_plot:
         Optimization run properties that should be plotted
@@ -42,17 +41,19 @@
     legends:
         Labels, one label per optimization property
     plot_type:
         Specifies plot type. Possible values: 'line' and 'hist'
 
     Returns
     -------
+    ax:
+        The plot axes.
 
     Examples
-    -------
+    --------
     optimization_properties_per_multistart(
         result1,
         properties_to_plot=['time'],
         colors=[.5, .9, .9, .3])
 
     optimization_properties_per_multistart(
         result1,
@@ -129,17 +130,16 @@
         Specifies plot type. Possible values: 'line' and 'hist'
 
     Returns
     -------
     ax:
     The plot axes.
 
-
     Examples
-    -------
+    --------
     optimization_properties_per_multistart(
         result1,
         properties_to_plot=['time'],
         colors=[.5, .9, .9, .3])
 
     optimization_properties_per_multistart(
         [result1, result2],
@@ -151,15 +151,14 @@
         properties_to_plot=['time', 'n_grad'],
         colors=[.5, .9, .9, .3])
 
     optimization_properties_per_multistart(
         [result1, result2], properties_to_plot=['time', 'n_fval'],
         colors=[[.5, .9, .9, .3], [.2, .1, .9, .5]])
     """
-
     if properties_to_plot is None:
         properties_to_plot = ['time', 'n_fval', 'n_grad', 'n_hess', 'n_res',
                               'n_sres']
 
     num_subplot = len(properties_to_plot)
     # compute, how many rows and columns we need for the subplots
     num_row = int(np.round(np.sqrt(num_subplot)))
@@ -185,14 +184,15 @@
         size: Tuple[float, float] = (18.5, 10.5),
         start_indices: Optional[Union[int, Iterable[int]]] = None,
         colors: Optional[Union[List[float], List[List[float]]]] = None,
         legends: Optional[Union[str, List[str]]] = None,
         plot_type: str = 'line') -> matplotlib.axes.Axes:
     """
     Plot stats for an optimization run property specified by opt_run_property.
+
     It is possible to plot a histogram or a line plot. In a line plot,
     on the x axis are the numbers of the multistarts, where the multistarts are
     ordered with respect to a function value. On the y axis of the line plot
     the value of the corresponding parameter for each multistart is displayed.
 
     Parameters
     ----------
@@ -219,15 +219,14 @@
         Specifies plot type. Possible values: 'line', 'hist', 'both'
 
     Returns
     -------
     ax:
         The plot axes.
     """
-
     supported_properties = {
         'time': 'Wall-clock time (seconds)',
         'n_fval': 'Number of function evaluations',
         'n_grad': 'Number of gradient evaluations',
         'n_hess': 'Number of Hessian evaluations',
         'n_res': 'Number of residuals evaluations',
         'n_sres': 'Number of residual sensitivity evaluations'
@@ -285,20 +284,18 @@
                    axis_label: str,
                    ax: matplotlib.axes.Axes,
                    start_indices: Optional[Union[int, Iterable[int]]] = None,
                    color: Union[str, List[float], List[List[float]]] = 'C0',
                    legend: Optional[str] = None,
                    plot_type: str = 'line'):
     """
-    Plot values of the optimization run property specified by property name
-    across different multistarts
+    Plot values of the optimization run property across different multistarts.
 
     Parameters
     ----------
-
     result:
         Optimization result obtained by 'optimize.py'
     property_name:
         name of the optimization result property which value should be plotted
     axis_label:
         Label for the y axis of the line plot or x axis of the histogram
     ax:
@@ -317,15 +314,14 @@
         Specifies plot type. Possible values: 'line' and 'hist'
 
     Returns
     -------
     ax:
         The plot axes.
     """
-
     fvals = result.optimize_result.get_for_key('fval')
     values = result.optimize_result.get_for_key(property_name)
     values, fvals = delete_nan_inf(fvals, values)
 
     if start_indices is not None:
         start_indices = process_start_indices(start_indices, len(values))
         values = values[start_indices]
```

### Comparing `pypesto-0.2.8/pypesto/visualize/optimizer_convergence.py` & `pypesto-0.2.9/pypesto/visualize/optimizer_convergence.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 
 def optimizer_convergence(result: pypesto.Result,
                           ax: Optional[plt.Axes] = None,
                           xscale: str = 'symlog',
                           yscale: str = 'log',
                           size: Tuple[float] = (18.5, 10.5)) -> plt.Axes:
     """
+    Visualize to help spotting convergence issues.
+
     Scatter plot of function values and gradient values at the end of
     optimization. Optimizer exit-message is encoded by color. Can help
     identifying convergence issues in optimization and guide tolerance
     refinement etc.
 
     Parameters
     ----------
-
     result:
         Optimization result obtained by 'optimize.py'
 
     ax:
         Axes object to use.
 
     size:
@@ -35,15 +36,14 @@
         Scale for x-axis
 
     yscale:
         Scale for y-axis
 
     Returns
     -------
-
     ax: matplotlib.Axes
         The plot axes.
     """
     if ax is None:
         ax = plt.subplots(figsize=size)[1]
 
     fvals = result.optimize_result.get_for_key('fval')
```

### Comparing `pypesto-0.2.8/pypesto/visualize/optimizer_history.py` & `pypesto-0.2.9/pypesto/visualize/optimizer_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,70 +22,58 @@
                       offset_y=None,
                       colors=None,
                       y_limits=None,
                       start_indices=None,
                       reference=None,
                       legends=None):
     """
-    Plot history of optimizer. Can plot either the history of the cost
-    function or of the gradient norm, over either the optimizer steps or
-    the computation time.
+    Plot history of optimizer.
+
+    Can plot either the history of the cost function or of the gradient
+    norm, over either the optimizer steps or the computation time.
 
     Parameters
     ----------
-
     results: pypesto.Result or list
         Optimization result obtained by 'optimize.py' or list of those
-
     ax: matplotlib.Axes, optional
         Axes object to use.
-
     size: tuple, optional
         Figure size (width, height) in inches. Is only applied when no ax
         object is specified
-
     trace_x: str, optional
         What should be plotted on the x-axis?
         Possibilities: 'time', 'steps'
         Default: 'steps'
-
     trace_y: str, optional
         What should be plotted on the y-axis?
         Possibilities: 'fval', 'gradnorm', 'stepsize'
         Default: 'fval'
-
     scale_y: str, optional
         May be logarithmic or linear ('log10' or 'lin')
-
     offset_y: float, optional
         Offset for the y-axis-values, as these are plotted on a log10-scale
         Will be computed automatically if necessary
-
     colors: list, or RGBA, optional
         list of colors, or single color
         color or list of colors for plotting. If not set, clustering is done
         and colors are assigned automatically
-
     y_limits: float or ndarray, optional
         maximum value to be plotted on the y-axis, or y-limits
-
     start_indices: list or int
         list of integers specifying the multistart to be plotted or
         int specifying up to which start index should be plotted
-
     reference: list, optional
         List of reference points for optimization results, containing et
         least a function value fval
-
     legends: list or str
         Labels for line plots, one label per result object
 
     Returns
     -------
-
     ax: matplotlib.Axes
         The plot axes.
     """
     if isinstance(start_indices, int):
         start_indices = list(range(start_indices))
 
     # parse input
@@ -119,48 +107,38 @@
                                size=(18.5, 10.5), x_label='Optimizer steps',
                                y_label='Objective value', legend_text=None):
     """
     Plot optimizer history using list of numpy arrays.
 
     Parameters
     ----------
-
     vals: list of numpy arrays
         list of 2xn-arrays (x_values and y_values of the trace)
-
     scale_y: str, optional
         May be logarithmic or linear ('log10' or 'lin')
-
     colors: list, or RGBA, optional
         list of colors, or single color
         color or list of colors for plotting. If not set, clustering is done
         and colors are assigned automatically
-
     ax: matplotlib.Axes, optional
         Axes object to use.
-
     size: tuple, optional
         see waterfall
-
     x_label: str
         label for x-axis
-
     y_label: str
         label for y-axis
-
     legend_text: str
         Label for line plots
 
     Returns
     -------
-
     ax: matplotlib.Axes
         The plot axes.
     """
-
     # axes
     if ax is None:
         ax = plt.subplots()[1]
         fig = plt.gcf()
         fig.set_size_inches(*size)
 
     # parse input
@@ -216,45 +194,38 @@
     return ax
 
 
 def get_trace(result: Result,
               trace_x: Optional[str],
               trace_y: Optional[str]) -> Tuple[str, str, List[np.ndarray]]:
     """
-    Get the values of the optimizer trace from the pypesto.Result object
+    Get the values of the optimizer trace from the pypesto.Result object.
 
     Parameters
     ----------
-
     result: pypesto.Result
         Optimization result obtained by 'optimize.py'.
-
     trace_x: str, optional
         What should be plotted on the x-axis?
         Possibilities: 'time', 'steps'
         Default: 'steps'
-
     trace_y: str, optional
         What should be plotted on the y-axis?
         Possibilities: 'fval'(later also: 'gradnorm', 'stepsize')
         Default: 'fval'
 
     Returns
     -------
-
     vals:
-        list of
-
+        list of (x,y)-values.
     x_label:
-        label for x-axis to be plotted later
-
+        label for x-axis to be plotted later.
     y_label:
-        label for y-axis to be plotted later
+        label for y-axis to be plotted later.
     """
-
     # get data frames
     histories: List[History] = result.optimize_result.get_for_key('history')
 
     vals = []
     x_label = ''
     y_label = ''
 
@@ -305,48 +276,41 @@
     vals: List[np.ndarray],
     scale_y: Optional[str],
     offset_y: float,
     y_label: str,
     start_indices: Iterable[int]
 ) -> Tuple[List[np.ndarray], float, str]:
     """
-    Postprocesses the values of the optimization history, depending on the
-    options set by the user (e.g. scale_y, offset_y, start_indices)
+    Postprocess the values of the optimization history.
+
+    Depending on the options set by the user (e.g. scale_y, offset_y,
+    start_indices).
 
     Parameters
     ----------
-
     vals: list
         list of numpy arrays of dimension 2 x len(start_indices)
-
     scale_y: str, optional
         May be logarithmic or linear ('log10' or 'lin')
-
     offset_y: float
         offset for the y-axis, as this is supposed to be in log10-scale
-
     y_label: str
         Label for y axis
-
     start_indices:
         list of integers specifying the multi start indices to be plotted
 
     Returns
     -------
-
     vals: list
         list of numpy arrays
-
     offset_y:
         offset for the y-axis, if this is supposed to be in log10-scale
-
     y_label:
         Label for y axis
     """
-
     # get list of indices
     if start_indices is None:
         start_indices = np.array(range(len(vals)))
     else:
         # check whether list or maximum value
         start_indices = np.array(start_indices)
 
@@ -379,44 +343,38 @@
 
 def handle_options(ax: plt.Axes,
                    vals: List[np.ndarray],
                    ref: List[ReferencePoint],
                    y_limits: Union[float, np.ndarray],
                    offset_y: float):
     """
+    Apply post-plotting transformations to the axis object.
+
     Get the limits for the y-axis, plots the reference points, will do
-    more at a later time point. This function is there to apply whatever
-    kind of post-plotting transformations to the axis object.
+    more at a later time point.
 
     Parameters
     ----------
-
     ref:
         List of reference points for optimization results, containing et
         least a function value fval
-
     vals:
         list of numpy arrays of size 2 x number of values
-
     ax:
         Axes object to use.
-
     y_limits:
         maximum value to be plotted on the y-axis, or y-limits
-
     offset_y:
         offset for the y-axis, if this is supposed to be in log10-scale
 
     Returns
     -------
-
     ax: matplotlib.Axes
         The plot axes.
     """
-
     # handle y-limits
     ax = process_y_limits(ax, y_limits)
 
     # handle reference points
     if len(ref) > 0:
         # plot reference points
         # get length of longest trajectory
```

### Comparing `pypesto-0.2.8/pypesto/visualize/parameters.py` & `pypesto-0.2.9/pypesto/visualize/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,30 +64,28 @@
         ``None`` to use bounds as determined by ``lb, ub``.
 
     Returns
     -------
     ax:
         The plot axes.
     """
-
     # parse input
     (results, colors, legends) = process_result_list(results, colors, legends)
 
     if isinstance(parameter_indices, str):
         if parameter_indices == 'all':
             parameter_indices = range(0, results[0].problem.dim_full)
         elif parameter_indices == 'free_only':
             parameter_indices = results[0].problem.x_free_indices
         else:
             raise ValueError("Permissible values for parameter_indices are "
                              "'all', 'free_only' or a list of indices")
 
     def scale_parameters(x):
-        """Scale ``x`` from [lb, ub] to interval given by ``scale_to_interval``
-        """
+        """Scale `x` from [lb, ub] to interval given by `scale_to_interval`."""
         if scale_to_interval is None or scale_to_interval is False:
             return x
 
         return (scale_to_interval[0] + (x - lb) / (ub - lb)
                 * (scale_to_interval[1] - scale_to_interval[0]))
 
     for j, result in enumerate(results):
@@ -155,22 +153,19 @@
         object is specified
     color:
         RGBA color.
     start_indices:
         List of integers specifying the multistarts to be plotted or
         int specifying up to which start index should be plotted
 
-
     Returns
     -------
     ax:
-    The plot axes.
-
+        The plot axes.
     """
-
     if ax is None:
         ax = plt.subplots()[1]
         fig = plt.gcf()
         fig.set_size_inches(*size)
 
     xs = result.optimize_result.get_for_key('x')
 
@@ -200,60 +195,47 @@
         ax: Optional[matplotlib.axes.Axes] = None,
         size: Optional[Tuple[float, float]] = None,
         colors: Optional[Sequence[Union[np.ndarray, List[float]]]] = None,
         linestyle: str = '-',
         legend_text: Optional[str] = None,
         balance_alpha: bool = True
 ) -> matplotlib.axes.Axes:
-
     """
     Plot parameters plot using list of parameters.
 
     Parameters
     ----------
-
     xs:
         Including optimized parameters for each startpoint.
         Shape: (n_starts, dim).
-
     fvals:
         Function values. Needed to assign cluster colors.
-
     lb, ub:
         The lower and upper bounds.
-
     x_labels:
         Labels to be used for the parameters.
-
     ax:
         Axes object to use.
-
     size:
         see parameters
-
     colors:
         One for each element in 'fvals'.
-
     linestyle:
         linestyle argument for parameter plot
-
     legend_text:
         Label for line plots
-
     balance_alpha:
         Flag indicating whether alpha for large clusters should be reduced to
         avoid overplotting (default: True)
 
     Returns
     -------
-
     ax:
         The plot axes.
     """
-
     # parse input
     xs = np.array(xs)
     fvals = np.array(fvals)
     # remove nan or inf values in fvals and xs
     xs, fvals = delete_nan_inf(fvals, xs, len(ub) if ub is not None else 1)
 
     if size is None:
@@ -310,50 +292,42 @@
 def handle_inputs(
         result: Result, parameter_indices: List[int],
         lb: Optional[Union[np.ndarray, List[float]]] = None,
         ub: Optional[Union[np.ndarray, List[float]]] = None,
         start_indices: Optional[Union[int, Iterable[int]]] = None
 ) -> Tuple[np.ndarray, np.ndarray, List[str], np.ndarray, List[np.ndarray]]:
     """
-    Computes the correct bounds for the parameter indices to be plotted and
-    outputs the corresponding parameters and their labels
+    Compute the correct bounds for the parameter indices to be plotted.
+
+    Outputs the corresponding parameters and their labels.
 
     Parameters
     ----------
-
     result:
         Optimization result obtained by 'optimize.py'.
-
     parameter_indices:
         Specifies which parameters should be plotted.
-
     lb, ub:
         If not None, override result.problem.lb, problem.problem.ub.
         Dimension either result.problem.dim or result.problem.dim_full.
-
     start_indices:
         list of integers specifying the multistarts to be plotted or
         int specifying up to which start index should be plotted
 
     Returns
     -------
-
     lb, ub:
         Dimension either result.problem.dim or result.problem.dim_full.
-
     x_labels:
         ytick labels to be applied later on
-
     fvals:
         objective function values which are needed for plotting later
-
     xs:
         parameter values which will be plotted later
     """
-
     # retrieve results
     fvals = result.optimize_result.get_for_key('fval')
     xs = result.optimize_result.get_for_key('x')
 
     # parse indices which should be plotted
     if start_indices is not None:
         start_indices = process_start_indices(start_indices, len(fvals))
```

### Comparing `pypesto-0.2.8/pypesto/visualize/profile_cis.py` & `pypesto-0.2.9/pypesto/visualize/profile_cis.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.2.8/pypesto/visualize/profiles.py` & `pypesto-0.2.9/pypesto/visualize/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,17 @@
              colors=None,
              legends: Sequence[str] = None,
              x_labels: Sequence[str] = None,
              profile_list_ids: Union[int, Sequence[int]] = 0,
              ratio_min: float = 0.,
              show_bounds: bool = False):
     """
-    Plot classical 1D profile plot (using the posterior, e.g. Gaussian like
-    profile)
+    Plot classical 1D profile plot.
+
+    Using the posterior, e.g. Gaussian like profile.
 
     Parameters
     ----------
     results: list or pypesto.Result
         List of or single `pypesto.Result` after profiling.
     ax: list of matplotlib.Axes, optional
         List of axes objects to use.
@@ -53,15 +54,14 @@
         Whether to show, and extend the plot to, the lower and upper bounds.
 
     Returns
     -------
     ax: matplotlib.Axes
         The plot axes.
     """
-
     # parse input
     results, profile_list_ids, colors, legends = process_result_list_profiles(
         results, profile_list_ids, colors, legends)
 
     # get the parameter ids to be plotted
     profile_indices = process_profile_indices(results, profile_indices,
                                               profile_list_ids)
@@ -106,16 +106,17 @@
 
 
 def profiles_lowlevel(
         fvals, ax=None, size: Tuple[float, float] = (18.5, 6.5),
         color=None, legend_text: str = None, x_labels=None,
         show_bounds: bool = False, lb_full=None, ub_full=None):
     """
-    Lowlevel routine for profile plotting, working with a list of arrays
-    only, opening different axes objects in case
+    Lowlevel routine for profile plotting.
+
+    Working with a list of arrays only, opening different axes objects in case.
 
     Parameters
     ----------
     fvals: numeric list or array
         Values to plot.
     ax: list of matplotlib.Axes, optional
         List of axes object to use.
@@ -139,15 +140,14 @@
         Upper bound.
 
     Returns
     -------
     ax: matplotlib.Axes
         The plot axes.
     """
-
     # axes
     if ax is None:
         ax = []
         fig = plt.figure()
         fig.set_size_inches(*size)
         create_new_ax = True
     else:
@@ -234,15 +234,15 @@
 
 
 def profile_lowlevel(
         fvals, ax=None, size: Tuple[float, float] = (18.5, 6.5),
         color=None, legend_text: str = None, show_bounds: bool = False,
         lb: float = None, ub: float = None):
     """
-    Lowlevel routine for plotting one profile, working with a numpy array only
+    Lowlevel routine for plotting one profile, working with a numpy array only.
 
     Parameters
     ----------
     fvals: numeric list or array
         Values to plot.
     ax: matplotlib.Axes, optional
         Axes object to use.
@@ -261,15 +261,14 @@
         Upper bound.
 
     Returns
     -------
     ax: matplotlib.Axes
         The plot axes.
     """
-
     # parse input
     fvals = np.asarray(fvals)
 
     # get colors
     color = assign_colors([1.], color)
 
     # axes
@@ -304,15 +303,14 @@
         List of reference points for optimization results, containing et
         least a function value fval
     ax: matplotlib.Axes, optional
         Axes object to use.
     profile_indices: list of integer values
         List of integer values specifying which profiles should be plotted.
     """
-
     if len(ref) > 0:
         # loop over axes objects
         for i_par, i_ax in enumerate(ax):
             for i_ref in ref:
                 current_x = i_ref['x'][profile_indices[i_par]]
                 i_ax.plot([current_x, current_x], [0., 1.],
                           color=i_ref.color, label=i_ref.legend)
@@ -326,32 +324,33 @@
 
 def handle_inputs(
         result: Result,
         profile_indices: Sequence[int],
         profile_list: int,
         ratio_min: float):
     """
-    Retrieves the values of the profiles to be plotted later from a
-    pypesto.ProfileResult object
+    Retrieve the values of the profiles to be plotted.
 
     Parameters
     ----------
     result: pypesto.Result
         Profile result obtained by 'profile.py'.
     profile_indices: list of integer values
         List of integer values specifying which profiles should be plotted.
     profile_list: int, optional
         Index of the profile list to be used for profiling.
+    ratio_min: int, optional
+        Exclude values where profile likelihood ratio is smaller than
+        ratio_min.
 
     Returns
     -------
     fvals: numeric list
         Including values that need to be plotted.
     """
-
     # extract ratio values values from result
     fvals = []
     for i_par in range(0, len(result.profile_result.list[profile_list])):
         if i_par in profile_indices and \
                 result.profile_result.list[profile_list][i_par] is not None:
             xs = result.profile_result.list[profile_list][i_par]\
                 .x_path[i_par, :]
@@ -372,16 +371,17 @@
 
 
 def process_result_list_profiles(results: Result,
                                  profile_list_ids: Sequence[int],
                                  colors: Sequence[np.array],
                                  legends: Union[str, list]) -> Sequence[int]:
     """
-    assigns colors and legends to a list of results while taking care of the
-    special cases for profile plotting
+    Assign colors and legends to a list of results.
+
+    Takes also care of the special cases for profile plotting.
 
     Parameters
     ----------
     results: list or pypesto.Result
         List of or single `pypesto.Result` after profiling.
     profile_list_ids: int or list of ints, optional
         Index or list of indices of the profile lists to be used for profiling.
@@ -392,15 +392,14 @@
 
     Returns
     -------
     profile_indices: list of integer values
         corrected list of integer values specifying which profiles should be
         plotted.
     """
-
     # ensure list of ids
     if isinstance(profile_list_ids, int):
         profile_list_ids = [profile_list_ids]
 
     # check if we have a single result
     if isinstance(results, list):
         if len(results) != 1:
@@ -421,18 +420,19 @@
 
 
 def process_profile_indices(
         results: Sequence[Result],
         profile_indices: Sequence[int],
         profile_list_ids: Union[int, Sequence[int]]):
     """
-    Retrieves the indices of the parameter for which profiles should be
-    plotted later from a list of pypesto.ProfileResult objects
-    """
+    Clean up profile_indices to be plotted.
 
+    Retrieve the indices of the parameter for which profiles should be
+    plotted later from a list of pypesto.ProfileResult objects.
+    """
     # get all parameter indices, for which profiles were computed
     plottable_indices = set()
     for result in results:
         for profile_list_id in profile_list_ids:
             # get parameter indices, for which profiles were computed
             if profile_list_id < len(result.profile_result.list):
                 tmp_indices = [
```

### Comparing `pypesto-0.2.8/pypesto/visualize/reference_points.py` & `pypesto-0.2.9/pypesto/visualize/reference_points.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 import numpy as np
 
 from typing import List
 
 
 class ReferencePoint(dict):
     """
-    Reference point for plotting. Should contain a parameter value and an
-    objective function value, may also contain a color and a legend.
+    Reference point for plotting.
+
+    Should contain a parameter value and an objective function value,
+    may also contain a color and a legend.
 
     Can be used like a dict.
 
     Attributes
     ----------
-
     x: ndarray
         Reference parameters.
-
     fval: float
         Function value, fun(x), for reference parameters.
-
     color: RGBA, optional
         Color which should be used for reference point.
-
     auto_color: boolean
         flag indicating whether color for this reference point should be
         assigned automatically or whether it was assigned by user
-
     legend: str
         legend text for reference point
     """
 
     def __init__(self,
                  reference=None,
                  x=None,
@@ -89,40 +86,38 @@
                 self.color = color
                 self.auto_color = False
             else:
                 self.color = None
                 self.auto_color = True
 
     def __getattr__(self, key):
+        """Allow usage of keys as attributes."""
         try:
             return self[key]
         except KeyError:
             raise AttributeError(key)
 
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
 
 def assign_colors(ref):
     """
-    Assigns colors to reference points, depending on user settings
+    Assign colors to reference points, depending on user settings.
 
     Parameters
     ----------
-
     ref: list of ReferencePoint
         Reference points, which need to get their color property filled
 
     Returns
     -------
-
     ref: list of ReferencePoint
         Reference points, which got their color property filled
     """
-
     # loop over reference points
     auto_color_count = 0
     for i_ref in ref:
         if i_ref['auto_color']:
             auto_color_count += 1
 
     auto_colors = [[0., 0.5 * (1. + i_auto / auto_color_count), 0., 0.9] for
@@ -137,40 +132,34 @@
 
     return ref
 
 
 def create_references(references=None, x=None, fval=None, color=None,
                       legend=None) -> List[ReferencePoint]:
     """
-    This function creates a list of reference point objects from user inputs
+    Create a list of reference point objects from user inputs.
 
     Parameters
     ----------
-
     references: ReferencePoint or dict or list, optional
         Will be converted into a list of RefPoints
-
     x: ndarray, optional
         Parameter vector which should be used for reference point
-
     fval: float, optional
         Objective function value which should be used for reference point
-
     color: RGBA, optional
         Color which should be used for reference point.
-
     legend: str
         legend text for reference point
+
     Returns
     -------
-
     colors: list of RGBA
         One for each element in 'vals'.
     """
-
     # parse input (reference)
     ref = []
     if references is not None:
         if isinstance(references, list):
             for reference in references:
                 ref.append(ReferencePoint(reference))
         else:
```

### Comparing `pypesto-0.2.8/pypesto/visualize/sampling.py` & `pypesto-0.2.9/pypesto/visualize/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,32 +26,24 @@
 )
 from .misc import rgba2rgb
 
 
 logger = logging.getLogger(__name__)
 
 
-def sampling_fval_trace(*args, **kwargs):
-    warnings.warn(
-        '`sampling_fval_trace` is deprecated in favor of '
-        '`sampling_fval_traces` and will be removed in a future version of '
-        'pyPESTO.'
-    )
-    return sampling_fval_traces(*args, **kwargs)
-
-
 def sampling_fval_traces(
         result: Result,
         i_chain: int = 0,
         full_trace: bool = False,
         stepsize: int = 1,
         title: str = None,
         size: Tuple[float, float] = None,
         ax: matplotlib.axes.Axes = None):
-    """Plot log-posterior (=function value) over iterations.
+    """
+    Plot log-posterior (=function value) over iterations.
 
     Parameters
     ----------
     result:
         The pyPESTO result object with filled sample result.
     i_chain:
         Which chain to plot. Default: First chain.
@@ -67,15 +59,14 @@
         Axes object to use.
 
     Returns
     -------
     ax:
         The plot axes.
     """
-
     # get data which should be plotted
     _, params_fval, _, _, _ = get_data_to_plot(result=result,
                                                i_chain=i_chain,
                                                stepsize=stepsize,
                                                full_trace=full_trace)
 
     # set axes and figure
@@ -575,15 +566,18 @@
         axis_label_padding: int = 50,
         groupby: str = CONDITION,
         condition_gap: float = 0.01,
         condition_ids: Sequence[str] = None,
         output_ids: Sequence[str] = None,
         weighting: bool = False
 ) -> matplotlib.axes.Axes:
-    """Plot MCMC-based prediction credibility intervals for the
+    """
+    Visualize prediction trajectory of an EnsemblePrediction.
+
+    Plot MCMC-based prediction credibility intervals for the
     model states or outputs. One or various credibility levels
     can be depicted. Plots are grouped by condition.
 
     Parameters
     ----------
     result:
         The pyPESTO result object with filled sample result.
@@ -628,15 +622,16 @@
     # Get the percentiles that correspond to the requested credibility levels.
     percentiles = [
         percentile
         for level in levels
         for percentile in _get_level_percentiles(level)
     ]
 
-    summary = ensemble_prediction.compute_summary(percentiles_list=percentiles)
+    summary = ensemble_prediction.compute_summary(
+        percentiles_list=percentiles, weighting=weighting)
 
     all_condition_ids, all_output_ids = _get_condition_and_output_ids(summary)
     if condition_ids is None:
         condition_ids = all_condition_ids
     if output_ids is None:
         output_ids = all_output_ids
 
@@ -748,16 +743,16 @@
         alpha: Sequence[int] = None,
         step: float = 0.05,
         show_median: bool = True,
         title: str = None,
         size: Tuple[float, float] = None,
         ax: matplotlib.axes.Axes = None
 ) -> matplotlib.axes.Axes:
-    """Plot MCMC-based parameter credibility intervals for one or more
-    credibility levels.
+    """
+    Plot MCMC-based parameter credibility intervals.
 
     Parameters
     ----------
     result:
         The pyPESTO result object with filled sample result.
     alpha:
         List of lower tail probabilities, defaults to 95% interval.
@@ -838,34 +833,26 @@
     handles, labels = plt.gca().get_legend_handles_labels()
     by_label = dict(zip(labels, handles))
     ax.legend(by_label.values(), by_label.keys(), bbox_to_anchor=(1.05, 1))
 
     return ax
 
 
-def sampling_parameters_trace(*args, **kwargs):
-    warnings.warn(
-        '`sampling_parameters_trace` is deprecated in favor of '
-        '`sampling_parameter_traces` and will be removed in a future version '
-        'of pyPESTO.'
-    )
-    return sampling_parameter_traces(*args, **kwargs)
-
-
 def sampling_parameter_traces(
         result: Result,
         i_chain: int = 0,
         par_indices: Sequence[int] = None,
         full_trace: bool = False,
         stepsize: int = 1,
         use_problem_bounds: bool = True,
         suptitle: str = None,
         size: Tuple[float, float] = None,
         ax: matplotlib.axes.Axes = None):
-    """Plot parameter values over iterations.
+    """
+    Plot parameter values over iterations.
 
     Parameters
     ----------
     result:
         The pyPESTO result object with filled sample result.
     i_chain:
         Which chain to plot. Default: First chain.
@@ -887,15 +874,14 @@
         Axes object to use.
 
     Returns
     -------
     ax:
         The plot axes.
     """
-
     # get data which should be plotted
     nr_params, params_fval, theta_lb, theta_ub, param_names = get_data_to_plot(
         result=result, i_chain=i_chain, stepsize=stepsize,
         full_trace=full_trace, par_indices=par_indices)
 
     # compute, how many rows and columns we need for the subplots
     num_row = int(np.round(np.sqrt(nr_params)))
@@ -958,15 +944,16 @@
 def sampling_scatter(
         result: Result,
         i_chain: int = 0,
         stepsize: int = 1,
         suptitle: str = None,
         diag_kind: str = "kde",
         size: Tuple[float, float] = None):
-    """Parameter scatter plot.
+    """
+    Parameter scatter plot.
 
     Parameters
     ----------
     result:
         The pyPESTO result object with filled sample result.
     i_chain:
         Which chain to plot. Default: First chain.
@@ -980,15 +967,14 @@
         Figure size in inches.
 
     Returns
     -------
     ax:
         The plot axes.
     """
-
     # get data which should be plotted
     nr_params, params_fval, theta_lb, theta_ub, _ = get_data_to_plot(
         result=result, i_chain=i_chain, stepsize=stepsize)
 
     sns.set(style="ticks")
 
     ax = sns.pairplot(
@@ -1035,17 +1021,17 @@
     suptitle:
         Figure super title.
     size:
         Figure size in inches.
 
     Return
     --------
-    ax: matplotlib-axes
+    ax:
+        matplotlib-axes
     """
-
     # get data which should be plotted
     nr_params, params_fval, theta_lb, theta_ub, param_names = get_data_to_plot(
         result=result, i_chain=i_chain,
         stepsize=stepsize, par_indices=par_indices)
 
     # compute, how many rows and columns we need for the subplots
     num_row = int(np.round(np.sqrt(nr_params)))
```

### Comparing `pypesto-0.2.8/pypesto/visualize/waterfall.py` & `pypesto-0.2.9/pypesto/visualize/waterfall.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,56 +23,44 @@
               colors: Optional[Union[RGBA, Sequence[RGBA]]] = None,
               legends: Optional[Union[Sequence[str], str]] = None):
     """
     Plot waterfall plot.
 
     Parameters
     ----------
-
     results:
         Optimization result obtained by 'optimize.py' or list of those
-
     ax: matplotlib.Axes, optional
         Axes object to use.
-
     size:
         Figure size (width, height) in inches. Is only applied when no ax
         object is specified
-
     y_limits: float or ndarray, optional
         maximum value to be plotted on the y-axis, or y-limits
-
     scale_y:
         May be logarithmic or linear ('log10' or 'lin')
-
     offset_y:
         offset for the y-axis, if it is supposed to be in log10-scale
-
     start_indices:
         Integers specifying the multistart to be plotted or int specifying
         up to which start index should be plotted
-
     reference:
         Reference points for optimization results, containing at least a
         function value fval
-
     colors:
         Colors or single color  for plotting. If not set, clustering is done
         and colors are assigned automatically
-
     legends:
         Labels for line plots, one label per result object
 
     Returns
     -------
-
     ax: matplotlib.Axes
         The plot axes.
     """
-
     # parse input
     (results, colors, legends) = process_result_list(results, colors, legends)
 
     refs = create_references(references=reference)
 
     # precompute y-offset, if needed and if a list of results was passed
     fvals_all, offset_y = process_offset_for_list(offset_y, results, scale_y,
@@ -99,45 +87,36 @@
 def waterfall_lowlevel(fvals, scale_y='log10', offset_y=0., ax=None,
                        size=(18.5, 10.5), colors=None, legend_text=None):
     """
     Plot waterfall plot using list of function values.
 
     Parameters
     ----------
-
     fvals: numeric list or array
         Including values need to be plotted.
-
     scale_y: str, optional
         May be logarithmic or linear ('log10' or 'lin')
-
     offset_y:
         offset for the y-axis, if it is supposed to be in log10-scale
-
     ax: matplotlib.Axes, optional
         Axes object to use.
-
     size: tuple, optional
         see waterfall
-
     colors: list, or RGBA, optional
         list of colors, or single color
         color or list of colors for plotting. If not set, clustering is done
         and colors are assigned automatically
-
     legend_text: str
         Label for line plots
 
     Returns
     -------
-
     ax: matplotlib.Axes
         The plot axes.
     """
-
     # axes
     if ax is None:
         ax = plt.subplots()[1]
         fig = plt.gcf()
         fig.set_size_inches(*size)
 
     # parse input
@@ -208,43 +187,34 @@
         offset_y: float,
         results: Sequence[Result],
         scale_y: Optional[str],
         start_indices: Optional[Sequence[int]] = None,
         references: Optional[Sequence[ReferencePoint]] = None,
 ) -> Tuple[List[np.ndarray], float]:
     """
-    If we have a list of results, all should use the same offset_y,
-    which is computed by this function and added to the fvals
+    Compute common offset_y and add it to `fvals` of results.
 
     Parameters
     ----------
-
     offset_y:
         User provided offset_y
-
     results:
         Optimization results obtained by 'optimize.py'
-
     scale_y:
         May be logarithmic or linear ('log10' or 'lin')
-
     start_indices:
         Integers specifying the multistart to be plotted or int specifying
         up to which start index should be plotted
-
-
     references:
         Reference points that will be plotted along with the results
 
     Returns
     -------
-
     fvals:
         List of arrays of function values for each result
-
     offset_y:
         offset for the y-axis
     """
     min_val = np.inf
     fvals_all = []
     for result in results:
         fvals = np.asarray([
@@ -270,44 +240,38 @@
 
     # return offsetted values
     return [fvals + offset_y for fvals in fvals_all], offset_y
 
 
 def handle_options(ax, max_len_fvals, ref, y_limits, offset_y):
     """
+    Apply post-plotting transformations to the axis object.
+
     Get the limits for the y-axis, plots the reference points, will do
-    more at a later time point. This function is there to apply whatever
-    kind of post-plotting transformations to the axis object.
+    more at a later time point.
 
     Parameters
     ----------
-
     ax: matplotlib.Axes, optional
         Axes object to use.
-
     max_len_fvals: int
         maximum number of points
-
     ref: list, optional
         List of reference points for optimization results, containing at
         least a function value fval
-
     y_limits: float or ndarray, optional
         maximum value to be plotted on the y-axis, or y-limits
-
     offset_y:
         offset for the y-axis, if it is supposed to be in log10-scale
 
     Returns
     -------
-
     ax: matplotlib.Axes
         The plot axes.
     """
-
     # handle reference points
     for i_ref in ref:
         # plot reference point as line
         ax.plot([0, max_len_fvals - 1],
                 [i_ref.fval + offset_y, i_ref.fval + offset_y], '--',
                 color=i_ref.color, label=i_ref.legend)
```

### Comparing `pypesto-0.2.8/pypesto.egg-info/PKG-INFO` & `pypesto-0.2.9/pypesto.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypesto
-Version: 0.2.8
+Version: 0.2.9
 Summary: python-based Parameter EStimation TOolbox
 Home-page: https://github.com/icb-dcm/pypesto
 Author: The pyPESTO developers
 Author-email: yannik.schaelte@gmail.com,jakob.vanhoefer@uni-bonn.de
 Maintainer: Yannik Schaelte, Jakob Vanhoefer
 Maintainer-email: yannik.schaelte@gmail.com,jakob.vanhoefer@uni-bonn.de
 License: BSD-3-Clause
@@ -14,18 +14,19 @@
 Project-URL: Changelog, https://pypesto.readthedocs.io/en/latest/changelog.html
 Keywords: parameter inference,optimization,sampling,profiles,ODE,AMICI,systems biology
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: all_optimizers
 Provides-Extra: amici
 Provides-Extra: petab
 Provides-Extra: ipopt
 Provides-Extra: dlib
@@ -51,15 +52,14 @@
 
 **pyPESTO** is a widely applicable and highly customizable toolbox for
 parameter estimation.
 
 [![PyPI](https://badge.fury.io/py/pypesto.svg)](https://badge.fury.io/py/pypesto)
 [![CI](https://github.com/ICB-DCM/pyPESTO/workflows/CI/badge.svg)](https://github.com/ICB-DCM/pyPESTO/actions)
 [![Coverage](https://codecov.io/gh/ICB-DCM/pyPESTO/branch/master/graph/badge.svg)](https://codecov.io/gh/ICB-DCM/pyPESTO)
-[![Quality](https://api.codacy.com/project/badge/Grade/134432ddad0e464b8494587ff370f661)](https://www.codacy.com/app/dweindl/pyPESTO?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ICB-DCM/pyPESTO&amp;utm_campaign=Badge_Grade)
 [![Documentation](https://readthedocs.org/projects/pypesto/badge/?version=latest)](https://pypesto.readthedocs.io)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2553546.svg)](https://doi.org/10.5281/zenodo.2553546)
 
 ## Feature overview
 
 pyPESTO features include:
```

### Comparing `pypesto-0.2.8/pypesto.egg-info/SOURCES.txt` & `pypesto-0.2.9/pypesto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypesto-0.2.8/pypesto.egg-info/requires.txt` & `pypesto-0.2.9/pypesto.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pypesto-0.2.8/setup.cfg` & `pypesto-0.2.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 license = BSD-3-Clause
 license_file = LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.7
 keywords = 
 	parameter inference
 	optimization
 	sampling
@@ -39,15 +40,15 @@
 	scipy >= 1.5.2
 	pandas >= 1.2.0
 	cloudpickle >= 1.5.0
 	matplotlib >= 3.3.0
 	seaborn >= 0.10.0
 	h5py >= 3.1.0
 	tqdm >= 4.46.0
-python_requires = >=3.6
+python_requires = >=3.7
 include_package_data = True
 packages = find:
 
 [options.packages.find]
 include = pypesto*
 
 [options.extras_require]
```

