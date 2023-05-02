# Comparing `tmp/matadi-0.1.8.tar.gz` & `tmp/matadi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matadi-0.1.8.tar", last modified: Sun Aug 14 21:57:20 2022, max compression
+gzip compressed data, was "matadi-0.1.9.tar", last modified: Sun Aug 14 22:36:21 2022, max compression
```

## Comparing `matadi-0.1.8.tar` & `matadi-0.1.9.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 21:57:20.689609 matadi-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-08-14 21:57:06.000000 matadi-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    60001 2022-08-14 21:57:20.689609 matadi-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18043 2022-08-14 21:57:06.000000 matadi-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 21:57:20.685609 matadi-0.1.8/matadi/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/_apply.py
--rw-r--r--   0 runner    (1001) docker     (121)    11132 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/_lab_compressible.py
--rw-r--r--   0 runner    (1001) docker     (121)     7941 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/_lab_incompressible.py
--rw-r--r--   0 runner    (1001) docker     (121)     8804 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/_material.py
--rw-r--r--   0 runner    (1001) docker     (121)     6800 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/_templates.py
--rw-r--r--   0 runner    (1001) docker     (121)     2918 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/math.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 21:57:20.685609 matadi-0.1.8/matadi/models/
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/models/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/models/_hyperelasticity_anisotropic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2577 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/models/_hyperelasticity_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1971 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/models/_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/models/_pseudo_elasticity.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 21:57:20.685609 matadi-0.1.8/matadi/models/microsphere/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/models/microsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/models/microsphere/_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 21:57:20.685609 matadi-0.1.8/matadi/models/microsphere/affine/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/models/microsphere/affine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/models/microsphere/affine/_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 21:57:20.689609 matadi-0.1.8/matadi/models/microsphere/nonaffine/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/models/microsphere/nonaffine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/models/microsphere/nonaffine/_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 21:57:20.689609 matadi-0.1.8/matadi/models/microsphere/quadrature/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/models/microsphere/quadrature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-08-14 21:57:06.000000 matadi-0.1.8/matadi/models/microsphere/quadrature/_bazant_oh.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 21:57:20.685609 matadi-0.1.8/matadi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    60001 2022-08-14 21:57:20.000000 matadi-0.1.8/matadi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-08-14 21:57:20.000000 matadi-0.1.8/matadi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-14 21:57:20.000000 matadi-0.1.8/matadi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-14 21:57:20.000000 matadi-0.1.8/matadi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-14 21:57:20.000000 matadi-0.1.8/matadi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-08-14 21:57:06.000000 matadi-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-08-14 21:57:20.693609 matadi-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 21:57:20.689609 matadi-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-14 21:57:06.000000 matadi-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3476 2022-08-14 21:57:06.000000 matadi-0.1.8/tests/test_displacement-pressure.py
--rw-r--r--   0 runner    (1001) docker     (121)     2658 2022-08-14 21:57:06.000000 matadi-0.1.8/tests/test_eigvals_grad.py
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-08-14 21:57:06.000000 matadi-0.1.8/tests/test_fiber.py
--rw-r--r--   0 runner    (1001) docker     (121)     3567 2022-08-14 21:57:06.000000 matadi-0.1.8/tests/test_lab.py
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-08-14 21:57:06.000000 matadi-0.1.8/tests/test_microsphere.py
--rw-r--r--   0 runner    (1001) docker     (121)     6690 2022-08-14 21:57:06.000000 matadi-0.1.8/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3375 2022-08-14 21:57:06.000000 matadi-0.1.8/tests/test_plane.py
--rw-r--r--   0 runner    (1001) docker     (121)     3124 2022-08-14 21:57:06.000000 matadi-0.1.8/tests/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3933 2022-08-14 21:57:06.000000 matadi-0.1.8/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.782534 matadi-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-08-14 22:36:13.000000 matadi-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    60192 2022-08-14 22:36:21.782534 matadi-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    18234 2022-08-14 22:36:13.000000 matadi-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.778534 matadi-0.1.9/matadi/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/_apply.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11132 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/_lab_compressible.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7941 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/_lab_incompressible.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8804 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/_material.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6800 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2918 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/math.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.778534 matadi-0.1.9/matadi/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/_hyperelasticity_anisotropic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2577 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/_hyperelasticity_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/_pseudo_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2382 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.778534 matadi-0.1.9/matadi/models/microsphere/
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.778534 matadi-0.1.9/matadi/models/microsphere/affine/
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/affine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/affine/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.778534 matadi-0.1.9/matadi/models/microsphere/nonaffine/
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/nonaffine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/nonaffine/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.778534 matadi-0.1.9/matadi/models/microsphere/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/quadrature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-08-14 22:36:13.000000 matadi-0.1.9/matadi/models/microsphere/quadrature/_bazant_oh.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.778534 matadi-0.1.9/matadi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    60192 2022-08-14 22:36:21.000000 matadi-0.1.9/matadi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-08-14 22:36:21.000000 matadi-0.1.9/matadi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-14 22:36:21.000000 matadi-0.1.9/matadi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-14 22:36:21.000000 matadi-0.1.9/matadi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-14 22:36:21.000000 matadi-0.1.9/matadi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-08-14 22:36:13.000000 matadi-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-08-14 22:36:21.782534 matadi-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:21.782534 matadi-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3476 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_displacement-pressure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2658 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_eigvals_grad.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_fiber.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3567 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_lab.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_microsphere.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6690 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3375 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_plane.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3124 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3933 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (121)      697 2022-08-14 22:36:13.000000 matadi-0.1.9/tests/test_template-materials.py
```

### Comparing `matadi-0.1.8/LICENSE` & `matadi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/PKG-INFO` & `matadi-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matadi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Material Definition with Automatic Differentiation
 Home-page: https://github.com/adtzlr/matadi
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -954,15 +954,15 @@
 for a in range(3):
     defgrad[a, a] += 1.0
 
 dWdF, dWdp, statevars_new = NH.function([defgrad, pressure, statevars])
 d2WdFdF, d2WdFdp, d2Wdpdp = NH.gradient([defgrad, pressure, statevars])
 ```
 
-**Hint**: *The state variable concept is also implemented for the `Material` class.*
+**Hint**: *The above Neo-Hooke as well as the MORPH material model formulation within the u/p-framework are available as template-materials in `matadi.models` as `NeoHookeOgdenRoxburgh()`and `Morph()`. The state variable concept is also implemented for the `Material` class.*
 
 Simple examples for using `matadi` with [`scikit-fem`](https://github.com/adtzlr/matadi/discussions/14#) as well as with [`felupe`](https://github.com/adtzlr/matadi/discussions/22) are shown in the Discussion section.
 
 ## References
 [1] J. A. E. Andersson, J. Gillis, G. Horn, J. B. Rawlings, and M. Diehl, *CasADi - A software framework for nonlinear optimization and optimal control*, Math. Prog. Comp., vol. 11, no. 1, pp. 1–36, 2019, [![DOI:10.1007/s12532-018-0139-4](https://zenodo.org/badge/DOI/10.1007/s12532-018-0139-4.svg)](https://doi.org/10.1007/s12532-018-0139-4)
 
 [2] C. Miehe, S. Göktepe and F. Lulei, *A micro-macro approach to rubber-like materials. Part I: the non-affine micro-sphere model of rubber elasticity*, Journal of the Mechanics and Physics of Solids, vol. 52, no. 11. Elsevier BV, pp. 2617–2660, Nov. 2004. [![DOI:10.1016/j.jmps.2004.03.011](https://zenodo.org/badge/DOI/10.1016/j.jmps.2004.03.011.svg)](https://doi.org/10.1016/j.jmps.2004.03.011)
```

