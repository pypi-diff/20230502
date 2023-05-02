# Comparing `tmp/pspy-1.5.9.tar.gz` & `tmp/pspy-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pspy-1.5.9.tar", last modified: Mon Aug  8 10:05:24 2022, max compression
+gzip compressed data, was "pspy-1.6.tar", last modified: Tue May  2 16:00:04 2023, max compression
```

## Comparing `pspy-1.5.9.tar` & `pspy-1.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.684031 pspy-1.5.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-08-08 10:05:18.000000 pspy-1.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-08-08 10:05:18.000000 pspy-1.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4389 2022-08-08 10:05:24.684031 pspy-1.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-08-08 10:05:18.000000 pspy-1.5.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.684031 pspy-1.5.9/pspy/
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-08-08 10:05:24.684031 pspy-1.5.9/pspy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.668031 pspy-1.5.9/pspy/cov_fortran/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/cov_fortran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13837 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/cov_fortran/cov_fortran.f90
--rw-r--r--   0 runner    (1001) docker     (121)     7612 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/flat_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.672031 pspy-1.5.9/pspy/mcm_fortran/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/mcm_fortran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11471 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/mcm_fortran/mcm_fortran.f90
--rw-r--r--   0 runner    (1001) docker     (121)    10991 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/pspy_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7662 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_consistency.py
--rw-r--r--   0 runner    (1001) docker     (121)    31992 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_cov.py
--rw-r--r--   0 runner    (1001) docker     (121)     2430 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)    31552 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     4392 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_map_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)    17469 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_mcm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4785 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_mpi.py
--rw-r--r--   0 runner    (1001) docker     (121)    11347 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_spectra.py
--rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/so_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     6885 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/sph_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.672031 pspy-1.5.9/pspy/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.672031 pspy-1.5.9/pspy/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)   468866 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat
--rw-r--r--   0 runner    (1001) docker     (121)     4807 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/data/generate_test_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/data/parameters_test_data.yml
--rw-r--r--   0 runner    (1001) docker     (121) 12059025 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/data/test_data.pkl
--rw-r--r--   0 runner    (1001) docker     (121)     4115 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/test_pspy_namaster.py
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/test_so_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     3987 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/test_so_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/tests/test_so_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.684031 pspy-1.5.9/pspy/wigner3j/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/wigner3j/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)   104274 2022-08-08 10:05:18.000000 pspy-1.5.9/pspy/wigner3j/wigner3j_sub.f
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.668031 pspy-1.5.9/pspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4389 2022-08-08 10:05:24.000000 pspy-1.5.9/pspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-08-08 10:05:24.000000 pspy-1.5.9/pspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-08 10:05:24.000000 pspy-1.5.9/pspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-08-08 10:05:24.000000 pspy-1.5.9/pspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-08 10:05:24.000000 pspy-1.5.9/pspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 10:05:24.684031 pspy-1.5.9/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      222 2022-08-08 10:05:18.000000 pspy-1.5.9/scripts/test-pspy
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-08-08 10:05:24.684031 pspy-1.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-08-08 10:05:18.000000 pspy-1.5.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-08-08 10:05:18.000000 pspy-1.5.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.288178 pspy-1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-02 15:59:57.000000 pspy-1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 15:59:57.000000 pspy-1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-02 16:00:04.288178 pspy-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-02 15:59:57.000000 pspy-1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.288178 pspy-1.6/pspy/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-02 15:59:57.000000 pspy-1.6/pspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-02 16:00:04.288178 pspy-1.6/pspy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.272177 pspy-1.6/pspy/cov_fortran/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 15:59:57.000000 pspy-1.6/pspy/cov_fortran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13837 2023-05-02 15:59:57.000000 pspy-1.6/pspy/cov_fortran/cov_fortran.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-05-02 15:59:57.000000 pspy-1.6/pspy/flat_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.272177 pspy-1.6/pspy/mcm_fortran/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 15:59:57.000000 pspy-1.6/pspy/mcm_fortran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-02 15:59:57.000000 pspy-1.6/pspy/mcm_fortran/mcm_fortran.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-05-02 15:59:57.000000 pspy-1.6/pspy/pspy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35399 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31739 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_map_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_mcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-05-02 15:59:57.000000 pspy-1.6/pspy/so_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-05-02 15:59:57.000000 pspy-1.6/pspy/sph_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.272177 pspy-1.6/pspy/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.272177 pspy-1.6/pspy/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   468866 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/data/generate_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/data/parameters_test_data.yml
+-rw-r--r--   0 runner    (1001) docker     (123) 12059025 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/data/test_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/test_pspy_namaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/test_so_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/test_so_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-02 15:59:57.000000 pspy-1.6/pspy/tests/test_so_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.288178 pspy-1.6/pspy/wigner3j/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 15:59:57.000000 pspy-1.6/pspy/wigner3j/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   104274 2023-05-02 15:59:57.000000 pspy-1.6/pspy/wigner3j/wigner3j_sub.f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.272177 pspy-1.6/pspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-02 16:00:04.000000 pspy-1.6/pspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-02 16:00:04.000000 pspy-1.6/pspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:00:04.000000 pspy-1.6/pspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 16:00:04.000000 pspy-1.6/pspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 16:00:04.000000 pspy-1.6/pspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:00:04.288178 pspy-1.6/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      222 2023-05-02 15:59:57.000000 pspy-1.6/scripts/test-pspy
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-02 16:00:04.288178 pspy-1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-02 15:59:57.000000 pspy-1.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-02 15:59:57.000000 pspy-1.6/versioneer.py
```

### Comparing `pspy-1.5.9/LICENSE` & `pspy-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/PKG-INFO` & `pspy-1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspy
-Version: 1.5.9
+Version: 1.6
 Summary: Python power spectrum code
 Home-page: https://github.com/simonsobs/pspy
 Author: Simons Observatory Collaboration Power Spectrum Task Force
 License: BSD license
 Description: ====
         pspy
         ====
@@ -13,15 +13,15 @@
         ``pspy`` is a cosmology code for calculating CMB power spectra and covariance matrices. See the
         python example notebooks for an introductory set of examples on how to use the package.
         
         .. image:: https://img.shields.io/pypi/v/pspy.svg?style=flat
            :target: https://pypi.python.org/pypi/pspy/
         .. image:: https://img.shields.io/badge/license-BSD-yellow
            :target: https://github.com/simonsobs/pspy/blob/master/LICENSE
-        .. image:: https://img.shields.io/github/workflow/status/simonsobs/pspy/Testing
+        .. image:: https://img.shields.io/github/actions/workflow/status/simonsobs/pspy/testing.yml?branch=master
            :target: https://github.com/simonsobs/pspy/actions?query=workflow%3ATesting
         .. image:: https://readthedocs.org/projects/pspy/badge/?version=latest
            :target: https://pspy.readthedocs.io/en/latest/?badge=latest
         .. image:: https://codecov.io/gh/simonsobs/pspy/branch/master/graph/badge.svg?token=HHAJ7NQ5CE
            :target: https://codecov.io/gh/simonsobs/pspy
         .. image:: https://mybinder.org/badge_logo.svg
            :target: https://mybinder.org/v2/gh/simonsobs/pspy/master?filepath=notebooks/%2Findex.ipynb
