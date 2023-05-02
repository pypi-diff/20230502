# Comparing `tmp/gwalk-2.0.4.tar.gz` & `tmp/gwalk-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwalk-2.0.4.tar", last modified: Thu Mar 23 18:30:44 2023, max compression
+gzip compressed data, was "gwalk-2.0.5.tar", last modified: Tue May  2 15:51:39 2023, max compression
```

## Comparing `gwalk-2.0.4.tar` & `gwalk-2.0.5.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-03-23 18:30:44.629101 gwalk-2.0.4/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      298 2023-03-10 19:59:26.000000 gwalk-2.0.4/MANIFEST.in
--rw-r--r--   0 vdelfave (669582709) staff       (20)      677 2023-03-23 18:30:44.629183 gwalk-2.0.4/PKG-INFO
--rw-r--r--   0 vdelfave (669582709) staff       (20)     2029 2022-11-15 19:49:14.000000 gwalk-2.0.4/README.md
--rw-r--r--   0 vdelfave (669582709) staff       (20)      512 2023-03-16 17:20:38.000000 gwalk-2.0.4/pyproject.toml
--rw-r--r--   0 vdelfave (669582709) staff       (20)       63 2023-03-23 18:30:44.629450 gwalk-2.0.4/setup.cfg
--rw-r--r--   0 vdelfave (669582709) staff       (20)     5329 2023-03-23 18:30:12.000000 gwalk-2.0.4/setup.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-03-23 18:30:44.603528 gwalk-2.0.4/src/
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-03-23 18:30:44.606790 gwalk-2.0.4/src/gwalk/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      307 2023-03-16 14:51:44.000000 gwalk-2.0.4/src/gwalk/__init__.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-03-23 18:30:44.608171 gwalk-2.0.4/src/gwalk/c_utils/
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1236 2023-03-08 20:05:46.000000 gwalk-2.0.4/src/gwalk/c_utils/dbg.h
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-03-23 18:30:44.610867 gwalk-2.0.4/src/gwalk/catalog/
--rw-r--r--   0 vdelfave (669582709) staff       (20)       23 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/catalog/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    29438 2023-03-23 17:18:11.000000 gwalk-2.0.4/src/gwalk/catalog/catalog.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    17506 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/catalog/coordinates.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-03-23 18:30:44.612167 gwalk-2.0.4/src/gwalk/catalog/prior/
--rw-r--r--   0 vdelfave (669582709) staff       (20)     4574 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/catalog/prior/CIP_prior_functions.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/catalog/prior/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    11432 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/catalog/prior/callister_prior.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     4176 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/catalog/prior/prior_methods.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     5703 2023-03-23 17:18:28.000000 gwalk-2.0.4/src/gwalk/catalog/read_catalog_GWTC_1.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3062 2023-03-23 17:18:42.000000 gwalk-2.0.4/src/gwalk/catalog/read_catalog_GWTC_2.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3061 2023-03-23 17:18:59.000000 gwalk-2.0.4/src/gwalk/catalog/read_catalog_GWTC_2p1.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3062 2023-03-23 17:19:11.000000 gwalk-2.0.4/src/gwalk/catalog/read_catalog_GWTC_3.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-03-23 18:30:44.612695 gwalk-2.0.4/src/gwalk/density/
--rw-r--r--   0 vdelfave (669582709) staff       (20)       23 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/density/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    50044 2023-01-24 15:58:53.000000 gwalk-2.0.4/src/gwalk/density/mesh.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-03-23 18:30:44.616943 gwalk-2.0.4/src/gwalk/multivariate_normal/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      108 2023-03-13 09:02:45.000000 gwalk-2.0.4/src/gwalk/multivariate_normal/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    24841 2023-03-16 17:20:38.000000 gwalk-2.0.4/src/gwalk/multivariate_normal/_decomposition.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)     6289 2023-03-16 17:20:38.000000 gwalk-2.0.4/src/gwalk/multivariate_normal/_mahalanobis_distance.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)    25977 2023-03-16 17:20:38.000000 gwalk-2.0.4/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)    27446 2023-03-12 15:39:56.000000 gwalk-2.0.4/src/gwalk/multivariate_normal/bounded_multivariate_normal.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    17947 2023-03-23 17:57:08.000000 gwalk-2.0.4/src/gwalk/multivariate_normal/decomposition.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    13587 2023-03-11 20:25:53.000000 gwalk-2.0.4/src/gwalk/multivariate_normal/decomposition_numpy.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    34127 2023-03-23 18:24:27.000000 gwalk-2.0.4/src/gwalk/multivariate_normal/object.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    11599 2023-03-14 17:22:13.000000 gwalk-2.0.4/src/gwalk/multivariate_normal/pdf.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    11686 2023-03-16 14:58:24.000000 gwalk-2.0.4/src/gwalk/multivariate_normal/utils.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     6920 2023-03-14 18:14:07.000000 gwalk-2.0.4/src/gwalk/optimize_likelihood_grid.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-03-23 18:30:44.618244 gwalk-2.0.4/src/gwalk/plots/
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/plots/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     7254 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/plots/axis.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     8166 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/plots/likelihood_corner.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1578 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/plots/percentile_levels.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)      686 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/plots/walker_plot.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-03-23 18:30:44.626028 gwalk-2.0.4/src/gwalk/tools/
--rw-r--r--   0 vdelfave (669582709) staff       (20)     5546 2023-01-24 15:58:53.000000 gwalk-2.0.4/src/gwalk/tools/NAL_event_pipeline.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/tools/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     2937 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/tools/collect.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    13900 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/tools/example_script.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    13076 2023-01-24 15:58:53.000000 gwalk-2.0.4/src/gwalk/tools/fit_catalog_samples.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1681 2023-02-14 21:15:16.000000 gwalk-2.0.4/src/gwalk/tools/fit_likelihood_grid.py
--rwxr-xr-x   0 vdelfave (669582709) staff       (20)     5595 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/tools/load_best_fits.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     4668 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/tools/plot_mesh_norm_corner.py
--rwxr-xr-x   0 vdelfave (669582709) staff       (20)     4068 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/tools/populate_nal_figures.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    11425 2023-01-24 15:58:53.000000 gwalk-2.0.4/src/gwalk/tools/test_catalog_samples.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-03-23 18:30:44.626680 gwalk-2.0.4/src/gwalk/utils/
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/utils/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3186 2022-11-15 19:49:15.000000 gwalk-2.0.4/src/gwalk/utils/hist.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)      133 2023-03-12 15:36:56.000000 gwalk-2.0.4/src/gwalk/utils/multivariate_normal.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-03-23 18:30:44.607984 gwalk-2.0.4/src/gwalk.egg-info/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      677 2023-03-23 18:30:44.000000 gwalk-2.0.4/src/gwalk.egg-info/PKG-INFO
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1997 2023-03-23 18:30:44.000000 gwalk-2.0.4/src/gwalk.egg-info/SOURCES.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)        1 2023-03-23 18:30:44.000000 gwalk-2.0.4/src/gwalk.egg-info/dependency_links.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)      139 2023-03-23 18:30:44.000000 gwalk-2.0.4/src/gwalk.egg-info/requires.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)        6 2023-03-23 18:30:44.000000 gwalk-2.0.4/src/gwalk.egg-info/top_level.txt
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-03-23 18:30:44.628796 gwalk-2.0.4/tests/
--rw-r--r--   0 vdelfave (669582709) staff       (20)    13966 2023-03-16 15:04:25.000000 gwalk-2.0.4/tests/test_decomposition.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3304 2023-03-16 14:56:31.000000 gwalk-2.0.4/tests/test_grid.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     5810 2023-03-16 15:04:43.000000 gwalk-2.0.4/tests/test_kl.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3882 2023-03-13 19:44:39.000000 gwalk-2.0.4/tests/test_maha.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    13133 2023-03-16 15:16:21.000000 gwalk-2.0.4/tests/test_object.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     4824 2023-03-16 14:57:03.000000 gwalk-2.0.4/tests/test_pdf.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:51:39.840623 gwalk-2.0.5/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      298 2023-04-25 18:43:04.000000 gwalk-2.0.5/MANIFEST.in
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      677 2023-05-02 15:51:39.840698 gwalk-2.0.5/PKG-INFO
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     2029 2022-11-15 19:49:14.000000 gwalk-2.0.5/README.md
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      512 2023-04-25 18:43:04.000000 gwalk-2.0.5/pyproject.toml
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       63 2023-05-02 15:51:39.840964 gwalk-2.0.5/setup.cfg
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     5328 2023-05-02 15:50:49.000000 gwalk-2.0.5/setup.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:51:39.808397 gwalk-2.0.5/src/
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:51:39.811799 gwalk-2.0.5/src/gwalk/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      307 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/__init__.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:51:39.814658 gwalk-2.0.5/src/gwalk/c_utils/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1236 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/c_utils/dbg.h
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:51:39.826507 gwalk-2.0.5/src/gwalk/catalog/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       23 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/catalog/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    29447 2023-05-02 15:45:34.000000 gwalk-2.0.5/src/gwalk/catalog/catalog.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    17506 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/catalog/coordinates.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:51:39.827336 gwalk-2.0.5/src/gwalk/catalog/prior/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     4574 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/catalog/prior/CIP_prior_functions.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/catalog/prior/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    11432 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/catalog/prior/callister_prior.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     4176 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/catalog/prior/prior_methods.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     5712 2023-05-02 15:46:03.000000 gwalk-2.0.5/src/gwalk/catalog/read_catalog_GWTC_1.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3071 2023-05-02 15:46:14.000000 gwalk-2.0.5/src/gwalk/catalog/read_catalog_GWTC_2.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3070 2023-05-02 15:46:22.000000 gwalk-2.0.5/src/gwalk/catalog/read_catalog_GWTC_2p1.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3071 2023-05-02 15:46:27.000000 gwalk-2.0.5/src/gwalk/catalog/read_catalog_GWTC_3.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:51:39.827698 gwalk-2.0.5/src/gwalk/density/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       23 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/density/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    50044 2023-01-24 15:58:53.000000 gwalk-2.0.5/src/gwalk/density/mesh.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:51:39.831431 gwalk-2.0.5/src/gwalk/multivariate_normal/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      108 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/multivariate_normal/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    24841 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/multivariate_normal/_decomposition.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     6289 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/multivariate_normal/_mahalanobis_distance.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    25977 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    27446 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/multivariate_normal/bounded_multivariate_normal.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    17947 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/multivariate_normal/decomposition.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    13587 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/multivariate_normal/decomposition_numpy.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    34127 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/multivariate_normal/object.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    11599 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/multivariate_normal/pdf.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    11686 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/multivariate_normal/utils.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     6814 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/optimize_likelihood_grid.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:51:39.832248 gwalk-2.0.5/src/gwalk/plots/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/plots/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     7254 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/plots/axis.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     8166 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/plots/likelihood_corner.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1578 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/plots/percentile_levels.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      686 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/plots/walker_plot.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:51:39.838912 gwalk-2.0.5/src/gwalk/tools/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     5546 2023-01-24 15:58:53.000000 gwalk-2.0.5/src/gwalk/tools/NAL_event_pipeline.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/tools/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     2937 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/tools/collect.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    13900 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/tools/example_script.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    13076 2023-01-24 15:58:53.000000 gwalk-2.0.5/src/gwalk/tools/fit_catalog_samples.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1681 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/tools/fit_likelihood_grid.py
+-rwxr-xr-x   0 vdelfave (669582709) staff       (20)     5595 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/tools/load_best_fits.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     4668 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/tools/plot_mesh_norm_corner.py
+-rwxr-xr-x   0 vdelfave (669582709) staff       (20)     4068 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/tools/populate_nal_figures.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    11425 2023-01-24 15:58:53.000000 gwalk-2.0.5/src/gwalk/tools/test_catalog_samples.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:51:39.839449 gwalk-2.0.5/src/gwalk/utils/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/utils/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3186 2022-11-15 19:49:15.000000 gwalk-2.0.5/src/gwalk/utils/hist.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      133 2023-04-25 18:43:04.000000 gwalk-2.0.5/src/gwalk/utils/multivariate_normal.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:51:39.814079 gwalk-2.0.5/src/gwalk.egg-info/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      677 2023-05-02 15:51:39.000000 gwalk-2.0.5/src/gwalk.egg-info/PKG-INFO
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1997 2023-05-02 15:51:39.000000 gwalk-2.0.5/src/gwalk.egg-info/SOURCES.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        1 2023-05-02 15:51:39.000000 gwalk-2.0.5/src/gwalk.egg-info/dependency_links.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      139 2023-05-02 15:51:39.000000 gwalk-2.0.5/src/gwalk.egg-info/requires.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        6 2023-05-02 15:51:39.000000 gwalk-2.0.5/src/gwalk.egg-info/top_level.txt
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-05-02 15:51:39.840469 gwalk-2.0.5/tests/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    13966 2023-04-25 18:43:04.000000 gwalk-2.0.5/tests/test_decomposition.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3304 2023-04-25 18:43:04.000000 gwalk-2.0.5/tests/test_grid.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     5810 2023-04-25 18:43:04.000000 gwalk-2.0.5/tests/test_kl.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3882 2023-04-25 18:43:04.000000 gwalk-2.0.5/tests/test_maha.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    13133 2023-04-25 18:43:04.000000 gwalk-2.0.5/tests/test_object.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     4824 2023-04-25 18:43:04.000000 gwalk-2.0.5/tests/test_pdf.py
```

### Comparing `gwalk-2.0.4/PKG-INFO` & `gwalk-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwalk
-Version: 2.0.4
+Version: 2.0.5
 Home-page: https://gitlab.com/xevra/gwalk
 Author: Vera Del Favero
 Author-email: msd8070@rit.edu
 Maintainer: Vera Del Favero
 Maintainer-email: msd8070@rit.edu
 License: MIT Lisence
 Keywords: Gravitational Wave,Likelihood