### Comparing `matadi-0.1.8/README.md` & `matadi-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
 for a in range(3):
     defgrad[a, a] += 1.0
 
 dWdF, dWdp, statevars_new = NH.function([defgrad, pressure, statevars])
 d2WdFdF, d2WdFdp, d2Wdpdp = NH.gradient([defgrad, pressure, statevars])
 ```
 
-**Hint**: *The state variable concept is also implemented for the `Material` class.*
+**Hint**: *The above Neo-Hooke as well as the MORPH material model formulation within the u/p-framework are available as template-materials in `matadi.models` as `NeoHookeOgdenRoxburgh()`and `Morph()`. The state variable concept is also implemented for the `Material` class.*
 
 Simple examples for using `matadi` with [`scikit-fem`](https://github.com/adtzlr/matadi/discussions/14#) as well as with [`felupe`](https://github.com/adtzlr/matadi/discussions/22) are shown in the Discussion section.
 
 ## References
 [1] J. A. E. Andersson, J. Gillis, G. Horn, J. B. Rawlings, and M. Diehl, *CasADi - A software framework for nonlinear optimization and optimal control*, Math. Prog. Comp., vol. 11, no. 1, pp. 1–36, 2019, [![DOI:10.1007/s12532-018-0139-4](https://zenodo.org/badge/DOI/10.1007/s12532-018-0139-4.svg)](https://doi.org/10.1007/s12532-018-0139-4)
 
 [2] C. Miehe, S. Göktepe and F. Lulei, *A micro-macro approach to rubber-like materials. Part I: the non-affine micro-sphere model of rubber elasticity*, Journal of the Mechanics and Physics of Solids, vol. 52, no. 11. Elsevier BV, pp. 2617–2660, Nov. 2004. [![DOI:10.1016/j.jmps.2004.03.011](https://zenodo.org/badge/DOI/10.1016/j.jmps.2004.03.011.svg)](https://doi.org/10.1016/j.jmps.2004.03.011)
```