@@ -96,9 +96,11 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `pspy-1.5.9/README.rst` & `pspy-1.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ``pspy`` is a cosmology code for calculating CMB power spectra and covariance matrices. See the
 python example notebooks for an introductory set of examples on how to use the package.
 
 .. image:: https://img.shields.io/pypi/v/pspy.svg?style=flat
    :target: https://pypi.python.org/pypi/pspy/
 .. image:: https://img.shields.io/badge/license-BSD-yellow
    :target: https://github.com/simonsobs/pspy/blob/master/LICENSE
-.. image:: https://img.shields.io/github/workflow/status/simonsobs/pspy/Testing
+.. image:: https://img.shields.io/github/actions/workflow/status/simonsobs/pspy/testing.yml?branch=master
    :target: https://github.com/simonsobs/pspy/actions?query=workflow%3ATesting
 .. image:: https://readthedocs.org/projects/pspy/badge/?version=latest
    :target: https://pspy.readthedocs.io/en/latest/?badge=latest
 .. image:: https://codecov.io/gh/simonsobs/pspy/branch/master/graph/badge.svg?token=HHAJ7NQ5CE
    :target: https://codecov.io/gh/simonsobs/pspy
 .. image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/simonsobs/pspy/master?filepath=notebooks/%2Findex.ipynb
```

### Comparing `pspy-1.5.9/pspy/cov_fortran/cov_fortran.f90` & `pspy-1.6/pspy/cov_fortran/cov_fortran.f90`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/flat_tools.py` & `pspy-1.6/pspy/flat_tools.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/mcm_fortran/mcm_fortran.f90` & `pspy-1.6/pspy/mcm_fortran/mcm_fortran.f90`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/pspy_utils.py` & `pspy-1.6/pspy/pspy_utils.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/so_config.py` & `pspy-1.6/pspy/so_config.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/so_consistency.py` & `pspy-1.6/pspy/so_consistency.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/so_cov.py` & `pspy-1.6/pspy/so_cov.py`

 * *Files 7% similar despite different names*