```

### Comparing `gwalk-2.0.4/README.md` & `gwalk-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/pyproject.toml` & `gwalk-2.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/setup.py` & `gwalk-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import numpy
 
 #----------------------------------------------------------------
 # General
 #----------------------------------------------------------------
 
 __name__        = "gwalk"
-__version__     = "2.0.4"
-__date__        = date(2023, 3, 10)
+__version__     = "2.0.5"
+__date__        = date(2023, 5, 2)
 __keywords__    = [
     "Gravitational Wave",
     "Likelihood",
     ]
 __status__      = "Alpha"
 
 #----------------------------------------------------------------
```

### Comparing `gwalk-2.0.4/src/gwalk/c_utils/dbg.h` & `gwalk-2.0.5/src/gwalk/c_utils/dbg.h`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/catalog/catalog.py` & `gwalk-2.0.5/src/gwalk/catalog/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/home/xevra/.local/bin/python3
 '''Reformulate package catalog samples'''
 
 ######## Imports ########
 import numpy as np
 import os
 from os.path import join, isdir, isfile
-from xdata import Database
+from xdata.database import Database
 from gwalk.catalog.coordinates import coord_tags as COORD_TAGS
 from gwalk.catalog.coordinates import coord_labels as COORD_LABELS
 from gwalk.catalog.coordinates import q_of_mc_eta
 from gwalk.catalog.prior.prior_methods import prior_mc_eta as prior_mass
 from gwalk.catalog.prior.prior_methods import prior_dist
 from gwalk.catalog.prior.callister_prior import chi_effective_prior_of_aligned_spins as chi_eff_aligned_prior
 from gwalk.catalog.prior.prior_methods import prior_full_spin
```

