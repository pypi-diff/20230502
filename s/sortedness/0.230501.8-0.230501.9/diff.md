# Comparing `tmp/sortedness-0.230501.8.tar.gz` & `tmp/sortedness-0.230501.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortedness-0.230501.8.tar", max compression
+gzip compressed data, was "sortedness-0.230501.9.tar", max compression
```

## Comparing `sortedness-0.230501.8.tar` & `sortedness-0.230501.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35149 2021-05-31 18:06:07.000000 sortedness-0.230501.8/LICENSE
--rw-r--r--   0        0        0     4291 2023-05-01 23:09:49.897114 sortedness-0.230501.8/README.md
--rw-r--r--   0        0        0      648 2023-05-01 23:16:29.856510 sortedness-0.230501.8/build.py
--rw-r--r--   0        0        0     1188 2023-05-02 01:10:21.914263 sortedness-0.230501.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-03 19:59:46.000000 sortedness-0.230501.8/src/sortedness/__init__.py
--rw-r--r--   0        0        0     1281 2023-05-01 23:25:35.123741 sortedness-0.230501.8/src/sortedness/config.py
--rw-r--r--   0        0        0        0 2023-05-01 18:42:18.444309 sortedness-0.230501.8/src/sortedness/evaluation/__init__.py
--rw-r--r--   0        0        0     2238 2023-05-01 21:01:18.170347 sortedness-0.230501.8/src/sortedness/evaluation/plot.py
--rw-r--r--   0        0        0     5145 2023-05-01 21:07:34.442703 sortedness-0.230501.8/src/sortedness/global.py
--rw-r--r--   0        0        0    22749 2023-05-01 23:40:16.090062 sortedness-0.230501.8/src/sortedness/local.py
--rw-r--r--   0        0        0      683 2023-05-01 20:56:36.954018 sortedness-0.230501.8/src/sortedness/matrices.py
--rw-r--r--   0        0        0     2962 2023-05-01 23:15:42.252581 sortedness-0.230501.8/src/sortedness/parallel.py
--rw-r--r--   0        0        0     7950 2022-08-03 19:59:46.000000 sortedness-0.230501.8/src/sortedness/rank.py
--rw-r--r--   0        0        0     4707 2022-08-03 19:59:46.000000 sortedness-0.230501.8/src/sortedness/trustworthiness.py
--rw-r--r--   0        0        0     3511 2023-05-01 23:16:29.848511 sortedness-0.230501.8/src/sortedness/wtau/__init__.py
--rw-r--r--   0        0        0  1265859 2023-05-02 00:51:00.643368 sortedness-0.230501.8/src/sortedness/wtau/wtau.c
--rwxr-xr-x   0        0        0  1129000 2023-05-01 19:08:03.000000 sortedness-0.230501.8/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so
--rw-r--r--   0        0        0   334715 2023-05-02 00:51:00.667368 sortedness-0.230501.8/src/sortedness/wtau/wtau.html
--rw-r--r--   0        0        0     7269 2023-05-01 23:57:54.883837 sortedness-0.230501.8/src/sortedness/wtau/wtau.pyx
--rw-r--r--   0        0        0     5436 1970-01-01 00:00:00.000000 sortedness-0.230501.8/setup.py
--rw-r--r--   0        0        0     4948 1970-01-01 00:00:00.000000 sortedness-0.230501.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-05-31 18:06:07.000000 sortedness-0.230501.9/LICENSE
+-rw-r--r--   0        0        0     4716 2023-05-02 18:09:37.648989 sortedness-0.230501.9/README.md
+-rw-r--r--   0        0        0      648 2023-05-01 23:16:29.856510 sortedness-0.230501.9/build.py
+-rw-r--r--   0        0        0     1188 2023-05-02 18:23:59.744072 sortedness-0.230501.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-08-03 19:59:46.000000 sortedness-0.230501.9/src/sortedness/__init__.py
+-rw-r--r--   0        0        0     1281 2023-05-01 23:25:35.123741 sortedness-0.230501.9/src/sortedness/config.py
+-rw-r--r--   0        0        0        0 2023-05-01 18:42:18.444309 sortedness-0.230501.9/src/sortedness/evaluation/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-01 21:01:18.170347 sortedness-0.230501.9/src/sortedness/evaluation/plot.py
+-rw-r--r--   0        0        0     5145 2023-05-01 21:07:34.442703 sortedness-0.230501.9/src/sortedness/global.py
+-rw-r--r--   0        0        0    22749 2023-05-01 23:40:16.090062 sortedness-0.230501.9/src/sortedness/local.py
+-rw-r--r--   0        0        0      683 2023-05-01 20:56:36.954018 sortedness-0.230501.9/src/sortedness/matrices.py
+-rw-r--r--   0        0        0     2962 2023-05-01 23:15:42.252581 sortedness-0.230501.9/src/sortedness/parallel.py
+-rw-r--r--   0        0        0     7950 2022-08-03 19:59:46.000000 sortedness-0.230501.9/src/sortedness/rank.py
+-rw-r--r--   0        0        0     4707 2022-08-03 19:59:46.000000 sortedness-0.230501.9/src/sortedness/trustworthiness.py
+-rw-r--r--   0        0        0     3511 2023-05-01 23:16:29.848511 sortedness-0.230501.9/src/sortedness/wtau/__init__.py
+-rw-r--r--   0        0        0  1265859 2023-05-02 01:10:35.986249 sortedness-0.230501.9/src/sortedness/wtau/wtau.c
+-rwxr-xr-x   0        0        0  1129000 2023-05-01 19:08:03.000000 sortedness-0.230501.9/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0   334715 2023-05-02 01:10:36.030249 sortedness-0.230501.9/src/sortedness/wtau/wtau.html
+-rw-r--r--   0        0        0     7269 2023-05-01 23:57:54.883837 sortedness-0.230501.9/src/sortedness/wtau/wtau.pyx
+-rw-r--r--   0        0        0     5866 1970-01-01 00:00:00.000000 sortedness-0.230501.9/setup.py
+-rw-r--r--   0        0        0     5373 1970-01-01 00:00:00.000000 sortedness-0.230501.9/PKG-INFO
```

### Comparing `sortedness-0.230501.8/LICENSE` & `sortedness-0.230501.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sortedness-0.230501.8/README.md` & `sortedness-0.230501.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 ![test](https://github.com/sortedness/sortedness/workflows/test/badge.svg)
 [![codecov](https://codecov.io/gh/sortedness/sortedness/branch/main/graph/badge.svg)](https://codecov.io/gh/sortedness/sortedness)
 <a href="https://pypi.org/project/sortedness">
 <img src="https://img.shields.io/github/v/release/sortedness/sortedness?display_name=tag&sort=semver&color=blue" alt="github">
 </a>
-![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)
+![Python version](https://img.shields.io/badge/python-3.8+-blue.svg)
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 <!--- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)
 [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) --->
 [![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness)
 [![Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness)
 
-# sortedness
-
 
+# sortedness
 
 `sortedness` is a measure of quality of data transformation, often dimensionality reduction.
 It is less sensitive to irrelevant distortions and return values in a more meaningful interval than Kruskal stress formula I.
-<br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the stress function presented [here (link broken until the paper is published)](https://arxiv.org/abs/2109.06028.9999).
+<br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the functions presented [here (paper unavailable until publication)](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).
 
 ## Overview
+Local variants return a value for each provided point. The global variant returns a single value for all points.
+Any local variant can be used as a global measure by taking the mean value.
+
+Local variants: `sortedness(X, X_)`, `pwsortedness(X, X_)`, `rsortedness(X, X_)`.
+
+Global variant: `global_sortedness(X, X_)`.
 
 ## Python installation
 ### from package through pip
 ```bash
 # Set up a virtualenv. 
 python3 -m venv venv
 source venv/bin/activate
```

#### html2text {}

```diff
@@ -1,27 +1,33 @@
 ![test](https://github.com/sortedness/sortedness/workflows/test/badge.svg) [!
 [codecov](https://codecov.io/gh/sortedness/sortedness/branch/main/graph/
 badge.svg)](https://codecov.io/gh/sortedness/sortedness) [github] ![Python
-version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg) [!
-[license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https:/
-/www.gnu.org/licenses/gpl-3.0)  [![API documentation](https://img.shields.io/
-badge/doc-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/
-sortedness) [![Downloads](https://static.pepy.tech/badge/sortedness)](https://
-pepy.tech/project/sortedness) # sortedness `sortedness` is a measure of quality
-of data transformation, often dimensionality reduction. It is less sensitive to
+version](https://img.shields.io/badge/python-3.8+-blue.svg) [![license: GPL v3]
+(https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
+licenses/gpl-3.0)  [![API documentation](https://img.shields.io/badge/doc-
+API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness) [!
+[Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/
+project/sortedness) # sortedness `sortedness` is a measure of quality of data
+transformation, often dimensionality reduction. It is less sensitive to
 irrelevant distortions and return values in a more meaningful interval than
 Kruskal stress formula I.
 This [Python library](https://pypi.org/project/sortedness) / [code](https://
 github.com/sortedness/sortedness) provides a reference implementation for the
-stress function presented [here (link broken until the paper is published)]
-(https://arxiv.org/abs/2109.06028.9999). ## Overview ## Python installation ###
-from package through pip ```bash # Set up a virtualenv. python3 -m venv venv
-source venv/bin/activate # Install from PyPI pip install -U sortedness ``` ###
-from source ```bash git clone https://github.com/sortedness/sortedness cd
-sortedness poetry install ``` ### Examples **Sortedness**
+functions presented [here (paper unavailable until publication)](https://
+scholar.google.com/
+scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).
+## Overview Local variants return a value for each provided point. The global
+variant returns a single value for all points. Any local variant can be used as
+a global measure by taking the mean value. Local variants: `sortedness(X, X_)`,
+`pwsortedness(X, X_)`, `rsortedness(X, X_)`. Global variant: `global_sortedness
+(X, X_)`. ## Python installation ### from package through pip ```bash # Set up
+a virtualenv. python3 -m venv venv source venv/bin/activate # Install from PyPI
+pip install -U sortedness ``` ### from source ```bash git clone https://
+github.com/sortedness/sortedness cd sortedness poetry install ``` ### Examples
+**Sortedness**
 ```python3 import numpy as np from numpy.random import permutation from
 sklearn.decomposition import PCA from sortedness.local import sortedness mean =
 (1, 2) cov = np.eye(2) rng = np.random.default_rng(seed=0) original =
 rng.multivariate_normal(mean, cov, size=12) projected2 = PCA
 (n_components=2).fit_transform(original) projected1 = PCA
 (n_components=1).fit_transform(original) np.random.seed(0) projectedrnd =
 permutation(original) s = sortedness(original, original) print(min(s), max(s),
```

### Comparing `sortedness-0.230501.8/build.py` & `sortedness-0.230501.9/build.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230501.8/pyproject.toml` & `sortedness-0.230501.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sortedness"
-version = "0.230501.8"
+version = "0.230501.9"
 description = "Measures of projection quality"
 authors = ["davips <dpsabc@gmail.com>", "tacito <tacito.neves@gmail.com>"]
 license = "GPLv3"
 build = "build.py"  # For Cython. apt-get package needed: python3-numpy
 readme = 'README.md'
 packages = [
     { include = "sortedness", from = "src" }
```

### Comparing `sortedness-0.230501.8/src/sortedness/config.py` & `sortedness-0.230501.9/src/sortedness/config.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230501.8/src/sortedness/evaluation/plot.py` & `sortedness-0.230501.9/src/sortedness/evaluation/plot.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230501.8/src/sortedness/global.py` & `sortedness-0.230501.9/src/sortedness/global.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230501.8/src/sortedness/local.py` & `sortedness-0.230501.9/src/sortedness/local.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230501.8/src/sortedness/matrices.py` & `sortedness-0.230501.9/src/sortedness/matrices.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230501.8/src/sortedness/parallel.py` & `sortedness-0.230501.9/src/sortedness/parallel.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230501.8/src/sortedness/rank.py` & `sortedness-0.230501.9/src/sortedness/rank.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230501.8/src/sortedness/trustworthiness.py` & `sortedness-0.230501.9/src/sortedness/trustworthiness.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230501.8/src/sortedness/wtau/__init__.py` & `sortedness-0.230501.9/src/sortedness/wtau/__init__.py`

 * *Files identical despite different names*

### Comparing `sortedness-0.230501.8/src/sortedness/wtau/wtau.c` & `sortedness-0.230501.9/src/sortedness/wtau/wtau.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/npy_math.h",
-            "/tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/npy_math.h",
+            "/tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O3",
             "-ffast-math",
             "-march=native",
             "-fopenmp"
         ],
         "extra_link_args": [
             "-fopenmp"
         ],
         "include_dirs": [
-            "/tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "sortedness.wtau.wtau",
         "sources": [
             "src/sortedness/wtau/wtau.pyx"
@@ -1130,195 +1130,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1349,42 +1349,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -10654,15 +10654,15 @@
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_perm, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10671,29 +10671,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -10704,15 +10704,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10721,29 +10721,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -10754,15 +10754,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10771,29 +10771,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -10804,15 +10804,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -10821,29 +10821,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -10854,15 +10854,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -10871,29 +10871,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -10904,212 +10904,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11125,15 +11125,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -11141,53 +11141,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -11195,30 +11195,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -11233,15 +11233,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11257,15 +11257,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11273,53 +11273,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -11327,30 +11327,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11365,15 +11365,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11389,15 +11389,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -11405,53 +11405,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -11459,30 +11459,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -11497,176 +11497,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -25652,26 +25652,26 @@
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_No_matching_signature_found); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_Function_call_with_ambiguous_arg); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../../../../tmp/tmp1s_vdu8t/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/tmpo6c436rj/.venv/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 950, __pyx_L1_error)
```

### Comparing `sortedness-0.230501.8/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so` & `sortedness-0.230501.9/src/sortedness/wtau/wtau.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `sortedness-0.230501.8/src/sortedness/wtau/wtau.html` & `sortedness-0.230501.9/src/sortedness/wtau/wtau.html`

 * *Files identical despite different names*

### Comparing `sortedness-0.230501.8/src/sortedness/wtau/wtau.pyx` & `sortedness-0.230501.9/src/sortedness/wtau/wtau.pyx`

 * *Files identical despite different names*

### Comparing `sortedness-0.230501.8/setup.py` & `sortedness-0.230501.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'shelchemy>=0.220906.5,<0.220907.0']
 
 extras_require = \
 {':python_version >= "3.8" and python_version < "3.11"': ['scipy>=1.10.1,<2.0.0']}
 
 setup_kwargs = {
     'name': 'sortedness',
-    'version': '0.230501.8',
+    'version': '0.230501.9',
     'description': 'Measures of projection quality',
-    'long_description': '![test](https://github.com/sortedness/sortedness/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/sortedness/sortedness/branch/main/graph/badge.svg)](https://codecov.io/gh/sortedness/sortedness)\n<a href="https://pypi.org/project/sortedness">\n<img src="https://img.shields.io/github/v/release/sortedness/sortedness?display_name=tag&sort=semver&color=blue" alt="github">\n</a>\n![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n<!--- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)\n[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) --->\n[![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness)\n[![Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness)\n\n# sortedness\n\n\n\n`sortedness` is a measure of quality of data transformation, often dimensionality reduction.\nIt is less sensitive to irrelevant distortions and return values in a more meaningful interval than Kruskal stress formula I.\n<br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the stress function presented [here (link broken until the paper is published)](https://arxiv.org/abs/2109.06028.9999).\n\n## Overview\n\n## Python installation\n### from package through pip\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip install -U sortedness\n```\n\n### from source\n```bash\ngit clone https://github.com/sortedness/sortedness\ncd sortedness\npoetry install\n```\n\n\n### Examples\n\n**Sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness.local import sortedness\n\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\ns = sortedness(original, original)\nprint(min(s), max(s), s)\n"""\n1.0 1.0 [1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1.]\n"""\n```\n\n```python3\n\ns = sortedness(original, projected2)\nprint(min(s), max(s), s)\n"""\n1.0 1.0 [1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1.]\n"""\n```\n\n```python3\n\ns = sortedness(original, projected1)\nprint(min(s), max(s), s)\n"""\n0.432937128932 0.944810120534 [0.43293713 0.53333015 0.88412753 0.94481012 0.81485109 0.81330052\n 0.76691474 0.91169619 0.88998817 0.90102615 0.61372341 0.86996213]\n"""\n```\n\n```python3\n\ns = sortedness(original, projectedrnd)\n```\n\n\n</p>\n</details>\n\n**Pairwise sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness.local import pwsortedness\n\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\ns = pwsortedness(original, original)\nprint(min(s), max(s), s)\n"""\n1.0 1.0 [1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1.]\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected2)\nprint(min(s), max(s), s)\n"""\n1.0 1.0 [1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1.]\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected1)\nprint(min(s), max(s), s)\n"""\n0.730078995423 0.837310352695 [0.75892647 0.730079   0.83496865 0.73161226 0.75376525 0.83301104\n 0.76695755 0.74759156 0.81434161 0.74067221 0.74425225 0.83731035]\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projectedrnd)\n```\n\n```python3\nprint(min(s), max(s), s)\n\n"""\n-0.198780473657 0.147224384381 [-0.19878047 -0.14125391  0.03276727 -0.092844   -0.0866695   0.14722438\n -0.07603536 -0.08916877 -0.1373848  -0.10933483 -0.07774488  0.05404383]\n"""\n```\n\n\n</p>\n</details>\n\n\n** Copyright (c) 2022. Davi Pereira dos Santos and Tacito Neves**\n\n\n\n\n\n## Grants\n',
+    'long_description': '![test](https://github.com/sortedness/sortedness/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/sortedness/sortedness/branch/main/graph/badge.svg)](https://codecov.io/gh/sortedness/sortedness)\n<a href="https://pypi.org/project/sortedness">\n<img src="https://img.shields.io/github/v/release/sortedness/sortedness?display_name=tag&sort=semver&color=blue" alt="github">\n</a>\n![Python version](https://img.shields.io/badge/python-3.8+-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n<!--- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)\n[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) --->\n[![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness)\n[![Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness)\n\n\n# sortedness\n\n`sortedness` is a measure of quality of data transformation, often dimensionality reduction.\nIt is less sensitive to irrelevant distortions and return values in a more meaningful interval than Kruskal stress formula I.\n<br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the functions presented [here (paper unavailable until publication)](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).\n\n## Overview\nLocal variants return a value for each provided point. The global variant returns a single value for all points.\nAny local variant can be used as a global measure by taking the mean value.\n\nLocal variants: `sortedness(X, X_)`, `pwsortedness(X, X_)`, `rsortedness(X, X_)`.\n\nGlobal variant: `global_sortedness(X, X_)`.\n\n## Python installation\n### from package through pip\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip install -U sortedness\n```\n\n### from source\n```bash\ngit clone https://github.com/sortedness/sortedness\ncd sortedness\npoetry install\n```\n\n\n### Examples\n\n**Sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness.local import sortedness\n\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\ns = sortedness(original, original)\nprint(min(s), max(s), s)\n"""\n1.0 1.0 [1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1.]\n"""\n```\n\n```python3\n\ns = sortedness(original, projected2)\nprint(min(s), max(s), s)\n"""\n1.0 1.0 [1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1.]\n"""\n```\n\n```python3\n\ns = sortedness(original, projected1)\nprint(min(s), max(s), s)\n"""\n0.432937128932 0.944810120534 [0.43293713 0.53333015 0.88412753 0.94481012 0.81485109 0.81330052\n 0.76691474 0.91169619 0.88998817 0.90102615 0.61372341 0.86996213]\n"""\n```\n\n```python3\n\ns = sortedness(original, projectedrnd)\n```\n\n\n</p>\n</details>\n\n**Pairwise sortedness**\n<details>\n<p>\n\n```python3\n\nimport numpy as np\nfrom numpy.random import permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness.local import pwsortedness\n\nmean = (1, 2)\ncov = np.eye(2)\nrng = np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov, size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd = permutation(original)\n\ns = pwsortedness(original, original)\nprint(min(s), max(s), s)\n"""\n1.0 1.0 [1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1.]\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected2)\nprint(min(s), max(s), s)\n"""\n1.0 1.0 [1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1. 1.]\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projected1)\nprint(min(s), max(s), s)\n"""\n0.730078995423 0.837310352695 [0.75892647 0.730079   0.83496865 0.73161226 0.75376525 0.83301104\n 0.76695755 0.74759156 0.81434161 0.74067221 0.74425225 0.83731035]\n"""\n```\n\n```python3\n\ns = pwsortedness(original, projectedrnd)\n```\n\n```python3\nprint(min(s), max(s), s)\n\n"""\n-0.198780473657 0.147224384381 [-0.19878047 -0.14125391  0.03276727 -0.092844   -0.0866695   0.14722438\n -0.07603536 -0.08916877 -0.1373848  -0.10933483 -0.07774488  0.05404383]\n"""\n```\n\n\n</p>\n</details>\n\n\n** Copyright (c) 2022. Davi Pereira dos Santos and Tacito Neves**\n\n\n\n\n\n## Grants\n',
     'author': 'davips',
     'author_email': 'dpsabc@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,36 +1,41 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['sortedness', 'sortedness.evaluation', 'sortedness.wtau']
 package_data = \ {'': ['*']} install_requires = \ ['lange>=1.230203.1,<2.0.0',
 'pathos>=0.3.0,<0.4.0', 'shelchemy>=0.220906.5,<0.220907.0'] extras_require = \
 {':python_version >= "3.8" and python_version < "3.11"':
 ['scipy>=1.10.1,<2.0.0']} setup_kwargs = { 'name': 'sortedness', 'version':
-'0.230501.8', 'description': 'Measures of projection quality',
+'0.230501.9', 'description': 'Measures of projection quality',
 'long_description': '![test](https://github.com/sortedness/sortedness/
 workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/sortedness/
 sortedness/branch/main/graph/badge.svg)](https://codecov.io/gh/sortedness/
 sortedness)\n\n[github]\n\n![Python version](https://img.shields.io/badge/
-python-3.8%20%7C%203.9-blue.svg)\n[![license: GPL v3](https://img.shields.io/
-badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n\n[!
-[API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-
-a0a0a0.svg)](https://sortedness.github.io/sortedness)\n[![Downloads](https://
-static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness)\n\n#
-sortedness\n\n\n\n`sortedness` is a measure of quality of data transformation,
-often dimensionality reduction.\nIt is less sensitive to irrelevant distortions
-and return values in a more meaningful interval than Kruskal stress formula
-I.\n
+python-3.8+-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/
+License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n\n[![API
+documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)]
+(https://sortedness.github.io/sortedness)\n[![Downloads](https://
+static.pepy.tech/badge/sortedness)](https://pepy.tech/project/
+sortedness)\n\n\n# sortedness\n\n`sortedness` is a measure of quality of data
+transformation, often dimensionality reduction.\nIt is less sensitive to
+irrelevant distortions and return values in a more meaningful interval than
+Kruskal stress formula I.\n
 This [Python library](https://pypi.org/project/sortedness) / [code](https://
 github.com/sortedness/sortedness) provides a reference implementation for the
-stress function presented [here (link broken until the paper is published)]
-(https://arxiv.org/abs/2109.06028.9999).\n\n## Overview\n\n## Python
-installation\n### from package through pip\n```bash\n# Set up a virtualenv.
-\npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip
-install -U sortedness\n```\n\n### from source\n```bash\ngit clone https://
-github.com/sortedness/sortedness\ncd sortedness\npoetry install\n```\n\n\n###
-Examples\n\n**Sortedness**\n\n
+functions presented [here (paper unavailable until publication)](https://
+scholar.google.com/
+scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).\n\n##
+Overview\nLocal variants return a value for each provided point. The global
+variant returns a single value for all points.\nAny local variant can be used
+as a global measure by taking the mean value.\n\nLocal variants: `sortedness(X,
+X_)`, `pwsortedness(X, X_)`, `rsortedness(X, X_)`.\n\nGlobal variant:
+`global_sortedness(X, X_)`.\n\n## Python installation\n### from package through
+pip\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/
+activate\n\n# Install from PyPI\npip install -U sortedness\n```\n\n### from
+source\n```bash\ngit clone https://github.com/sortedness/sortedness\ncd
+sortedness\npoetry install\n```\n\n\n### Examples\n\n**Sortedness**\n\n
 \n\n```python3\n\nimport numpy as np\nfrom numpy.random import
 permutation\nfrom sklearn.decomposition import PCA\n\nfrom sortedness.local
 import sortedness\n\nmean = (1, 2)\ncov = np.eye(2)\nrng =
 np.random.default_rng(seed=0)\noriginal = rng.multivariate_normal(mean, cov,
 size=12)\nprojected2 = PCA(n_components=2).fit_transform(original)\nprojected1
 = PCA(n_components=1).fit_transform(original)\nnp.random.seed(0)\nprojectedrnd
 = permutation(original)\n\ns = sortedness(original, original)\nprint(min(s),
```

### Comparing `sortedness-0.230501.8/PKG-INFO` & `sortedness-0.230501.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortedness
-Version: 0.230501.8
+Version: 0.230501.9
 Summary: Measures of projection quality
 License: GPLv3
 Author: davips
 Author-email: dpsabc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -17,31 +17,36 @@
 Description-Content-Type: text/markdown
 
 ![test](https://github.com/sortedness/sortedness/workflows/test/badge.svg)
 [![codecov](https://codecov.io/gh/sortedness/sortedness/branch/main/graph/badge.svg)](https://codecov.io/gh/sortedness/sortedness)
 <a href="https://pypi.org/project/sortedness">
 <img src="https://img.shields.io/github/v/release/sortedness/sortedness?display_name=tag&sort=semver&color=blue" alt="github">
 </a>
-![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)
+![Python version](https://img.shields.io/badge/python-3.8+-blue.svg)
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 <!--- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)
 [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) --->
 [![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness)
 [![Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness)
 
-# sortedness
-
 
+# sortedness
 
 `sortedness` is a measure of quality of data transformation, often dimensionality reduction.
 It is less sensitive to irrelevant distortions and return values in a more meaningful interval than Kruskal stress formula I.
-<br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the stress function presented [here (link broken until the paper is published)](https://arxiv.org/abs/2109.06028.9999).
+<br>This [Python library](https://pypi.org/project/sortedness) / [code](https://github.com/sortedness/sortedness) provides a reference implementation for the functions presented [here (paper unavailable until publication)](https://scholar.google.com/scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).
 
 ## Overview
+Local variants return a value for each provided point. The global variant returns a single value for all points.
+Any local variant can be used as a global measure by taking the mean value.
+
+Local variants: `sortedness(X, X_)`, `pwsortedness(X, X_)`, `rsortedness(X, X_)`.
+
+Global variant: `global_sortedness(X, X_)`.
 
 ## Python installation
 ### from package through pip
 ```bash
 # Set up a virtualenv. 
 python3 -m venv venv
 source venv/bin/activate
```

#### html2text {}

```diff
@@ -1,36 +1,41 @@
-Metadata-Version: 2.1 Name: sortedness Version: 0.230501.8 Summary: Measures of
+Metadata-Version: 2.1 Name: sortedness Version: 0.230501.9 Summary: Measures of
 projection quality License: GPLv3 Author: davips Author-email: dpsabc@gmail.com
 Requires-Python: >=3.10,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lange (>=1.230203.1,<2.0.0) Requires-Dist: pathos
 (>=0.3.0,<0.4.0) Requires-Dist: scipy (>=1.10.1,<2.0.0) ; python_version >=
 "3.8" and python_version < "3.11" Requires-Dist: shelchemy
 (>=0.220906.5,<0.220907.0) Description-Content-Type: text/markdown ![test]
 (https://github.com/sortedness/sortedness/workflows/test/badge.svg) [![codecov]
 (https://codecov.io/gh/sortedness/sortedness/branch/main/graph/badge.svg)]
 (https://codecov.io/gh/sortedness/sortedness) [github] ![Python version](https:
-//img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg) [![license: GPL v3]
-(https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
-licenses/gpl-3.0)  [![API documentation](https://img.shields.io/badge/doc-
-API%20%28auto%29-a0a0a0.svg)](https://sortedness.github.io/sortedness) [!
-[Downloads](https://static.pepy.tech/badge/sortedness)](https://pepy.tech/
-project/sortedness) # sortedness `sortedness` is a measure of quality of data
-transformation, often dimensionality reduction. It is less sensitive to
-irrelevant distortions and return values in a more meaningful interval than
-Kruskal stress formula I.
+//img.shields.io/badge/python-3.8+-blue.svg) [![license: GPL v3](https://
+img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
+3.0)  [![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-
+a0a0a0.svg)](https://sortedness.github.io/sortedness) [![Downloads](https://
+static.pepy.tech/badge/sortedness)](https://pepy.tech/project/sortedness) #
+sortedness `sortedness` is a measure of quality of data transformation, often
+dimensionality reduction. It is less sensitive to irrelevant distortions and
+return values in a more meaningful interval than Kruskal stress formula I.
 This [Python library](https://pypi.org/project/sortedness) / [code](https://
 github.com/sortedness/sortedness) provides a reference implementation for the
-stress function presented [here (link broken until the paper is published)]
-(https://arxiv.org/abs/2109.06028.9999). ## Overview ## Python installation ###
-from package through pip ```bash # Set up a virtualenv. python3 -m venv venv
-source venv/bin/activate # Install from PyPI pip install -U sortedness ``` ###
-from source ```bash git clone https://github.com/sortedness/sortedness cd
-sortedness poetry install ``` ### Examples **Sortedness**
+functions presented [here (paper unavailable until publication)](https://
+scholar.google.com/
+scholar?hl=en&as_sdt=0%2C5&q=Nonparametric+Dimensionality+Reduction+Quality+Assessment+based+on+Sortedness+of+Unrestricted+Neighborhood&btnG=).
+## Overview Local variants return a value for each provided point. The global
+variant returns a single value for all points. Any local variant can be used as
+a global measure by taking the mean value. Local variants: `sortedness(X, X_)`,
+`pwsortedness(X, X_)`, `rsortedness(X, X_)`. Global variant: `global_sortedness
+(X, X_)`. ## Python installation ### from package through pip ```bash # Set up
+a virtualenv. python3 -m venv venv source venv/bin/activate # Install from PyPI
+pip install -U sortedness ``` ### from source ```bash git clone https://
+github.com/sortedness/sortedness cd sortedness poetry install ``` ### Examples
+**Sortedness**
 ```python3 import numpy as np from numpy.random import permutation from
 sklearn.decomposition import PCA from sortedness.local import sortedness mean =
 (1, 2) cov = np.eye(2) rng = np.random.default_rng(seed=0) original =
 rng.multivariate_normal(mean, cov, size=12) projected2 = PCA
 (n_components=2).fit_transform(original) projected1 = PCA
 (n_components=1).fit_transform(original) np.random.seed(0) projectedrnd =
 permutation(original) s = sortedness(original, original) print(min(s), max(s),
```