```diff
@@ -422,15 +422,23 @@
         analytic_cov = np.dot(np.dot(mbb_inv_ab, analytic_cov), mbb_inv_cd.T)
     else:
         full_analytic_cov = np.dot(np.dot(mbb_inv_ab, cov), mbb_inv_cd.T)
         analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax)
         
     return analytic_cov
 
-def cov_spin0and2(Clth_dict, coupling_dict, binning_file, lmax, mbb_inv_ab, mbb_inv_cd, binned_mcm=True):
+def cov_spin0and2(Clth_dict,
+                  coupling_dict,
+                  binning_file,
+                  lmax,
+                  mbb_inv_ab,
+                  mbb_inv_cd,
+                  binned_mcm=True,
+                  cov_T_E_only=True):
+                  
     """From the two point functions and the coupling kernel construct the T and E analytical covariance matrix of <(C_ab- Clth)(C_cd-Clth)>
 
     Parameters
     ----------
 
     Clth_dict: dictionnary
         A dictionnary of theoretical power spectrum (auto and cross) for the different split combinaison ('XaYb' etc)
@@ -442,51 +450,79 @@
         the maximum multipole to consider
     mbb_inv_ab: 2d array
         the inverse mode coupling matrix for the 'XaYb' power spectrum
     mbb_inv_cd: 2d array
         the inverse mode coupling matrix for the 'XcYd' power spectrum
     binned_mcm: boolean
       specify if the mode coupling matrices are binned or not
-
+    binned_mcm: boolean
+      specify if the mode coupling matrices are binned or not
+    cov_T_E_only: boolean
+        if true don't do B
     """
 
     bin_lo, bin_hi, bin_c, bin_size = pspy_utils.read_binning_file(binning_file, lmax)
     n_ell = Clth_dict["TaTb"].shape[0]
-        
-    full_analytic_cov = np.zeros((4 * n_ell, 4 * n_ell))
     
-    speclist = ["TT", "TE", "ET", "EE"]
+    if cov_T_E_only:
+        speclist = ["TT", "TE", "ET", "EE"]
+    else:
+        speclist =  ["TT", "TE", "TB", "ET", "BT", "EE", "EB", "BE", "BB"]
+    
+    nspec = len(speclist)
+    full_analytic_cov = np.zeros((nspec * n_ell, nspec * n_ell))
+
     for i, (W, X) in enumerate(speclist):
         for j, (Y, Z) in enumerate(speclist):
             if i > j : continue
             id0 = W + "a" + Y + "c"
             id1 = X + "b" + Z + "d"
             id2 = W + "a" + Z + "d"
             id3 = X + "b" + Y + "c"
-
-            M = symmetrize(Clth_dict[id0]) * symmetrize(Clth_dict[id1]) * coupling_dict[id0.replace("E","P") + id1.replace("E","P")]
-            M += symmetrize(Clth_dict[id2]) * symmetrize(Clth_dict[id3]) * coupling_dict[id2.replace("E","P") + id3.replace("E","P")]
             
+            Cl0Cl1 = symmetrize(Clth_dict[id0]) * symmetrize(Clth_dict[id1])
+            Cl2Cl3 = symmetrize(Clth_dict[id2]) * symmetrize(Clth_dict[id3])
+            
+            for field in ["E", "B"]:
+                id0 = id0.replace(field, "P")
+                id1 = id1.replace(field, "P")
+                id2 = id2.replace(field, "P")
+                id3 = id3.replace(field, "P")
+                
+            M = Cl0Cl1 * coupling_dict[id0 + id1]
+            M += Cl2Cl3 * coupling_dict[id2 + id3]
+
             full_analytic_cov[i * n_ell:(i + 1) * n_ell, j * n_ell:(j + 1) * n_ell] = M
     
     full_analytic_cov = np.triu(full_analytic_cov) + np.tril(full_analytic_cov.T, -1)
     
-    mbb_inv_ab = extract_TTTEEE_mbb(mbb_inv_ab)
-    mbb_inv_cd = extract_TTTEEE_mbb(mbb_inv_cd)
+    mbb_inv_ab = extract_mbb(mbb_inv_ab, cov_T_E_only=cov_T_E_only)
+    mbb_inv_cd = extract_mbb(mbb_inv_cd, cov_T_E_only=cov_T_E_only)
 
     if binned_mcm == True:
         analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
         analytic_cov = np.dot(np.dot(mbb_inv_ab, analytic_cov), mbb_inv_cd.T)
     else:
         full_analytic_cov = np.dot(np.dot(mbb_inv_ab, full_analytic_cov), mbb_inv_cd.T)
         analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
 
     return analytic_cov
 
-def generalized_cov_spin0and2(coupling_dict, id_element, ns, ps_all, nl_all, lmax, binning_file, mbb_inv_ab, mbb_inv_cd, binned_mcm=True, return_full_cov=False):
+def generalized_cov_spin0and2(coupling_dict,
+                              id_element,
+                              ns,
+                              ps_all,
+                              nl_all,
+                              lmax,
+                              binning_file,
+                              mbb_inv_ab,
+                              mbb_inv_cd,
+                              binned_mcm=True,
+                              return_full_cov=False,
+                              cov_T_E_only=True):
 
     """
     This routine deserves some explanation
     We want to compute the covariance between two power spectra
     C1 = Wa * Xb, C2 =  Yc * Zd
     Here W, X, Y, Z can be either T or E and a,b,c,d will be an index
     corresponding to the survey and array we consider so for example a = s17&pa5_150 or a = dr6&pa4_090
@@ -516,53 +552,72 @@
     mbb_inv_ab and mbb_inv_cd:
         the inverse mode coupling matrices corresponding to the C1 = Wa * Xb and C2 =  Yc * Zd power spectra
     binned_mcm: boolean
         specify if the mode coupling matrices are binned or not
     return_full_cov: boolean
         an option to return the lbyl cov (if binned_mcm=False)
         mostly used for debugging
-
+    cov_T_E_only: boolean
+        if true don't do B
     """
 
     na, nb, nc, nd = id_element
 
     n_ell = coupling_dict["TaTcTbTd"].shape[0]
     bin_lo, bin_hi, bin_c, bin_size = pspy_utils.read_binning_file(binning_file, n_ell)
-    full_analytic_cov = np.zeros((4 * n_ell, 4 * n_ell))
 
-    speclist = ["TT", "TE", "ET", "EE"]
+    if cov_T_E_only:
+        speclist = ["TT", "TE", "ET", "EE"]
+    else:
+        speclist =  ["TT", "TE", "TB", "ET", "BT", "EE", "EB", "BE", "BB"]
+    
+    nspec = len(speclist)
+    full_analytic_cov = np.zeros((nspec * n_ell, nspec * n_ell))
+
     for i, (W, X) in enumerate(speclist):
         for j, (Y, Z) in enumerate(speclist):
     
             id0 = W + "a" + Y + "c"
             id1 = X + "b" + Z + "d"
             id2 = W + "a" + Z + "d"
             id3 = X + "b" + Y + "c"
+            
+            for field in ["E", "B"]:
+                id0 = id0.replace(field, "P")
+                id1 = id1.replace(field, "P")
+                id2 = id2.replace(field, "P")
+                id3 = id3.replace(field, "P")
+
         
-            M = coupling_dict[id0.replace("E","P") + id1.replace("E","P")] * chi(na, nc, nb, nd, ns, ps_all, nl_all, W + Y + X + Z)
-            M += coupling_dict[id2.replace("E","P") + id3.replace("E","P")] * chi(na, nd, nb, nc, ns, ps_all, nl_all, W + Z + X + Y)
+            M = coupling_dict[id0 + id1] * chi(na, nc, nb, nd, ns, ps_all, nl_all, W + Y + X + Z)
+            M += coupling_dict[id2 + id3] * chi(na, nd, nb, nc, ns, ps_all, nl_all, W + Z + X + Y)
             full_analytic_cov[i * n_ell: (i + 1) * n_ell, j * n_ell: (j + 1) * n_ell] = M
 
-    mbb_inv_ab = extract_TTTEEE_mbb(mbb_inv_ab)
-    mbb_inv_cd = extract_TTTEEE_mbb(mbb_inv_cd)
+    mbb_inv_ab = extract_mbb(mbb_inv_ab, cov_T_E_only=cov_T_E_only)
+    mbb_inv_cd = extract_mbb(mbb_inv_cd, cov_T_E_only=cov_T_E_only)
 
     if binned_mcm == True:
         analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
         analytic_cov = np.dot(np.dot(mbb_inv_ab, analytic_cov), mbb_inv_cd.T)
     else:
         full_analytic_cov = np.dot(np.dot(mbb_inv_ab, full_analytic_cov), mbb_inv_cd.T)
         if return_full_cov == True:
             return full_analytic_cov
 
         analytic_cov = bin_mat(full_analytic_cov, binning_file, lmax, speclist=speclist)
 
     return analytic_cov
 
 
-def covariance_element_beam(id_element, ps_all, norm_beam_cov, binning_file, lmax):
+def covariance_element_beam(id_element,
+                            ps_all,
+                            norm_beam_cov,
+                            binning_file,
+                            lmax,
+                            cov_T_E_only=True):
     """
     This routine compute the contribution from beam errors to the analytical covariance of the power spectra
     We want to compute the beam covariance between the two spectra
     C1 = Wa * Xb, C2 =  Yc * Zd
     Here W, X, Y, Z can be either T or E and a,b,c,d will be an index
     corresponding to the survey and array we consider so for example a = dr6&pa5_150 or a = dr6&pa4_090
     The formula for the analytic covariance of C1, C2 is given by
@@ -579,122 +634,178 @@
         ps["dr6&pa5_150", "dr6&pa4_150", "TT"] =  (Dl^{CMB}_TT + fg_TT)
     norm_beam_cov: dict
         this dict contains the normalized beam covariance for each survey and array
     binning_file: str
         a binning file with three columns bin low, bin high, bin mean
     lmax: int
         the maximum multipole to consider
+    cov_T_E_only: boolean
+        if true don't do B
+
     """
     na, nb, nc, nd = id_element
 
     sv_alpha, ar_alpha = na.split("&")
     sv_beta, ar_beta = nb.split("&")
     sv_gamma, ar_gamma = nc.split("&")
     sv_eta, ar_eta = nd.split("&")
 
     bin_lo, bin_hi, bin_c, bin_size = pspy_utils.read_binning_file(binning_file, lmax)
     nbins = len(bin_hi)
 
-    speclist = ["TT", "TE", "ET", "EE"]
+    if cov_T_E_only:
+        speclist = ["TT", "TE", "ET", "EE"]
+    else:
+        speclist = ["TT", "TE", "TB", "ET", "BT", "EE", "EB", "BE", "BB"]
 
     nspec = len(speclist)
     analytic_cov_from_beam = np.zeros((nspec * nbins, nspec * nbins))
+    
     for i, spec1 in enumerate(speclist):
         for j, spec2 in enumerate(speclist):
 
             M =  (delta2(na, nc) + delta2(na, nd)) * norm_beam_cov[sv_alpha, ar_alpha]
             M += (delta2(nb, nc) + delta2(nb, nd)) * norm_beam_cov[sv_beta, ar_beta]
             M *=  np.outer(ps_all[na, nb, spec1], ps_all[nc, nd, spec2])
         
             analytic_cov_from_beam[i * nbins: (i + 1) * nbins, j * nbins: (j + 1) * nbins] = bin_mat(M, binning_file, lmax)
 
     return analytic_cov_from_beam
 
 
-def extract_TTTEEE_mbb(mbb_inv):
+def extract_mbb(mbb_inv, cov_T_E_only=True):
     """The mode coupling marix is computed for T,E,B but for now we only construct analytical covariance matrix for T and E
     The B modes is complex with important E->B leakage, this routine extract the T and E part of the mode coupling matrix
 
     Parameters
     ----------
 
     mbb_inv: 2d array
       the inverse spin0 and 2 mode coupling matrix
+    cov_T_E_only: boolean
+        if true don't do B
     """
     nbins = mbb_inv["spin0xspin0"].shape[0]
-    mbb_inv_array = np.zeros((4*nbins, 4*nbins))
-    # TT
-    mbb_inv_array[0*nbins:1*nbins, 0*nbins:1*nbins] = mbb_inv["spin0xspin0"]
-    # TE
-    mbb_inv_array[1*nbins:2*nbins, 1*nbins:2*nbins] = mbb_inv["spin0xspin2"]
-    # ET
-    mbb_inv_array[2*nbins:3*nbins, 2*nbins:3*nbins] = mbb_inv["spin2xspin0"]
-    # EE
-    mbb_inv_array[3*nbins:4*nbins, 3*nbins:4*nbins] = mbb_inv["spin2xspin2"][0:nbins, 0:nbins]
+    if cov_T_E_only:
+        mbb_inv_array = np.zeros((4*nbins, 4*nbins))
+        # TT
+        mbb_inv_array[0*nbins:1*nbins, 0*nbins:1*nbins] = mbb_inv["spin0xspin0"]
+        # TE
+        mbb_inv_array[1*nbins:2*nbins, 1*nbins:2*nbins] = mbb_inv["spin0xspin2"]
+        # ET
+        mbb_inv_array[2*nbins:3*nbins, 2*nbins:3*nbins] = mbb_inv["spin2xspin0"]
+        # EE
+        mbb_inv_array[3*nbins:4*nbins, 3*nbins:4*nbins] = mbb_inv["spin2xspin2"][0:nbins, 0:nbins]
+    else:
+        mbb_inv_array = np.zeros((9*nbins, 9*nbins))
+        # TT
+        mbb_inv_array[0*nbins:1*nbins, 0*nbins:1*nbins] = mbb_inv["spin0xspin0"]
+        # TE
+        mbb_inv_array[1*nbins:2*nbins, 1*nbins:2*nbins] = mbb_inv["spin0xspin2"]
+        # TB
+        mbb_inv_array[2*nbins:3*nbins, 2*nbins:3*nbins] = mbb_inv["spin0xspin2"]
+        # ET
+        mbb_inv_array[3*nbins:4*nbins, 3*nbins:4*nbins] = mbb_inv["spin2xspin0"]
+        # BT
+        mbb_inv_array[4*nbins:5*nbins, 4*nbins:5*nbins] = mbb_inv["spin2xspin0"]
+        # EE-EB-BE-BB
+        mbb_inv_array[5*nbins:9*nbins, 5*nbins:9*nbins] = mbb_inv["spin2xspin2"]
 
-    
     return mbb_inv_array
 
 def extract_EEEBBB_mbb(mbb_inv):
     """this routine extract the E and B part of the mode coupling matrix
 
     Parameters
     ----------
 
     mbb_inv: 2d array
         the inverse spin0 and 2 mode coupling matrix
     """
 
     return mbb_inv["spin2xspin2"]
 
+def corr2cov(corr, var):
+    """Go from correlation and variance to covariance matrix
+
+    Parameters
+    ----------
+    corr: 2d array
+      the correlation matrix
+    var: 1d array
+      vector of variance of the random variables
+    """
+    return corr * np.sqrt(var[:, None] * var[None, :])
+
 
-def cov2corr(cov, remove_diag=True):
+def cov2corr(cov, remove_diag=False):
     """Go from covariance to correlation matrix, also setting the diagonal to zero
 
     Parameters
     ----------
     cov: 2d array
       the covariance matrix
     """
 
     d = np.sqrt(cov.diagonal())
     corr = ((cov.T/d).T)/d
     if remove_diag == True:
         corr -= np.identity(cov.shape[0])
     return corr
 
-def selectblock(cov, spectra, n_bins, block="TTTT"):
+def selectblock(cov, spectra_order, n_bins, block="TTTT"):
     """Select a block in a spin0 and 2 covariance matrix
 
     Parameters
     ----------
 
     cov: 2d array
       the covariance matrix
-    spectra: list of strings
+    spectra_order: list of strings
       the arangement of the different block
     n_bins: int
       the number of bins for each block
     block: string
       the block you want to look at
     """
 
-    if spectra == None:
+    if spectra_order == None:
         print ("cov mat of spin 0, no block selection needed")
         return
     else:
         blockindex = {}
-        for c1,s1 in enumerate(spectra):
-            for c2,s2 in enumerate(spectra):
+        for c1,s1 in enumerate(spectra_order):
+            for c2,s2 in enumerate(spectra_order):
                 blockindex[s1 + s2] = [c1 * n_bins, c2 * n_bins]
     id1 = blockindex[block][0]
     id2 = blockindex[block][1]
     cov_select = cov[id1:id1 + n_bins, id2:id2 + n_bins]
     return cov_select
 
+def get_sigma(cov, spectra_order, n_bins, spectrum):
+    """get the error of the spectrum for the given cov mat
+
+    Parameters
+    ----------
+
+    cov: 2d array
+      the covariance matrix
+    spectra_order: list of strings
+      the arangement of the different block
+    n_bins: int
+      the number of bins for each block
+    spectrum: string
+      the spectrum we consider
+    """
+    cov_sub = selectblock(cov, spectra_order, n_bins, block=spectrum+spectrum)
+    err = np.sqrt(cov_sub.diagonal())
+    return err
+
+
+
 def delta2(a, b):
     """Simple delta function
     """
 
     if a == b:
         return 1
     else:
```