### Comparing `gwalk-2.0.4/src/gwalk/catalog/coordinates.py` & `gwalk-2.0.5/src/gwalk/catalog/coordinates.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/catalog/prior/CIP_prior_functions.py` & `gwalk-2.0.5/src/gwalk/catalog/prior/CIP_prior_functions.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/catalog/prior/callister_prior.py` & `gwalk-2.0.5/src/gwalk/catalog/prior/callister_prior.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/catalog/prior/prior_methods.py` & `gwalk-2.0.5/src/gwalk/catalog/prior/prior_methods.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/catalog/read_catalog_GWTC_1.py` & `gwalk-2.0.5/src/gwalk/catalog/read_catalog_GWTC_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from gwalk.catalog.coordinates import source_from_detector
 from gwalk.catalog.coordinates import detector_from_source
 from gwalk.catalog.coordinates import chieff_from_m1m2s1s2
 from gwalk.catalog.coordinates import coord_labels
 from gwalk.catalog.coordinates import lambdatilde_of_eta_lam1_lam2
 from gwalk.catalog.coordinates import deltalambda_of_eta_lam1_lam2
 from os.path import join, isfile
-from xdata import Database
+from xdata.database import Database
 
 ######## Functions ########
 #### Database handling ####
 
 def get_samples(
                 fname_event,
                 names,
```

### Comparing `gwalk-2.0.4/src/gwalk/catalog/read_catalog_GWTC_2.py` & `gwalk-2.0.5/src/gwalk/catalog/read_catalog_GWTC_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ######## Imports ########
 import numpy as np
 from gwalk.catalog.coordinates import m1m2_from_mc_eta, mc_eta_from_m1m2
 from gwalk.catalog.coordinates import z_from_lum_dist_interp
 from gwalk.catalog.coordinates import source_from_detector
 from gwalk.catalog.coordinates import chieff_from_m1m2s1s2
 from gwalk.catalog.coordinates import coord_labels
-from xdata import Database
+from xdata.database import Database
 from os.path import join, isfile
 
 ######## Functions ########
 #### Database handling ####
 def get_samples(
                 fname_event,
                 names,
```

### Comparing `gwalk-2.0.4/src/gwalk/catalog/read_catalog_GWTC_2p1.py` & `gwalk-2.0.5/src/gwalk/catalog/read_catalog_GWTC_2p1.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ######## Imports ########
 import numpy as np
 from gwalk.catalog.coordinates import m1m2_from_mc_eta, mc_eta_from_m1m2
 from gwalk.catalog.coordinates import z_from_lum_dist_interp
 from gwalk.catalog.coordinates import source_from_detector
 from gwalk.catalog.coordinates import chieff_from_m1m2s1s2
 from gwalk.catalog.coordinates import coord_labels
-from xdata import Database
+from xdata.database import Database
 from os.path import join, isfile
 
 ######## Functions ########
 #### Database handling ####
 def get_samples(
                 fname_event,
                 names,
```

### Comparing `gwalk-2.0.4/src/gwalk/catalog/read_catalog_GWTC_3.py` & `gwalk-2.0.5/src/gwalk/catalog/read_catalog_GWTC_3.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ######## Imports ########
 import numpy as np
 from gwalk.catalog.coordinates import m1m2_from_mc_eta, mc_eta_from_m1m2
 from gwalk.catalog.coordinates import z_from_lum_dist_interp
 from gwalk.catalog.coordinates import source_from_detector
 from gwalk.catalog.coordinates import chieff_from_m1m2s1s2
 from gwalk.catalog.coordinates import coord_labels
-from xdata import Database
+from xdata.database import Database
 from os.path import join, isfile
 
 ######## Functions ########
 #### Database handling ####
 def get_samples(
                 fname_event,
                 names,
```

### Comparing `gwalk-2.0.4/src/gwalk/density/mesh.py` & `gwalk-2.0.5/src/gwalk/density/mesh.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/multivariate_normal/_decomposition.c` & `gwalk-2.0.5/src/gwalk/multivariate_normal/_decomposition.c`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/multivariate_normal/_mahalanobis_distance.c` & `gwalk-2.0.5/src/gwalk/multivariate_normal/_mahalanobis_distance.c`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c` & `gwalk-2.0.5/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/multivariate_normal/bounded_multivariate_normal.py` & `gwalk-2.0.5/src/gwalk/multivariate_normal/bounded_multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/multivariate_normal/decomposition.py` & `gwalk-2.0.5/src/gwalk/multivariate_normal/decomposition.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/multivariate_normal/decomposition_numpy.py` & `gwalk-2.0.5/src/gwalk/multivariate_normal/decomposition_numpy.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/multivariate_normal/object.py` & `gwalk-2.0.5/src/gwalk/multivariate_normal/object.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/multivariate_normal/pdf.py` & `gwalk-2.0.5/src/gwalk/multivariate_normal/pdf.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/multivariate_normal/utils.py` & `gwalk-2.0.5/src/gwalk/multivariate_normal/utils.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/optimize_likelihood_grid.py` & `gwalk-2.0.5/src/gwalk/optimize_likelihood_grid.py`

 * *Files 5% similar despite different names*

```diff
@@ -185,15 +185,14 @@
                                         bounds=MV.plimits,
                                         constraints=cons,
                                        )
 
     # Extract parameters
     X_scipy = scipy_out.x.flatten()
 
-    print(X_scipy)
     # Still need to handle normalization constant for kl divergence
     if objective == "kl":
         # Still need a least squares fit for the normalization constant
         def lstsq_norm(X0):
             X_norm = np.copy(X_scipy)
             X_norm[0] = X0
             X_norm = X_norm.reshape((1, X_norm.size))
@@ -205,11 +204,9 @@
                                                  offset_of_params(X_scipy),
                                                  method=method,
                                                  bounds=[MV.plimits[0]],
                                                  #constraints=cons,
                                                 )
         X_scipy[0] = norm_scipy_out.x.flatten()
             
-    print(eigvals_satisfy_constraints(X_scipy))
-    print(cov_eigvals_by_eps(X_scipy))
     MV.params = X_scipy
     return MV
```

### Comparing `gwalk-2.0.4/src/gwalk/plots/axis.py` & `gwalk-2.0.5/src/gwalk/plots/axis.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/plots/likelihood_corner.py` & `gwalk-2.0.5/src/gwalk/plots/likelihood_corner.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/plots/percentile_levels.py` & `gwalk-2.0.5/src/gwalk/plots/percentile_levels.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/plots/walker_plot.py` & `gwalk-2.0.5/src/gwalk/plots/walker_plot.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/tools/NAL_event_pipeline.py` & `gwalk-2.0.5/src/gwalk/tools/NAL_event_pipeline.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/tools/collect.py` & `gwalk-2.0.5/src/gwalk/tools/collect.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/tools/example_script.py` & `gwalk-2.0.5/src/gwalk/tools/example_script.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/tools/fit_catalog_samples.py` & `gwalk-2.0.5/src/gwalk/tools/fit_catalog_samples.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/tools/fit_likelihood_grid.py` & `gwalk-2.0.5/src/gwalk/tools/fit_likelihood_grid.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/tools/load_best_fits.py` & `gwalk-2.0.5/src/gwalk/tools/load_best_fits.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/tools/plot_mesh_norm_corner.py` & `gwalk-2.0.5/src/gwalk/tools/plot_mesh_norm_corner.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/tools/populate_nal_figures.py` & `gwalk-2.0.5/src/gwalk/tools/populate_nal_figures.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/tools/test_catalog_samples.py` & `gwalk-2.0.5/src/gwalk/tools/test_catalog_samples.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk/utils/hist.py` & `gwalk-2.0.5/src/gwalk/utils/hist.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/src/gwalk.egg-info/PKG-INFO` & `gwalk-2.0.5/src/gwalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwalk
-Version: 2.0.4
+Version: 2.0.5
 Home-page: https://gitlab.com/xevra/gwalk
 Author: Vera Del Favero
 Author-email: msd8070@rit.edu
 Maintainer: Vera Del Favero
 Maintainer-email: msd8070@rit.edu
 License: MIT Lisence
 Keywords: Gravitational Wave,Likelihood
```

### Comparing `gwalk-2.0.4/src/gwalk.egg-info/SOURCES.txt` & `gwalk-2.0.5/src/gwalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/tests/test_decomposition.py` & `gwalk-2.0.5/tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/tests/test_grid.py` & `gwalk-2.0.5/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/tests/test_kl.py` & `gwalk-2.0.5/tests/test_kl.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/tests/test_maha.py` & `gwalk-2.0.5/tests/test_maha.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/tests/test_object.py` & `gwalk-2.0.5/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.0.4/tests/test_pdf.py` & `gwalk-2.0.5/tests/test_pdf.py`

 * *Files identical despite different names*