### Comparing `matadi-0.1.8/matadi/__init__.py` & `matadi-0.1.9/matadi/__init__.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi/_apply.py` & `matadi-0.1.9/matadi/_apply.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi/_lab_compressible.py` & `matadi-0.1.9/matadi/_lab_compressible.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi/_lab_incompressible.py` & `matadi-0.1.9/matadi/_lab_incompressible.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi/_material.py` & `matadi-0.1.9/matadi/_material.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi/_templates.py` & `matadi-0.1.9/matadi/_templates.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi/math.py` & `matadi-0.1.9/matadi/math.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi/models/__init__.py` & `matadi-0.1.9/matadi/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,7 +24,9 @@
 )
 
 from ._pseudo_elasticity import ogden_roxburgh
 from ._misc import morph
 
 from . import microsphere
 from .microsphere.nonaffine import miehe_goektepe_lulei
+
+from ._templates import NeoHookeOgdenRoxburgh, Morph
```

### Comparing `matadi-0.1.8/matadi/models/_helpers.py` & `matadi-0.1.9/matadi/models/_helpers.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi/models/_hyperelasticity_anisotropic.py` & `matadi-0.1.9/matadi/models/_hyperelasticity_anisotropic.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi/models/_hyperelasticity_isotropic.py` & `matadi-0.1.9/matadi/models/_hyperelasticity_isotropic.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi/models/_misc.py` & `matadi-0.1.9/matadi/models/_misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     tresca,
     mexp,
     gradient,
 )
 
 
 def morph(x, p1, p2, p3, p4, p5, p6, p7, p8):
-    "MORPH consitututive material formulation."
+    "MORPH consitutive material formulation."
 
     # split input into the deformation gradient and the vector of state variables
     F, statevars = x[0], x[-1]
 
     # split state variables
     CTSn, Cn, SZn = vertsplit(statevars, [0, 1, 7, 13])
     Cn, SZn = astensor(Cn), astensor(SZn)