### Comparing `pspy-1.5.9/pspy/so_dict.py` & `pspy-1.6/pspy/so_dict.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/so_map.py` & `pspy-1.6/pspy/so_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,16 @@
             the polarisation efficiency
         """
 
         if self.ncomp == 1:
             self.data *= cal
         else:
             self.data[0] *= cal
-            self.data[1] *= cal * pol_eff
-            self.data[2] *= cal * pol_eff
+            self.data[1] *= cal / pol_eff
+            self.data[2] *= cal / pol_eff
 
         return self
 
     def upgrade(self, factor):
         """Upgrade the ``so_map``.
 
         Parameters
@@ -152,25 +152,27 @@
         if self.pixel == "HEALPIX":
             l_max_limit = 3 * self.nside - 1
         elif self.pixel == "CAR":
             cdelt = self.data.wcs.wcs.cdelt[1]
             l_max_limit = 360 / cdelt / 4
         return l_max_limit
 
-    def get_pixwin(self):
+    def get_pixwin(self, order=0):
         """compute the pixel window function corresponding to the map pixellisation
+           order stands for the map making pointing matrix
+           order=0 is Neareast Neighbour while order=1 is bilinear interpolation
         """
         if self.pixel == "HEALPIX":
             pixwin = hp.pixwin(self.nside)
         if self.pixel == "CAR":
