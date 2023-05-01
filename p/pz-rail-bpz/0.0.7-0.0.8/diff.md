# Comparing `tmp/pz-rail-bpz-0.0.7.tar.gz` & `tmp/pz-rail-bpz-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-bpz-0.0.7.tar", last modified: Mon Mar 20 18:12:55 2023, max compression
+gzip compressed data, was "pz-rail-bpz-0.0.8.tar", last modified: Mon May  1 22:21:09 2023, max compression
```

## Comparing `pz-rail-bpz-0.0.7.tar` & `pz-rail-bpz-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-03-20 18:12:47.000000 pz-rail-bpz-0.0.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-03-20 18:12:47.000000 pz-rail-bpz-0.0.7/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-03-20 18:12:47.000000 pz-rail-bpz-0.0.7/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-03-20 18:12:47.000000 pz-rail-bpz-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-03-20 18:12:47.000000 pz-rail-bpz-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-03-20 18:12:47.000000 pz-rail-bpz-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     3058 2023-03-20 18:12:47.000000 pz-rail-bpz-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-03-20 18:12:47.000000 pz-rail-bpz-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/src/pz_rail_bpz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-03-20 18:12:55.000000 pz-rail-bpz-0.0.7/src/pz_rail_bpz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      568 2023-03-20 18:12:55.000000 pz-rail-bpz-0.0.7/src/pz_rail_bpz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-20 18:12:55.000000 pz-rail-bpz-0.0.7/src/pz_rail_bpz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-03-20 18:12:55.000000 pz-rail-bpz-0.0.7/src/pz_rail_bpz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-03-20 18:12:55.000000 pz-rail-bpz-0.0.7/src/pz_rail_bpz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (122)    26634 2023-03-20 18:12:47.000000 pz-rail-bpz-0.0.7/src/rail/estimation/algos/bpz_lite.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/src/rail/estimation/algos/bpz_version/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-03-20 18:12:47.000000 pz-rail-bpz-0.0.7/src/rail/estimation/algos/bpz_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-03-20 18:12:55.000000 pz-rail-bpz-0.0.7/src/rail/estimation/algos/bpz_version/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-03-20 18:12:47.000000 pz-rail-bpz-0.0.7/src/rail/estimation/algos/bpz_version/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/src/rail/examples/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/src/rail/examples/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/src/rail/examples/estimation/configs/
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-03-20 18:12:47.000000 pz-rail-bpz-0.0.7/src/rail/examples/estimation/configs/test_bpz.columns
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 18:12:55.483873 pz-rail-bpz-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     5949 2023-03-20 18:12:47.000000 pz-rail-bpz-0.0.7/tests/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      548 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 22:21:09.440036 pz-rail-bpz-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-01 22:21:09.000000 pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-05-01 22:21:09.000000 pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 22:21:09.000000 pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-01 22:21:09.000000 pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-01 22:21:09.000000 pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (122)    27982 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/src/rail/estimation/algos/bpz_lite.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/rail/estimation/algos/bpz_version/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/src/rail/estimation/algos/bpz_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-01 22:21:08.000000 pz-rail-bpz-0.0.8/src/rail/estimation/algos/bpz_version/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/src/rail/estimation/algos/bpz_version/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/rail/examples/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/rail/examples/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/src/rail/examples/estimation/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/src/rail/examples/estimation/configs/test_bpz.columns
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 22:21:09.436036 pz-rail-bpz-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     6168 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/tests/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10624 2023-05-01 22:20:52.000000 pz-rail-bpz-0.0.8/tests/validation_10gal.pq
```

### Comparing `pz-rail-bpz-0.0.7/.github/workflows/main.yml` & `pz-rail-bpz-0.0.8/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.7/.github/workflows/pypi.yaml` & `pz-rail-bpz-0.0.8/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.7/.gitignore` & `pz-rail-bpz-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.7/LICENSE` & `pz-rail-bpz-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.7/PKG-INFO` & `pz-rail-bpz-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-bpz
-Version: 0.0.7
+Version: 0.0.8
 Summary: RAIL BPZ Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-bpz-0.0.7/README.md` & `pz-rail-bpz-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.7/pyproject.toml` & `pz-rail-bpz-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     "Programming Language :: Python :: 3.10",
     "Natural Language :: English",
     "Operating System :: POSIX"
 ]
 dynamic = ["version"]
 dependencies = [
     "desc-bpz",
+    "pandas",
     "pz-rail",
+    "tables-io[full]",
 ]
 
 [project.optional-dependencies]
 dev = [
     "coverage",
     "pylint",
     "pytest",
```

### Comparing `pz-rail-bpz-0.0.7/src/pz_rail_bpz.egg-info/PKG-INFO` & `pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-bpz
-Version: 0.0.7
+Version: 0.0.8
 Summary: RAIL BPZ Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-bpz-0.0.7/src/pz_rail_bpz.egg-info/SOURCES.txt` & `pz-rail-bpz-0.0.8/src/pz_rail_bpz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 src/pz_rail_bpz.egg-info/requires.txt
 src/pz_rail_bpz.egg-info/top_level.txt
 src/rail/estimation/algos/bpz_lite.py
 src/rail/estimation/algos/bpz_version/__init__.py
 src/rail/estimation/algos/bpz_version/_version.py
 src/rail/estimation/algos/bpz_version/utils.py
 src/rail/examples/estimation/configs/test_bpz.columns
-tests/test_algos.py
+tests/test_algos.py
+tests/validation_10gal.pq
```

### Comparing `pz-rail-bpz-0.0.7/src/rail/estimation/algos/bpz_lite.py` & `pz-rail-bpz-0.0.8/src/rail/estimation/algos/bpz_lite.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 -no 'ONLY_TYPE' mode
 
 """
 
 import os
 import numpy as np
 import scipy.optimize as sciop
+import pandas as pd
 import scipy.integrate
 import glob
 import qp
 import tables_io
 from ceci.config import StageParameter as Param
 from rail.estimation.estimator import CatEstimator, CatInformer
-from rail.estimation.algos import bpz_version
 from rail.core.utils import RAILDIR
 from rail.estimation.algos.bpz_version.utils import RAIL_BPZ_DIR
 
 def_bands = ['u', 'g', 'r', 'i', 'z', 'y']
 def_bandnames = [f"mag_{band}_lsst" for band in def_bands]
 def_errnames = [f"mag_err_{band}_lsst" for band in def_bands]
 def_maglims = dict(mag_u_lsst=27.79,
@@ -118,29 +118,30 @@
     def _frac_likelihood(self, frac_params):
         ngal = len(self.mags)
         probs = np.zeros([self.ntyp, ngal])
         foarr = frac_params[:self.ntyp - 1]
         ktarr = frac_params[self.ntyp - 1:]
         for i in range(self.ntyp - 1):
             probs[i, :] = [foarr[i] * np.exp(-1. * ktarr[i] * (mag - self.m0)) for mag in self.mags]
-        # set the probability of last element to 1 - sum of the others to keep normalized
-        # this is the weird way BPZ does things, though it does it with the last
+        # set the probability of last element to 1 - sum of the others to
+        # keep normalized, this is the way BPZ does things
         probs[self.ntyp - 1, :] = 1. - np.sum(probs[:-1, :], axis=0)
         likelihood = 0.0
         for i, typ in enumerate(self.besttypes):
-            likelihood += -2. * np.log10(probs[typ, i])
+            if probs[typ, i] > 0.0:
+                likelihood += -2. * np.log10(probs[typ, i])
         return likelihood
 
     def _find_fractions(self):
         # set up fo and kt arrays, choose default start values
         if self.ntyp == 1:
             fo_init = np.array([1.0])
             kt_init = np.array([self.config.init_kt])
         else:
-            fo_init = np.ones(self.ntyp - 1) / (self.ntyp - 1)
+            fo_init = np.ones(self.ntyp - 1) / (self.ntyp)
             kt_init = np.ones(self.ntyp - 1) * self.config.init_kt
         fracparams = np.hstack([fo_init, kt_init])
         # run scipy optimize to find best params
         # note that best fit vals are stored as "x" for some reason
         frac_results = sciop.minimize(self._frac_likelihood, fracparams, method='nelder-mead').x
         if self.ntyp == 1:
             self.fo_arr = np.array([frac_results[0]])
@@ -161,15 +162,15 @@
 
         # This is a vector of loglike per object
         loglike = alpha * np.log(szs) - ((szs / zm)**alpha) - np.log(Inorm)
 
         # We are minimizing not maximizing so return the negative
         mloglike = -(loglike.sum())
 
-        print(params, mloglike)
+        # print(params, mloglike)
         return mloglike
 
     def _find_dndz_params(self):
 
         # initial parameters for zo, alpha, and km
         zo_arr = np.ones(self.ntyp)
         a_arr = np.ones(self.ntyp)
@@ -178,14 +179,15 @@
             print(f"minimizing for type {i}")
             self.typmask = (self.besttypes == i)
             dndzparams = np.hstack([self.config.init_zo, self.config.init_alpha, self.config.init_km])
             result = sciop.minimize(self._dndz_likelihood, dndzparams, method='nelder-mead').x
             zo_arr[i] = result[0]
             a_arr[i] = result[1]
             km_arr[i] = result[2]
+            print(f"best fit z0, alpha, km for type {i}: {result}")
         return zo_arr, km_arr, a_arr
 
     def _get_broad_type(self, ngal):
         typefile = self.config.type_file
         if typefile == "":  # pragma: no cover
             typedata = np.zeros(ngal, dtype=int)
         else:
@@ -212,14 +214,18 @@
         # cal function to get broad types
         Ntyp, broad_types = self._get_broad_type(ngal)
         self.ntyp = Ntyp
         # trim data to between mmin and mmax
         ref_mags = training_data[self.config.prior_band]
         mask = ((ref_mags >= self.config.mmin) & (ref_mags <= self.config.mmax))
         self.mags = ref_mags[mask]
+        # To not screw up likelihood calculation, set objs with mag
+        # brighter than m0 to value of m0
+        brightmask = (self.mags < self.m0)
+        self.mags[brightmask] = self.m0
         self.szs = training_data[self.config.redshift_col][mask]
         self.besttypes = broad_types[mask]
 
         numused = len(self.besttypes)
         print(f"using {numused} galaxies in calculation")
 
         self._find_fractions()
@@ -253,14 +259,15 @@
                           dz=Param(float, 0.01, msg="delta z in grid"),
                           nzbins=Param(int, 301, msg="# of bins in zgrid"),
                           band_names=Param(list, def_bandnames,
                                            msg="band names to be used, *ASSUMED TO BE IN INCREASING WL ORDER!*"),
                           band_err_names=Param(list, def_errnames,
                                                msg="band error column names to be used * ASSUMED TO BE IN INCREASING WL ORDER!*"),
                           nondetect_val=Param(float, 99.0, msg="value to be replaced with magnitude limit for non detects"),
+                          unobserved_val=Param(float, -99.0, msg="value to be replaced with zero flux and given large errors for non-observed filters"),
                           data_path=Param(str, "None",
                                           msg="data_path (str): file path to the "
                                           "SED, FILTER, and AB directories.  If left to "
                                           "default `None` it will use the install "
                                           "directory for rail + ../examples/estimation/data"),
                           columns_file=Param(str, os.path.join(RAIL_BPZ_DIR, 'rail/examples/estimation/configs/test_bpz.columns'),
                                              msg="name of the file specifying the columns"),
@@ -384,26 +391,48 @@
 
     def _preprocess_magnitudes(self, data):
         from desc_bpz.bpz_tools_py3 import e_mag2frac
 
         bands = self.config.band_names
         errs = self.config.band_err_names
 
+        fluxdict = {}
+        
         # Load the magnitudes
         zp_frac = e_mag2frac(np.array(self.config.zp_errors))
 
         # replace non-detects with 99 and mag_err with lim_mag for consistency
         # with typical BPZ performance
         for bandname, errname in zip(bands, errs):
             if np.isnan(self.config.nondetect_val):  # pragma: no cover
                 detmask = np.isnan(data[bandname])
             else:
                 detmask = np.isclose(data[bandname], self.config.nondetect_val)
-            data[bandname][detmask] = 99.0
-            data[errname][detmask] = self.config.mag_limits[bandname]
+            if isinstance(data, pd.DataFrame):
+                data.loc[detmask, bandname] = 99.0
+                data.loc[detmask, errname] = self.config.mag_limits[bandname]
+            else:
+                data[bandname][detmask] = 99.0
+                data[errname][detmask] = self.config.mag_limits[bandname]
+
+        # replace non-observations with -99, again to match BPZ standard
+        # below the fluxes for these will be set to zero but with enormous
+        # flux errors
+        for bandname, errname in zip(bands, errs):
+            if np.isnan(self.config.unobserved_val):  # pragma: no cover
+                obsmask = np.isnan(data[bandname])
+            else:
+                obsmask = np.isclose(data[bandname], self.config.unobserved_val)
+            if isinstance(data, pd.DataFrame):
+                data.loc[obsmask, bandname] = -99.0
+                data.loc[obsmask, errname] = 20.0
+            else:
+                data[bandname][obsmask] = -99.0
+                data[errname][obsmask] = 20.0
+
 
         # Only one set of mag errors
         mag_errs = np.array([data[er] for er in errs]).T
 
         # Group the magnitudes and errors into one big array
         mags = np.array([data[b] for b in bands]).T
 
@@ -449,38 +478,42 @@
         # and enormous error, so that their likelihood will be
         # flat. This follows what's done in the bpz script.
         nonobserved = -99.
         unobserved = np.isclose(mags, nonobserved)
         flux[unobserved] = 0.0
         flux_err[unobserved] = 1e108
 
-        # Upate the input dictionary with new things we have calculated
-        data['flux'] = flux
-        data['flux_err'] = flux_err
-        data['mags'] = mags
-        return data
+        # Upate the flux dictionary with new things we have calculated
+        fluxdict['flux'] = flux
+        fluxdict['flux_err'] = flux_err
+        m_0_col = self.config.band_names.index(self.config.prior_band)
+        fluxdict['mag0'] = mags[:, m_0_col]
+        
+        return fluxdict
 
     def _estimate_pdf(self, flux_templates, kernel, flux, flux_err, mag_0, z):
-
-        from desc_bpz.bpz_tools_py3 import p_c_z_t, prior_with_dict
+        from desc_bpz.bpz_tools_py3 import p_c_z_t
+        from desc_bpz.prior_from_dict import prior_function
 
         modeldict = self.modeldict
         p_min = self.config.p_min
         nt = flux_templates.shape[1]
 
         # The likelihood and prior...
         pczt = p_c_z_t(flux, flux_err, flux_templates)
         L = pczt.likelihood
 
         # old prior code returns NoneType for prior if "flat" or "none"
         # just hard code the no prior case for now for backward compatibility
         if self.config.no_prior:  # pragma: no cover
             P = np.ones(L.shape)
         else:
-            P = prior_with_dict(z, mag_0, modeldict, nt)  # hardcode interp 0
+            # set num templates to nt, which is hardcoding to "interp=0"
+            # in BPZ, i.e. do not create any interpolated templates
+            P = prior_function(z, mag_0, modeldict, nt)
 
         post = L * P
         # Right now we jave the joint PDF of p(z,template). Marginalize
         # over the templates to just get p(z)
         post_z = post.sum(axis=1)
 
         # Convolve with Gaussian kernel, if present
@@ -517,18 +550,17 @@
     def _process_chunk(self, start, end, data, first):
         """
         Run BPZ on a chunk of data
         """
         # replace non-detects, traditional BPZ had nondet=99 and err = maglim
         # put in that format here
         test_data = self._preprocess_magnitudes(data)
-        m_0_col = self.config.band_names.index(self.config.prior_band)
 
         nz = len(self.zgrid)
-        ng = test_data['mags'].shape[0]
+        ng = test_data['flux'].shape[0]
 
         # Set up Gauss kernel for extra smoothing, if needed
         if self.config.gauss_kernel > 0:  # pragma: no cover
             dz = self.config.dz
             x = np.arange(-3. * self.config.gauss_kernel,
                           3. * self.config.gauss_kernel + dz / 10., dz)
             kernel = np.exp(-(x / self.config.gauss_kernel)**2)
@@ -540,22 +572,18 @@
         zmean = np.zeros(ng)
         tb = np.zeros(ng)
         todds = np.zeros(ng)
         flux_temps = self.flux_templates
         zgrid = self.zgrid
         # Loop over all ng galaxies!
         for i in range(ng):
-            mag_0 = test_data['mags'][i, m_0_col]
+            mag_0 = test_data['mag0'][i]
             flux = test_data['flux'][i]
             flux_err = test_data['flux_err'][i]
             pdfs[i], zmode[i], tb[i], todds[i] = self._estimate_pdf(flux_temps,
                                                                     kernel, flux,
                                                                     flux_err, mag_0,
                                                                     zgrid)
             zmean[i] = (zgrid * pdfs[i]).sum() / pdfs[i].sum()
-        # remove the keys added to the data file by BPZ
-        test_data.pop('flux', None)
-        test_data.pop('flux_err', None)
-        test_data.pop('mags', None)
         qp_dstn = qp.Ensemble(qp.interp, data=dict(xvals=self.zgrid, yvals=pdfs))
         qp_dstn.set_ancil(dict(zmode=zmode, zmean=zmean, tb=tb, todds=todds))
         self._do_chunk_output(qp_dstn, start, end, first)
```

### Comparing `pz-rail-bpz-0.0.7/src/rail/examples/estimation/configs/test_bpz.columns` & `pz-rail-bpz-0.0.8/src/rail/examples/estimation/configs/test_bpz.columns`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.0.7/tests/test_algos.py` & `pz-rail-bpz-0.0.8/tests/test_algos.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 from rail.estimation.algos import bpz_lite
 from rail.estimation.algos.bpz_version.utils import RAIL_BPZ_DIR
 
 import scipy.special
 sci_ver_str = scipy.__version__.split('.')
 
 
-traindata = os.path.join(RAILDIR, 'rail/examples/testdata/training_100gal.hdf5')
-validdata = os.path.join(RAILDIR, 'rail/examples/testdata/validation_10gal.hdf5')
+traindata = os.path.join(RAILDIR, "rail/examples/testdata/training_100gal.hdf5")
+validdata = os.path.join(RAILDIR, "rail/examples/testdata/validation_10gal.hdf5")
+parquetdata = "./tests/validation_10gal.pq"
 DS = RailStage.data_store
 DS.__class__.allow_overwrite = True
 
 
 @pytest.mark.parametrize(
     "ntarray",
     [[8], [4, 4]]
@@ -73,37 +74,43 @@
     zb_expected = np.array([0.16, 0.12, 0.14, 0.14, 0.06, 0.14, 0.12, 0.14, 0.06, 0.16])
     train_algo = None
     pz_algo = bpz_lite.BPZ_lite
     results, rerun_results, rerun3_results = one_algo("BPZ_lite", train_algo, pz_algo, train_config_dict, estim_config_dict)
     assert np.isclose(results.ancil['zmode'], zb_expected).all()
     assert np.isclose(results.ancil['zmode'], rerun_results.ancil['zmode']).all()
 
-
-def test_bpz_wHDFN_prior():
+@pytest.mark.parametrize(
+    "inputdata, groupname",
+    [
+        (parquetdata, ""),
+        (validdata, "photometry")
+        ]
+)
+def test_bpz_wHDFN_prior(inputdata, groupname):
     estim_config_dict = {'zmin': 0.0, 'zmax': 3.0,
                          'dz': 0.01,
                          'nzbins': 301,
                          'data_path': None,
                          'columns_file': os.path.join(RAIL_BPZ_DIR, "rail/examples/estimation/configs/test_bpz.columns"),
                          'spectra_file': "SED/CWWSB4.list",
                          'madau_flag': 'no',
                          'bands': 'ugrizy',
                          'prior_band': 'mag_i_lsst',
                          'prior_file': 'flat',
                          'p_min': 0.005,
                          'gauss_kernel': 0.1,
                          'zp_errors': np.array([0.01, 0.01, 0.01, 0.01, 0.01, 0.01]),
                          'mag_err_min': 0.005,
-                         'hdf5_groupname': 'photometry',
+                         'hdf5_groupname': groupname,
                          'nt_array': [1, 2, 5],
-                         'model': './examples/estimation/CWW_HDFN_prior.pkl'}
+                         'model': os.path.join(RAILDIR, "rail/examples/estimation/CWW_HDFN_prior.pkl")}
     zb_expected = np.array([0.18, 2.88, 0.12, 0.15, 2.97, 2.78, 0.11, 0.19,
                             2.98, 2.92])
 
-    validation_data = DS.read_file('validation_data', TableHandle, validdata)
+    validation_data = DS.read_file('validation_data', TableHandle, inputdata)
     pz = bpz_lite.BPZ_lite.make_stage(name='bpz_hdfn', **estim_config_dict)
     results = pz.estimate(validation_data)
     assert np.isclose(results.data.ancil['zmode'], zb_expected).all()
     DS.clear()
     os.remove(pz.get_output(pz.get_aliased_tag('output'), final_name=True))
```