```

### Comparing `matadi-0.1.8/matadi/models/_pseudo_elasticity.py` & `matadi-0.1.9/matadi/models/_pseudo_elasticity.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi/models/microsphere/_chain.py` & `matadi-0.1.9/matadi/models/microsphere/_chain.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi/models/microsphere/affine/_models.py` & `matadi-0.1.9/matadi/models/microsphere/affine/_models.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi/models/microsphere/nonaffine/_models.py` & `matadi-0.1.9/matadi/models/microsphere/nonaffine/_models.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi/models/microsphere/quadrature/_bazant_oh.py` & `matadi-0.1.9/matadi/models/microsphere/quadrature/_bazant_oh.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/matadi.egg-info/PKG-INFO` & `matadi-0.1.9/matadi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matadi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Material Definition with Automatic Differentiation
 Home-page: https://github.com/adtzlr/matadi
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -954,15 +954,15 @@
 for a in range(3):
     defgrad[a, a] += 1.0
 
 dWdF, dWdp, statevars_new = NH.function([defgrad, pressure, statevars])
 d2WdFdF, d2WdFdp, d2Wdpdp = NH.gradient([defgrad, pressure, statevars])
 ```
 
-**Hint**: *The state variable concept is also implemented for the `Material` class.*
+**Hint**: *The above Neo-Hooke as well as the MORPH material model formulation within the u/p-framework are available as template-materials in `matadi.models` as `NeoHookeOgdenRoxburgh()`and `Morph()`. The state variable concept is also implemented for the `Material` class.*
 
 Simple examples for using `matadi` with [`scikit-fem`](https://github.com/adtzlr/matadi/discussions/14#) as well as with [`felupe`](https://github.com/adtzlr/matadi/discussions/22) are shown in the Discussion section.
 
 ## References
 [1] J. A. E. Andersson, J. Gillis, G. Horn, J. B. Rawlings, and M. Diehl, *CasADi - A software framework for nonlinear optimization and optimal control*, Math. Prog. Comp., vol. 11, no. 1, pp. 1–36, 2019, [![DOI:10.1007/s12532-018-0139-4](https://zenodo.org/badge/DOI/10.1007/s12532-018-0139-4.svg)](https://doi.org/10.1007/s12532-018-0139-4)
 
 [2] C. Miehe, S. Göktepe and F. Lulei, *A micro-macro approach to rubber-like materials. Part I: the non-affine micro-sphere model of rubber elasticity*, Journal of the Mechanics and Physics of Solids, vol. 52, no. 11. Elsevier BV, pp. 2617–2660, Nov. 2004. [![DOI:10.1016/j.jmps.2004.03.011](https://zenodo.org/badge/DOI/10.1016/j.jmps.2004.03.011.svg)](https://doi.org/10.1016/j.jmps.2004.03.011)
```

### Comparing `matadi-0.1.8/matadi.egg-info/SOURCES.txt` & `matadi-0.1.9/matadi.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 matadi.egg-info/top_level.txt
 matadi/models/__init__.py
 matadi/models/_helpers.py
 matadi/models/_hyperelasticity_anisotropic.py
 matadi/models/_hyperelasticity_isotropic.py
 matadi/models/_misc.py
 matadi/models/_pseudo_elasticity.py
+matadi/models/_templates.py
 matadi/models/microsphere/__init__.py
 matadi/models/microsphere/_chain.py
 matadi/models/microsphere/affine/__init__.py
 matadi/models/microsphere/affine/_models.py
 matadi/models/microsphere/nonaffine/__init__.py
 matadi/models/microsphere/nonaffine/_models.py
 matadi/models/microsphere/quadrature/__init__.py
@@ -34,8 +35,9 @@
 tests/test_eigvals_grad.py
 tests/test_fiber.py
 tests/test_lab.py
 tests/test_microsphere.py
 tests/test_models.py
 tests/test_plane.py
 tests/test_scalar.py
-tests/test_simple.py
+tests/test_simple.py
+tests/test_template-materials.py
```

### Comparing `matadi-0.1.8/pyproject.toml` & `matadi-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "matadi"
-version = "0.1.8"
+version = "0.1.9"
 description = "Material Definition with Automatic Differentiation"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 keywords = [
   "python", 
   "constitution",
```

### Comparing `matadi-0.1.8/setup.cfg` & `matadi-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = matadi
-version = 0.1.8
+version = 0.1.9
 author = Andreas Dutzler
 author_email = a.dutzler@gmail.com
 description = Material Definition with Automatic Differentiation
 url = https://github.com/adtzlr/matadi
 project_urls = 
 	Code=https://github.com/adtzlr/matadi
 	Issues=https://github.com/adtzlr/matadi/issues
```

### Comparing `matadi-0.1.8/tests/test_displacement-pressure.py` & `matadi-0.1.9/tests/test_displacement-pressure.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/tests/test_eigvals_grad.py` & `matadi-0.1.9/tests/test_eigvals_grad.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/tests/test_fiber.py` & `matadi-0.1.9/tests/test_fiber.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/tests/test_lab.py` & `matadi-0.1.9/tests/test_lab.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/tests/test_microsphere.py` & `matadi-0.1.9/tests/test_microsphere.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/tests/test_models.py` & `matadi-0.1.9/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/tests/test_plane.py` & `matadi-0.1.9/tests/test_plane.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/tests/test_scalar.py` & `matadi-0.1.9/tests/test_scalar.py`

 * *Files identical despite different names*

### Comparing `matadi-0.1.8/tests/test_simple.py` & `matadi-0.1.9/tests/test_simple.py`

 * *Files identical despite different names*