-            wy, wx = enmap.calc_window(self.data.shape)
+            wy, wx = enmap.calc_window(self.data.shape, order=order)
             pixwin = (wy[:,None] * wx[None,:])
         return pixwin
 
-    def convolve_with_pixwin(self, niter=3, binary=None, pixwin=None):
+    def convolve_with_pixwin(self, niter=3, binary=None, pixwin=None, order=0):
         """Convolve a ``so_map`` object with a pixel window function
         The convolution is done in harmonics space, for CAR maps
         the pixwin is anisotropic (the pixel varies in size across the maps)
         and the convolution is done in Fourier space.
         We optionaly apply a binary before doing the operation to remove pathological pixels, note
         that this operation is dangerous since we do harmonic transform of a masked map.
 
@@ -185,15 +187,15 @@
         pixwin: 1d array for healpix, 2d array for CAR
             this allow you to pass a precomputed pixel window function
         """
 
         lmax = self.get_lmax_limit()
 
         if binary is not None: self.data *= binary.data
-        if pixwin is None: pixwin = self.get_pixwin()
+        if pixwin is None: pixwin = self.get_pixwin(order=order)
 
         if self.pixel == "HEALPIX":
             alms = map2alm(self, niter, lmax)
             alms = curvedsky.almxfl(alms, pixwin)
             self = alm2map(alms, self)
         if self.pixel == "CAR":
             self = fourier_convolution(self, pixwin)
@@ -576,18 +578,17 @@
       the enmap we want to use to define the ``so_map``
     """
 
     new_map = so_map()
     hdulist = emap.wcs.to_fits()
     header = hdulist[0].header
     new_map.pixel = header["CTYPE1"][-3:]
-    try:
-        new_map.ncomp = header["NAXIS3"]
-    except:
-        new_map.ncomp = 1
+    shape, wcs = emap.geometry
+    new_map.geometry = shape[1:]
+    new_map.ncomp = shape[0]
     new_map.data = emap.copy()
     new_map.nside = None
     new_map.geometry = new_map.data.geometry[1:]
     new_map.coordinate = header["RADESYS"]
     if new_map.coordinate == "ICRS":
         new_map.coordinate = "equ"
```

### Comparing `pspy-1.5.9/pspy/so_map_preprocessing.py` & `pspy-1.6/pspy/so_map_preprocessing.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/so_mcm.py` & `pspy-1.6/pspy/so_mcm.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/so_misc.py` & `pspy-1.6/pspy/so_misc.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/so_mpi.py` & `pspy-1.6/pspy/so_mpi.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/so_spectra.py` & `pspy-1.6/pspy/so_spectra.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/so_window.py` & `pspy-1.6/pspy/so_window.py`

 * *Files 18% similar despite different names*

```diff
@@ -51,18 +51,15 @@
         rmax = None
 
     if apo_type == "C1":
         window = apod_C1(binary, apo_radius_degree, rmax)
     if apo_type == "C2":
         window = apod_C2(binary, apo_radius_degree, rmax)
     if apo_type == "Rectangle":
-        if binary.pixel == "HEALPIX":
-            raise ValueError("No rectangle apodization for HEALPIX map")
-        if binary.pixel == "CAR":
-            window = apod_rectangle(binary, apo_radius_degree)
+        raise ValueError("Not supported anymore")
 
     return window
 
 
 def apod_C2(binary, radius, rmax=None):
     """Create a C2 apodisation as defined in https://arxiv.org/pdf/0903.2350.pdf
 
@@ -107,59 +104,14 @@
         idx = np.where(dist.data > radius)
         win.data = 1.0 / 2 - 1.0 / 2 * np.cos(-np.pi * dist.data / radius)
         win.data[idx] = 1
 
     return win
 
 
-def apod_rectangle(binary, radius):
-    """Create an apodisation for rectangle window (in CAR) (smoother at the corner)
-
-    Parameters
-    ----------
-    binary: ``so_map``
-      a so_map with binary data (1 is observed, 0 is masked)
-    apo_radius: float
-      the apodisation radius in degrees
-
-    """
-
-    # TODO: clean this one
-
-    if radius == 0:
-        return binary
-    else:
-        shape = binary.data.shape
-        wcs = binary.data.wcs
-        Ny, Nx = shape
-        pix_scale_y, pix_scale_x = enmap.pixshape(shape, wcs)
-        win = binary.copy()
-        win.data = win.data * 0 + 1
-        win_x = win.copy()
-        win_y = win.copy()
-        ones = np.ones((Ny, Nx))
-        deg_to_pix_x = np.pi / 180 / pix_scale_x
-        deg_to_pix_y = np.pi / 180 / pix_scale_y
-        lenApod_x = int(radius * deg_to_pix_x)
-        lenApod_y = int(radius * deg_to_pix_y)
-
-        for i in range(lenApod_x):
-            r = float(i)
-            win_x.data[:, i] = 1.0 / 2 * (ones[:, i] - np.cos(-np.pi * r / lenApod_x))
-            win_x.data[:, Nx - i - 1] = win_x.data[:, i]
-        for j in range(lenApod_y):
-            r = float(j)
-            win_y.data[j, :] = 1.0 / 2 * (ones[j, :] - np.cos(-np.pi * r / lenApod_y))
-            win_y.data[Ny - j - 1, :] = win_y.data[j, :]
-
-        win.data = win_x.data * win_y.data
-
-        return win
-
-
 def get_spinned_windows(w, lmax, niter):
     """Compute the spinned window functions (for pure B modes method)
 
     Parameters
     ----------
     w: ``so_map``
       map of the window function
```

### Comparing `pspy-1.5.9/pspy/sph_tools.py` & `pspy-1.6/pspy/sph_tools.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat` & `pspy-1.6/pspy/tests/data/bode_almost_wmap5_lmax_1e4_lensedCls_startAt2.dat`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/tests/data/generate_test_data.py` & `pspy-1.6/pspy/tests/data/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/tests/data/test_data.pkl` & `pspy-1.6/pspy/tests/data/test_data.pkl`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/tests/test_pspy_namaster.py` & `pspy-1.6/pspy/tests/test_pspy_namaster.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/tests/test_so_dict.py` & `pspy-1.6/pspy/tests/test_so_dict.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/tests/test_so_map.py` & `pspy-1.6/pspy/tests/test_so_map.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/tests/test_so_spectra.py` & `pspy-1.6/pspy/tests/test_so_spectra.py`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy/wigner3j/wigner3j_sub.f` & `pspy-1.6/pspy/wigner3j/wigner3j_sub.f`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/pspy.egg-info/PKG-INFO` & `pspy-1.6/pspy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspy
-Version: 1.5.9
+Version: 1.6
 Summary: Python power spectrum code
 Home-page: https://github.com/simonsobs/pspy
 Author: Simons Observatory Collaboration Power Spectrum Task Force
 License: BSD license
 Description: ====
         pspy
         ====
@@ -13,15 +13,15 @@
         ``pspy`` is a cosmology code for calculating CMB power spectra and covariance matrices. See the
         python example notebooks for an introductory set of examples on how to use the package.
         
         .. image:: https://img.shields.io/pypi/v/pspy.svg?style=flat
            :target: https://pypi.python.org/pypi/pspy/
         .. image:: https://img.shields.io/badge/license-BSD-yellow
            :target: https://github.com/simonsobs/pspy/blob/master/LICENSE
-        .. image:: https://img.shields.io/github/workflow/status/simonsobs/pspy/Testing
+        .. image:: https://img.shields.io/github/actions/workflow/status/simonsobs/pspy/testing.yml?branch=master
            :target: https://github.com/simonsobs/pspy/actions?query=workflow%3ATesting
         .. image:: https://readthedocs.org/projects/pspy/badge/?version=latest
            :target: https://pspy.readthedocs.io/en/latest/?badge=latest
         .. image:: https://codecov.io/gh/simonsobs/pspy/branch/master/graph/badge.svg?token=HHAJ7NQ5CE
            :target: https://codecov.io/gh/simonsobs/pspy
         .. image:: https://mybinder.org/badge_logo.svg
            :target: https://mybinder.org/v2/gh/simonsobs/pspy/master?filepath=notebooks/%2Findex.ipynb
@@ -96,9 +96,11 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `pspy-1.5.9/pspy.egg-info/SOURCES.txt` & `pspy-1.6/pspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pspy-1.5.9/setup.py` & `pspy-1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,18 +26,25 @@
 )
 cov = Extension(
     name="pspy.cov_fortran.cov_fortran",
     sources=["pspy/cov_fortran/cov_fortran.f90", "pspy/wigner3j/wigner3j_sub.f"],
     **compile_opts
 )
 
+# The 'build_ext' command from latest versioneer is breaking the data installation from MANIFEST.in
+# Overloading this command with numpy_cmdclass do not solve the issue. So far the only way to
+# install properly the pspy/tests/data is to remove the 'build_ext' command and leave
+# numpy.distutils doing its job
+cmdclass = versioneer.get_cmdclass().copy()
+cmdclass.pop("build_ext")
+
 setup(
     name="pspy",
     version=versioneer.get_version(),
-    cmdclass=versioneer.get_cmdclass(),
+    cmdclass=cmdclass,
     author="Simons Observatory Collaboration Power Spectrum Task Force",
     url="https://github.com/simonsobs/pspy",
     description="Python power spectrum code",
     long_description=readme,
     long_description_content_type="text/x-rst",
     license="BSD license",
     python_requires=">=3.7",
@@ -45,22 +52,23 @@
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     entry_points={},
     ext_modules=[mcm, cov],
     install_requires=[
         "numpy>=1.20",
         "healpy",
         "pyFFTW",
         "pillow",  # this one should be installed by pixell
         "pixell>=0.7.0",
     ],
     packages=find_packages(),
-    package_data={"pspy": ["pspy/tests/data/*.pkl"]},
     include_package_data=True,
     scripts=["scripts/test-pspy"],
 )
```

### Comparing `pspy-1.5.9/versioneer.py` & `pspy-1.6/versioneer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,64 @@
 
-# Version: 0.18
+# Version: 0.28
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
-* https://github.com/warner/python-versioneer
+* https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain
-* Compatible With: python2.6, 2.7, 3.2, 3.3, 3.4, 3.5, 3.6, and pypy
-* [![Latest Version]
-(https://pypip.in/version/versioneer/badge.svg?style=flat)
-](https://pypi.python.org/pypi/versioneer/)
-* [![Build Status]
-(https://travis-ci.org/warner/python-versioneer.png?branch=master)
-](https://travis-ci.org/warner/python-versioneer)
+* License: Public Domain (Unlicense)
+* Compatible with: Python 3.7, 3.8, 3.9, 3.10 and pypy3
+* [![Latest Version][pypi-image]][pypi-url]
+* [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
-* `pip install versioneer` to somewhere to your $PATH
-* add a `[versioneer]` section to your setup.cfg (see below)
-* run `versioneer install` in your source tree, commit the results
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -57,15 +82,15 @@
 unreleased software (between tags), the version identifier should provide
 enough information to help developers recreate the same tree, while also
 giving them an idea of roughly how old the tree is (after version 1.2, before
 version 1.3). Many VCS systems can report a description that captures this,
 for example `git describe --tags --dirty --always` reports things like
 "0.7-1-g574ab98-dirty" to indicate that the checkout is one revision past the
 0.7 tag, has a unique revision id of "574ab98", and is "dirty" (it has
-uncommitted changes.
+uncommitted changes).
 
 The version identifier is used for multiple purposes:
 
 * to allow the module to self-identify its version: `myproject.__version__`
 * to choose a name and prefix for a 'setup.py sdist' tarball
 
 ## Theory of Operation
@@ -162,45 +187,45 @@
 display the full contents of `get_versions()` (including the `error` string,
 which may help identify what went wrong).
 
 ## Known Limitations
 
 Some situations are known to cause problems for Versioneer. This details the
 most significant ones. More can be found on Github
-[issues page](https://github.com/warner/python-versioneer/issues).
+[issues page](https://github.com/python-versioneer/python-versioneer/issues).
 
 ### Subprojects
 
 Versioneer has limited support for source trees in which `setup.py` is not in
 the root directory (e.g. `setup.py` and `.git/` are *not* siblings). The are
 two common reasons why `setup.py` might not be in the root:
 
 * Source trees which contain multiple subprojects, such as
   [Buildbot](https://github.com/buildbot/buildbot), which contains both
   "master" and "slave" subprojects, each with their own `setup.py`,
   `setup.cfg`, and `tox.ini`. Projects like these produce multiple PyPI
   distributions (and upload multiple independently-installable tarballs).
 * Source trees whose main purpose is to contain a C library, but which also
-  provide bindings to Python (and perhaps other langauges) in subdirectories.
+  provide bindings to Python (and perhaps other languages) in subdirectories.
 
 Versioneer will look for `.git` in parent directories, and most operations
 should get the right version string. However `pip` and `setuptools` have bugs
 and implementation details which frequently cause `pip install .` from a
 subproject directory to fail to find a correct version string (so it usually
 defaults to `0+unknown`).
 
 `pip install --editable .` should work correctly. `setup.py install` might
 work too.
 
 Pip-8.1.1 is known to have this problem, but hopefully it will get fixed in
 some later version.
 
-[Bug #38](https://github.com/warner/python-versioneer/issues/38) is tracking
+[Bug #38](https://github.com/python-versioneer/python-versioneer/issues/38) is tracking
 this issue. The discussion in
-[PR #61](https://github.com/warner/python-versioneer/pull/61) describes the
+[PR #61](https://github.com/python-versioneer/python-versioneer/pull/61) describes the
 issue from the Versioneer side in more detail.
 [pip PR#3176](https://github.com/pypa/pip/pull/3176) and
 [pip PR#3615](https://github.com/pypa/pip/pull/3615) contain work to improve
 pip to let Versioneer work correctly.
 
 Versioneer-0.16 and earlier only looked for a `.git` directory next to the
 `setup.cfg`, so subprojects were completely unsupported with those releases.
@@ -220,39 +245,28 @@
 `pkg_resources.DistributionNotFound` errors when running the entrypoint
 script, which must be resolved by re-installing the package. This happens
 when the install happens with one version, then the egg_info data is
 regenerated while a different version is checked out. Many setup.py commands
 cause egg_info to be rebuilt (including `sdist`, `wheel`, and installing into
 a different virtualenv), so this can be surprising.
 
-[Bug #83](https://github.com/warner/python-versioneer/issues/83) describes
+[Bug #83](https://github.com/python-versioneer/python-versioneer/issues/83) describes
 this one, but upgrading to a newer version of setuptools should probably
 resolve it.
 
-### Unicode version strings
-
-While Versioneer works (and is continually tested) with both Python 2 and
-Python 3, it is not entirely consistent with bytes-vs-unicode distinctions.
-Newer releases probably generate unicode version strings on py2. It's not
-clear that this is wrong, but it may be surprising for applications when then
-write these strings to a network connection or include them in bytes-oriented
-APIs like cryptographic checksums.
-
-[Bug #71](https://github.com/warner/python-versioneer/issues/71) investigates
-this question.
-
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -261,36 +275,62 @@
 will take a VCS name as an argument, and will construct a version of
 `versioneer.py` that is specific to the given VCS. It might also take the
 configuration arguments that are currently provided manually during
 installation by editing setup.py . Alternatively, it might go the other
 direction and include code from all supported VCS systems, reducing the
 number of intermediate scripts.
 
+## Similar projects
+
+* [setuptools_scm](https://github.com/pypa/setuptools_scm/) - a non-vendored build-time
+  dependency
+* [minver](https://github.com/jbweston/miniver) - a lightweight reimplementation of
+  versioneer
+* [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
+  plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
+
+[pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
+[pypi-url]: https://pypi.python.org/pypi/versioneer/
+[travis-image]:
+https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
+[travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
 """
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
-from __future__ import print_function
-try:
-    import configparser
-except ImportError:
-    import ConfigParser as configparser
+import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
+from pathlib import Path
+from typing import Callable, Dict
+import functools
+
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
 
 def get_root():
@@ -317,128 +357,144 @@
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
-        me = os.path.realpath(os.path.abspath(__file__))
-        me_dir = os.path.normcase(os.path.splitext(me)[0])
+        my_path = os.path.realpath(os.path.abspath(__file__))
+        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+                  % (os.path.dirname(my_path), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise EnvironmentError (if setup.cfg is missing), or
+    # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.readfp(f)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
-
-    def get(parser, name):
-        if parser.has_option("versioneer", name):
-            return parser.get("versioneer", name)
-        return None
+    root = Path(root)
+    pyproject_toml = root / "pyproject.toml"
+    setup_cfg = root / "setup.cfg"
+    section = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, 'rb') as fobj:
+                pp = tomllib.load(fobj)
+            section = pp['tool']['versioneer']
+        except (tomllib.TOMLDecodeError, KeyError):
+            pass
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
+
+        section = parser["versioneer"]
+
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
-    cfg.style = get(parser, "style") or ""
-    cfg.versionfile_source = get(parser, "versionfile_source")
-    cfg.versionfile_build = get(parser, "versionfile_build")
-    cfg.tag_prefix = get(parser, "tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    cfg.VCS = section['VCS']
+    cfg.style = section.get("style", "")
+    cfg.versionfile_source = section.get("versionfile_source")
+    cfg.versionfile_build = section.get("versionfile_build")
+    cfg.tag_prefix = section.get("tag_prefix")
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
-    cfg.parentdir_prefix = get(parser, "parentdir_prefix")
-    cfg.verbose = get(parser, "verbose")
+    cfg.parentdir_prefix = section.get("parentdir_prefix")
+    cfg.verbose = section.get("verbose")
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
+    """Create decorator to mark a method as the handler of a VCS."""
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
-        if vcs not in HANDLERS:
-            HANDLERS[vcs] = {}
-        HANDLERS[vcs][method] = f
+        HANDLERS.setdefault(vcs, {})[method] = f
         return f
     return decorate
 
 
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
+        except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %s" % (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
-LONG_VERSION_PY['git'] = '''
+LONG_VERSION_PY['git'] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.18 (https://github.com/warner/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.28
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
+from typing import Callable, Dict
+import functools
 
 
 def get_keywords():
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
@@ -468,84 +524,89 @@
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
-LONG_VERSION_PY = {}
-HANDLERS = {}
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
+    """Create decorator to mark a method as the handler of a VCS."""
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
+        except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %%s" %% (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
 def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
@@ -554,75 +615,83 @@
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
 def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %%s" %% r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -630,52 +699,92 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%%s*" %% tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -684,15 +793,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -709,21 +818,22 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def plus_or_dot(pieces):
     """Return a + if we don't already have one, else return a ."""
@@ -753,27 +863,75 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces):
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver):
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces):
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%%d" %% pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%%d" %% pieces["distance"]
+        rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
 def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
@@ -796,20 +954,49 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
+def render_pep440_post_branch(pieces):
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%%d" %% pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%%s" %% pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%%d" %% pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%%s" %% pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
 def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%%d" %% pieces["distance"]
             if pieces["dirty"]:
@@ -872,18 +1059,22 @@
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -911,15 +1102,15 @@
         pass
 
     try:
         root = os.path.realpath(__file__)
         # versionfile_source is the relative path from the top of the source
         # tree (where the .git directory might live) to this file. Invert
         # this to find the root from __file__.
-        for i in cfg.versionfile_source.split('/'):
+        for _ in cfg.versionfile_source.split('/'):
             root = os.path.dirname(root)
     except NameError:
         return {"version": "0+unknown", "full-revisionid": None,
                 "dirty": None,
                 "error": "unable to find root of source tree",
                 "date": None}
 
@@ -946,75 +1137,83 @@
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
 def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %s" % r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -1022,52 +1221,92 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%s*" % tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -1076,15 +1315,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%s'"
                                % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -1101,91 +1340,91 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        me = __file__
-        if me.endswith(".pyc") or me.endswith(".pyo"):
-            me = os.path.splitext(me)[0] + ".py"
-        versioneer_file = os.path.relpath(me)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
-        f = open(".gitattributes", "r")
-        for line in f.readlines():
-            if line.strip().startswith(versionfile_source):
-                if "export-subst" in line.strip().split()[1:]:
-                    present = True
-        f.close()
-    except EnvironmentError:
+        with open(".gitattributes", "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith(versionfile_source):
+                    if "export-subst" in line.strip().split()[1:]:
+                        present = True
+                        break
+    except OSError:
         pass
     if not present:
-        f = open(".gitattributes", "a+")
-        f.write("%s export-subst\n" % versionfile_source)
-        f.close()
+        with open(".gitattributes", "a+") as fobj:
+            fobj.write(f"{versionfile_source} export-subst\n")
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
 def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %s but none started with prefix %s" %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.18) from
+# This file was generated by 'versioneer.py' (0.28) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1199,15 +1438,15 @@
 
 
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
                    contents, re.M | re.S)
     if not mo:
         mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
                        contents, re.M | re.S)
     if not mo:
@@ -1254,27 +1493,75 @@
         rendered = "0+untagged.%d.g%s" % (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces):
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver):
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces):
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%d" % pieces["distance"]
+        rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
 def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
@@ -1297,20 +1584,49 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
+def render_pep440_post_branch(pieces):
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%d" % pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%s" % pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%d" % pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%s" % pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
 def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%d" % pieces["distance"]
             if pieces["dirty"]:
@@ -1373,18 +1689,22 @@
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
@@ -1476,35 +1796,39 @@
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass():
-    """Get the custom setuptools/distutils subclasses used by Versioneer."""
+def get_cmdclass(cmdclass=None):
+    """Get the custom setuptools subclasses used by Versioneer.
+
+    If the package uses a different cmdclass (e.g. one from numpy), it
+    should be provide as an argument.
+    """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
         # 'easy_install .'), in which subdependencies of the main project are
         # built (using setup.py bdist_egg) in the same python process. Assume
         # a main project A and a dependency B, which use different versions
         # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
         # sys.modules by the time B's setup.py is executed, causing B to run
         # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
         # sandbox that restores sys.modules to it's pre-build state, so the
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
-        # Also see https://github.com/warner/python-versioneer/issues/52
+        # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
-    cmds = {}
+    cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to both distutils and setuptools
-    from distutils.core import Command
+    # we add "version" to setuptools
+    from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
         user_options = []
         boolean_options = []
 
         def initialize_options(self):
@@ -1519,50 +1843,89 @@
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
+
     # we override different "build_py" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
+    if 'build_py' in cmds:
+        _build_py = cmds['build_py']
     else:
-        from distutils.command.build_py import build_py as _build_py
+        from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib,
                                                   cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
     cmds["build_py"] = cmd_build_py
 
+    if 'build_ext' in cmds:
+        _build_ext = cmds['build_ext']
+    else:
+        from setuptools.command.build_ext import build_ext as _build_ext
+
+    class cmd_build_ext(_build_ext):
+        def run(self):
+            root = get_root()
+            cfg = get_config_from_root(root)
+            versions = get_versions()
+            _build_ext.run(self)
+            if self.inplace:
+                # build_ext --inplace will only build extensions in
+                # build/lib<..> dir with no _version.py to write to.
+                # As in place builds will already have a _version.py
+                # in the module dir, we do not need to write one.
+                return
+            # now locate _version.py in the new build/ directory and replace
+            # it with an updated value
+            if not cfg.versionfile_build:
+                return
+            target_versionfile = os.path.join(self.build_lib,
+                                              cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print(f"Warning: {target_versionfile} does not exist, skipping "
+                      "version update. This can happen if you are running build_ext "
+                      "without first running build_py.")
+                return
+            print("UPDATING %s" % target_versionfile)
+            write_to_version_file(target_versionfile, versions)
+    cmds["build_ext"] = cmd_build_ext
+
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
@@ -1589,17 +1952,17 @@
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if 'py2exe' in sys.modules:  # py2exe enabled?
         try:
-            from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
+            from py2exe.setuptools_buildexe import py2exe as _py2exe
         except ImportError:
-            from py2exe.build_exe import py2exe as _py2exe  # py2
+            from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
@@ -1615,19 +1978,56 @@
                              "STYLE": cfg.style,
                              "TAG_PREFIX": cfg.tag_prefix,
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
         cmds["py2exe"] = cmd_py2exe
 
+    # sdist farms its file list building out to egg_info
+    if 'egg_info' in cmds:
+        _egg_info = cmds['egg_info']
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info):
+        def find_sources(self):
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super().find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append('versioneer.py')
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
+                          for f in self.filelist.files]
+
+            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
+            with open(manifest_filename, 'w') as fobj:
+                fobj.write('\n'.join(normalized))
+
+    cmds['egg_info'] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
+    if 'sdist' in cmds:
+        _sdist = cmds['sdist']
     else:
-        from distutils.command.sdist import sdist as _sdist
+        from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
         def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
@@ -1683,29 +2083,34 @@
 #versionfile_source =
 #versionfile_build =
 #tag_prefix =
 #parentdir_prefix =
 
 """
 
-INIT_PY_SNIPPET = """
+OLD_SNIPPET = """
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
 """
 
+INIT_PY_SNIPPET = """
+from . import {0}
+__version__ = {0}.get_versions()['version']
+"""
+
 
 def do_setup():
-    """Main VCS-independent setup function for installing Versioneer."""
+    """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
+    except (OSError, configparser.NoSectionError,
             configparser.NoOptionError) as e:
-        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
+        if isinstance(e, (OSError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg",
                   file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
@@ -1721,62 +2126,36 @@
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
                        "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
-        if INIT_PY_SNIPPET not in old:
+        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
+        snippet = INIT_PY_SNIPPET.format(module)
+        if OLD_SNIPPET in old:
+            print(" replacing boilerplate in %s" % ipy)
+            with open(ipy, "w") as f:
+                f.write(old.replace(OLD_SNIPPET, snippet))
+        elif snippet not in old:
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
-                f.write(INIT_PY_SNIPPET)
+                f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
         ipy = None
 
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except EnvironmentError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
-
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, ipy)
     return 0
 
 
 def scan_setup_py():
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
@@ -1809,14 +2188,18 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command():
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```

