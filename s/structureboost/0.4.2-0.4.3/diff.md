# Comparing `tmp/structureboost-0.4.2.tar.gz` & `tmp/structureboost-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structureboost-0.4.2.tar", last modified: Thu Apr 27 21:51:57 2023, max compression
+gzip compressed data, was "structureboost-0.4.3.tar", last modified: Tue May  2 21:19:20 2023, max compression
```

## Comparing `structureboost-0.4.2.tar` & `structureboost-0.4.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-04-27 21:51:57.303902 structureboost-0.4.2/
--rw-r--r--   0 brianlucena   (501) staff       (20)     1069 2020-02-12 23:26:49.000000 structureboost-0.4.2/LICENSE
--rw-r--r--   0 brianlucena   (501) staff       (20)     2269 2023-04-27 21:51:57.303463 structureboost-0.4.2/PKG-INFO
--rw-r--r--   0 brianlucena   (501) staff       (20)     1379 2020-07-30 21:19:11.000000 structureboost-0.4.2/README.md
--rw-r--r--   0 brianlucena   (501) staff       (20)      216 2020-03-27 21:03:03.000000 structureboost-0.4.2/README.rst
--rw-r--r--   0 brianlucena   (501) staff       (20)       68 2022-05-16 23:30:25.000000 structureboost-0.4.2/pyproject.toml
--rw-r--r--   0 brianlucena   (501) staff       (20)       38 2023-04-27 21:51:57.304016 structureboost-0.4.2/setup.cfg
--rw-r--r--   0 brianlucena   (501) staff       (20)     3745 2023-04-27 21:29:17.000000 structureboost-0.4.2/setup.py
-drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-04-27 21:51:57.296860 structureboost-0.4.2/structureboost/
--rw-r--r--   0 brianlucena   (501) staff       (20)      771 2023-04-27 21:29:07.000000 structureboost-0.4.2/structureboost/__init__.py
--rw-r--r--   0 brianlucena   (501) staff       (20)  1292117 2023-04-27 21:30:02.000000 structureboost-0.4.2/structureboost/coarsage.c
--rw-r--r--   0 brianlucena   (501) staff       (20)  1627393 2023-04-27 21:30:03.000000 structureboost-0.4.2/structureboost/graphs.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   768847 2023-04-27 21:30:03.000000 structureboost-0.4.2/structureboost/pdf_discrete.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   685166 2023-04-27 21:30:04.000000 structureboost-0.4.2/structureboost/pdf_group.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   369766 2023-04-27 21:30:04.000000 structureboost-0.4.2/structureboost/pdf_set.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   331763 2023-04-27 21:30:04.000000 structureboost-0.4.2/structureboost/prob_regr_unit.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   791318 2023-04-27 21:30:04.000000 structureboost-0.4.2/structureboost/prob_regressor.c
--rw-r--r--   0 brianlucena   (501) staff       (20)  2549702 2023-04-27 21:30:07.000000 structureboost-0.4.2/structureboost/structure_dt.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   690000 2023-04-27 21:30:08.000000 structureboost-0.4.2/structureboost/structure_dt_multi.c
--rw-r--r--   0 brianlucena   (501) staff       (20)  2191823 2023-04-27 21:30:10.000000 structureboost-0.4.2/structureboost/structure_gb.c
--rw-r--r--   0 brianlucena   (501) staff       (20)  1662806 2023-04-27 21:30:13.000000 structureboost-0.4.2/structureboost/structure_gb_multi.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   802064 2023-04-27 21:30:13.000000 structureboost-0.4.2/structureboost/structure_rf.c
--rw-r--r--   0 brianlucena   (501) staff       (20)   754981 2023-04-27 21:30:14.000000 structureboost-0.4.2/structureboost/structure_rfdt.c
--rw-r--r--   0 brianlucena   (501) staff       (20)     9676 2022-10-26 21:11:48.000000 structureboost-0.4.2/structureboost/utils.py
-drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-04-27 21:51:57.303012 structureboost-0.4.2/structureboost.egg-info/
--rw-r--r--   0 brianlucena   (501) staff       (20)     2269 2023-04-27 21:51:57.000000 structureboost-0.4.2/structureboost.egg-info/PKG-INFO
--rw-r--r--   0 brianlucena   (501) staff       (20)      719 2023-04-27 21:51:57.000000 structureboost-0.4.2/structureboost.egg-info/SOURCES.txt
--rw-r--r--   0 brianlucena   (501) staff       (20)        1 2023-04-27 21:51:57.000000 structureboost-0.4.2/structureboost.egg-info/dependency_links.txt
--rw-r--r--   0 brianlucena   (501) staff       (20)        1 2022-02-04 23:34:24.000000 structureboost-0.4.2/structureboost.egg-info/not-zip-safe
--rw-r--r--   0 brianlucena   (501) staff       (20)       85 2023-04-27 21:51:57.000000 structureboost-0.4.2/structureboost.egg-info/requires.txt
--rw-r--r--   0 brianlucena   (501) staff       (20)      176 2023-04-27 21:51:57.000000 structureboost-0.4.2/structureboost.egg-info/top_level.txt
+drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-05-02 21:19:20.674373 structureboost-0.4.3/
+-rw-r--r--   0 brianlucena   (501) staff       (20)     1069 2020-02-12 23:26:49.000000 structureboost-0.4.3/LICENSE
+-rw-r--r--   0 brianlucena   (501) staff       (20)     2269 2023-05-02 21:19:20.673995 structureboost-0.4.3/PKG-INFO
+-rw-r--r--   0 brianlucena   (501) staff       (20)     1379 2020-07-30 21:19:11.000000 structureboost-0.4.3/README.md
+-rw-r--r--   0 brianlucena   (501) staff       (20)      216 2020-03-27 21:03:03.000000 structureboost-0.4.3/README.rst
+-rw-r--r--   0 brianlucena   (501) staff       (20)       68 2022-05-16 23:30:25.000000 structureboost-0.4.3/pyproject.toml
+-rw-r--r--   0 brianlucena   (501) staff       (20)       38 2023-05-02 21:19:20.674454 structureboost-0.4.3/setup.cfg
+-rw-r--r--   0 brianlucena   (501) staff       (20)     3745 2023-05-02 21:13:55.000000 structureboost-0.4.3/setup.py
+drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-05-02 21:19:20.670253 structureboost-0.4.3/structureboost/
+-rw-r--r--   0 brianlucena   (501) staff       (20)      771 2023-05-02 21:13:39.000000 structureboost-0.4.3/structureboost/__init__.py
+-rw-r--r--   0 brianlucena   (501) staff       (20)  1293914 2023-05-02 20:59:40.000000 structureboost-0.4.3/structureboost/coarsage.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)  1627393 2023-05-02 20:59:41.000000 structureboost-0.4.3/structureboost/graphs.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   768847 2023-05-02 20:59:41.000000 structureboost-0.4.3/structureboost/pdf_discrete.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   685166 2023-05-02 20:59:42.000000 structureboost-0.4.3/structureboost/pdf_group.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   369766 2023-05-02 20:59:42.000000 structureboost-0.4.3/structureboost/pdf_set.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   331763 2023-05-02 20:59:42.000000 structureboost-0.4.3/structureboost/prob_regr_unit.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   791318 2023-05-02 20:59:42.000000 structureboost-0.4.3/structureboost/prob_regressor.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)  2547001 2023-05-02 20:59:45.000000 structureboost-0.4.3/structureboost/structure_dt.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   690114 2023-05-02 20:59:45.000000 structureboost-0.4.3/structureboost/structure_dt_multi.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)  2197134 2023-05-02 20:59:48.000000 structureboost-0.4.3/structureboost/structure_gb.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)  1663763 2023-05-02 20:59:50.000000 structureboost-0.4.3/structureboost/structure_gb_multi.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   802575 2023-05-02 20:59:51.000000 structureboost-0.4.3/structureboost/structure_rf.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)   755482 2023-05-02 20:59:51.000000 structureboost-0.4.3/structureboost/structure_rfdt.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)     9676 2022-10-26 21:11:48.000000 structureboost-0.4.3/structureboost/utils.py
+drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-05-02 21:19:20.673631 structureboost-0.4.3/structureboost.egg-info/
+-rw-r--r--   0 brianlucena   (501) staff       (20)     2269 2023-05-02 21:19:20.000000 structureboost-0.4.3/structureboost.egg-info/PKG-INFO
+-rw-r--r--   0 brianlucena   (501) staff       (20)      719 2023-05-02 21:19:20.000000 structureboost-0.4.3/structureboost.egg-info/SOURCES.txt
+-rw-r--r--   0 brianlucena   (501) staff       (20)        1 2023-05-02 21:19:20.000000 structureboost-0.4.3/structureboost.egg-info/dependency_links.txt
+-rw-r--r--   0 brianlucena   (501) staff       (20)        1 2022-02-04 23:34:24.000000 structureboost-0.4.3/structureboost.egg-info/not-zip-safe
+-rw-r--r--   0 brianlucena   (501) staff       (20)       85 2023-05-02 21:19:20.000000 structureboost-0.4.3/structureboost.egg-info/requires.txt
+-rw-r--r--   0 brianlucena   (501) staff       (20)      176 2023-05-02 21:19:20.000000 structureboost-0.4.3/structureboost.egg-info/top_level.txt
```

### Comparing `structureboost-0.4.2/LICENSE` & `structureboost-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.2/PKG-INFO` & `structureboost-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structureboost
-Version: 0.4.2
+Version: 0.4.3
 Summary: StructureBoost is a Python package for gradient boosting using categorical structure.  See documentation at: https://structureboost.readthedocs.io/
 Home-page: https://github.com/numeristical/structureboost
 Author: Brian Lucena
 Author-email: brianlucena@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `structureboost-0.4.2/README.md` & `structureboost-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.2/setup.py` & `structureboost-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 setup(
     author="Brian Lucena",
     author_email="brianlucena@gmail.com",
     name='structureboost',
     license="MIT",
     license_files=['LICENSE'],
     description="StructureBoost is a Python package for gradient boosting using categorical structure.  See documentation at: https://structureboost.readthedocs.io/",
-    version='0.4.2',
+    version='0.4.3',
     long_description=README,
     zip_safe=False,
     url='https://github.com/numeristical/structureboost',
     packages=['structureboost'],
     package_dir={'structureboost':
                  'structureboost'},
     python_requires=">=3.5",
```

### Comparing `structureboost-0.4.2/structureboost/__init__.py` & `structureboost-0.4.3/structureboost/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from prob_regr_unit import ProbRegressorUnit
 from prob_regressor import PrestoBoost
 from coarsage import Coarsage
 from pdf_discrete import PdfDiscrete, average_densities
 from pdf_group import PdfGroup, log_loss_pdf, test_between_quantiles_pdf, test_in_pred_regions
 from .utils import get_basic_config, apply_defaults, default_config_dict, ice_plot, log_loss
 
-__version__ = '0.4.2'
+__version__ = '0.4.3'
```

### Comparing `structureboost-0.4.2/structureboost/coarsage.c` & `structureboost-0.4.3/structureboost/coarsage.c`

 * *Files 0% similar despite different names*

```diff
@@ -2378,15 +2378,15 @@
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'libc.math' */
 
 /* Module declarations from 'structureboost.coarsage' */
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int_t = { "int_t", NULL, sizeof(__pyx_t_5numpy_int_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int_t), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t = { "int32_t", NULL, sizeof(__pyx_t_5numpy_int32_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int32_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int32_t), 0 };
 #define __Pyx_MODULE_NAME "structureboost.coarsage"
 extern int __pyx_module_is_main_structureboost__coarsage;
 int __pyx_module_is_main_structureboost__coarsage = 0;
 
 /* Implementation of 'structureboost.coarsage' */
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_range;
@@ -2414,15 +2414,14 @@
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_dtm[] = "dtm";
 static const char __pyx_k_eps[] = "eps";
 static const char __pyx_k_fbp[] = "fbp";
 static const char __pyx_k_fbw[] = "fbw";
 static const char __pyx_k_fit[] = "fit";
 static const char __pyx_k_ind[] = "ind";
-static const char __pyx_k_int[] = "int_";
 static const char __pyx_k_log[] = "log";
 static const char __pyx_k_max[] = "max";
 static const char __pyx_k_min[] = "min";
 static const char __pyx_k_mpv[] = "mpv";
 static const char __pyx_k_ngm[] = "ngm";
 static const char __pyx_k_rpt[] = "rpt";
 static const char __pyx_k_sum[] = "sum";
@@ -2450,14 +2449,15 @@
 static const char __pyx_k_CATEG[] = "CATEG";
 static const char __pyx_k_NUMER[] = "NUMER";
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_fixed[] = "fixed";
 static const char __pyx_k_gamma[] = "gamma";
 static const char __pyx_k_index[] = "index";
+static const char __pyx_k_int32[] = "int32";
 static const char __pyx_k_isnan[] = "isnan";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_midpt[] = "midpt";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_print[] = "print";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_round[] = "round";
@@ -2961,15 +2961,15 @@
 static PyObject *__pyx_n_s_init_bin_pts;
 static PyObject *__pyx_n_s_init_logprobmat_fine;
 static PyObject *__pyx_n_s_init_pdf;
 static PyObject *__pyx_n_s_init_pdf_fine;
 static PyObject *__pyx_n_s_initial_growth_steps;
 static PyObject *__pyx_n_s_initial_model;
 static PyObject *__pyx_n_s_initial_pred;
-static PyObject *__pyx_n_s_int;
+static PyObject *__pyx_n_s_int32;
 static PyObject *__pyx_n_s_inv_cti;
 static PyObject *__pyx_n_s_isin;
 static PyObject *__pyx_n_s_isnan;
 static PyObject *__pyx_n_s_isnan_array;
 static PyObject *__pyx_n_s_items;
 static PyObject *__pyx_n_s_j;
 static PyObject *__pyx_n_s_k;
@@ -6691,19 +6691,19 @@
   PyObject *__pyx_r = NULL;
   __Pyx_TraceDeclarations
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  int __pyx_t_7;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
-  PyObject *__pyx_t_9 = NULL;
+  int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   PyObject *(*__pyx_t_11)(PyObject *);
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__12)
@@ -6726,141 +6726,165 @@
   __pyx_t_2 = 0;
 
   /* "structureboost/coarsage.pyx":263
  *         # Bin the y-values according to the bins for this specific tree
  *         curr_binpts = self.binpt_vec_list[index]
  *         curr_num_classes = len(curr_binpts)-1             # <<<<<<<<<<<<<<
  *         y_bin = (np.digitize(y_train, curr_binpts) -1
- *                     -(y_train==curr_binpts[-1]))
+ *                     -(y_train==curr_binpts[-1])).astype(np.int32)
  */
   __pyx_t_3 = PyObject_Length(__pyx_v_curr_binpts); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 263, __pyx_L1_error)
   __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_3 - 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 263, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_curr_num_classes = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "structureboost/coarsage.pyx":264
  *         curr_binpts = self.binpt_vec_list[index]
  *         curr_num_classes = len(curr_binpts)-1
  *         y_bin = (np.digitize(y_train, curr_binpts) -1             # <<<<<<<<<<<<<<
- *                     -(y_train==curr_binpts[-1]))
+ *                     -(y_train==curr_binpts[-1])).astype(np.int32)
  *         curr_answer_bin_probs = curr_answer.bins_to_probs(curr_binpts)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_digitize); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 264, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 264, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = NULL;
-  __pyx_t_5 = 0;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_1)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_1);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_digitize); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 264, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = NULL;
+  __pyx_t_6 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
-      __pyx_t_5 = 1;
+      __Pyx_DECREF_SET(__pyx_t_5, function);
+      __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_4)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_y_train, __pyx_v_curr_binpts};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_GOTREF(__pyx_t_2);
+  if (PyFunction_Check(__pyx_t_5)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_y_train, __pyx_v_curr_binpts};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_v_y_train, __pyx_v_curr_binpts};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_y_train, __pyx_v_curr_binpts};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 264, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    if (__pyx_t_1) {
-      __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1); __pyx_t_1 = NULL;
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 264, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    if (__pyx_t_4) {
+      __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_y_train);
     __Pyx_GIVEREF(__pyx_v_y_train);
-    PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_y_train);
+    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_y_train);
     __Pyx_INCREF(__pyx_v_curr_binpts);
     __Pyx_GIVEREF(__pyx_v_curr_binpts);
-    PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_v_curr_binpts);
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_v_curr_binpts);
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 264, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyInt_SubtractObjC(__pyx_t_1, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 264, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/coarsage.pyx":265
  *         curr_num_classes = len(curr_binpts)-1
  *         y_bin = (np.digitize(y_train, curr_binpts) -1
- *                     -(y_train==curr_binpts[-1]))             # <<<<<<<<<<<<<<
+ *                     -(y_train==curr_binpts[-1])).astype(np.int32)             # <<<<<<<<<<<<<<
  *         curr_answer_bin_probs = curr_answer.bins_to_probs(curr_binpts)
  *         if not self.structured_loss:
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_curr_binpts, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 265, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = PyObject_RichCompare(__pyx_v_y_train, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 265, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Subtract(__pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_curr_binpts, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_7 = PyObject_RichCompare(__pyx_v_y_train, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyNumber_Subtract(__pyx_t_5, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_astype); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_7);
+    if (likely(__pyx_t_1)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+      __Pyx_INCREF(__pyx_t_1);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_7, function);
+    }
+  }
+  __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_1, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_y_bin = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "structureboost/coarsage.pyx":266
  *         y_bin = (np.digitize(y_train, curr_binpts) -1
- *                     -(y_train==curr_binpts[-1]))
+ *                     -(y_train==curr_binpts[-1])).astype(np.int32)
  *         curr_answer_bin_probs = curr_answer.bins_to_probs(curr_binpts)             # <<<<<<<<<<<<<<
  *         if not self.structured_loss:
  *             self.ts_dict = None
  */
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_curr_answer, __pyx_n_s_bins_to_probs); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 266, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_curr_answer, __pyx_n_s_bins_to_probs); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_7);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
+      __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_4, __pyx_v_curr_binpts) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_curr_binpts);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_5, __pyx_v_curr_binpts) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_curr_binpts);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 266, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_curr_answer_bin_probs = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "structureboost/coarsage.pyx":267
- *                     -(y_train==curr_binpts[-1]))
+ *                     -(y_train==curr_binpts[-1])).astype(np.int32)
  *         curr_answer_bin_probs = curr_answer.bins_to_probs(curr_binpts)
  *         if not self.structured_loss:             # <<<<<<<<<<<<<<
  *             self.ts_dict = None
  *             y_g_h_mat = c_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_structured_loss); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_8 = ((!__pyx_t_7) != 0);
-  if (__pyx_t_8) {
+  __pyx_t_9 = ((!__pyx_t_8) != 0);
+  if (__pyx_t_9) {
 
     /* "structureboost/coarsage.pyx":268
  *         curr_answer_bin_probs = curr_answer.bins_to_probs(curr_binpts)
  *         if not self.structured_loss:
  *             self.ts_dict = None             # <<<<<<<<<<<<<<
  *             y_g_h_mat = c_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,
  *                                                 np.ones(len(y_train)))
@@ -6870,98 +6894,98 @@
     /* "structureboost/coarsage.pyx":269
  *         if not self.structured_loss:
  *             self.ts_dict = None
  *             y_g_h_mat = c_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,             # <<<<<<<<<<<<<<
  *                                                 np.ones(len(y_train)))
  *             return y_g_h_mat
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_c_entropy_link_der_12_vec_sp); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 269, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_c_entropy_link_der_12_vec_sp); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 269, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
 
     /* "structureboost/coarsage.pyx":270
  *             self.ts_dict = None
  *             y_g_h_mat = c_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,
  *                                                 np.ones(len(y_train)))             # <<<<<<<<<<<<<<
  *             return y_g_h_mat
  *         else:
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ones); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 270, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_ones); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 270, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_3 = PyObject_Length(__pyx_v_y_train); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 270, __pyx_L1_error)
     __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_10 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
-      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_10)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_9, function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_10, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_1);
+    __pyx_t_5 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_10, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_1);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 270, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_9 = NULL;
-    __pyx_t_5 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_9)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_9);
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 270, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = NULL;
+    __pyx_t_6 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_4)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-        __pyx_t_5 = 1;
+        __Pyx_DECREF_SET(__pyx_t_7, function);
+        __pyx_t_6 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_6)) {
-      PyObject *__pyx_temp[4] = {__pyx_t_9, __pyx_v_y_bin, __pyx_v_curr_answer_bin_probs, __pyx_t_4};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    if (PyFunction_Check(__pyx_t_7)) {
+      PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_v_y_bin, __pyx_v_curr_answer_bin_probs, __pyx_t_5};
+      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
-      PyObject *__pyx_temp[4] = {__pyx_t_9, __pyx_v_y_bin, __pyx_v_curr_answer_bin_probs, __pyx_t_4};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
+      PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_v_y_bin, __pyx_v_curr_answer_bin_probs, __pyx_t_5};
+      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     {
-      __pyx_t_1 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
+      __pyx_t_1 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (__pyx_t_9) {
-        __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_9); __pyx_t_9 = NULL;
+      if (__pyx_t_4) {
+        __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
       __Pyx_INCREF(__pyx_v_y_bin);
       __Pyx_GIVEREF(__pyx_v_y_bin);
-      PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_5, __pyx_v_y_bin);
+      PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_6, __pyx_v_y_bin);
       __Pyx_INCREF(__pyx_v_curr_answer_bin_probs);
       __Pyx_GIVEREF(__pyx_v_curr_answer_bin_probs);
-      PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_5, __pyx_v_curr_answer_bin_probs);
-      __Pyx_GIVEREF(__pyx_t_4);
-      PyTuple_SET_ITEM(__pyx_t_1, 2+__pyx_t_5, __pyx_t_4);
-      __pyx_t_4 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
+      PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_6, __pyx_v_curr_answer_bin_probs);
+      __Pyx_GIVEREF(__pyx_t_5);
+      PyTuple_SET_ITEM(__pyx_t_1, 2+__pyx_t_6, __pyx_t_5);
+      __pyx_t_5 = 0;
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_v_y_g_h_mat = __pyx_t_2;
     __pyx_t_2 = 0;
 
     /* "structureboost/coarsage.pyx":271
  *             y_g_h_mat = c_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,
  *                                                 np.ones(len(y_train)))
  *             return y_g_h_mat             # <<<<<<<<<<<<<<
@@ -6970,15 +6994,15 @@
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_y_g_h_mat);
     __pyx_r = __pyx_v_y_g_h_mat;
     goto __pyx_L0;
 
     /* "structureboost/coarsage.pyx":267
- *                     -(y_train==curr_binpts[-1]))
+ *                     -(y_train==curr_binpts[-1])).astype(np.int32)
  *         curr_answer_bin_probs = curr_answer.bins_to_probs(curr_binpts)
  *         if not self.structured_loss:             # <<<<<<<<<<<<<<
  *             self.ts_dict = None
  *             y_g_h_mat = c_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,
  */
   }
 
@@ -6988,157 +7012,157 @@
  *             self.stride_list = list(range(self.structure_block_size, self.structure_block_size+1))             # <<<<<<<<<<<<<<
  *             pl = []
  *             for i in self.stride_list:
  */
   /*else*/ {
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_structure_block_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_structure_block_size); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 273, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_t_6, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_structure_block_size); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 273, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_t_7, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 273, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 273, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_1);
-    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_1);
     __pyx_t_2 = 0;
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 273, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 273, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_stride_list, __pyx_t_6) < 0) __PYX_ERR(0, 273, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_stride_list, __pyx_t_7) < 0) __PYX_ERR(0, 273, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
     /* "structureboost/coarsage.pyx":274
  *         else:
  *             self.stride_list = list(range(self.structure_block_size, self.structure_block_size+1))
  *             pl = []             # <<<<<<<<<<<<<<
  *             for i in self.stride_list:
  *                 pl = pl+chain_partition(curr_num_classes,i)
  */
-    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 274, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_v_pl = __pyx_t_6;
-    __pyx_t_6 = 0;
+    __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 274, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_v_pl = __pyx_t_7;
+    __pyx_t_7 = 0;
 
     /* "structureboost/coarsage.pyx":275
  *             self.stride_list = list(range(self.structure_block_size, self.structure_block_size+1))
  *             pl = []
  *             for i in self.stride_list:             # <<<<<<<<<<<<<<
  *                 pl = pl+chain_partition(curr_num_classes,i)
  *             ts={}
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_stride_list); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 275, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    if (likely(PyList_CheckExact(__pyx_t_6)) || PyTuple_CheckExact(__pyx_t_6)) {
-      __pyx_t_1 = __pyx_t_6; __Pyx_INCREF(__pyx_t_1); __pyx_t_3 = 0;
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_stride_list); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 275, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    if (likely(PyList_CheckExact(__pyx_t_7)) || PyTuple_CheckExact(__pyx_t_7)) {
+      __pyx_t_1 = __pyx_t_7; __Pyx_INCREF(__pyx_t_1); __pyx_t_3 = 0;
       __pyx_t_11 = NULL;
     } else {
-      __pyx_t_3 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 275, __pyx_L1_error)
+      __pyx_t_3 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 275, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_11 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 275, __pyx_L1_error)
     }
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     for (;;) {
       if (likely(!__pyx_t_11)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_6); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 275, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_7); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 275, __pyx_L1_error)
           #else
-          __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 275, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_6);
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 275, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_6); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 275, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_7); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 275, __pyx_L1_error)
           #else
-          __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 275, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_6);
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 275, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
-        __pyx_t_6 = __pyx_t_11(__pyx_t_1);
-        if (unlikely(!__pyx_t_6)) {
+        __pyx_t_7 = __pyx_t_11(__pyx_t_1);
+        if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
             else __PYX_ERR(0, 275, __pyx_L1_error)
           }
           break;
         }
-        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_GOTREF(__pyx_t_7);
       }
-      __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_6);
-      __pyx_t_6 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_7);
+      __pyx_t_7 = 0;
 
       /* "structureboost/coarsage.pyx":276
  *             pl = []
  *             for i in self.stride_list:
  *                 pl = pl+chain_partition(curr_num_classes,i)             # <<<<<<<<<<<<<<
  *             ts={}
  *             ts['partition_type']='fixed'
  */
       __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_chain_partition); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = NULL;
-      __pyx_t_5 = 0;
+      __pyx_t_5 = NULL;
+      __pyx_t_6 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-        if (likely(__pyx_t_4)) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+        if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-          __Pyx_INCREF(__pyx_t_4);
+          __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
-          __pyx_t_5 = 1;
+          __pyx_t_6 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_2)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_curr_num_classes, __pyx_v_i};
-        __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 276, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __Pyx_GOTREF(__pyx_t_6);
+        PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_curr_num_classes, __pyx_v_i};
+        __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 276, __pyx_L1_error)
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_GOTREF(__pyx_t_7);
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
-        PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_curr_num_classes, __pyx_v_i};
-        __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 276, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __Pyx_GOTREF(__pyx_t_6);
+        PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_curr_num_classes, __pyx_v_i};
+        __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 276, __pyx_L1_error)
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_GOTREF(__pyx_t_7);
       } else
       #endif
       {
-        __pyx_t_9 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 276, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_9);
-        if (__pyx_t_4) {
-          __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_4); __pyx_t_4 = NULL;
+        __pyx_t_4 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 276, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        if (__pyx_t_5) {
+          __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5); __pyx_t_5 = NULL;
         }
         __Pyx_INCREF(__pyx_v_curr_num_classes);
         __Pyx_GIVEREF(__pyx_v_curr_num_classes);
-        PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_5, __pyx_v_curr_num_classes);
+        PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_6, __pyx_v_curr_num_classes);
         __Pyx_INCREF(__pyx_v_i);
         __Pyx_GIVEREF(__pyx_v_i);
-        PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_5, __pyx_v_i);
-        __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 276, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_6, __pyx_v_i);
+        __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 276, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = PyNumber_Add(__pyx_v_pl, __pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
+      __pyx_t_2 = PyNumber_Add(__pyx_v_pl, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 276, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF_SET(__pyx_v_pl, __pyx_t_2);
       __pyx_t_2 = 0;
 
       /* "structureboost/coarsage.pyx":275
  *             self.stride_list = list(range(self.structure_block_size, self.structure_block_size+1))
  *             pl = []
  *             for i in self.stride_list:             # <<<<<<<<<<<<<<
@@ -7195,51 +7219,51 @@
  *             ts['singleton_weight'] = self.singleton_weight
  *             ts['partition_weight_vec'] = np.ones(len(pl))*(1-self.singleton_weight)/len(pl)             # <<<<<<<<<<<<<<
  *             self.ts_dict=ts
  *             self.part_weight_vec = np.array(self.ts_dict['partition_weight_vec'])
  */
     __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 281, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 281, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_3 = PyObject_Length(__pyx_v_pl); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 281, __pyx_L1_error)
     __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_9)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_9);
+    __pyx_t_4 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_4)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_9, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_2);
-    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_2);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_singleton_weight); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 281, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_2 = __Pyx_PyInt_SubtractCObj(__pyx_int_1, __pyx_t_6, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_singleton_weight); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 281, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_2 = __Pyx_PyInt_SubtractCObj(__pyx_int_1, __pyx_t_7, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 281, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 281, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_3 = PyObject_Length(__pyx_v_pl); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 281, __pyx_L1_error)
     __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_t_6, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyNumber_Divide(__pyx_t_7, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (unlikely(PyDict_SetItem(__pyx_v_ts, __pyx_n_u_partition_weight_vec, __pyx_t_1) < 0)) __PYX_ERR(0, 281, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "structureboost/coarsage.pyx":282
  *             ts['singleton_weight'] = self.singleton_weight
  *             ts['partition_weight_vec'] = np.ones(len(pl))*(1-self.singleton_weight)/len(pl)
@@ -7254,235 +7278,235 @@
  *             self.ts_dict=ts
  *             self.part_weight_vec = np.array(self.ts_dict['partition_weight_vec'])             # <<<<<<<<<<<<<<
  *             self.rpt = self._create_rpt_from_list(self.ts_dict['partition_list'], curr_num_classes)
  *             y_g_h_mat = c_str_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,
  */
     __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 283, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 283, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_ts_dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_partition_weight_vec); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 283, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_partition_weight_vec); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 283, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_6);
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_2)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
-    __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_2, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_9);
+    __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_part_weight_vec, __pyx_t_1) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "structureboost/coarsage.pyx":284
  *             self.ts_dict=ts
  *             self.part_weight_vec = np.array(self.ts_dict['partition_weight_vec'])
  *             self.rpt = self._create_rpt_from_list(self.ts_dict['partition_list'], curr_num_classes)             # <<<<<<<<<<<<<<
  *             y_g_h_mat = c_str_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,
  *                                                 np.ones(len(y_train)),
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_create_rpt_from_list); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 284, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_ts_dict); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 284, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_9, __pyx_n_u_partition_list); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 284, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_create_rpt_from_list); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 284, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_ts_dict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 284, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_n_u_partition_list); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 284, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __pyx_t_9 = NULL;
-    __pyx_t_5 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_9)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_9);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = NULL;
+    __pyx_t_6 = 0;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_4)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-        __pyx_t_5 = 1;
+        __Pyx_DECREF_SET(__pyx_t_7, function);
+        __pyx_t_6 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_6)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_2, __pyx_v_curr_num_classes};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    if (PyFunction_Check(__pyx_t_7)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_2, __pyx_v_curr_num_classes};
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_2, __pyx_v_curr_num_classes};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
+      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_2, __pyx_v_curr_num_classes};
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     } else
     #endif
     {
-      __pyx_t_4 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 284, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      if (__pyx_t_9) {
-        __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_9); __pyx_t_9 = NULL;
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 284, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      if (__pyx_t_4) {
+        __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_2);
-      PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_5, __pyx_t_2);
+      PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_6, __pyx_t_2);
       __Pyx_INCREF(__pyx_v_curr_num_classes);
       __Pyx_GIVEREF(__pyx_v_curr_num_classes);
-      PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_5, __pyx_v_curr_num_classes);
+      PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_6, __pyx_v_curr_num_classes);
       __pyx_t_2 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_rpt, __pyx_t_1) < 0) __PYX_ERR(0, 284, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "structureboost/coarsage.pyx":285
  *             self.part_weight_vec = np.array(self.ts_dict['partition_weight_vec'])
  *             self.rpt = self._create_rpt_from_list(self.ts_dict['partition_list'], curr_num_classes)
  *             y_g_h_mat = c_str_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,             # <<<<<<<<<<<<<<
  *                                                 np.ones(len(y_train)),
  *                                         self.part_weight_vec, self.rpt)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_c_str_entropy_link_der_12_vec_sp); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 285, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_c_str_entropy_link_der_12_vec_sp); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 285, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
 
     /* "structureboost/coarsage.pyx":286
  *             self.rpt = self._create_rpt_from_list(self.ts_dict['partition_list'], curr_num_classes)
  *             y_g_h_mat = c_str_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,
  *                                                 np.ones(len(y_train)),             # <<<<<<<<<<<<<<
  *                                         self.part_weight_vec, self.rpt)
  *             if self.singleton_weight>0:
  */
     __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 286, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 286, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_3 = PyObject_Length(__pyx_v_y_train); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 286, __pyx_L1_error)
     __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 286, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_10 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
-      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_10)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_9, function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
-    __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_10, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_2);
+    __pyx_t_5 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_10, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_2);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 286, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 286, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "structureboost/coarsage.pyx":287
  *             y_g_h_mat = c_str_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,
  *                                                 np.ones(len(y_train)),
  *                                         self.part_weight_vec, self.rpt)             # <<<<<<<<<<<<<<
  *             if self.singleton_weight>0:
  *                 y_g_h_mat_reg = c_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,
  */
-    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_part_weight_vec); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 287, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_part_weight_vec); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 287, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rpt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 287, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_10 = NULL;
-    __pyx_t_5 = 0;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_6);
+    __pyx_t_6 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_10)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-        __pyx_t_5 = 1;
+        __Pyx_DECREF_SET(__pyx_t_7, function);
+        __pyx_t_6 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_6)) {
-      PyObject *__pyx_temp[6] = {__pyx_t_10, __pyx_v_y_bin, __pyx_v_curr_answer_bin_probs, __pyx_t_4, __pyx_t_9, __pyx_t_2};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_5, 5+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
+    if (PyFunction_Check(__pyx_t_7)) {
+      PyObject *__pyx_temp[6] = {__pyx_t_10, __pyx_v_y_bin, __pyx_v_curr_answer_bin_probs, __pyx_t_5, __pyx_t_4, __pyx_t_2};
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_6, 5+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
-      PyObject *__pyx_temp[6] = {__pyx_t_10, __pyx_v_y_bin, __pyx_v_curr_answer_bin_probs, __pyx_t_4, __pyx_t_9, __pyx_t_2};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_5, 5+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
+      PyObject *__pyx_temp[6] = {__pyx_t_10, __pyx_v_y_bin, __pyx_v_curr_answer_bin_probs, __pyx_t_5, __pyx_t_4, __pyx_t_2};
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_6, 5+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     } else
     #endif
     {
-      __pyx_t_12 = PyTuple_New(5+__pyx_t_5); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 285, __pyx_L1_error)
+      __pyx_t_12 = PyTuple_New(5+__pyx_t_6); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 285, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       if (__pyx_t_10) {
         __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10); __pyx_t_10 = NULL;
       }
       __Pyx_INCREF(__pyx_v_y_bin);
       __Pyx_GIVEREF(__pyx_v_y_bin);
-      PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_5, __pyx_v_y_bin);
+      PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_6, __pyx_v_y_bin);
       __Pyx_INCREF(__pyx_v_curr_answer_bin_probs);
       __Pyx_GIVEREF(__pyx_v_curr_answer_bin_probs);
-      PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_5, __pyx_v_curr_answer_bin_probs);
+      PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_6, __pyx_v_curr_answer_bin_probs);
+      __Pyx_GIVEREF(__pyx_t_5);
+      PyTuple_SET_ITEM(__pyx_t_12, 2+__pyx_t_6, __pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_4);
-      PyTuple_SET_ITEM(__pyx_t_12, 2+__pyx_t_5, __pyx_t_4);
-      __Pyx_GIVEREF(__pyx_t_9);
-      PyTuple_SET_ITEM(__pyx_t_12, 3+__pyx_t_5, __pyx_t_9);
+      PyTuple_SET_ITEM(__pyx_t_12, 3+__pyx_t_6, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_2);
-      PyTuple_SET_ITEM(__pyx_t_12, 4+__pyx_t_5, __pyx_t_2);
+      PyTuple_SET_ITEM(__pyx_t_12, 4+__pyx_t_6, __pyx_t_2);
+      __pyx_t_5 = 0;
       __pyx_t_4 = 0;
-      __pyx_t_9 = 0;
       __pyx_t_2 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     }
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_v_y_g_h_mat = __pyx_t_1;
     __pyx_t_1 = 0;
 
     /* "structureboost/coarsage.pyx":288
  *                                                 np.ones(len(y_train)),
  *                                         self.part_weight_vec, self.rpt)
  *             if self.singleton_weight>0:             # <<<<<<<<<<<<<<
  *                 y_g_h_mat_reg = c_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,
  *                                                 np.ones(len(y_train)))
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_singleton_weight); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = PyObject_RichCompare(__pyx_t_1, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 288, __pyx_L1_error)
+    __pyx_t_7 = PyObject_RichCompare(__pyx_t_1, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 288, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 288, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (__pyx_t_8) {
+    __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 288, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    if (__pyx_t_9) {
 
       /* "structureboost/coarsage.pyx":289
  *                                         self.part_weight_vec, self.rpt)
  *             if self.singleton_weight>0:
  *                 y_g_h_mat_reg = c_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,             # <<<<<<<<<<<<<<
  *                                                 np.ones(len(y_train)))
  *                 y_g_h_mat = y_g_h_mat + self.singleton_weight*y_g_h_mat_reg
@@ -7495,106 +7519,106 @@
  *                 y_g_h_mat_reg = c_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,
  *                                                 np.ones(len(y_train)))             # <<<<<<<<<<<<<<
  *                 y_g_h_mat = y_g_h_mat + self.singleton_weight*y_g_h_mat_reg
  *             return y_g_h_mat
  */
       __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 290, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_9);
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ones); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 290, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_3 = PyObject_Length(__pyx_v_y_train); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 290, __pyx_L1_error)
       __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = NULL;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
-        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_9);
-        if (likely(__pyx_t_4)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-          __Pyx_INCREF(__pyx_t_4);
+      __pyx_t_5 = NULL;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_5)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+          __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_9, function);
+          __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
-      __pyx_t_12 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_t_2);
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_12 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_2);
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 290, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __pyx_t_9 = NULL;
-      __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_4 = NULL;
+      __pyx_t_6 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-        __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_1);
-        if (likely(__pyx_t_9)) {
+        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
+        if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-          __Pyx_INCREF(__pyx_t_9);
+          __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
-          __pyx_t_5 = 1;
+          __pyx_t_6 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_1)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_9, __pyx_v_y_bin, __pyx_v_curr_answer_bin_probs, __pyx_t_12};
-        __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 289, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-        __Pyx_GOTREF(__pyx_t_6);
+        PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_v_y_bin, __pyx_v_curr_answer_bin_probs, __pyx_t_12};
+        __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 289, __pyx_L1_error)
+        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_9, __pyx_v_y_bin, __pyx_v_curr_answer_bin_probs, __pyx_t_12};
-        __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 289, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-        __Pyx_GOTREF(__pyx_t_6);
+        PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_v_y_bin, __pyx_v_curr_answer_bin_probs, __pyx_t_12};
+        __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 289, __pyx_L1_error)
+        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       } else
       #endif
       {
-        __pyx_t_2 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        if (__pyx_t_9) {
-          __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_9); __pyx_t_9 = NULL;
+        if (__pyx_t_4) {
+          __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4); __pyx_t_4 = NULL;
         }
         __Pyx_INCREF(__pyx_v_y_bin);
         __Pyx_GIVEREF(__pyx_v_y_bin);
-        PyTuple_SET_ITEM(__pyx_t_2, 0+__pyx_t_5, __pyx_v_y_bin);
+        PyTuple_SET_ITEM(__pyx_t_2, 0+__pyx_t_6, __pyx_v_y_bin);
         __Pyx_INCREF(__pyx_v_curr_answer_bin_probs);
         __Pyx_GIVEREF(__pyx_v_curr_answer_bin_probs);
-        PyTuple_SET_ITEM(__pyx_t_2, 1+__pyx_t_5, __pyx_v_curr_answer_bin_probs);
+        PyTuple_SET_ITEM(__pyx_t_2, 1+__pyx_t_6, __pyx_v_curr_answer_bin_probs);
         __Pyx_GIVEREF(__pyx_t_12);
-        PyTuple_SET_ITEM(__pyx_t_2, 2+__pyx_t_5, __pyx_t_12);
+        PyTuple_SET_ITEM(__pyx_t_2, 2+__pyx_t_6, __pyx_t_12);
         __pyx_t_12 = 0;
-        __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 289, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
+        __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 289, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_v_y_g_h_mat_reg = __pyx_t_6;
-      __pyx_t_6 = 0;
+      __pyx_v_y_g_h_mat_reg = __pyx_t_7;
+      __pyx_t_7 = 0;
 
       /* "structureboost/coarsage.pyx":291
  *                 y_g_h_mat_reg = c_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,
  *                                                 np.ones(len(y_train)))
  *                 y_g_h_mat = y_g_h_mat + self.singleton_weight*y_g_h_mat_reg             # <<<<<<<<<<<<<<
  *             return y_g_h_mat
  * 
  */
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_singleton_weight); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 291, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_1 = PyNumber_Multiply(__pyx_t_6, __pyx_v_y_g_h_mat_reg); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 291, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_singleton_weight); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 291, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_1 = PyNumber_Multiply(__pyx_t_7, __pyx_v_y_g_h_mat_reg); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 291, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyNumber_Add(__pyx_v_y_g_h_mat, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 291, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __pyx_t_7 = PyNumber_Add(__pyx_v_y_g_h_mat, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 291, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_DECREF_SET(__pyx_v_y_g_h_mat, __pyx_t_6);
-      __pyx_t_6 = 0;
+      __Pyx_DECREF_SET(__pyx_v_y_g_h_mat, __pyx_t_7);
+      __pyx_t_7 = 0;
 
       /* "structureboost/coarsage.pyx":288
  *                                                 np.ones(len(y_train)),
  *                                         self.part_weight_vec, self.rpt)
  *             if self.singleton_weight>0:             # <<<<<<<<<<<<<<
  *                 y_g_h_mat_reg = c_entropy_link_der_12_vec_sp(y_bin, curr_answer_bin_probs,
  *                                                 np.ones(len(y_train)))
@@ -7623,16 +7647,16 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_AddTraceback("structureboost.coarsage.Coarsage.compute_gh_mat", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_curr_binpts);
   __Pyx_XDECREF(__pyx_v_curr_num_classes);
@@ -7778,24 +7802,24 @@
   __Pyx_TraceCall("_create_rpt_from_list", __pyx_f[0], 294, 0, __PYX_ERR(0, 294, __pyx_L1_error));
 
   /* "structureboost/coarsage.pyx":295
  * 
  *     def _create_rpt_from_list(self, partition_list, num_classes):
  *         num_part = len(partition_list)             # <<<<<<<<<<<<<<
  *         max_part_size = np.max(np.array([len(qq) for qq in partition_list]))
- *         rpt = np.zeros((num_part, max_part_size, num_classes), dtype=np.int_)
+ *         rpt = np.zeros((num_part, max_part_size, num_classes), dtype=np.int32)
  */
   __pyx_t_1 = PyObject_Length(__pyx_v_partition_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 295, __pyx_L1_error)
   __pyx_v_num_part = __pyx_t_1;
 
   /* "structureboost/coarsage.pyx":296
  *     def _create_rpt_from_list(self, partition_list, num_classes):
  *         num_part = len(partition_list)
  *         max_part_size = np.max(np.array([len(qq) for qq in partition_list]))             # <<<<<<<<<<<<<<
- *         rpt = np.zeros((num_part, max_part_size, num_classes), dtype=np.int_)
+ *         rpt = np.zeros((num_part, max_part_size, num_classes), dtype=np.int32)
  *         flat_list = [j for sl in partition_list for i in sl for j in i]
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 296, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_max); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 296, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -7896,15 +7920,15 @@
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_max_part_size = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "structureboost/coarsage.pyx":297
  *         num_part = len(partition_list)
  *         max_part_size = np.max(np.array([len(qq) for qq in partition_list]))
- *         rpt = np.zeros((num_part, max_part_size, num_classes), dtype=np.int_)             # <<<<<<<<<<<<<<
+ *         rpt = np.zeros((num_part, max_part_size, num_classes), dtype=np.int32)             # <<<<<<<<<<<<<<
  *         flat_list = [j for sl in partition_list for i in sl for j in i]
  *         min_val, max_val = np.min(flat_list), np.max(flat_list)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
@@ -7927,30 +7951,30 @@
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
   __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_rpt = __pyx_t_5;
   __pyx_t_5 = 0;
 
   /* "structureboost/coarsage.pyx":298
  *         max_part_size = np.max(np.array([len(qq) for qq in partition_list]))
- *         rpt = np.zeros((num_part, max_part_size, num_classes), dtype=np.int_)
+ *         rpt = np.zeros((num_part, max_part_size, num_classes), dtype=np.int32)
  *         flat_list = [j for sl in partition_list for i in sl for j in i]             # <<<<<<<<<<<<<<
  *         min_val, max_val = np.min(flat_list), np.max(flat_list)
  *         if (min_val<0) or (max_val>num_classes-1):
  */
   { /* enter inner scope */
     __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 298, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_5);
@@ -8095,15 +8119,15 @@
     goto __pyx_L1_error;
     __pyx_L18_exit_scope:;
   } /* exit inner scope */
   __pyx_v_flat_list = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
   /* "structureboost/coarsage.pyx":299
- *         rpt = np.zeros((num_part, max_part_size, num_classes), dtype=np.int_)
+ *         rpt = np.zeros((num_part, max_part_size, num_classes), dtype=np.int32)
  *         flat_list = [j for sl in partition_list for i in sl for j in i]
  *         min_val, max_val = np.min(flat_list), np.max(flat_list)             # <<<<<<<<<<<<<<
  *         if (min_val<0) or (max_val>num_classes-1):
  *             w_str = "Elements of partition must be >=0 and <=(num_classes-1). "
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
@@ -8941,15 +8965,15 @@
     __pyx_v_num_dt = __pyx_t_9;
 
     /* "structureboost/coarsage.pyx":327
  *             cat_size = np.max(np.array([dt.get_max_split_size() for dt in self.dec_tree_list]))
  *             num_dt = len(self.dec_tree_list)
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))             # <<<<<<<<<<<<<<
  *             max_num_classes = np.max(self.num_classes)
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  */
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 327, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_max); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 327, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 327, __pyx_L1_error)
@@ -9052,15 +9076,15 @@
     __pyx_v_max_nodes = __pyx_t_1;
     __pyx_t_1 = 0;
 
     /* "structureboost/coarsage.pyx":328
  *             num_dt = len(self.dec_tree_list)
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))
  *             max_num_classes = np.max(self.num_classes)             # <<<<<<<<<<<<<<
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, max_num_classes+2))
  */
     __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_max); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -9084,15 +9108,15 @@
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_max_num_classes = __pyx_t_1;
     __pyx_t_1 = 0;
 
     /* "structureboost/coarsage.pyx":329
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))
  *             max_num_classes = np.max(self.num_classes)
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1             # <<<<<<<<<<<<<<
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1             # <<<<<<<<<<<<<<
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, max_num_classes+2))
  *             for i in range(num_dt):
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
@@ -9117,15 +9141,15 @@
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 329, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
@@ -9135,15 +9159,15 @@
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int, __pyx_t_5) < 0) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
     /* "structureboost/coarsage.pyx":330
  *             max_num_classes = np.max(self.num_classes)
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, max_num_classes+2))             # <<<<<<<<<<<<<<
  *             for i in range(num_dt):
  *                 self.convert_dt_to_matrix(i)
  */
     __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 330, __pyx_L1_error)
@@ -9180,15 +9204,15 @@
     if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_float, __pyx_t_5) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
     /* "structureboost/coarsage.pyx":331
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, max_num_classes+2))
  *             for i in range(num_dt):             # <<<<<<<<<<<<<<
  *                 self.convert_dt_to_matrix(i)
  *             self.optimized=True
  */
     __pyx_t_9 = __pyx_v_num_dt;
     __pyx_t_13 = __pyx_t_9;
@@ -10199,42 +10223,42 @@
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
     /* "structureboost/coarsage.pyx":418
  *             curr_binpt_vec = self.get_bin_pts(y_train, self.random_seed+i, no_growth_mode=True)
  *             self.binpt_vec_list.append(curr_binpt_vec.copy())
  *             self.num_classes.append(len(curr_binpt_vec)-1)             # <<<<<<<<<<<<<<
  *             i+=1
- *         self.num_classes=np.array(self.num_classes, dtype=np.int_)
+ *         self.num_classes=np.array(self.num_classes, dtype=np.int32)
  */
     __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_num_classes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_11 = PyObject_Length(__pyx_v_curr_binpt_vec); if (unlikely(__pyx_t_11 == ((Py_ssize_t)-1))) __PYX_ERR(0, 418, __pyx_L1_error)
     __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_11 - 1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_10 = __Pyx_PyObject_Append(__pyx_t_7, __pyx_t_2); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
     /* "structureboost/coarsage.pyx":419
  *             self.binpt_vec_list.append(curr_binpt_vec.copy())
  *             self.num_classes.append(len(curr_binpt_vec)-1)
  *             i+=1             # <<<<<<<<<<<<<<
- *         self.num_classes=np.array(self.num_classes, dtype=np.int_)
+ *         self.num_classes=np.array(self.num_classes, dtype=np.int32)
  * 
  */
     __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_v_i, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_i, __pyx_t_2);
     __pyx_t_2 = 0;
   }
 
   /* "structureboost/coarsage.pyx":420
  *             self.num_classes.append(len(curr_binpt_vec)-1)
  *             i+=1
- *         self.num_classes=np.array(self.num_classes, dtype=np.int_)             # <<<<<<<<<<<<<<
+ *         self.num_classes=np.array(self.num_classes, dtype=np.int32)             # <<<<<<<<<<<<<<
  * 
  *         super().fit(X_train, y_train, eval_set=eval_set, eval_freq=eval_freq,
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_array); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
@@ -10246,29 +10270,29 @@
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2);
   __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_int); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_int32); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_num_classes, __pyx_t_12) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
   /* "structureboost/coarsage.pyx":422
- *         self.num_classes=np.array(self.num_classes, dtype=np.int_)
+ *         self.num_classes=np.array(self.num_classes, dtype=np.int32)
  * 
  *         super().fit(X_train, y_train, eval_set=eval_set, eval_freq=eval_freq,             # <<<<<<<<<<<<<<
  *             early_stop_past_steps=early_stop_past_steps,
  *             choose_best_eval=choose_best_eval, verbose=verbose)
  */
   __pyx_t_12 = __Pyx_CyFunction_GetClassObj(__pyx_self);
   if (!__pyx_t_12) { PyErr_SetString(PyExc_SystemError, "super(): empty __class__ cell"); __PYX_ERR(0, 422, __pyx_L1_error) }
@@ -10316,15 +10340,15 @@
  * 
  * 
  */
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_choose_best_eval, __pyx_v_choose_best_eval) < 0) __PYX_ERR(0, 422, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_verbose, __pyx_v_verbose) < 0) __PYX_ERR(0, 422, __pyx_L1_error)
 
   /* "structureboost/coarsage.pyx":422
- *         self.num_classes=np.array(self.num_classes, dtype=np.int_)
+ *         self.num_classes=np.array(self.num_classes, dtype=np.int32)
  * 
  *         super().fit(X_train, y_train, eval_set=eval_set, eval_freq=eval_freq,             # <<<<<<<<<<<<<<
  *             early_stop_past_steps=early_stop_past_steps,
  *             choose_best_eval=choose_best_eval, verbose=verbose)
  */
   __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 422, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
@@ -17167,15 +17191,15 @@
   return __pyx_r;
 }
 
 /* "structureboost/coarsage.pyx":628
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[np.int_t, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_8coarsage_9predict_with_tensor_c_mc(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_14structureboost_8coarsage_8predict_with_tensor_c_mc[] = "This is the same as the structure_gb_multi version except for num_classes.\n\n    Specifically, this permits that different trees may have a different \n    number of classes.";
 static PyMethodDef __pyx_mdef_14structureboost_8coarsage_9predict_with_tensor_c_mc = {"predict_with_tensor_c_mc", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_8coarsage_9predict_with_tensor_c_mc, METH_VARARGS|METH_KEYWORDS, __pyx_doc_14structureboost_8coarsage_8predict_with_tensor_c_mc};
@@ -17334,15 +17358,15 @@
   Py_ssize_t __pyx_t_18;
   long __pyx_t_19;
   long __pyx_t_20;
   long __pyx_t_21;
   Py_ssize_t __pyx_t_22;
   Py_ssize_t __pyx_t_23;
   Py_ssize_t __pyx_t_24;
-  __pyx_t_5numpy_int_t __pyx_t_25;
+  __pyx_t_5numpy_int32_t __pyx_t_25;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__34)
   __Pyx_RefNannySetupContext("predict_with_tensor_c_mc", 0);
   __Pyx_TraceCall("predict_with_tensor_c_mc", __pyx_f[0], 628, 0, __PYX_ERR(0, 628, __pyx_L1_error));
   __pyx_pybuffer_res_tens.pybuffer.buf = NULL;
@@ -17372,25 +17396,25 @@
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm_float.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm_float, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 628, __pyx_L1_error)
   }
   __pyx_pybuffernd_dtm_float.diminfo[0].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_dtm_float.diminfo[0].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_dtm_float.diminfo[1].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_dtm_float.diminfo[1].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_dtm_float.diminfo[2].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_dtm_float.diminfo[2].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[2];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 628, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 628, __pyx_L1_error)
   }
   __pyx_pybuffernd_dtm.diminfo[0].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_dtm.diminfo[0].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_dtm.diminfo[1].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_dtm.diminfo[1].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_dtm.diminfo[2].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_dtm.diminfo[2].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[2];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feat_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_feat_array, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 628, __pyx_L1_error)
   }
   __pyx_pybuffernd_feat_array.diminfo[0].strides = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_feat_array.diminfo[0].shape = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_feat_array.diminfo[1].strides = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_feat_array.diminfo[1].shape = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.shape[1];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_num_classes_arr.rcbuffer->pybuffer, (PyObject*)__pyx_v_num_classes_arr, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 628, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_num_classes_arr.rcbuffer->pybuffer, (PyObject*)__pyx_v_num_classes_arr, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 628, __pyx_L1_error)
   }
   __pyx_pybuffernd_num_classes_arr.diminfo[0].strides = __pyx_pybuffernd_num_classes_arr.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_num_classes_arr.diminfo[0].shape = __pyx_pybuffernd_num_classes_arr.rcbuffer->pybuffer.shape[0];
 
   /* "structureboost/coarsage.pyx":637
  *     number of classes."""
  *     cdef long cat_vals_end
  *     cdef long max_num_classes = np.max(num_classes_arr)             # <<<<<<<<<<<<<<
@@ -17495,15 +17519,15 @@
   __pyx_t_8 = 0;
   __pyx_v_res_tens = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "structureboost/coarsage.pyx":644
  *     cdef double curr_val, ind_doub
  *     cdef bint at_leaf, found_val
- *     cdef np.ndarray[np.int_t, ndim=2] isnan_array = np.isnan(feat_array).astype(int)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.int32_t, ndim=2] isnan_array = np.isnan(feat_array).astype(np.int32)             # <<<<<<<<<<<<<<
  * 
  *     # These are in dtm_float
  */
   __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 644, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_isnan); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 644, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
@@ -17522,34 +17546,40 @@
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 644, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_astype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 644, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 644, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 644, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_2, ((PyObject *)(&PyInt_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_6, ((PyObject *)(&PyInt_Type)));
+  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_2, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_7);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 644, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 644, __pyx_L1_error)
   __pyx_t_9 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_isnan_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_isnan_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_isnan_array = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 644, __pyx_L1_error)
     } else {__pyx_pybuffernd_isnan_array.diminfo[0].strides = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_isnan_array.diminfo[0].shape = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_isnan_array.diminfo[1].strides = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_isnan_array.diminfo[1].shape = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_9 = 0;
   __pyx_v_isnan_array = ((PyArrayObject *)__pyx_t_1);
@@ -17688,15 +17718,15 @@
  * 
  *     for k in range(dtm.shape[0]):
  *         num_classes=num_classes_arr[k]             # <<<<<<<<<<<<<<
  *         for ri in range(feat_array.shape[0]):
  *             cn = 0
  */
     __pyx_t_12 = __pyx_v_k;
-    __pyx_v_num_classes = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_num_classes_arr.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_num_classes_arr.diminfo[0].strides));
+    __pyx_v_num_classes = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_num_classes_arr.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_num_classes_arr.diminfo[0].strides));
 
     /* "structureboost/coarsage.pyx":668
  *     for k in range(dtm.shape[0]):
  *         num_classes=num_classes_arr[k]
  *         for ri in range(feat_array.shape[0]):             # <<<<<<<<<<<<<<
  *             cn = 0
  *             at_leaf = 0
@@ -17741,15 +17771,15 @@
  *                 if dtm[k,cn, NODE_TYPE]==LEAF:             # <<<<<<<<<<<<<<
  *                     at_leaf = 1
  *                     for q in range(num_classes):
  */
         __pyx_t_12 = __pyx_v_k;
         __pyx_t_17 = __pyx_v_cn;
         __pyx_t_18 = __pyx_v_NODE_TYPE;
-        __pyx_t_16 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_LEAF) != 0);
+        __pyx_t_16 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_LEAF) != 0);
         if (__pyx_t_16) {
 
           /* "structureboost/coarsage.pyx":674
  *                 cn = int(cn)
  *                 if dtm[k,cn, NODE_TYPE]==LEAF:
  *                     at_leaf = 1             # <<<<<<<<<<<<<<
  *                     for q in range(num_classes):
@@ -17801,61 +17831,61 @@
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:             # <<<<<<<<<<<<<<
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:
  */
         __pyx_t_12 = __pyx_v_k;
         __pyx_t_17 = __pyx_v_cn;
         __pyx_t_18 = __pyx_v_NODE_TYPE;
-        __pyx_t_16 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_NUMER) != 0);
+        __pyx_t_16 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_NUMER) != 0);
         if (__pyx_t_16) {
 
           /* "structureboost/coarsage.pyx":678
  *                         res_tens[ri,k,q] = dtm_float[k,cn,NODE_VALUE_START+q]
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]             # <<<<<<<<<<<<<<
  *                     if isnan_array[ri,ind]:
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]
  */
           __pyx_t_18 = __pyx_v_k;
           __pyx_t_17 = __pyx_v_cn;
           __pyx_t_12 = __pyx_v_FEATURE_COL;
-          __pyx_v_ind = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides));
+          __pyx_v_ind = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides));
 
           /* "structureboost/coarsage.pyx":679
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:             # <<<<<<<<<<<<<<
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]
  *                     else:
  */
           __pyx_t_12 = __pyx_v_ri;
           __pyx_t_17 = __pyx_v_ind;
-          __pyx_t_16 = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_isnan_array.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_isnan_array.diminfo[1].strides)) != 0);
+          __pyx_t_16 = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_isnan_array.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_isnan_array.diminfo[1].strides)) != 0);
           if (__pyx_t_16) {
 
             /* "structureboost/coarsage.pyx":680
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]             # <<<<<<<<<<<<<<
  *                     else:
  *                         curr_val = feat_array[ri,ind]
  */
             __pyx_t_17 = __pyx_v_k;
             __pyx_t_12 = __pyx_v_cn;
             __pyx_t_18 = __pyx_v_NA_LEFT;
-            if (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) != 0)) {
+            if (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) != 0)) {
               __pyx_t_24 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_22 = __pyx_v_LEFT_CHILD;
-              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
             } else {
               __pyx_t_22 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_24 = __pyx_v_RIGHT_CHILD;
-              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
             }
             __pyx_v_cn = __pyx_t_25;
 
             /* "structureboost/coarsage.pyx":679
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:             # <<<<<<<<<<<<<<
@@ -17887,20 +17917,20 @@
             __pyx_t_12 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_17 = __pyx_v_THRESH;
             if (((__pyx_v_curr_val < (*__Pyx_BufPtrStrided3d(double *, __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm_float.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm_float.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm_float.diminfo[2].strides))) != 0)) {
               __pyx_t_24 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_22 = __pyx_v_LEFT_CHILD;
-              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
             } else {
               __pyx_t_22 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_24 = __pyx_v_RIGHT_CHILD;
-              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
             }
             __pyx_v_cn = __pyx_t_25;
           }
           __pyx_L12:;
 
           /* "structureboost/coarsage.pyx":677
  *                     for q in range(num_classes):
@@ -17918,29 +17948,29 @@
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:             # <<<<<<<<<<<<<<
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]
  *                     found_val = 0
  */
         __pyx_t_17 = __pyx_v_k;
         __pyx_t_18 = __pyx_v_cn;
         __pyx_t_12 = __pyx_v_NODE_TYPE;
-        __pyx_t_16 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_CATEG) != 0);
+        __pyx_t_16 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_CATEG) != 0);
         if (__pyx_t_16) {
 
           /* "structureboost/coarsage.pyx":685
  *                         cn = dtm[k,cn, LEFT_CHILD] if curr_val<dtm_float[k,cn, THRESH] else dtm[k,cn, RIGHT_CHILD]
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]             # <<<<<<<<<<<<<<
  *                     found_val = 0
  *                     j = CAT_VALS_START
  */
           __pyx_t_12 = __pyx_v_k;
           __pyx_t_18 = __pyx_v_cn;
           __pyx_t_17 = __pyx_v_FEATURE_COL;
           __pyx_t_24 = __pyx_v_ri;
-          __pyx_t_23 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
+          __pyx_t_23 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
           __pyx_v_curr_val = (*__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_feat_array.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_feat_array.diminfo[1].strides));
 
           /* "structureboost/coarsage.pyx":686
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]
  *                     found_val = 0             # <<<<<<<<<<<<<<
  *                     j = CAT_VALS_START
@@ -17963,15 +17993,15 @@
  *                     cat_vals_end = CAT_VALS_START + dtm[k, cn, NUM_CAT_VALS]             # <<<<<<<<<<<<<<
  *                     while ((not found_val) & (j<cat_vals_end)):
  *                         if curr_val==dtm[k,cn, j]:
  */
           __pyx_t_17 = __pyx_v_k;
           __pyx_t_18 = __pyx_v_cn;
           __pyx_t_12 = __pyx_v_NUM_CAT_VALS;
-          __pyx_v_cat_vals_end = (__pyx_v_CAT_VALS_START + (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides)));
+          __pyx_v_cat_vals_end = (__pyx_v_CAT_VALS_START + (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides)));
 
           /* "structureboost/coarsage.pyx":689
  *                     j = CAT_VALS_START
  *                     cat_vals_end = CAT_VALS_START + dtm[k, cn, NUM_CAT_VALS]
  *                     while ((not found_val) & (j<cat_vals_end)):             # <<<<<<<<<<<<<<
  *                         if curr_val==dtm[k,cn, j]:
  *                             found_val=1
@@ -17986,15 +18016,15 @@
  *                         if curr_val==dtm[k,cn, j]:             # <<<<<<<<<<<<<<
  *                             found_val=1
  *                         else:
  */
             __pyx_t_12 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_17 = __pyx_v_j;
-            __pyx_t_16 = ((__pyx_v_curr_val == (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides))) != 0);
+            __pyx_t_16 = ((__pyx_v_curr_val == (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides))) != 0);
             if (__pyx_t_16) {
 
               /* "structureboost/coarsage.pyx":691
  *                     while ((not found_val) & (j<cat_vals_end)):
  *                         if curr_val==dtm[k,cn, j]:
  *                             found_val=1             # <<<<<<<<<<<<<<
  *                         else:
@@ -18032,20 +18062,20 @@
  *     return(res_tens)
  * 
  */
           if ((__pyx_v_found_val != 0)) {
             __pyx_t_17 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_12 = __pyx_v_LEFT_CHILD;
-            __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides));
+            __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[2].strides));
           } else {
             __pyx_t_12 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_17 = __pyx_v_RIGHT_CHILD;
-            __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
+            __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
           }
           __pyx_v_cn = __pyx_t_25;
 
           /* "structureboost/coarsage.pyx":684
  *                         curr_val = feat_array[ri,ind]
  *                         cn = dtm[k,cn, LEFT_CHILD] if curr_val<dtm_float[k,cn, THRESH] else dtm[k,cn, RIGHT_CHILD]
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:             # <<<<<<<<<<<<<<
@@ -18070,15 +18100,15 @@
   __pyx_r = ((PyObject *)__pyx_v_res_tens);
   goto __pyx_L0;
 
   /* "structureboost/coarsage.pyx":628
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[np.int_t, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -18896,15 +18926,15 @@
   __pyx_v_num_fi = ((__pyx_v_fine_binpts->dimensions[0]) - 1);
 
   /* "structureboost/coarsage.pyx":738
  *     cdef long nt = coarse_pred.shape[1]
  *     cdef long num_fi = fine_binpts.shape[0]-1
  *     cdef np.ndarray[double, ndim=2] outmat = np.zeros((num_rows,num_fi))             # <<<<<<<<<<<<<<
  *     cdef long fi_ptr = 0
- *     cdef np.ndarray[np.int_t] coarse_ptr_arr = np.zeros(nt, dtype=np.int_)
+ *     cdef np.ndarray[np.int32_t] coarse_ptr_arr = np.zeros(nt, dtype=np.int32)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_num_rows); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 738, __pyx_L1_error)
@@ -18949,23 +18979,23 @@
   __pyx_v_outmat = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "structureboost/coarsage.pyx":739
  *     cdef long num_fi = fine_binpts.shape[0]-1
  *     cdef np.ndarray[double, ndim=2] outmat = np.zeros((num_rows,num_fi))
  *     cdef long fi_ptr = 0             # <<<<<<<<<<<<<<
- *     cdef np.ndarray[np.int_t] coarse_ptr_arr = np.zeros(nt, dtype=np.int_)
+ *     cdef np.ndarray[np.int32_t] coarse_ptr_arr = np.zeros(nt, dtype=np.int32)
  *     cdef long row_ptr = 0
  */
   __pyx_v_fi_ptr = 0;
 
   /* "structureboost/coarsage.pyx":740
  *     cdef np.ndarray[double, ndim=2] outmat = np.zeros((num_rows,num_fi))
  *     cdef long fi_ptr = 0
- *     cdef np.ndarray[np.int_t] coarse_ptr_arr = np.zeros(nt, dtype=np.int_)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.int32_t] coarse_ptr_arr = np.zeros(nt, dtype=np.int32)             # <<<<<<<<<<<<<<
  *     cdef long row_ptr = 0
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 740, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 740, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
@@ -18977,41 +19007,41 @@
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 740, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 740, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 740, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 740, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 740, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 740, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 740, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_2);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_coarse_ptr_arr = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 740, __pyx_L1_error)
     } else {__pyx_pybuffernd_coarse_ptr_arr.diminfo[0].strides = __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_coarse_ptr_arr.diminfo[0].shape = __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_coarse_ptr_arr = ((PyArrayObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "structureboost/coarsage.pyx":741
  *     cdef long fi_ptr = 0
- *     cdef np.ndarray[np.int_t] coarse_ptr_arr = np.zeros(nt, dtype=np.int_)
+ *     cdef np.ndarray[np.int32_t] coarse_ptr_arr = np.zeros(nt, dtype=np.int32)
  *     cdef long row_ptr = 0             # <<<<<<<<<<<<<<
  * 
  *     for fi_ptr in range(num_fi):
  */
   __pyx_v_row_ptr = 0;
 
   /* "structureboost/coarsage.pyx":743
@@ -19056,15 +19086,15 @@
  *                 outmat[row_ptr, fi_ptr] += coarse_pred[row_ptr, i, coarse_ptr_arr[i]] * lr             # <<<<<<<<<<<<<<
  *             if fine_binpts[fi_ptr+1] >= bv_mat[i,coarse_ptr_arr[i]+1]:
  *                 coarse_ptr_arr[i]+=1
  */
         __pyx_t_17 = __pyx_v_i;
         __pyx_t_18 = __pyx_v_row_ptr;
         __pyx_t_19 = __pyx_v_i;
-        __pyx_t_20 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_coarse_ptr_arr.diminfo[0].strides));
+        __pyx_t_20 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_coarse_ptr_arr.diminfo[0].strides));
         __pyx_t_21 = __pyx_v_row_ptr;
         __pyx_t_22 = __pyx_v_fi_ptr;
         *__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_outmat.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_outmat.diminfo[0].strides, __pyx_t_22, __pyx_pybuffernd_outmat.diminfo[1].strides) += ((*__Pyx_BufPtrStrided3d(double *, __pyx_pybuffernd_coarse_pred.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_coarse_pred.diminfo[0].strides, __pyx_t_19, __pyx_pybuffernd_coarse_pred.diminfo[1].strides, __pyx_t_20, __pyx_pybuffernd_coarse_pred.diminfo[2].strides)) * __pyx_v_lr);
       }
 
       /* "structureboost/coarsage.pyx":747
  *             for row_ptr in range(num_rows):
@@ -19072,27 +19102,27 @@
  *             if fine_binpts[fi_ptr+1] >= bv_mat[i,coarse_ptr_arr[i]+1]:             # <<<<<<<<<<<<<<
  *                 coarse_ptr_arr[i]+=1
  *     return(outmat)
  */
       __pyx_t_17 = (__pyx_v_fi_ptr + 1);
       __pyx_t_20 = __pyx_v_i;
       __pyx_t_19 = __pyx_v_i;
-      __pyx_t_18 = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_coarse_ptr_arr.diminfo[0].strides)) + 1);
+      __pyx_t_18 = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_coarse_ptr_arr.diminfo[0].strides)) + 1);
       __pyx_t_23 = (((*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_fine_binpts.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_fine_binpts.diminfo[0].strides)) >= (*__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_bv_mat.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_bv_mat.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_bv_mat.diminfo[1].strides))) != 0);
       if (__pyx_t_23) {
 
         /* "structureboost/coarsage.pyx":748
  *                 outmat[row_ptr, fi_ptr] += coarse_pred[row_ptr, i, coarse_ptr_arr[i]] * lr
  *             if fine_binpts[fi_ptr+1] >= bv_mat[i,coarse_ptr_arr[i]+1]:
  *                 coarse_ptr_arr[i]+=1             # <<<<<<<<<<<<<<
  *     return(outmat)
  * 
  */
         __pyx_t_20 = __pyx_v_i;
-        *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_coarse_ptr_arr.diminfo[0].strides) += 1;
+        *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_coarse_ptr_arr.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_coarse_ptr_arr.diminfo[0].strides) += 1;
 
         /* "structureboost/coarsage.pyx":747
  *             for row_ptr in range(num_rows):
  *                 outmat[row_ptr, fi_ptr] += coarse_pred[row_ptr, i, coarse_ptr_arr[i]] * lr
  *             if fine_binpts[fi_ptr+1] >= bv_mat[i,coarse_ptr_arr[i]+1]:             # <<<<<<<<<<<<<<
  *                 coarse_ptr_arr[i]+=1
  *     return(outmat)
@@ -20504,15 +20534,15 @@
   {&__pyx_n_s_init_bin_pts, __pyx_k_init_bin_pts, sizeof(__pyx_k_init_bin_pts), 0, 0, 1, 1},
   {&__pyx_n_s_init_logprobmat_fine, __pyx_k_init_logprobmat_fine, sizeof(__pyx_k_init_logprobmat_fine), 0, 0, 1, 1},
   {&__pyx_n_s_init_pdf, __pyx_k_init_pdf, sizeof(__pyx_k_init_pdf), 0, 0, 1, 1},
   {&__pyx_n_s_init_pdf_fine, __pyx_k_init_pdf_fine, sizeof(__pyx_k_init_pdf_fine), 0, 0, 1, 1},
   {&__pyx_n_s_initial_growth_steps, __pyx_k_initial_growth_steps, sizeof(__pyx_k_initial_growth_steps), 0, 0, 1, 1},
   {&__pyx_n_s_initial_model, __pyx_k_initial_model, sizeof(__pyx_k_initial_model), 0, 0, 1, 1},
   {&__pyx_n_s_initial_pred, __pyx_k_initial_pred, sizeof(__pyx_k_initial_pred), 0, 0, 1, 1},
-  {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
+  {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
   {&__pyx_n_s_inv_cti, __pyx_k_inv_cti, sizeof(__pyx_k_inv_cti), 0, 0, 1, 1},
   {&__pyx_n_s_isin, __pyx_k_isin, sizeof(__pyx_k_isin), 0, 0, 1, 1},
   {&__pyx_n_s_isnan, __pyx_k_isnan, sizeof(__pyx_k_isnan), 0, 0, 1, 1},
   {&__pyx_n_s_isnan_array, __pyx_k_isnan_array, sizeof(__pyx_k_isnan_array), 0, 0, 1, 1},
   {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
   {&__pyx_n_s_j, __pyx_k_j, sizeof(__pyx_k_j), 0, 0, 1, 1},
   {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
@@ -21139,15 +21169,15 @@
   __Pyx_GIVEREF(__pyx_tuple__67);
   __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(7, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_coarsage_pyx, __pyx_n_s_expand_result_mat, 609, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 609, __pyx_L1_error)
 
   /* "structureboost/coarsage.pyx":628
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[np.int_t, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
   __pyx_tuple__68 = PyTuple_Pack(32, __pyx_n_s_dtm_float, __pyx_n_s_dtm, __pyx_n_s_feat_array, __pyx_n_s_num_classes_arr, __pyx_n_s_cat_vals_end, __pyx_n_s_max_num_classes, __pyx_n_s_num_classes, __pyx_n_s_res_tens, __pyx_n_s_cn, __pyx_n_s_ri, __pyx_n_s_ind, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_q, __pyx_n_s_curr_val, __pyx_n_s_ind_doub, __pyx_n_s_at_leaf, __pyx_n_s_found_val, __pyx_n_s_isnan_array, __pyx_n_s_THRESH, __pyx_n_s_NODE_WEIGHT, __pyx_n_s_NODE_VALUE_START, __pyx_n_s_NODE_TYPE, __pyx_n_s_FEATURE_COL, __pyx_n_s_LEFT_CHILD, __pyx_n_s_RIGHT_CHILD, __pyx_n_s_NA_LEFT, __pyx_n_s_NUM_CAT_VALS, __pyx_n_s_CAT_VALS_START, __pyx_n_s_LEAF, __pyx_n_s_NUMER, __pyx_n_s_CATEG); if (unlikely(!__pyx_tuple__68)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__68);
   __Pyx_GIVEREF(__pyx_tuple__68);
   __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(4, 0, 32, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_coarsage_pyx, __pyx_n_s_predict_with_tensor_c_mc, 628, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 628, __pyx_L1_error)
 
@@ -22087,15 +22117,15 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_expand_result_mat, __pyx_t_2) < 0) __PYX_ERR(0, 609, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "structureboost/coarsage.pyx":628
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[np.int_t, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_8coarsage_9predict_with_tensor_c_mc, NULL, __pyx_n_s_structureboost_coarsage); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_predict_with_tensor_c_mc, __pyx_t_2) < 0) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
```

### Comparing `structureboost-0.4.2/structureboost/graphs.c` & `structureboost-0.4.3/structureboost/graphs.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.2/structureboost/pdf_discrete.c` & `structureboost-0.4.3/structureboost/pdf_discrete.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.2/structureboost/pdf_group.c` & `structureboost-0.4.3/structureboost/pdf_group.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.2/structureboost/pdf_set.c` & `structureboost-0.4.3/structureboost/pdf_set.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.2/structureboost/prob_regr_unit.c` & `structureboost-0.4.3/structureboost/prob_regr_unit.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.2/structureboost/prob_regressor.c` & `structureboost-0.4.3/structureboost/prob_regressor.c`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.2/structureboost/structure_dt.c` & `structureboost-0.4.3/structureboost/structure_dt.c`

 * *Files 0% similar despite different names*

```diff
@@ -2813,15 +2813,15 @@
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *, int, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int_t = { "int_t", NULL, sizeof(__pyx_t_5numpy_int_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int_t), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t = { "int32_t", NULL, sizeof(__pyx_t_5numpy_int32_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int32_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int32_t), 0 };
 #define __Pyx_MODULE_NAME "structureboost.structure_dt"
 extern int __pyx_module_is_main_structureboost__structure_dt;
 int __pyx_module_is_main_structureboost__structure_dt = 0;
 
 /* Implementation of 'structureboost.structure_dt' */
 static PyObject *__pyx_builtin_object;
 static PyObject *__pyx_builtin_range;
@@ -2854,15 +2854,14 @@
 static const char __pyx_k_col[] = "col";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_drd[] = "drd";
 static const char __pyx_k_esm[] = "esm";
 static const char __pyx_k_fit[] = "fit";
 static const char __pyx_k_ind[] = "ind";
 static const char __pyx_k_inf[] = "inf";
-static const char __pyx_k_int[] = "int_";
 static const char __pyx_k_lni[] = "lni";
 static const char __pyx_k_loc[] = "loc";
 static const char __pyx_k_lvi[] = "lvi";
 static const char __pyx_k_max[] = "max";
 static const char __pyx_k_mid[] = "mid";
 static const char __pyx_k_min[] = "min";
 static const char __pyx_k_nan[] = "nan";
@@ -2916,14 +2915,15 @@
 static const char __pyx_k_enter[] = "__enter__";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_gamma[] = "gamma";
 static const char __pyx_k_graph[] = "graph";
 static const char __pyx_k_ind_a[] = "ind_a";
 static const char __pyx_k_ind_b[] = "ind_b";
+static const char __pyx_k_int32[] = "int32";
 static const char __pyx_k_isnan[] = "isnan";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_lsize[] = "lsize";
 static const char __pyx_k_max_i[] = "max_i";
 static const char __pyx_k_min_i[] = "min_i";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
@@ -3673,15 +3673,15 @@
 static PyObject *__pyx_n_s_ind_subset_right;
 static PyObject *__pyx_n_s_index_range;
 static PyObject *__pyx_n_s_inds;
 static PyObject *__pyx_n_s_inf;
 static PyObject *__pyx_n_s_init;
 static PyObject *__pyx_n_s_init_for_span_trees;
 static PyObject *__pyx_n_s_initialize_best_split_dict;
-static PyObject *__pyx_n_s_int;
+static PyObject *__pyx_n_s_int32;
 static PyObject *__pyx_n_u_interior;
 static PyObject *__pyx_n_s_interp_mode;
 static PyObject *__pyx_n_u_interp_mode;
 static PyObject *__pyx_n_s_is_integer_valued;
 static PyObject *__pyx_n_s_isin;
 static PyObject *__pyx_n_s_isnan;
 static PyObject *__pyx_n_s_isnull;
@@ -10623,43 +10623,43 @@
   __pyx_t_3 = 0;
 
   /* "structureboost/structure_dt.pyx":311
  *                                                 'subfeature_list']]
  *         data_array = self.X_train.to_numpy()[:, subfeature_indices]
  *         num_query_pts = data_array.shape[0]             # <<<<<<<<<<<<<<
  *         num_vor_dims = data_array.shape[1]
- *         feat_vec = np.zeros(num_query_pts,dtype=np.int_)
+ *         feat_vec = np.zeros(num_query_pts,dtype=np.int32)
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 311, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 311, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_num_query_pts = __pyx_t_6;
   __pyx_t_6 = 0;
 
   /* "structureboost/structure_dt.pyx":312
  *         data_array = self.X_train.to_numpy()[:, subfeature_indices]
  *         num_query_pts = data_array.shape[0]
  *         num_vor_dims = data_array.shape[1]             # <<<<<<<<<<<<<<
- *         feat_vec = np.zeros(num_query_pts,dtype=np.int_)
+ *         feat_vec = np.zeros(num_query_pts,dtype=np.int32)
  *         feat_vec = map_to_nn_point_index(best_split_dict['vor_pts'],
  */
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_6, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_num_vor_dims = __pyx_t_3;
   __pyx_t_3 = 0;
 
   /* "structureboost/structure_dt.pyx":313
  *         num_query_pts = data_array.shape[0]
  *         num_vor_dims = data_array.shape[1]
- *         feat_vec = np.zeros(num_query_pts,dtype=np.int_)             # <<<<<<<<<<<<<<
+ *         feat_vec = np.zeros(num_query_pts,dtype=np.int32)             # <<<<<<<<<<<<<<
  *         feat_vec = map_to_nn_point_index(best_split_dict['vor_pts'],
  *                                          data_array,
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
@@ -10669,61 +10669,61 @@
   __Pyx_INCREF(__pyx_v_num_query_pts);
   __Pyx_GIVEREF(__pyx_v_num_query_pts);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_num_query_pts);
   __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_feat_vec = __pyx_t_7;
   __pyx_t_7 = 0;
 
   /* "structureboost/structure_dt.pyx":314
  *         num_vor_dims = data_array.shape[1]
- *         feat_vec = np.zeros(num_query_pts,dtype=np.int_)
+ *         feat_vec = np.zeros(num_query_pts,dtype=np.int32)
  *         feat_vec = map_to_nn_point_index(best_split_dict['vor_pts'],             # <<<<<<<<<<<<<<
  *                                          data_array,
  *                                          feat_vec,
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_map_to_nn_point_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_best_split_dict, __pyx_n_u_vor_pts); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
   /* "structureboost/structure_dt.pyx":317
  *                                          data_array,
  *                                          feat_vec,
  *                                          best_split_dict['vor_pts'].shape[0],             # <<<<<<<<<<<<<<
  *                                          num_query_pts, num_vor_dims)
- *         fs_array = np.fromiter(best_split_dict['left_split'], int,
+ *         fs_array = np.fromiter(best_split_dict['left_split'], np.int32,
  */
   __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_best_split_dict, __pyx_n_u_vor_pts); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "structureboost/structure_dt.pyx":318
  *                                          feat_vec,
  *                                          best_split_dict['vor_pts'].shape[0],
  *                                          num_query_pts, num_vor_dims)             # <<<<<<<<<<<<<<
- *         fs_array = np.fromiter(best_split_dict['left_split'], int,
- *                                len(best_split_dict['left_split'])).astype(np.int_)
+ *         fs_array = np.fromiter(best_split_dict['left_split'], np.int32,
+ *                                len(best_split_dict['left_split']))
  */
   __pyx_t_2 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -10784,251 +10784,234 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF_SET(__pyx_v_feat_vec, __pyx_t_7);
   __pyx_t_7 = 0;
 
   /* "structureboost/structure_dt.pyx":319
  *                                          best_split_dict['vor_pts'].shape[0],
  *                                          num_query_pts, num_vor_dims)
- *         fs_array = np.fromiter(best_split_dict['left_split'], int,             # <<<<<<<<<<<<<<
- *                                len(best_split_dict['left_split'])).astype(np.int_)
+ *         fs_array = np.fromiter(best_split_dict['left_split'], np.int32,             # <<<<<<<<<<<<<<
+ *                                len(best_split_dict['left_split']))
  *         vec_len = len(feat_vec)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_fromiter); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_fromiter); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_best_split_dict, __pyx_n_u_left_split); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_best_split_dict, __pyx_n_u_left_split); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 319, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_int32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "structureboost/structure_dt.pyx":320
  *                                          num_query_pts, num_vor_dims)
- *         fs_array = np.fromiter(best_split_dict['left_split'], int,
- *                                len(best_split_dict['left_split'])).astype(np.int_)             # <<<<<<<<<<<<<<
+ *         fs_array = np.fromiter(best_split_dict['left_split'], np.int32,
+ *                                len(best_split_dict['left_split']))             # <<<<<<<<<<<<<<
  *         vec_len = len(feat_vec)
  *         lsplit_len = len(fs_array)
  */
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_best_split_dict, __pyx_n_u_left_split); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 320, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyObject_Length(__pyx_t_3); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 320, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 320, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_best_split_dict, __pyx_n_u_left_split); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 320, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_4 = PyObject_Length(__pyx_t_6); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 320, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = PyInt_FromSsize_t(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 320, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_2 = NULL;
   __pyx_t_8 = 0;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_6);
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
+      __Pyx_DECREF_SET(__pyx_t_9, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_6)) {
-    PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_t_9, ((PyObject *)(&PyInt_Type)), __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
+  if (PyFunction_Check(__pyx_t_9)) {
+    PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_t_1, __pyx_t_3, __pyx_t_6};
+    __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
-    PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_t_9, ((PyObject *)(&PyInt_Type)), __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
+    PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_t_1, __pyx_t_3, __pyx_t_6};
+    __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
     __pyx_t_10 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
-    __Pyx_GIVEREF(__pyx_t_9);
-    PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_8, __pyx_t_9);
-    __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
-    __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
-    PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_8, ((PyObject *)(&PyInt_Type)));
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_8, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_10, 2+__pyx_t_8, __pyx_t_3);
-    __pyx_t_9 = 0;
+    PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_8, __pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_10, 2+__pyx_t_8, __pyx_t_6);
+    __pyx_t_1 = 0;
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_6 = 0;
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_10, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_astype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 320, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 320, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 320, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_10);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_6);
-    if (likely(__pyx_t_1)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_1);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
-    }
-  }
-  __pyx_t_7 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_1, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_10);
-  __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 320, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_v_fs_array = __pyx_t_7;
   __pyx_t_7 = 0;
 
   /* "structureboost/structure_dt.pyx":321
- *         fs_array = np.fromiter(best_split_dict['left_split'], int,
- *                                len(best_split_dict['left_split'])).astype(np.int_)
+ *         fs_array = np.fromiter(best_split_dict['left_split'], np.int32,
+ *                                len(best_split_dict['left_split']))
  *         vec_len = len(feat_vec)             # <<<<<<<<<<<<<<
  *         lsplit_len = len(fs_array)
- *         left_mask = np.zeros(vec_len, dtype=np.int_)
+ *         left_mask = np.zeros(vec_len, dtype=np.int32)
  */
   __pyx_t_4 = PyObject_Length(__pyx_v_feat_vec); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 321, __pyx_L1_error)
   __pyx_v_vec_len = __pyx_t_4;
 
   /* "structureboost/structure_dt.pyx":322
- *                                len(best_split_dict['left_split'])).astype(np.int_)
+ *                                len(best_split_dict['left_split']))
  *         vec_len = len(feat_vec)
  *         lsplit_len = len(fs_array)             # <<<<<<<<<<<<<<
- *         left_mask = np.zeros(vec_len, dtype=np.int_)
+ *         left_mask = np.zeros(vec_len, dtype=np.int32)
  *         left_mask = get_mask_int_c(feat_vec, fs_array, vec_len,
  */
   __pyx_t_4 = PyObject_Length(__pyx_v_fs_array); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 322, __pyx_L1_error)
   __pyx_v_lsplit_len = __pyx_t_4;
 
   /* "structureboost/structure_dt.pyx":323
  *         vec_len = len(feat_vec)
  *         lsplit_len = len(fs_array)
- *         left_mask = np.zeros(vec_len, dtype=np.int_)             # <<<<<<<<<<<<<<
+ *         left_mask = np.zeros(vec_len, dtype=np.int32)             # <<<<<<<<<<<<<<
  *         left_mask = get_mask_int_c(feat_vec, fs_array, vec_len,
  *                                    lsplit_len, left_mask)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 323, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = PyInt_FromSsize_t(__pyx_v_vec_len); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_GIVEREF(__pyx_t_7);
   PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_7);
   __pyx_t_7 = 0;
   __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 323, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_int32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_10, __pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_left_mask = __pyx_t_3;
   __pyx_t_3 = 0;
 
   /* "structureboost/structure_dt.pyx":324
  *         lsplit_len = len(fs_array)
- *         left_mask = np.zeros(vec_len, dtype=np.int_)
+ *         left_mask = np.zeros(vec_len, dtype=np.int32)
  *         left_mask = get_mask_int_c(feat_vec, fs_array, vec_len,             # <<<<<<<<<<<<<<
  *                                    lsplit_len, left_mask)
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_get_mask_int_c); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 324, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_10 = PyInt_FromSsize_t(__pyx_v_vec_len); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 324, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
 
   /* "structureboost/structure_dt.pyx":325
- *         left_mask = np.zeros(vec_len, dtype=np.int_)
+ *         left_mask = np.zeros(vec_len, dtype=np.int32)
  *         left_mask = get_mask_int_c(feat_vec, fs_array, vec_len,
  *                                    lsplit_len, left_mask)             # <<<<<<<<<<<<<<
  * 
  *         # record info about current node
  */
-  __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_lsplit_len); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 325, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_1 = NULL;
+  __pyx_t_9 = PyInt_FromSsize_t(__pyx_v_lsplit_len); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __pyx_t_6 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
-    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_7);
-    if (likely(__pyx_t_1)) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
+    if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-      __Pyx_INCREF(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_7)) {
-    PyObject *__pyx_temp[6] = {__pyx_t_1, __pyx_v_feat_vec, __pyx_v_fs_array, __pyx_t_10, __pyx_t_6, __pyx_v_left_mask};
+    PyObject *__pyx_temp[6] = {__pyx_t_6, __pyx_v_feat_vec, __pyx_v_fs_array, __pyx_t_10, __pyx_t_9, __pyx_v_left_mask};
     __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_8, 5+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 324, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
-    PyObject *__pyx_temp[6] = {__pyx_t_1, __pyx_v_feat_vec, __pyx_v_fs_array, __pyx_t_10, __pyx_t_6, __pyx_v_left_mask};
+    PyObject *__pyx_temp[6] = {__pyx_t_6, __pyx_v_feat_vec, __pyx_v_fs_array, __pyx_t_10, __pyx_t_9, __pyx_v_left_mask};
     __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_8, 5+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 324, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   } else
   #endif
   {
-    __pyx_t_9 = PyTuple_New(5+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 324, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    if (__pyx_t_1) {
-      __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_1); __pyx_t_1 = NULL;
+    __pyx_t_1 = PyTuple_New(5+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 324, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    if (__pyx_t_6) {
+      __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_INCREF(__pyx_v_feat_vec);
     __Pyx_GIVEREF(__pyx_v_feat_vec);
-    PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_v_feat_vec);
+    PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_8, __pyx_v_feat_vec);
     __Pyx_INCREF(__pyx_v_fs_array);
     __Pyx_GIVEREF(__pyx_v_fs_array);
-    PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_fs_array);
+    PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_8, __pyx_v_fs_array);
     __Pyx_GIVEREF(__pyx_t_10);
-    PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_t_10);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_9, 3+__pyx_t_8, __pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_1, 2+__pyx_t_8, __pyx_t_10);
+    __Pyx_GIVEREF(__pyx_t_9);
+    PyTuple_SET_ITEM(__pyx_t_1, 3+__pyx_t_8, __pyx_t_9);
     __Pyx_INCREF(__pyx_v_left_mask);
     __Pyx_GIVEREF(__pyx_v_left_mask);
-    PyTuple_SET_ITEM(__pyx_t_9, 4+__pyx_t_8, __pyx_v_left_mask);
+    PyTuple_SET_ITEM(__pyx_t_1, 4+__pyx_t_8, __pyx_v_left_mask);
     __pyx_t_10 = 0;
-    __pyx_t_6 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 324, __pyx_L1_error)
+    __pyx_t_9 = 0;
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 324, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF_SET(__pyx_v_left_mask, __pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "structureboost/structure_dt.pyx":328
  * 
@@ -11068,33 +11051,33 @@
   /* "structureboost/structure_dt.pyx":329
  *         # record info about current node
  *         curr_node['left_split'] = best_split_dict['left_split']
  *         curr_node['right_split'] = (best_split_dict['voronoi_graph'].vertices -             # <<<<<<<<<<<<<<
  *                                     best_split_dict['left_split'])
  *         curr_node['num_voronoi_edges'] = len(best_split_dict['voronoi_graph'].edges)
  */
-  __pyx_t_9 = PyNumber_Subtract(__pyx_t_7, __pyx_t_3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 329, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
+  __pyx_t_1 = PyNumber_Subtract(__pyx_t_7, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(PyObject_SetItem(__pyx_v_curr_node, __pyx_n_u_right_split, __pyx_t_9) < 0)) __PYX_ERR(0, 329, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  if (unlikely(PyObject_SetItem(__pyx_v_curr_node, __pyx_n_u_right_split, __pyx_t_1) < 0)) __PYX_ERR(0, 329, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_dt.pyx":331
  *         curr_node['right_split'] = (best_split_dict['voronoi_graph'].vertices -
  *                                     best_split_dict['left_split'])
  *         curr_node['num_voronoi_edges'] = len(best_split_dict['voronoi_graph'].edges)             # <<<<<<<<<<<<<<
  *         curr_node['loss_score'] = best_split_dict['loss_score']
  *         curr_node['split_feature'] = best_split_dict['split_feature']
  */
-  __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_best_split_dict, __pyx_n_u_voronoi_graph); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 331, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_edges); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 331, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_best_split_dict, __pyx_n_u_voronoi_graph); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 331, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_edges); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_4 = PyObject_Length(__pyx_t_3); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (unlikely(PyObject_SetItem(__pyx_v_curr_node, __pyx_n_u_num_voronoi_edges, __pyx_t_3) < 0)) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
@@ -11146,92 +11129,92 @@
   /* "structureboost/structure_dt.pyx":336
  *         sub_feat_list = best_split_dict['subfeature_list']
  *         curr_node['subfeature_list'] = sub_feat_list
  *         sub_feat_cols = np.array([self.train_column_to_int_dict[col] for col in sub_feat_list])             # <<<<<<<<<<<<<<
  *         curr_node['subfeature_cols'] = sub_feat_cols
  *         curr_node['vor_pts'] = best_split_dict['vor_pts']
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_np); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 336, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_array); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_array); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   { /* enter inner scope */
-    __pyx_t_9 = PyList_New(0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 336, __pyx_L11_error)
-    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L11_error)
+    __Pyx_GOTREF(__pyx_t_1);
     if (likely(PyList_CheckExact(__pyx_v_sub_feat_list)) || PyTuple_CheckExact(__pyx_v_sub_feat_list)) {
-      __pyx_t_6 = __pyx_v_sub_feat_list; __Pyx_INCREF(__pyx_t_6); __pyx_t_4 = 0;
+      __pyx_t_9 = __pyx_v_sub_feat_list; __Pyx_INCREF(__pyx_t_9); __pyx_t_4 = 0;
       __pyx_t_5 = NULL;
     } else {
-      __pyx_t_4 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_sub_feat_list); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 336, __pyx_L11_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 336, __pyx_L11_error)
+      __pyx_t_4 = -1; __pyx_t_9 = PyObject_GetIter(__pyx_v_sub_feat_list); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 336, __pyx_L11_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __pyx_t_5 = Py_TYPE(__pyx_t_9)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 336, __pyx_L11_error)
     }
     for (;;) {
       if (likely(!__pyx_t_5)) {
-        if (likely(PyList_CheckExact(__pyx_t_6))) {
-          if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_6)) break;
+        if (likely(PyList_CheckExact(__pyx_t_9))) {
+          if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_9)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_10 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_4); __Pyx_INCREF(__pyx_t_10); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 336, __pyx_L11_error)
+          __pyx_t_10 = PyList_GET_ITEM(__pyx_t_9, __pyx_t_4); __Pyx_INCREF(__pyx_t_10); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 336, __pyx_L11_error)
           #else
-          __pyx_t_10 = PySequence_ITEM(__pyx_t_6, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 336, __pyx_L11_error)
+          __pyx_t_10 = PySequence_ITEM(__pyx_t_9, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 336, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_10);
           #endif
         } else {
-          if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
+          if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_9)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_10 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_4); __Pyx_INCREF(__pyx_t_10); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 336, __pyx_L11_error)
+          __pyx_t_10 = PyTuple_GET_ITEM(__pyx_t_9, __pyx_t_4); __Pyx_INCREF(__pyx_t_10); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 336, __pyx_L11_error)
           #else
-          __pyx_t_10 = PySequence_ITEM(__pyx_t_6, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 336, __pyx_L11_error)
+          __pyx_t_10 = PySequence_ITEM(__pyx_t_9, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 336, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_10);
           #endif
         }
       } else {
-        __pyx_t_10 = __pyx_t_5(__pyx_t_6);
+        __pyx_t_10 = __pyx_t_5(__pyx_t_9);
         if (unlikely(!__pyx_t_10)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
             else __PYX_ERR(0, 336, __pyx_L11_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_10);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr3__pyx_v_col, __pyx_t_10);
       __pyx_t_10 = 0;
       __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_train_column_to_int_dict); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 336, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_10, __pyx_8genexpr3__pyx_v_col); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 336, __pyx_L11_error)
-      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_10, __pyx_8genexpr3__pyx_v_col); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 336, __pyx_L11_error)
+      __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_9, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 336, __pyx_L11_error)
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 336, __pyx_L11_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_col); __pyx_8genexpr3__pyx_v_col = 0;
     goto __pyx_L14_exit_scope;
     __pyx_L11_error:;
     __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_col); __pyx_8genexpr3__pyx_v_col = 0;
     goto __pyx_L1_error;
     __pyx_L14_exit_scope:;
   } /* exit inner scope */
-  __pyx_t_6 = NULL;
+  __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
-    if (likely(__pyx_t_6)) {
+    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
+    if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-      __Pyx_INCREF(__pyx_t_6);
+      __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_6, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_9);
-  __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __pyx_t_3 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_9, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_sub_feat_cols = __pyx_t_3;
   __pyx_t_3 = 0;
 
   /* "structureboost/structure_dt.pyx":337
@@ -11281,26 +11264,26 @@
  *         curr_node['feature_type'] = best_split_dict['feature_type']
  *         curr_mask = curr_node.pop('mask')             # <<<<<<<<<<<<<<
  * 
  *         # Create feature graphs for children
  */
   __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_curr_node, __pyx_n_s_pop); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_9 = NULL;
+  __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
-    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
-    if (likely(__pyx_t_9)) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_7);
+    if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-      __Pyx_INCREF(__pyx_t_9);
+      __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_9, __pyx_n_u_mask) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_n_u_mask);
-  __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_1, __pyx_n_u_mask) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_n_u_mask);
+  __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_curr_mask = __pyx_t_3;
   __pyx_t_3 = 0;
 
   /* "structureboost/structure_dt.pyx":344
@@ -11308,26 +11291,26 @@
  *         # Create feature graphs for children
  *         feature_graphs_left = feature_graphs_node.copy()             # <<<<<<<<<<<<<<
  *         feature_graphs_right = feature_graphs_node.copy()
  * 
  */
   __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_feature_graphs_node, __pyx_n_s_copy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 344, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_9 = NULL;
+  __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
-    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
-    if (likely(__pyx_t_9)) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_7);
+    if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-      __Pyx_INCREF(__pyx_t_9);
+      __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_9) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_9) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 344, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_feature_graphs_left = __pyx_t_3;
   __pyx_t_3 = 0;
 
   /* "structureboost/structure_dt.pyx":345
@@ -11335,26 +11318,26 @@
  *         feature_graphs_left = feature_graphs_node.copy()
  *         feature_graphs_right = feature_graphs_node.copy()             # <<<<<<<<<<<<<<
  * 
  *         self._create_children_nodes(curr_node, feature_graphs_left,
  */
   __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_feature_graphs_node, __pyx_n_s_copy); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_9 = NULL;
+  __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
-    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
-    if (likely(__pyx_t_9)) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_7);
+    if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-      __Pyx_INCREF(__pyx_t_9);
+      __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_9) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_9) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_feature_graphs_right = __pyx_t_3;
   __pyx_t_3 = 0;
 
   /* "structureboost/structure_dt.pyx":347
@@ -11370,66 +11353,66 @@
   /* "structureboost/structure_dt.pyx":348
  * 
  *         self._create_children_nodes(curr_node, feature_graphs_left,
  *                                     feature_graphs_right, curr_mask, left_mask)             # <<<<<<<<<<<<<<
  * 
  *     def evaluate_feature(self, feature_config, feature_graphs, feature_name,
  */
-  __pyx_t_9 = NULL;
+  __pyx_t_1 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
-    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
-    if (likely(__pyx_t_9)) {
+    __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_7);
+    if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-      __Pyx_INCREF(__pyx_t_9);
+      __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_7)) {
-    PyObject *__pyx_temp[6] = {__pyx_t_9, __pyx_v_curr_node, __pyx_v_feature_graphs_left, __pyx_v_feature_graphs_right, __pyx_v_curr_mask, __pyx_v_left_mask};
+    PyObject *__pyx_temp[6] = {__pyx_t_1, __pyx_v_curr_node, __pyx_v_feature_graphs_left, __pyx_v_feature_graphs_right, __pyx_v_curr_mask, __pyx_v_left_mask};
     __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_8, 5+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
-    PyObject *__pyx_temp[6] = {__pyx_t_9, __pyx_v_curr_node, __pyx_v_feature_graphs_left, __pyx_v_feature_graphs_right, __pyx_v_curr_mask, __pyx_v_left_mask};
+    PyObject *__pyx_temp[6] = {__pyx_t_1, __pyx_v_curr_node, __pyx_v_feature_graphs_left, __pyx_v_feature_graphs_right, __pyx_v_curr_mask, __pyx_v_left_mask};
     __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_8, 5+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(5+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 347, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    if (__pyx_t_9) {
-      __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_9); __pyx_t_9 = NULL;
+    __pyx_t_9 = PyTuple_New(5+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 347, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    if (__pyx_t_1) {
+      __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_1); __pyx_t_1 = NULL;
     }
     __Pyx_INCREF(__pyx_v_curr_node);
     __Pyx_GIVEREF(__pyx_v_curr_node);
-    PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_8, __pyx_v_curr_node);
+    PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_v_curr_node);
     __Pyx_INCREF(__pyx_v_feature_graphs_left);
     __Pyx_GIVEREF(__pyx_v_feature_graphs_left);
-    PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_8, __pyx_v_feature_graphs_left);
+    PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_feature_graphs_left);
     __Pyx_INCREF(__pyx_v_feature_graphs_right);
     __Pyx_GIVEREF(__pyx_v_feature_graphs_right);
-    PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_8, __pyx_v_feature_graphs_right);
+    PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_v_feature_graphs_right);
     __Pyx_INCREF(__pyx_v_curr_mask);
     __Pyx_GIVEREF(__pyx_v_curr_mask);
-    PyTuple_SET_ITEM(__pyx_t_6, 3+__pyx_t_8, __pyx_v_curr_mask);
+    PyTuple_SET_ITEM(__pyx_t_9, 3+__pyx_t_8, __pyx_v_curr_mask);
     __Pyx_INCREF(__pyx_v_left_mask);
     __Pyx_GIVEREF(__pyx_v_left_mask);
-    PyTuple_SET_ITEM(__pyx_t_6, 4+__pyx_t_8, __pyx_v_left_mask);
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_6, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
+    PyTuple_SET_ITEM(__pyx_t_9, 4+__pyx_t_8, __pyx_v_left_mask);
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "structureboost/structure_dt.pyx":303
  *                                     left_mask)
  * 
@@ -14060,75 +14043,75 @@
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_dt.pyx":438
  * 
  *         has_na_vals = np.isnan(split_vec[-1])
  *         bin_result_vec = np.searchsorted(split_vec,             # <<<<<<<<<<<<<<
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 438, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_searchsorted); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 438, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "structureboost/structure_dt.pyx":439
  *         has_na_vals = np.isnan(split_vec[-1])
  *         bin_result_vec = np.searchsorted(split_vec,
  *                                          feature_vec,             # <<<<<<<<<<<<<<
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  *         g_sum_bins, h_sum_bins = get_bin_sums_c(g_h_mat,
  */
   __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 438, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_split_vec);
   __Pyx_GIVEREF(__pyx_v_split_vec);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_split_vec);
   __Pyx_INCREF(__pyx_v_feature_vec);
   __Pyx_GIVEREF(__pyx_v_feature_vec);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_feature_vec);
 
   /* "structureboost/structure_dt.pyx":440
  *         bin_result_vec = np.searchsorted(split_vec,
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)             # <<<<<<<<<<<<<<
+ *                                          side='right').astype(np.int32)             # <<<<<<<<<<<<<<
  *         g_sum_bins, h_sum_bins = get_bin_sums_c(g_h_mat,
  *                                                 bin_result_vec,
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 440, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_side, __pyx_n_u_right) < 0) __PYX_ERR(0, 440, __pyx_L1_error)
 
   /* "structureboost/structure_dt.pyx":438
  * 
  *         has_na_vals = np.isnan(split_vec[-1])
  *         bin_result_vec = np.searchsorted(split_vec,             # <<<<<<<<<<<<<<
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  */
   __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 438, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "structureboost/structure_dt.pyx":440
  *         bin_result_vec = np.searchsorted(split_vec,
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)             # <<<<<<<<<<<<<<
+ *                                          side='right').astype(np.int32)             # <<<<<<<<<<<<<<
  *         g_sum_bins, h_sum_bins = get_bin_sums_c(g_h_mat,
  *                                                 bin_result_vec,
  */
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 440, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 440, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 440, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 440, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -14144,15 +14127,15 @@
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_bin_result_vec = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_dt.pyx":441
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  *         g_sum_bins, h_sum_bins = get_bin_sums_c(g_h_mat,             # <<<<<<<<<<<<<<
  *                                                 bin_result_vec,
  *                                                 len(split_vec)+1)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_get_bin_sums_c); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 441, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
@@ -14261,15 +14244,15 @@
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
     __PYX_ERR(0, 441, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
 
   /* "structureboost/structure_dt.pyx":441
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  *         g_sum_bins, h_sum_bins = get_bin_sums_c(g_h_mat,             # <<<<<<<<<<<<<<
  *                                                 bin_result_vec,
  *                                                 len(split_vec)+1)
  */
   __pyx_v_g_sum_bins = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_v_h_sum_bins = __pyx_t_2;
@@ -15806,234 +15789,217 @@
     __pyx_t_3 = 0;
 
     /* "structureboost/structure_dt.pyx":504
  *             curr_partition = list(partition)
  *             left_split = curr_partition[0]
  *             right_split = curr_partition[1]             # <<<<<<<<<<<<<<
  *             if is_integer_valued:
- *                 fs_array = np.fromiter(left_split, int,
+ *                 fs_array = np.fromiter(left_split, np.int32,
  */
     __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_curr_partition, 1, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 504, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_XDECREF_SET(__pyx_v_right_split, __pyx_t_3);
     __pyx_t_3 = 0;
 
     /* "structureboost/structure_dt.pyx":505
  *             left_split = curr_partition[0]
  *             right_split = curr_partition[1]
  *             if is_integer_valued:             # <<<<<<<<<<<<<<
- *                 fs_array = np.fromiter(left_split, int,
- *                                        len(left_split)).astype(np.int_)
+ *                 fs_array = np.fromiter(left_split, np.int32,
+ *                                        len(left_split))
  */
     __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_is_integer_valued); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 505, __pyx_L1_error)
     if (__pyx_t_5) {
 
       /* "structureboost/structure_dt.pyx":506
  *             right_split = curr_partition[1]
  *             if is_integer_valued:
- *                 fs_array = np.fromiter(left_split, int,             # <<<<<<<<<<<<<<
- *                                        len(left_split)).astype(np.int_)
+ *                 fs_array = np.fromiter(left_split, np.int32,             # <<<<<<<<<<<<<<
+ *                                        len(left_split))
  *                 vec_len = len(feature_vec_node)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 506, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_fromiter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 506, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_fromiter); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 506, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 506, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
       /* "structureboost/structure_dt.pyx":507
  *             if is_integer_valued:
- *                 fs_array = np.fromiter(left_split, int,
- *                                        len(left_split)).astype(np.int_)             # <<<<<<<<<<<<<<
+ *                 fs_array = np.fromiter(left_split, np.int32,
+ *                                        len(left_split))             # <<<<<<<<<<<<<<
  *                 vec_len = len(feature_vec_node)
  *                 lsplit_len = len(fs_array)
  */
       __pyx_t_9 = PyObject_Length(__pyx_v_left_split); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 507, __pyx_L1_error)
-      __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 507, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 507, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_10 = NULL;
       __pyx_t_11 = 0;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
-        __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_8);
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+        __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_10)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_8, function);
+          __Pyx_DECREF_SET(__pyx_t_2, function);
           __pyx_t_11 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
-      if (PyFunction_Check(__pyx_t_8)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_10, __pyx_v_left_split, ((PyObject *)(&PyInt_Type)), __pyx_t_2};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_11, 3+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
+      if (PyFunction_Check(__pyx_t_2)) {
+        PyObject *__pyx_temp[4] = {__pyx_t_10, __pyx_v_left_split, __pyx_t_8, __pyx_t_1};
+        __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 3+__pyx_t_11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 506, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_GOTREF(__pyx_t_3);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
-      if (__Pyx_PyFastCFunction_Check(__pyx_t_8)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_10, __pyx_v_left_split, ((PyObject *)(&PyInt_Type)), __pyx_t_2};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_11, 3+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
+      if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
+        PyObject *__pyx_temp[4] = {__pyx_t_10, __pyx_v_left_split, __pyx_t_8, __pyx_t_1};
+        __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 3+__pyx_t_11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 506, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-        __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        __Pyx_GOTREF(__pyx_t_3);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       } else
       #endif
       {
         __pyx_t_12 = PyTuple_New(3+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 506, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         if (__pyx_t_10) {
           __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10); __pyx_t_10 = NULL;
         }
         __Pyx_INCREF(__pyx_v_left_split);
         __Pyx_GIVEREF(__pyx_v_left_split);
         PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, __pyx_v_left_split);
-        __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
-        __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
-        PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, ((PyObject *)(&PyInt_Type)));
-        __Pyx_GIVEREF(__pyx_t_2);
-        PyTuple_SET_ITEM(__pyx_t_12, 2+__pyx_t_11, __pyx_t_2);
-        __pyx_t_2 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_GIVEREF(__pyx_t_8);
+        PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, __pyx_t_8);
+        __Pyx_GIVEREF(__pyx_t_1);
+        PyTuple_SET_ITEM(__pyx_t_12, 2+__pyx_t_11, __pyx_t_1);
+        __pyx_t_8 = 0;
+        __pyx_t_1 = 0;
+        __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 506, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       }
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_astype); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 507, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 507, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 507, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_12);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = NULL;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-        __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_8);
-        if (likely(__pyx_t_1)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-          __Pyx_INCREF(__pyx_t_1);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_8, function);
-        }
-      }
-      __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_1, __pyx_t_12) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_12);
-      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 507, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF_SET(__pyx_v_fs_array, __pyx_t_3);
       __pyx_t_3 = 0;
 
       /* "structureboost/structure_dt.pyx":508
- *                 fs_array = np.fromiter(left_split, int,
- *                                        len(left_split)).astype(np.int_)
+ *                 fs_array = np.fromiter(left_split, np.int32,
+ *                                        len(left_split))
  *                 vec_len = len(feature_vec_node)             # <<<<<<<<<<<<<<
  *                 lsplit_len = len(fs_array)
- *                 mask_left = np.zeros(vec_len, dtype=np.int_)
+ *                 mask_left = np.zeros(vec_len, dtype=np.int32)
  */
       __pyx_t_9 = PyObject_Length(__pyx_v_feature_vec_node); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 508, __pyx_L1_error)
       __pyx_v_vec_len = __pyx_t_9;
 
       /* "structureboost/structure_dt.pyx":509
- *                                        len(left_split)).astype(np.int_)
+ *                                        len(left_split))
  *                 vec_len = len(feature_vec_node)
  *                 lsplit_len = len(fs_array)             # <<<<<<<<<<<<<<
- *                 mask_left = np.zeros(vec_len, dtype=np.int_)
- *                 mask_left = get_mask_int_c(feature_vec_node.astype(np.int_),
+ *                 mask_left = np.zeros(vec_len, dtype=np.int32)
+ *                 mask_left = get_mask_int_c(feature_vec_node.astype(np.int32),
  */
       __pyx_t_9 = PyObject_Length(__pyx_v_fs_array); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 509, __pyx_L1_error)
       __pyx_v_lsplit_len = __pyx_t_9;
 
       /* "structureboost/structure_dt.pyx":510
  *                 vec_len = len(feature_vec_node)
  *                 lsplit_len = len(fs_array)
- *                 mask_left = np.zeros(vec_len, dtype=np.int_)             # <<<<<<<<<<<<<<
- *                 mask_left = get_mask_int_c(feature_vec_node.astype(np.int_),
+ *                 mask_left = np.zeros(vec_len, dtype=np.int32)             # <<<<<<<<<<<<<<
+ *                 mask_left = get_mask_int_c(feature_vec_node.astype(np.int32),
  *                                                fs_array, vec_len, lsplit_len,
  */
       __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 510, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 510, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 510, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_vec_len); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 510, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_12 = PyTuple_New(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 510, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_3);
       __pyx_t_3 = 0;
       __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 510, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 510, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 510, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 510, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 510, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_12, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 510, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 510, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 510, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_XDECREF_SET(__pyx_v_mask_left, __pyx_t_2);
-      __pyx_t_2 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_mask_left, __pyx_t_8);
+      __pyx_t_8 = 0;
 
       /* "structureboost/structure_dt.pyx":511
  *                 lsplit_len = len(fs_array)
- *                 mask_left = np.zeros(vec_len, dtype=np.int_)
- *                 mask_left = get_mask_int_c(feature_vec_node.astype(np.int_),             # <<<<<<<<<<<<<<
+ *                 mask_left = np.zeros(vec_len, dtype=np.int32)
+ *                 mask_left = get_mask_int_c(feature_vec_node.astype(np.int32),             # <<<<<<<<<<<<<<
  *                                                fs_array, vec_len, lsplit_len,
  *                                                mask_left)
  */
       __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_get_mask_int_c); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 511, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_feature_vec_node, __pyx_n_s_astype); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 511, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_feature_vec_node, __pyx_n_s_astype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 511, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
       __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 511, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 511, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 511, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = NULL;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
-        __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_8);
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+        __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_1)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_1);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_8, function);
+          __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
-      __pyx_t_12 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_1, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_10);
+      __pyx_t_12 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_1, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_10);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 511, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_12);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
       /* "structureboost/structure_dt.pyx":512
- *                 mask_left = np.zeros(vec_len, dtype=np.int_)
- *                 mask_left = get_mask_int_c(feature_vec_node.astype(np.int_),
+ *                 mask_left = np.zeros(vec_len, dtype=np.int32)
+ *                 mask_left = get_mask_int_c(feature_vec_node.astype(np.int32),
  *                                                fs_array, vec_len, lsplit_len,             # <<<<<<<<<<<<<<
  *                                                mask_left)
  *             else:
  */
-      __pyx_t_8 = PyInt_FromSsize_t(__pyx_v_vec_len); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 512, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_vec_len); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 512, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_10 = PyInt_FromSsize_t(__pyx_v_lsplit_len); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 512, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
 
       /* "structureboost/structure_dt.pyx":513
- *                 mask_left = get_mask_int_c(feature_vec_node.astype(np.int_),
+ *                 mask_left = get_mask_int_c(feature_vec_node.astype(np.int32),
  *                                                fs_array, vec_len, lsplit_len,
  *                                                mask_left)             # <<<<<<<<<<<<<<
  *             else:
  *                 mask_left = get_mask(feature_vec_node, left_split)
  */
       __pyx_t_1 = NULL;
       __pyx_t_11 = 0;
@@ -16045,69 +16011,69 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_3, function);
           __pyx_t_11 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_3)) {
-        PyObject *__pyx_temp[6] = {__pyx_t_1, __pyx_t_12, __pyx_v_fs_array, __pyx_t_8, __pyx_t_10, __pyx_v_mask_left};
-        __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 5+__pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 511, __pyx_L1_error)
+        PyObject *__pyx_temp[6] = {__pyx_t_1, __pyx_t_12, __pyx_v_fs_array, __pyx_t_2, __pyx_t_10, __pyx_v_mask_left};
+        __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 5+__pyx_t_11); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 511, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-        PyObject *__pyx_temp[6] = {__pyx_t_1, __pyx_t_12, __pyx_v_fs_array, __pyx_t_8, __pyx_t_10, __pyx_v_mask_left};
-        __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 5+__pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 511, __pyx_L1_error)
+        PyObject *__pyx_temp[6] = {__pyx_t_1, __pyx_t_12, __pyx_v_fs_array, __pyx_t_2, __pyx_t_10, __pyx_v_mask_left};
+        __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 5+__pyx_t_11); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 511, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       } else
       #endif
       {
         __pyx_t_13 = PyTuple_New(5+__pyx_t_11); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 511, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_13);
         if (__pyx_t_1) {
           __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_1); __pyx_t_1 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_12);
         PyTuple_SET_ITEM(__pyx_t_13, 0+__pyx_t_11, __pyx_t_12);
         __Pyx_INCREF(__pyx_v_fs_array);
         __Pyx_GIVEREF(__pyx_v_fs_array);
         PyTuple_SET_ITEM(__pyx_t_13, 1+__pyx_t_11, __pyx_v_fs_array);
-        __Pyx_GIVEREF(__pyx_t_8);
-        PyTuple_SET_ITEM(__pyx_t_13, 2+__pyx_t_11, __pyx_t_8);
+        __Pyx_GIVEREF(__pyx_t_2);
+        PyTuple_SET_ITEM(__pyx_t_13, 2+__pyx_t_11, __pyx_t_2);
         __Pyx_GIVEREF(__pyx_t_10);
         PyTuple_SET_ITEM(__pyx_t_13, 3+__pyx_t_11, __pyx_t_10);
         __Pyx_INCREF(__pyx_v_mask_left);
         __Pyx_GIVEREF(__pyx_v_mask_left);
         PyTuple_SET_ITEM(__pyx_t_13, 4+__pyx_t_11, __pyx_v_mask_left);
         __pyx_t_12 = 0;
-        __pyx_t_8 = 0;
+        __pyx_t_2 = 0;
         __pyx_t_10 = 0;
-        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 511, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 511, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       }
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_DECREF_SET(__pyx_v_mask_left, __pyx_t_2);
-      __pyx_t_2 = 0;
+      __Pyx_DECREF_SET(__pyx_v_mask_left, __pyx_t_8);
+      __pyx_t_8 = 0;
 
       /* "structureboost/structure_dt.pyx":505
  *             left_split = curr_partition[0]
  *             right_split = curr_partition[1]
  *             if is_integer_valued:             # <<<<<<<<<<<<<<
- *                 fs_array = np.fromiter(left_split, int,
- *                                        len(left_split)).astype(np.int_)
+ *                 fs_array = np.fromiter(left_split, np.int32,
+ *                                        len(left_split))
  */
       goto __pyx_L7;
     }
 
     /* "structureboost/structure_dt.pyx":515
  *                                                mask_left)
  *             else:
@@ -16129,46 +16095,46 @@
           __Pyx_DECREF_SET(__pyx_t_3, function);
           __pyx_t_11 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_3)) {
         PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_v_feature_vec_node, __pyx_v_left_split};
-        __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 515, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 515, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_GOTREF(__pyx_t_8);
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
         PyObject *__pyx_temp[3] = {__pyx_t_13, __pyx_v_feature_vec_node, __pyx_v_left_split};
-        __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 515, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 515, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_GOTREF(__pyx_t_8);
       } else
       #endif
       {
         __pyx_t_10 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 515, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         if (__pyx_t_13) {
           __Pyx_GIVEREF(__pyx_t_13); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_13); __pyx_t_13 = NULL;
         }
         __Pyx_INCREF(__pyx_v_feature_vec_node);
         __Pyx_GIVEREF(__pyx_v_feature_vec_node);
         PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_11, __pyx_v_feature_vec_node);
         __Pyx_INCREF(__pyx_v_left_split);
         __Pyx_GIVEREF(__pyx_v_left_split);
         PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_11, __pyx_v_left_split);
-        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 515, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
+        __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 515, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_XDECREF_SET(__pyx_v_mask_left, __pyx_t_2);
-      __pyx_t_2 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_mask_left, __pyx_t_8);
+      __pyx_t_8 = 0;
     }
     __pyx_L7:;
 
     /* "structureboost/structure_dt.pyx":517
  *                 mask_left = get_mask(feature_vec_node, left_split)
  * 
  *             curr_loss = self.get_score_of_split(g_h_train_node, mask_left, g_h_sum)             # <<<<<<<<<<<<<<
@@ -16188,25 +16154,25 @@
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_11 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[4] = {__pyx_t_10, __pyx_v_g_h_train_node, __pyx_v_mask_left, __pyx_v_g_h_sum};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 3+__pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 517, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 3+__pyx_t_11); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 517, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_GOTREF(__pyx_t_8);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[4] = {__pyx_t_10, __pyx_v_g_h_train_node, __pyx_v_mask_left, __pyx_v_g_h_sum};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 3+__pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 517, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 3+__pyx_t_11); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 517, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_GOTREF(__pyx_t_8);
     } else
     #endif
     {
       __pyx_t_13 = PyTuple_New(3+__pyx_t_11); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 517, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
       if (__pyx_t_10) {
         __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_10); __pyx_t_10 = NULL;
@@ -16216,33 +16182,33 @@
       PyTuple_SET_ITEM(__pyx_t_13, 0+__pyx_t_11, __pyx_v_g_h_train_node);
       __Pyx_INCREF(__pyx_v_mask_left);
       __Pyx_GIVEREF(__pyx_v_mask_left);
       PyTuple_SET_ITEM(__pyx_t_13, 1+__pyx_t_11, __pyx_v_mask_left);
       __Pyx_INCREF(__pyx_v_g_h_sum);
       __Pyx_GIVEREF(__pyx_v_g_h_sum);
       PyTuple_SET_ITEM(__pyx_t_13, 2+__pyx_t_11, __pyx_v_g_h_sum);
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 517, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 517, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_curr_loss, __pyx_t_2);
-    __pyx_t_2 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_curr_loss, __pyx_t_8);
+    __pyx_t_8 = 0;
 
     /* "structureboost/structure_dt.pyx":519
  *             curr_loss = self.get_score_of_split(g_h_train_node, mask_left, g_h_sum)
  * 
  *             if curr_loss < best_split_of_feat['loss_score']:             # <<<<<<<<<<<<<<
  *                 best_split_of_feat['loss_score'] = curr_loss
  *                 best_split_of_feat['left_split'] = left_split
  */
-    __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_best_split_of_feat, __pyx_n_u_loss_score); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 519, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyObject_RichCompare(__pyx_v_curr_loss, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 519, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_best_split_of_feat, __pyx_n_u_loss_score); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 519, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_3 = PyObject_RichCompare(__pyx_v_curr_loss, __pyx_t_8, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 519, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 519, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (__pyx_t_5) {
 
       /* "structureboost/structure_dt.pyx":520
  * 
  *             if curr_loss < best_split_of_feat['loss_score']:
@@ -16273,31 +16239,31 @@
       /* "structureboost/structure_dt.pyx":524
  *                 best_split_of_feat['feature_type'] = feature_type
  *                 # Next two lines may be unnecessary...
  *                 best_split_of_feat['na_left'] = int(random.random() < .5)             # <<<<<<<<<<<<<<
  *                 best_split_of_feat['na_dir_random'] = 1
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 524, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_random); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 524, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_random); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 524, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_random); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_13);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_2 = NULL;
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __pyx_t_8 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_13))) {
-        __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_13);
-        if (likely(__pyx_t_2)) {
+        __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_13);
+        if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
-          __Pyx_INCREF(__pyx_t_2);
+          __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_13, function);
         }
       }
-      __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_13);
-      __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_13);
+      __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       __pyx_t_13 = PyObject_RichCompare(__pyx_t_3, __pyx_float__5, Py_LT); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = __Pyx_PyNumber_Int(__pyx_t_13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 524, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
@@ -17142,43 +17108,43 @@
   }
 
   /* "structureboost/structure_dt.pyx":560
  *         # Map data points to regions
  * 
  *         num_query_pts = data_array.shape[0]             # <<<<<<<<<<<<<<
  *         num_vor_dims = data_array.shape[1]
- *         feature_vec_node = np.zeros(num_query_pts,dtype=np.int_)
+ *         feature_vec_node = np.zeros(num_query_pts,dtype=np.int32)
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_7 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 560, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_num_query_pts = __pyx_t_7;
   __pyx_t_7 = 0;
 
   /* "structureboost/structure_dt.pyx":561
  * 
  *         num_query_pts = data_array.shape[0]
  *         num_vor_dims = data_array.shape[1]             # <<<<<<<<<<<<<<
- *         feature_vec_node = np.zeros(num_query_pts,dtype=np.int_)
+ *         feature_vec_node = np.zeros(num_query_pts,dtype=np.int32)
  *         feature_vec_node = map_to_nn_point_index(vor_pts,
  */
   __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_array, __pyx_n_s_shape); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_7, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_num_vor_dims = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_dt.pyx":562
  *         num_query_pts = data_array.shape[0]
  *         num_vor_dims = data_array.shape[1]
- *         feature_vec_node = np.zeros(num_query_pts,dtype=np.int_)             # <<<<<<<<<<<<<<
+ *         feature_vec_node = np.zeros(num_query_pts,dtype=np.int32)             # <<<<<<<<<<<<<<
  *         feature_vec_node = map_to_nn_point_index(vor_pts,
  *                                          data_array,
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
@@ -17188,30 +17154,30 @@
   __Pyx_INCREF(__pyx_v_num_query_pts);
   __Pyx_GIVEREF(__pyx_v_num_query_pts);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_num_query_pts);
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_feature_vec_node = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "structureboost/structure_dt.pyx":563
  *         num_vor_dims = data_array.shape[1]
- *         feature_vec_node = np.zeros(num_query_pts,dtype=np.int_)
+ *         feature_vec_node = np.zeros(num_query_pts,dtype=np.int32)
  *         feature_vec_node = map_to_nn_point_index(vor_pts,             # <<<<<<<<<<<<<<
  *                                          data_array,
  *                                          feature_vec_node,
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_map_to_nn_point_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 563, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
@@ -18917,15 +18883,15 @@
   __Pyx_TraceCall("get_gh_val_mat", __pyx_f[0], 638, 0, __PYX_ERR(0, 638, __pyx_L1_error));
 
   /* "structureboost/structure_dt.pyx":640
  *     def get_gh_val_mat(self, feature_vec_node,g_h_train_node,
  *                        max_num_vertices):
  *         g_h_val_arr = np.zeros((max_num_vertices,2))             # <<<<<<<<<<<<<<
  *         g_h_val_arr = get_g_h_feature_sum_arrays(
- *                                             feature_vec_node.astype(np.int_),
+ *                                             feature_vec_node.astype(np.int32),
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 640, __pyx_L1_error)
@@ -18955,32 +18921,32 @@
   __pyx_v_g_h_val_arr = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_dt.pyx":641
  *                        max_num_vertices):
  *         g_h_val_arr = np.zeros((max_num_vertices,2))
  *         g_h_val_arr = get_g_h_feature_sum_arrays(             # <<<<<<<<<<<<<<
- *                                             feature_vec_node.astype(np.int_),
+ *                                             feature_vec_node.astype(np.int32),
  *                                             g_h_train_node,
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_get_g_h_feature_sum_arrays); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 641, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
   /* "structureboost/structure_dt.pyx":642
  *         g_h_val_arr = np.zeros((max_num_vertices,2))
  *         g_h_val_arr = get_g_h_feature_sum_arrays(
- *                                             feature_vec_node.astype(np.int_),             # <<<<<<<<<<<<<<
+ *                                             feature_vec_node.astype(np.int32),             # <<<<<<<<<<<<<<
  *                                             g_h_train_node,
  *                                             g_h_val_arr)
  */
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_feature_vec_node, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 642, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 642, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 642, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 642, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -18993,15 +18959,15 @@
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 642, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "structureboost/structure_dt.pyx":644
- *                                             feature_vec_node.astype(np.int_),
+ *                                             feature_vec_node.astype(np.int32),
  *                                             g_h_train_node,
  *                                             g_h_val_arr)             # <<<<<<<<<<<<<<
  *         return g_h_val_arr
  * 
  */
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
@@ -22028,15 +21994,15 @@
   return __pyx_r;
 }
 
 /* "structureboost/structure_dt.pyx":767
  * 
  * 
  *     def get_prediction(self, tree_node, X_te, dict col_to_int_dict):             # <<<<<<<<<<<<<<
- *         cdef np.ndarray[np.int_t] ind_subset_left, ind_subset_right
+ *         cdef np.ndarray[np.int32_t] ind_subset_left, ind_subset_right
  *         cdef long vec_len, lsize
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_12structure_dt_21StructureDecisionTree_61get_prediction(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_12structure_dt_21StructureDecisionTree_61get_prediction = {"get_prediction", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_12structure_dt_21StructureDecisionTree_61get_prediction, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_12structure_dt_21StructureDecisionTree_61get_prediction(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -22329,25 +22295,25 @@
     __pyx_t_1 = 0;
 
     /* "structureboost/structure_dt.pyx":776
  *         else:
  *             split_bool = get_node_response_df_val(X_te, tree_node, col_to_int_dict)
  *             vec_len = len(split_bool)             # <<<<<<<<<<<<<<
  *             next_vec = np.zeros(vec_len)
- *             ind_subset_left = np.empty(vec_len, dtype=np.int_)
+ *             ind_subset_left = np.empty(vec_len, dtype=np.int32)
  */
     __pyx_t_8 = PyObject_Length(__pyx_v_split_bool); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 776, __pyx_L1_error)
     __pyx_v_vec_len = __pyx_t_8;
 
     /* "structureboost/structure_dt.pyx":777
  *             split_bool = get_node_response_df_val(X_te, tree_node, col_to_int_dict)
  *             vec_len = len(split_bool)
  *             next_vec = np.zeros(vec_len)             # <<<<<<<<<<<<<<
- *             ind_subset_left = np.empty(vec_len, dtype=np.int_)
- *             ind_subset_right = np.empty(vec_len, dtype=np.int_)
+ *             ind_subset_left = np.empty(vec_len, dtype=np.int32)
+ *             ind_subset_right = np.empty(vec_len, dtype=np.int32)
  */
     __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 777, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 777, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v_vec_len); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 777, __pyx_L1_error)
@@ -22390,16 +22356,16 @@
     __pyx_t_9 = 0;
     __pyx_v_next_vec = ((PyArrayObject *)__pyx_t_1);
     __pyx_t_1 = 0;
 
     /* "structureboost/structure_dt.pyx":778
  *             vec_len = len(split_bool)
  *             next_vec = np.zeros(vec_len)
- *             ind_subset_left = np.empty(vec_len, dtype=np.int_)             # <<<<<<<<<<<<<<
- *             ind_subset_right = np.empty(vec_len, dtype=np.int_)
+ *             ind_subset_left = np.empty(vec_len, dtype=np.int32)             # <<<<<<<<<<<<<<
+ *             ind_subset_right = np.empty(vec_len, dtype=np.int32)
  *             ind_subset_left, ind_subset_right, lsize = separate_indices(
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 778, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 778, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -22410,33 +22376,33 @@
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
     __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 778, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 778, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 778, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 778, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 778, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 778, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 778, __pyx_L1_error)
     __pyx_t_13 = ((PyArrayObject *)__pyx_t_4);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer);
-      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_12, &__pyx_t_11, &__pyx_t_10);
-        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_left, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_left, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_10);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_12, __pyx_t_11, __pyx_t_10);
         }
         __pyx_t_12 = __pyx_t_11 = __pyx_t_10 = 0;
       }
@@ -22445,16 +22411,16 @@
     }
     __pyx_t_13 = 0;
     __pyx_v_ind_subset_left = ((PyArrayObject *)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "structureboost/structure_dt.pyx":779
  *             next_vec = np.zeros(vec_len)
- *             ind_subset_left = np.empty(vec_len, dtype=np.int_)
- *             ind_subset_right = np.empty(vec_len, dtype=np.int_)             # <<<<<<<<<<<<<<
+ *             ind_subset_left = np.empty(vec_len, dtype=np.int32)
+ *             ind_subset_right = np.empty(vec_len, dtype=np.int32)             # <<<<<<<<<<<<<<
  *             ind_subset_left, ind_subset_right, lsize = separate_indices(
  *                                                     ind_subset_left,
  */
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
@@ -22466,33 +22432,33 @@
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
     __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 779, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 779, __pyx_L1_error)
     __pyx_t_13 = ((PyArrayObject *)__pyx_t_7);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer);
-      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
-        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_right, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_right, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_10); Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_12);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_10, __pyx_t_11, __pyx_t_12);
         }
         __pyx_t_10 = __pyx_t_11 = __pyx_t_12 = 0;
       }
@@ -22500,35 +22466,35 @@
       if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 779, __pyx_L1_error)
     }
     __pyx_t_13 = 0;
     __pyx_v_ind_subset_right = ((PyArrayObject *)__pyx_t_7);
     __pyx_t_7 = 0;
 
     /* "structureboost/structure_dt.pyx":780
- *             ind_subset_left = np.empty(vec_len, dtype=np.int_)
- *             ind_subset_right = np.empty(vec_len, dtype=np.int_)
+ *             ind_subset_left = np.empty(vec_len, dtype=np.int32)
+ *             ind_subset_right = np.empty(vec_len, dtype=np.int32)
  *             ind_subset_left, ind_subset_right, lsize = separate_indices(             # <<<<<<<<<<<<<<
  *                                                     ind_subset_left,
  *                                                     ind_subset_right,
  */
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_separate_indices); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 780, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
 
     /* "structureboost/structure_dt.pyx":783
  *                                                     ind_subset_left,
  *                                                     ind_subset_right,
- *                                                     split_bool.astype(np.int_),             # <<<<<<<<<<<<<<
+ *                                                     split_bool.astype(np.int32),             # <<<<<<<<<<<<<<
  *                                                     vec_len)
  *             ind_subset_left = ind_subset_left[:lsize]
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_split_bool, __pyx_n_s_astype); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 783, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 783, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 783, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 783, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_14);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -22542,15 +22508,15 @@
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 783, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "structureboost/structure_dt.pyx":784
  *                                                     ind_subset_right,
- *                                                     split_bool.astype(np.int_),
+ *                                                     split_bool.astype(np.int32),
  *                                                     vec_len)             # <<<<<<<<<<<<<<
  *             ind_subset_left = ind_subset_left[:lsize]
  *             ind_subset_right = ind_subset_right[:(vec_len-lsize)]
  */
     __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_vec_len); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 784, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_14 = NULL;
@@ -22659,32 +22625,32 @@
       __pyx_t_15 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
       __PYX_ERR(0, 780, __pyx_L1_error)
       __pyx_L5_unpacking_done:;
     }
 
     /* "structureboost/structure_dt.pyx":780
- *             ind_subset_left = np.empty(vec_len, dtype=np.int_)
- *             ind_subset_right = np.empty(vec_len, dtype=np.int_)
+ *             ind_subset_left = np.empty(vec_len, dtype=np.int32)
+ *             ind_subset_right = np.empty(vec_len, dtype=np.int32)
  *             ind_subset_left, ind_subset_right, lsize = separate_indices(             # <<<<<<<<<<<<<<
  *                                                     ind_subset_left,
  *                                                     ind_subset_right,
  */
     if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 780, __pyx_L1_error)
     if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 780, __pyx_L1_error)
     __pyx_t_16 = __Pyx_PyInt_As_long(__pyx_t_1); if (unlikely((__pyx_t_16 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 780, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_13 = ((PyArrayObject *)__pyx_t_4);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer);
-      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_12, &__pyx_t_11, &__pyx_t_10);
-        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_left, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_left, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_10);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_12, __pyx_t_11, __pyx_t_10);
         }
         __pyx_t_12 = __pyx_t_11 = __pyx_t_10 = 0;
       }
@@ -22694,18 +22660,18 @@
     __pyx_t_13 = 0;
     __Pyx_DECREF_SET(__pyx_v_ind_subset_left, ((PyArrayObject *)__pyx_t_4));
     __pyx_t_4 = 0;
     __pyx_t_13 = ((PyArrayObject *)__pyx_t_5);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer);
-      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
-        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_right, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_right, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_10); Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_12);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_10, __pyx_t_11, __pyx_t_12);
         }
         __pyx_t_10 = __pyx_t_11 = __pyx_t_12 = 0;
       }
@@ -22714,15 +22680,15 @@
     }
     __pyx_t_13 = 0;
     __Pyx_DECREF_SET(__pyx_v_ind_subset_right, ((PyArrayObject *)__pyx_t_5));
     __pyx_t_5 = 0;
     __pyx_v_lsize = __pyx_t_16;
 
     /* "structureboost/structure_dt.pyx":785
- *                                                     split_bool.astype(np.int_),
+ *                                                     split_bool.astype(np.int32),
  *                                                     vec_len)
  *             ind_subset_left = ind_subset_left[:lsize]             # <<<<<<<<<<<<<<
  *             ind_subset_right = ind_subset_right[:(vec_len-lsize)]
  * 
  */
     __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_v_lsize); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 785, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
@@ -22733,18 +22699,18 @@
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 785, __pyx_L1_error)
     __pyx_t_13 = ((PyArrayObject *)__pyx_t_7);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer);
-      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_12, &__pyx_t_11, &__pyx_t_10);
-        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_left, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_left, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_10);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_12, __pyx_t_11, __pyx_t_10);
         }
         __pyx_t_12 = __pyx_t_11 = __pyx_t_10 = 0;
       }
@@ -22771,18 +22737,18 @@
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 786, __pyx_L1_error)
     __pyx_t_13 = ((PyArrayObject *)__pyx_t_7);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer);
-      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
-        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_right, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_right, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_10); Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_12);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_10, __pyx_t_11, __pyx_t_12);
         }
         __pyx_t_10 = __pyx_t_11 = __pyx_t_12 = 0;
       }
@@ -23054,15 +23020,15 @@
     goto __pyx_L0;
   }
 
   /* "structureboost/structure_dt.pyx":767
  * 
  * 
  *     def get_prediction(self, tree_node, X_te, dict col_to_int_dict):             # <<<<<<<<<<<<<<
- *         cdef np.ndarray[np.int_t] ind_subset_left, ind_subset_right
+ *         cdef np.ndarray[np.int32_t] ind_subset_left, ind_subset_right
  *         cdef long vec_len, lsize
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
@@ -25424,15 +25390,15 @@
   return __pyx_r;
 }
 
 /* "structureboost/structure_dt.pyx":898
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def get_bin_sums_c(np.ndarray[double, ndim=2] g_h_mat,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] bin_result_vec, long out_vec_size):
+ *                    np.ndarray[np.int32_t] bin_result_vec, long out_vec_size):
  *     cdef int i
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_12structure_dt_15get_bin_sums_c(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_12structure_dt_15get_bin_sums_c = {"get_bin_sums_c", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_12structure_dt_15get_bin_sums_c, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_12structure_dt_15get_bin_sums_c(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -25568,20 +25534,20 @@
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_g_h_mat.rcbuffer->pybuffer, (PyObject*)__pyx_v_g_h_mat, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 898, __pyx_L1_error)
   }
   __pyx_pybuffernd_g_h_mat.diminfo[0].strides = __pyx_pybuffernd_g_h_mat.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_g_h_mat.diminfo[0].shape = __pyx_pybuffernd_g_h_mat.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_g_h_mat.diminfo[1].strides = __pyx_pybuffernd_g_h_mat.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_g_h_mat.diminfo[1].shape = __pyx_pybuffernd_g_h_mat.rcbuffer->pybuffer.shape[1];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_bin_result_vec, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 898, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_bin_result_vec, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 898, __pyx_L1_error)
   }
   __pyx_pybuffernd_bin_result_vec.diminfo[0].strides = __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_bin_result_vec.diminfo[0].shape = __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.shape[0];
 
   /* "structureboost/structure_dt.pyx":901
- *                    np.ndarray[np.int_t] bin_result_vec, long out_vec_size):
+ *                    np.ndarray[np.int32_t] bin_result_vec, long out_vec_size):
  *     cdef int i
  *     cdef int m = bin_result_vec.shape[0]             # <<<<<<<<<<<<<<
  * 
  *     cdef np.ndarray[double] g_sum_bins = np.zeros(out_vec_size)
  */
   __pyx_v_m = (__pyx_v_bin_result_vec->dimensions[0]);
 
@@ -25691,28 +25657,28 @@
  *         g_sum_bins[bin_result_vec[i]] += g_h_mat[i,0]             # <<<<<<<<<<<<<<
  *         h_sum_bins[bin_result_vec[i]] += g_h_mat[i,1]
  *     return g_sum_bins, h_sum_bins
  */
     __pyx_t_10 = __pyx_v_i;
     __pyx_t_11 = 0;
     __pyx_t_12 = __pyx_v_i;
-    __pyx_t_13 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_bin_result_vec.diminfo[0].strides));
+    __pyx_t_13 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_bin_result_vec.diminfo[0].strides));
     *__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_g_sum_bins.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_g_sum_bins.diminfo[0].strides) += (*__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_g_h_mat.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_g_h_mat.diminfo[0].strides, __pyx_t_11, __pyx_pybuffernd_g_h_mat.diminfo[1].strides));
 
     /* "structureboost/structure_dt.pyx":908
  *     for i in range(m):
  *         g_sum_bins[bin_result_vec[i]] += g_h_mat[i,0]
  *         h_sum_bins[bin_result_vec[i]] += g_h_mat[i,1]             # <<<<<<<<<<<<<<
  *     return g_sum_bins, h_sum_bins
  * 
  */
     __pyx_t_11 = __pyx_v_i;
     __pyx_t_10 = 1;
     __pyx_t_12 = __pyx_v_i;
-    __pyx_t_13 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_bin_result_vec.diminfo[0].strides));
+    __pyx_t_13 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_bin_result_vec.diminfo[0].strides));
     *__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_h_sum_bins.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_h_sum_bins.diminfo[0].strides) += (*__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_g_h_mat.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_g_h_mat.diminfo[0].strides, __pyx_t_10, __pyx_pybuffernd_g_h_mat.diminfo[1].strides));
   }
 
   /* "structureboost/structure_dt.pyx":909
  *         g_sum_bins[bin_result_vec[i]] += g_h_mat[i,0]
  *         h_sum_bins[bin_result_vec[i]] += g_h_mat[i,1]
  *     return g_sum_bins, h_sum_bins             # <<<<<<<<<<<<<<
@@ -25732,15 +25698,15 @@
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "structureboost/structure_dt.pyx":898
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def get_bin_sums_c(np.ndarray[double, ndim=2] g_h_mat,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] bin_result_vec, long out_vec_size):
+ *                    np.ndarray[np.int32_t] bin_result_vec, long out_vec_size):
  *     cdef int i
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -27461,15 +27427,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "structureboost/structure_dt.pyx":975
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_g_h_feature_sum_arrays(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ * def get_g_h_feature_sum_arrays(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
  *                                np.ndarray[double, ndim=2] g_h_train_node,
  *                                np.ndarray[double, ndim=2] g_h_val_arr):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_12structure_dt_31get_g_h_feature_sum_arrays(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_12structure_dt_31get_g_h_feature_sum_arrays = {"get_g_h_feature_sum_arrays", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_12structure_dt_31get_g_h_feature_sum_arrays, METH_VARARGS|METH_KEYWORDS, 0};
@@ -27592,15 +27558,15 @@
   __pyx_pybuffernd_g_h_train_node.rcbuffer = &__pyx_pybuffer_g_h_train_node;
   __pyx_pybuffer_g_h_val_arr.pybuffer.buf = NULL;
   __pyx_pybuffer_g_h_val_arr.refcount = 0;
   __pyx_pybuffernd_g_h_val_arr.data = NULL;
   __pyx_pybuffernd_g_h_val_arr.rcbuffer = &__pyx_pybuffer_g_h_val_arr;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer, (PyObject*)__pyx_v_feature_vec_node, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 975, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer, (PyObject*)__pyx_v_feature_vec_node, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 975, __pyx_L1_error)
   }
   __pyx_pybuffernd_feature_vec_node.diminfo[0].strides = __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_feature_vec_node.diminfo[0].shape = __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_g_h_train_node.rcbuffer->pybuffer, (PyObject*)__pyx_v_g_h_train_node, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 975, __pyx_L1_error)
   }
   __pyx_pybuffernd_g_h_train_node.diminfo[0].strides = __pyx_pybuffernd_g_h_train_node.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_g_h_train_node.diminfo[0].shape = __pyx_pybuffernd_g_h_train_node.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_g_h_train_node.diminfo[1].strides = __pyx_pybuffernd_g_h_train_node.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_g_h_train_node.diminfo[1].shape = __pyx_pybuffernd_g_h_train_node.rcbuffer->pybuffer.shape[1];
@@ -27636,15 +27602,15 @@
  *     cdef long array_size = len(feature_vec_node)
  *     for i in range(array_size):
  *         ind = feature_vec_node[i]             # <<<<<<<<<<<<<<
  *         g_h_val_arr[ind,0] = g_h_val_arr[ind,0]+g_h_train_node[i,0]
  *         g_h_val_arr[ind,1] = g_h_val_arr[ind,1]+g_h_train_node[i,1]
  */
     __pyx_t_5 = __pyx_v_i;
-    __pyx_v_ind = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_feature_vec_node.diminfo[0].strides));
+    __pyx_v_ind = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.buf, __pyx_t_5, __pyx_pybuffernd_feature_vec_node.diminfo[0].strides));
 
     /* "structureboost/structure_dt.pyx":982
  *     for i in range(array_size):
  *         ind = feature_vec_node[i]
  *         g_h_val_arr[ind,0] = g_h_val_arr[ind,0]+g_h_train_node[i,0]             # <<<<<<<<<<<<<<
  *         g_h_val_arr[ind,1] = g_h_val_arr[ind,1]+g_h_train_node[i,1]
  *     return g_h_val_arr
@@ -27684,15 +27650,15 @@
   __Pyx_INCREF(((PyObject *)__pyx_v_g_h_val_arr));
   __pyx_r = ((PyObject *)__pyx_v_g_h_val_arr);
   goto __pyx_L0;
 
   /* "structureboost/structure_dt.pyx":975
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_g_h_feature_sum_arrays(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ * def get_g_h_feature_sum_arrays(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
  *                                np.ndarray[double, ndim=2] g_h_train_node,
  *                                np.ndarray[double, ndim=2] g_h_val_arr):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
@@ -29004,16 +28970,16 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "structureboost/structure_dt.pyx":1045
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_mask_int_c(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] left_split,
+ * def get_mask_int_c(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ *                    np.ndarray[np.int32_t] left_split,
  *                    long vec_len, long lsplit_len,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_12structure_dt_39get_mask_int_c(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_12structure_dt_39get_mask_int_c = {"get_mask_int_c", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_12structure_dt_39get_mask_int_c, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_12structure_dt_39get_mask_int_c(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -29158,30 +29124,30 @@
   __pyx_pybuffernd_left_split.rcbuffer = &__pyx_pybuffer_left_split;
   __pyx_pybuffer_mask_vec.pybuffer.buf = NULL;
   __pyx_pybuffer_mask_vec.refcount = 0;
   __pyx_pybuffernd_mask_vec.data = NULL;
   __pyx_pybuffernd_mask_vec.rcbuffer = &__pyx_pybuffer_mask_vec;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer, (PyObject*)__pyx_v_feature_vec_node, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1045, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer, (PyObject*)__pyx_v_feature_vec_node, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1045, __pyx_L1_error)
   }
   __pyx_pybuffernd_feature_vec_node.diminfo[0].strides = __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_feature_vec_node.diminfo[0].shape = __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_left_split.rcbuffer->pybuffer, (PyObject*)__pyx_v_left_split, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1045, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_left_split.rcbuffer->pybuffer, (PyObject*)__pyx_v_left_split, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1045, __pyx_L1_error)
   }
   __pyx_pybuffernd_left_split.diminfo[0].strides = __pyx_pybuffernd_left_split.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_left_split.diminfo[0].shape = __pyx_pybuffernd_left_split.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mask_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_mask_vec, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1045, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mask_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_mask_vec, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1045, __pyx_L1_error)
   }
   __pyx_pybuffernd_mask_vec.diminfo[0].strides = __pyx_pybuffernd_mask_vec.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mask_vec.diminfo[0].shape = __pyx_pybuffernd_mask_vec.rcbuffer->pybuffer.shape[0];
 
   /* "structureboost/structure_dt.pyx":1050
- *                    np.ndarray[np.int_t] mask_vec):
+ *                    np.ndarray[np.int32_t] mask_vec):
  *     cdef int i, j
  *     for i in range(vec_len):             # <<<<<<<<<<<<<<
  *         for j in range(lsplit_len):
  *             if feature_vec_node[i] == left_split[j]:
  */
   __pyx_t_1 = __pyx_v_vec_len;
   __pyx_t_2 = __pyx_t_1;
@@ -29205,26 +29171,26 @@
  *         for j in range(lsplit_len):
  *             if feature_vec_node[i] == left_split[j]:             # <<<<<<<<<<<<<<
  *                 mask_vec[i] = 1
  *                 break
  */
       __pyx_t_7 = __pyx_v_i;
       __pyx_t_8 = __pyx_v_j;
-      __pyx_t_9 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.buf, __pyx_t_7, __pyx_pybuffernd_feature_vec_node.diminfo[0].strides)) == (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_left_split.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_left_split.diminfo[0].strides))) != 0);
+      __pyx_t_9 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.buf, __pyx_t_7, __pyx_pybuffernd_feature_vec_node.diminfo[0].strides)) == (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_left_split.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_left_split.diminfo[0].strides))) != 0);
       if (__pyx_t_9) {
 
         /* "structureboost/structure_dt.pyx":1053
  *         for j in range(lsplit_len):
  *             if feature_vec_node[i] == left_split[j]:
  *                 mask_vec[i] = 1             # <<<<<<<<<<<<<<
  *                 break
  *     return mask_vec.astype(bool)
  */
         __pyx_t_8 = __pyx_v_i;
-        *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_mask_vec.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_mask_vec.diminfo[0].strides) = 1;
+        *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_mask_vec.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_mask_vec.diminfo[0].strides) = 1;
 
         /* "structureboost/structure_dt.pyx":1054
  *             if feature_vec_node[i] == left_split[j]:
  *                 mask_vec[i] = 1
  *                 break             # <<<<<<<<<<<<<<
  *     return mask_vec.astype(bool)
  * 
@@ -29271,16 +29237,16 @@
   __pyx_r = __pyx_t_10;
   __pyx_t_10 = 0;
   goto __pyx_L0;
 
   /* "structureboost/structure_dt.pyx":1045
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_mask_int_c(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] left_split,
+ * def get_mask_int_c(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ *                    np.ndarray[np.int32_t] left_split,
  *                    long vec_len, long lsplit_len,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
@@ -29306,16 +29272,16 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "structureboost/structure_dt.pyx":1060
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
- * def separate_indices(np.ndarray[np.int_t] a, np.ndarray[np.int_t] b,             # <<<<<<<<<<<<<<
- *                      np.ndarray[np.int_t] c, long vec_len):
+ * def separate_indices(np.ndarray[np.int32_t] a, np.ndarray[np.int32_t] b,             # <<<<<<<<<<<<<<
+ *                      np.ndarray[np.int32_t] c, long vec_len):
  *     cdef long ind_a = 0, ind_b = 0, i
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_12structure_dt_41separate_indices(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_12structure_dt_41separate_indices = {"separate_indices", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_12structure_dt_41separate_indices, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_12structure_dt_41separate_indices(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -29445,40 +29411,40 @@
   __pyx_pybuffernd_b.rcbuffer = &__pyx_pybuffer_b;
   __pyx_pybuffer_c.pybuffer.buf = NULL;
   __pyx_pybuffer_c.refcount = 0;
   __pyx_pybuffernd_c.data = NULL;
   __pyx_pybuffernd_c.rcbuffer = &__pyx_pybuffer_c;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_a.rcbuffer->pybuffer, (PyObject*)__pyx_v_a, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1060, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_a.rcbuffer->pybuffer, (PyObject*)__pyx_v_a, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1060, __pyx_L1_error)
   }
   __pyx_pybuffernd_a.diminfo[0].strides = __pyx_pybuffernd_a.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_a.diminfo[0].shape = __pyx_pybuffernd_a.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_b.rcbuffer->pybuffer, (PyObject*)__pyx_v_b, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1060, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_b.rcbuffer->pybuffer, (PyObject*)__pyx_v_b, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1060, __pyx_L1_error)
   }
   __pyx_pybuffernd_b.diminfo[0].strides = __pyx_pybuffernd_b.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_b.diminfo[0].shape = __pyx_pybuffernd_b.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_c.rcbuffer->pybuffer, (PyObject*)__pyx_v_c, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1060, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_c.rcbuffer->pybuffer, (PyObject*)__pyx_v_c, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1060, __pyx_L1_error)
   }
   __pyx_pybuffernd_c.diminfo[0].strides = __pyx_pybuffernd_c.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_c.diminfo[0].shape = __pyx_pybuffernd_c.rcbuffer->pybuffer.shape[0];
 
   /* "structureboost/structure_dt.pyx":1062
- * def separate_indices(np.ndarray[np.int_t] a, np.ndarray[np.int_t] b,
- *                      np.ndarray[np.int_t] c, long vec_len):
+ * def separate_indices(np.ndarray[np.int32_t] a, np.ndarray[np.int32_t] b,
+ *                      np.ndarray[np.int32_t] c, long vec_len):
  *     cdef long ind_a = 0, ind_b = 0, i             # <<<<<<<<<<<<<<
  *     for i in range(vec_len):
  *         if c[i] == 0:
  */
   __pyx_v_ind_a = 0;
   __pyx_v_ind_b = 0;
 
   /* "structureboost/structure_dt.pyx":1063
- *                      np.ndarray[np.int_t] c, long vec_len):
+ *                      np.ndarray[np.int32_t] c, long vec_len):
  *     cdef long ind_a = 0, ind_b = 0, i
  *     for i in range(vec_len):             # <<<<<<<<<<<<<<
  *         if c[i] == 0:
  *             b[ind_b] = i
  */
   __pyx_t_1 = __pyx_v_vec_len;
   __pyx_t_2 = __pyx_t_1;
@@ -29489,26 +29455,26 @@
  *     cdef long ind_a = 0, ind_b = 0, i
  *     for i in range(vec_len):
  *         if c[i] == 0:             # <<<<<<<<<<<<<<
  *             b[ind_b] = i
  *             ind_b = ind_b+1
  */
     __pyx_t_4 = __pyx_v_i;
-    __pyx_t_5 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_c.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_c.diminfo[0].strides)) == 0) != 0);
+    __pyx_t_5 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_c.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_c.diminfo[0].strides)) == 0) != 0);
     if (__pyx_t_5) {
 
       /* "structureboost/structure_dt.pyx":1065
  *     for i in range(vec_len):
  *         if c[i] == 0:
  *             b[ind_b] = i             # <<<<<<<<<<<<<<
  *             ind_b = ind_b+1
  *         else:
  */
       __pyx_t_4 = __pyx_v_ind_b;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_b.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_b.diminfo[0].strides) = __pyx_v_i;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_b.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_b.diminfo[0].strides) = __pyx_v_i;
 
       /* "structureboost/structure_dt.pyx":1066
  *         if c[i] == 0:
  *             b[ind_b] = i
  *             ind_b = ind_b+1             # <<<<<<<<<<<<<<
  *         else:
  *             a[ind_a] = i
@@ -29530,15 +29496,15 @@
  *         else:
  *             a[ind_a] = i             # <<<<<<<<<<<<<<
  *             ind_a = ind_a+1
  *     return a, b, ind_a
  */
     /*else*/ {
       __pyx_t_4 = __pyx_v_ind_a;
-      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_a.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_a.diminfo[0].strides) = __pyx_v_i;
+      *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_a.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_a.diminfo[0].strides) = __pyx_v_i;
 
       /* "structureboost/structure_dt.pyx":1069
  *         else:
  *             a[ind_a] = i
  *             ind_a = ind_a+1             # <<<<<<<<<<<<<<
  *     return a, b, ind_a
  * 
@@ -29572,16 +29538,16 @@
   __pyx_r = __pyx_t_7;
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
   /* "structureboost/structure_dt.pyx":1060
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
- * def separate_indices(np.ndarray[np.int_t] a, np.ndarray[np.int_t] b,             # <<<<<<<<<<<<<<
- *                      np.ndarray[np.int_t] c, long vec_len):
+ * def separate_indices(np.ndarray[np.int32_t] a, np.ndarray[np.int32_t] b,             # <<<<<<<<<<<<<<
+ *                      np.ndarray[np.int32_t] c, long vec_len):
  *     cdef long ind_a = 0, ind_b = 0, i
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
@@ -29607,15 +29573,15 @@
   return __pyx_r;
 }
 
 /* "structureboost/structure_dt.pyx":1073
  * 
  * 
  * def get_node_response_graphical_int(feature_vec, node):             # <<<<<<<<<<<<<<
- *     # fs_array = np.array(list(node['left_split'])).astype(np.int_)
+ *     # fs_array = np.array(list(node['left_split'])).astype(np.int32)
  *     cdef int vec_len, lsplit_len
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_12structure_dt_43get_node_response_graphical_int(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_12structure_dt_43get_node_response_graphical_int = {"get_node_response_graphical_int", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_12structure_dt_43get_node_response_graphical_int, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_12structure_dt_43get_node_response_graphical_int(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -29703,281 +29669,264 @@
   __Pyx_TraceFrameInit(__pyx_codeobj__63)
   __Pyx_RefNannySetupContext("get_node_response_graphical_int", 0);
   __Pyx_TraceCall("get_node_response_graphical_int", __pyx_f[0], 1073, 0, __PYX_ERR(0, 1073, __pyx_L1_error));
 
   /* "structureboost/structure_dt.pyx":1077
  *     cdef int vec_len, lsplit_len
  * 
- *     fs_array = np.fromiter(node['left_split'], int,             # <<<<<<<<<<<<<<
- *                            len(node['left_split'])).astype(np.int_)
+ *     fs_array = np.fromiter(node['left_split'], np.int32,             # <<<<<<<<<<<<<<
+ *                            len(node['left_split']))
  *     vec_len = len(feature_vec)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1077, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1077, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_fromiter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1077, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_fromiter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1077, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_split); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1077, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1077, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_split); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1077, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1077, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "structureboost/structure_dt.pyx":1078
  * 
- *     fs_array = np.fromiter(node['left_split'], int,
- *                            len(node['left_split'])).astype(np.int_)             # <<<<<<<<<<<<<<
+ *     fs_array = np.fromiter(node['left_split'], np.int32,
+ *                            len(node['left_split']))             # <<<<<<<<<<<<<<
  *     vec_len = len(feature_vec)
  *     lsplit_len = len(fs_array)
  */
-  __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_split); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1078, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyObject_Length(__pyx_t_5); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1078, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1078, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_split); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1078, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_6 = PyObject_Length(__pyx_t_4); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1078, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1078, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_7)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_4)) {
-    PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_3, ((PyObject *)(&PyInt_Type)), __pyx_t_5};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1077, __pyx_L1_error)
+  if (PyFunction_Check(__pyx_t_3)) {
+    PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_2, __pyx_t_5, __pyx_t_4};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1077, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-    PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_3, ((PyObject *)(&PyInt_Type)), __pyx_t_5};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1077, __pyx_L1_error)
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
+    PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_t_2, __pyx_t_5, __pyx_t_4};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1077, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
     __pyx_t_9 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1077, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_3);
-    __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
-    __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
-    PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, ((PyObject *)(&PyInt_Type)));
+    __Pyx_GIVEREF(__pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_t_5);
-    __pyx_t_3 = 0;
+    PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_t_4);
+    __pyx_t_2 = 0;
     __pyx_t_5 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_9, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1077, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = 0;
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1077, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1078, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1078, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1078, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_2);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_t_9) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_9);
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1078, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_fs_array = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_dt.pyx":1079
- *     fs_array = np.fromiter(node['left_split'], int,
- *                            len(node['left_split'])).astype(np.int_)
+ *     fs_array = np.fromiter(node['left_split'], np.int32,
+ *                            len(node['left_split']))
  *     vec_len = len(feature_vec)             # <<<<<<<<<<<<<<
  *     lsplit_len = len(fs_array)
- *     mask_vec = np.zeros(vec_len, dtype=np.int_)
+ *     mask_vec = np.zeros(vec_len, dtype=np.int32)
  */
   __pyx_t_6 = PyObject_Length(__pyx_v_feature_vec); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1079, __pyx_L1_error)
   __pyx_v_vec_len = __pyx_t_6;
 
   /* "structureboost/structure_dt.pyx":1080
- *                            len(node['left_split'])).astype(np.int_)
+ *                            len(node['left_split']))
  *     vec_len = len(feature_vec)
  *     lsplit_len = len(fs_array)             # <<<<<<<<<<<<<<
- *     mask_vec = np.zeros(vec_len, dtype=np.int_)
- *     mask_vec = get_mask_int_c(feature_vec.astype(np.int_),
+ *     mask_vec = np.zeros(vec_len, dtype=np.int32)
+ *     mask_vec = get_mask_int_c(feature_vec.astype(np.int32),
  */
   __pyx_t_6 = PyObject_Length(__pyx_v_fs_array); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1080, __pyx_L1_error)
   __pyx_v_lsplit_len = __pyx_t_6;
 
   /* "structureboost/structure_dt.pyx":1081
  *     vec_len = len(feature_vec)
  *     lsplit_len = len(fs_array)
- *     mask_vec = np.zeros(vec_len, dtype=np.int_)             # <<<<<<<<<<<<<<
- *     mask_vec = get_mask_int_c(feature_vec.astype(np.int_),
+ *     mask_vec = np.zeros(vec_len, dtype=np.int32)             # <<<<<<<<<<<<<<
+ *     mask_vec = get_mask_int_c(feature_vec.astype(np.int32),
  *                               fs_array, vec_len,
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1081, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1081, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1081, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_vec_len); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1081, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_9 = PyTuple_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1081, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1081, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1081, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1081, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1081, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1081, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1081, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_9, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1081, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_9, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1081, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_mask_vec = __pyx_t_5;
   __pyx_t_5 = 0;
 
   /* "structureboost/structure_dt.pyx":1082
  *     lsplit_len = len(fs_array)
- *     mask_vec = np.zeros(vec_len, dtype=np.int_)
- *     mask_vec = get_mask_int_c(feature_vec.astype(np.int_),             # <<<<<<<<<<<<<<
+ *     mask_vec = np.zeros(vec_len, dtype=np.int32)
+ *     mask_vec = get_mask_int_c(feature_vec.astype(np.int32),             # <<<<<<<<<<<<<<
  *                               fs_array, vec_len,
  *                               lsplit_len, mask_vec)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_mask_int_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1082, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_feature_vec, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1082, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_feature_vec, __pyx_n_s_astype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1082, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1082, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1082, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1082, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1082, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_9 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_9 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 1082, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "structureboost/structure_dt.pyx":1083
- *     mask_vec = np.zeros(vec_len, dtype=np.int_)
- *     mask_vec = get_mask_int_c(feature_vec.astype(np.int_),
+ *     mask_vec = np.zeros(vec_len, dtype=np.int32)
+ *     mask_vec = get_mask_int_c(feature_vec.astype(np.int32),
  *                               fs_array, vec_len,             # <<<<<<<<<<<<<<
  *                               lsplit_len, mask_vec)
  *     return mask_vec
  */
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_vec_len); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1083, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_vec_len); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1083, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
 
   /* "structureboost/structure_dt.pyx":1084
- *     mask_vec = get_mask_int_c(feature_vec.astype(np.int_),
+ *     mask_vec = get_mask_int_c(feature_vec.astype(np.int32),
  *                               fs_array, vec_len,
  *                               lsplit_len, mask_vec)             # <<<<<<<<<<<<<<
  *     return mask_vec
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_lsplit_len); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1084, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = NULL;
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_lsplit_len); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1084, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-    if (likely(__pyx_t_2)) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_1)) {
-    PyObject *__pyx_temp[6] = {__pyx_t_2, __pyx_t_9, __pyx_v_fs_array, __pyx_t_4, __pyx_t_3, __pyx_v_mask_vec};
+    PyObject *__pyx_temp[6] = {__pyx_t_4, __pyx_t_9, __pyx_v_fs_array, __pyx_t_3, __pyx_t_2, __pyx_v_mask_vec};
     __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 5+__pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1082, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-    PyObject *__pyx_temp[6] = {__pyx_t_2, __pyx_t_9, __pyx_v_fs_array, __pyx_t_4, __pyx_t_3, __pyx_v_mask_vec};
+    PyObject *__pyx_temp[6] = {__pyx_t_4, __pyx_t_9, __pyx_v_fs_array, __pyx_t_3, __pyx_t_2, __pyx_v_mask_vec};
     __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 5+__pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1082, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   {
     __pyx_t_7 = PyTuple_New(5+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1082, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    if (__pyx_t_2) {
-      __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_2); __pyx_t_2 = NULL;
+    if (__pyx_t_4) {
+      __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_8, __pyx_t_9);
     __Pyx_INCREF(__pyx_v_fs_array);
     __Pyx_GIVEREF(__pyx_v_fs_array);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_8, __pyx_v_fs_array);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_8, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_7, 3+__pyx_t_8, __pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_8, __pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_7, 3+__pyx_t_8, __pyx_t_2);
     __Pyx_INCREF(__pyx_v_mask_vec);
     __Pyx_GIVEREF(__pyx_v_mask_vec);
     PyTuple_SET_ITEM(__pyx_t_7, 4+__pyx_t_8, __pyx_v_mask_vec);
     __pyx_t_9 = 0;
-    __pyx_t_4 = 0;
     __pyx_t_3 = 0;
+    __pyx_t_2 = 0;
     __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1082, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF_SET(__pyx_v_mask_vec, __pyx_t_5);
   __pyx_t_5 = 0;
@@ -29994,15 +29943,15 @@
   __pyx_r = __pyx_v_mask_vec;
   goto __pyx_L0;
 
   /* "structureboost/structure_dt.pyx":1073
  * 
  * 
  * def get_node_response_graphical_int(feature_vec, node):             # <<<<<<<<<<<<<<
- *     # fs_array = np.array(list(node['left_split'])).astype(np.int_)
+ *     # fs_array = np.array(list(node['left_split'])).astype(np.int32)
  *     cdef int vec_len, lsplit_len
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -30117,43 +30066,43 @@
   __Pyx_TraceCall("get_node_response_graphical_vor", __pyx_f[0], 1088, 0, __PYX_ERR(0, 1088, __pyx_L1_error));
 
   /* "structureboost/structure_dt.pyx":1089
  * 
  * def get_node_response_graphical_vor(feature_mat, node):
  *     num_query_pts = feature_mat.shape[0]             # <<<<<<<<<<<<<<
  *     num_vor_dims = feature_mat.shape[1]
- *     feature_vec = np.zeros(num_query_pts,dtype=np.int_)
+ *     feature_vec = np.zeros(num_query_pts,dtype=np.int32)
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_feature_mat, __pyx_n_s_shape); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1089, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1089, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_num_query_pts = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "structureboost/structure_dt.pyx":1090
  * def get_node_response_graphical_vor(feature_mat, node):
  *     num_query_pts = feature_mat.shape[0]
  *     num_vor_dims = feature_mat.shape[1]             # <<<<<<<<<<<<<<
- *     feature_vec = np.zeros(num_query_pts,dtype=np.int_)
+ *     feature_vec = np.zeros(num_query_pts,dtype=np.int32)
  *     feature_vec = map_to_nn_point_index(node['vor_pts'],
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_feature_mat, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1090, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1090, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_num_vor_dims = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_dt.pyx":1091
  *     num_query_pts = feature_mat.shape[0]
  *     num_vor_dims = feature_mat.shape[1]
- *     feature_vec = np.zeros(num_query_pts,dtype=np.int_)             # <<<<<<<<<<<<<<
+ *     feature_vec = np.zeros(num_query_pts,dtype=np.int32)             # <<<<<<<<<<<<<<
  *     feature_vec = map_to_nn_point_index(node['vor_pts'],
  *                                         feature_mat,
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1091, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1091, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -30163,30 +30112,30 @@
   __Pyx_INCREF(__pyx_v_num_query_pts);
   __Pyx_GIVEREF(__pyx_v_num_query_pts);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_num_query_pts);
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1091, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1091, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1091, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1091, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1091, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1091, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_feature_vec = __pyx_t_5;
   __pyx_t_5 = 0;
 
   /* "structureboost/structure_dt.pyx":1092
  *     num_vor_dims = feature_mat.shape[1]
- *     feature_vec = np.zeros(num_query_pts,dtype=np.int_)
+ *     feature_vec = np.zeros(num_query_pts,dtype=np.int32)
  *     feature_vec = map_to_nn_point_index(node['vor_pts'],             # <<<<<<<<<<<<<<
  *                                         feature_mat,
  *                                         feature_vec,
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_map_to_nn_point_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1092, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_vor_pts); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1092, __pyx_L1_error)
@@ -32638,15 +32587,15 @@
   return __pyx_r;
 }
 
 /* "structureboost/structure_dt.pyx":1165
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def map_to_nn_point_index(double[:,:] core_pts, double[:,:] query_pts,             # <<<<<<<<<<<<<<
- *                           np.ndarray[np.int_t] out_mat, long num_core_pts,
+ *                           np.ndarray[np.int32_t] out_mat, long num_core_pts,
  *                           long num_query_pts, long ndim):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_12structure_dt_61map_to_nn_point_index(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_12structure_dt_61map_to_nn_point_index = {"map_to_nn_point_index", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_12structure_dt_61map_to_nn_point_index, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_12structure_dt_61map_to_nn_point_index(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -32795,15 +32744,15 @@
   __Pyx_TraceCall("map_to_nn_point_index", __pyx_f[0], 1165, 0, __PYX_ERR(0, 1165, __pyx_L1_error));
   __pyx_pybuffer_out_mat.pybuffer.buf = NULL;
   __pyx_pybuffer_out_mat.refcount = 0;
   __pyx_pybuffernd_out_mat.data = NULL;
   __pyx_pybuffernd_out_mat.rcbuffer = &__pyx_pybuffer_out_mat;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_out_mat.rcbuffer->pybuffer, (PyObject*)__pyx_v_out_mat, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1165, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_out_mat.rcbuffer->pybuffer, (PyObject*)__pyx_v_out_mat, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1165, __pyx_L1_error)
   }
   __pyx_pybuffernd_out_mat.diminfo[0].strides = __pyx_pybuffernd_out_mat.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_out_mat.diminfo[0].shape = __pyx_pybuffernd_out_mat.rcbuffer->pybuffer.shape[0];
 
   /* "structureboost/structure_dt.pyx":1170
  *     cdef double curr_dist, tnum, best_dist
  *     cdef int i,j, best_j
  *     for i in range(num_query_pts):             # <<<<<<<<<<<<<<
@@ -32931,15 +32880,15 @@
  *                 best_dist = curr_dist
  *                 best_j = j
  *         out_mat[i] = best_j             # <<<<<<<<<<<<<<
  *     return(out_mat)
  * 
  */
     __pyx_t_13 = __pyx_v_i;
-    *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_out_mat.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_out_mat.diminfo[0].strides) = __pyx_v_best_j;
+    *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_out_mat.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_out_mat.diminfo[0].strides) = __pyx_v_best_j;
   }
 
   /* "structureboost/structure_dt.pyx":1184
  *                 best_j = j
  *         out_mat[i] = best_j
  *     return(out_mat)             # <<<<<<<<<<<<<<
  * 
@@ -32950,15 +32899,15 @@
   __pyx_r = ((PyObject *)__pyx_v_out_mat);
   goto __pyx_L0;
 
   /* "structureboost/structure_dt.pyx":1165
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def map_to_nn_point_index(double[:,:] core_pts, double[:,:] query_pts,             # <<<<<<<<<<<<<<
- *                           np.ndarray[np.int_t] out_mat, long num_core_pts,
+ *                           np.ndarray[np.int32_t] out_mat, long num_core_pts,
  *                           long num_query_pts, long ndim):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
@@ -48918,15 +48867,15 @@
   {&__pyx_n_s_ind_subset_right, __pyx_k_ind_subset_right, sizeof(__pyx_k_ind_subset_right), 0, 0, 1, 1},
   {&__pyx_n_s_index_range, __pyx_k_index_range, sizeof(__pyx_k_index_range), 0, 0, 1, 1},
   {&__pyx_n_s_inds, __pyx_k_inds, sizeof(__pyx_k_inds), 0, 0, 1, 1},
   {&__pyx_n_s_inf, __pyx_k_inf, sizeof(__pyx_k_inf), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
   {&__pyx_n_s_init_for_span_trees, __pyx_k_init_for_span_trees, sizeof(__pyx_k_init_for_span_trees), 0, 0, 1, 1},
   {&__pyx_n_s_initialize_best_split_dict, __pyx_k_initialize_best_split_dict, sizeof(__pyx_k_initialize_best_split_dict), 0, 0, 1, 1},
-  {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
+  {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
   {&__pyx_n_u_interior, __pyx_k_interior, sizeof(__pyx_k_interior), 0, 1, 0, 1},
   {&__pyx_n_s_interp_mode, __pyx_k_interp_mode, sizeof(__pyx_k_interp_mode), 0, 0, 1, 1},
   {&__pyx_n_u_interp_mode, __pyx_k_interp_mode, sizeof(__pyx_k_interp_mode), 0, 1, 0, 1},
   {&__pyx_n_s_is_integer_valued, __pyx_k_is_integer_valued, sizeof(__pyx_k_is_integer_valued), 0, 0, 1, 1},
   {&__pyx_n_s_isin, __pyx_k_isin, sizeof(__pyx_k_isin), 0, 0, 1, 1},
   {&__pyx_n_s_isnan, __pyx_k_isnan, sizeof(__pyx_k_isnan), 0, 0, 1, 1},
   {&__pyx_n_s_isnull, __pyx_k_isnull, sizeof(__pyx_k_isnull), 0, 0, 1, 1},
@@ -49856,15 +49805,15 @@
   __Pyx_GIVEREF(__pyx_tuple__129);
   __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(5, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__129, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_pyx, __pyx_n_s_evaluate_feature_onehot, 740, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 740, __pyx_L1_error)
 
   /* "structureboost/structure_dt.pyx":767
  * 
  * 
  *     def get_prediction(self, tree_node, X_te, dict col_to_int_dict):             # <<<<<<<<<<<<<<
- *         cdef np.ndarray[np.int_t] ind_subset_left, ind_subset_right
+ *         cdef np.ndarray[np.int32_t] ind_subset_left, ind_subset_right
  *         cdef long vec_len, lsize
  */
   __pyx_tuple__130 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_tree_node, __pyx_n_s_X_te, __pyx_n_s_col_to_int_dict, __pyx_n_s_ind_subset_left, __pyx_n_s_ind_subset_right, __pyx_n_s_vec_len, __pyx_n_s_lsize, __pyx_n_s_next_vec, __pyx_n_s_split_bool); if (unlikely(!__pyx_tuple__130)) __PYX_ERR(0, 767, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__130);
   __Pyx_GIVEREF(__pyx_tuple__130);
   __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(4, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__130, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_pyx, __pyx_n_s_get_prediction, 767, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 767, __pyx_L1_error)
 
@@ -49976,15 +49925,15 @@
   __Pyx_GIVEREF(__pyx_tuple__139);
   __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__139, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_pyx, __pyx_n_s_get_best_vals, 888, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 888, __pyx_L1_error)
 
   /* "structureboost/structure_dt.pyx":898
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def get_bin_sums_c(np.ndarray[double, ndim=2] g_h_mat,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] bin_result_vec, long out_vec_size):
+ *                    np.ndarray[np.int32_t] bin_result_vec, long out_vec_size):
  *     cdef int i
  */
   __pyx_tuple__140 = PyTuple_Pack(7, __pyx_n_s_g_h_mat, __pyx_n_s_bin_result_vec, __pyx_n_s_out_vec_size, __pyx_n_s_i, __pyx_n_s_m, __pyx_n_s_g_sum_bins, __pyx_n_s_h_sum_bins); if (unlikely(!__pyx_tuple__140)) __PYX_ERR(0, 898, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__140);
   __Pyx_GIVEREF(__pyx_tuple__140);
   __pyx_codeobj__47 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__140, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_pyx, __pyx_n_s_get_bin_sums_c, 898, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__47)) __PYX_ERR(0, 898, __pyx_L1_error)
 
@@ -50071,15 +50020,15 @@
   __Pyx_GOTREF(__pyx_tuple__147);
   __Pyx_GIVEREF(__pyx_tuple__147);
   __pyx_codeobj__56 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__147, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_pyx, __pyx_n_s_get_voronoi_obj, 965, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__56)) __PYX_ERR(0, 965, __pyx_L1_error)
 
   /* "structureboost/structure_dt.pyx":975
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_g_h_feature_sum_arrays(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ * def get_g_h_feature_sum_arrays(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
  *                                np.ndarray[double, ndim=2] g_h_train_node,
  *                                np.ndarray[double, ndim=2] g_h_val_arr):
  */
   __pyx_tuple__148 = PyTuple_Pack(6, __pyx_n_s_feature_vec_node, __pyx_n_s_g_h_train_node, __pyx_n_s_g_h_val_arr, __pyx_n_s_i, __pyx_n_s_ind, __pyx_n_s_array_size); if (unlikely(!__pyx_tuple__148)) __PYX_ERR(0, 975, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__148);
   __Pyx_GIVEREF(__pyx_tuple__148);
   __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(3, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__148, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_pyx, __pyx_n_s_get_g_h_feature_sum_arrays, 975, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 975, __pyx_L1_error)
@@ -50119,40 +50068,40 @@
   __Pyx_GOTREF(__pyx_tuple__151);
   __Pyx_GIVEREF(__pyx_tuple__151);
   __pyx_codeobj__60 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__151, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_pyx, __pyx_n_s_get_mask, 1039, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__60)) __PYX_ERR(0, 1039, __pyx_L1_error)
 
   /* "structureboost/structure_dt.pyx":1045
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_mask_int_c(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] left_split,
+ * def get_mask_int_c(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ *                    np.ndarray[np.int32_t] left_split,
  *                    long vec_len, long lsplit_len,
  */
   __pyx_tuple__152 = PyTuple_Pack(7, __pyx_n_s_feature_vec_node, __pyx_n_s_left_split, __pyx_n_s_vec_len, __pyx_n_s_lsplit_len, __pyx_n_s_mask_vec, __pyx_n_s_i, __pyx_n_s_j); if (unlikely(!__pyx_tuple__152)) __PYX_ERR(0, 1045, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__152);
   __Pyx_GIVEREF(__pyx_tuple__152);
   __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(5, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__152, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_pyx, __pyx_n_s_get_mask_int_c, 1045, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(0, 1045, __pyx_L1_error)
 
   /* "structureboost/structure_dt.pyx":1060
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
- * def separate_indices(np.ndarray[np.int_t] a, np.ndarray[np.int_t] b,             # <<<<<<<<<<<<<<
- *                      np.ndarray[np.int_t] c, long vec_len):
+ * def separate_indices(np.ndarray[np.int32_t] a, np.ndarray[np.int32_t] b,             # <<<<<<<<<<<<<<
+ *                      np.ndarray[np.int32_t] c, long vec_len):
  *     cdef long ind_a = 0, ind_b = 0, i
  */
   __pyx_tuple__153 = PyTuple_Pack(7, __pyx_n_s_a, __pyx_n_s_b, __pyx_n_s_c, __pyx_n_s_vec_len, __pyx_n_s_ind_a, __pyx_n_s_ind_b, __pyx_n_s_i); if (unlikely(!__pyx_tuple__153)) __PYX_ERR(0, 1060, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__153);
   __Pyx_GIVEREF(__pyx_tuple__153);
   __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(4, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__153, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_pyx, __pyx_n_s_separate_indices, 1060, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(0, 1060, __pyx_L1_error)
 
   /* "structureboost/structure_dt.pyx":1073
  * 
  * 
  * def get_node_response_graphical_int(feature_vec, node):             # <<<<<<<<<<<<<<
- *     # fs_array = np.array(list(node['left_split'])).astype(np.int_)
+ *     # fs_array = np.array(list(node['left_split'])).astype(np.int32)
  *     cdef int vec_len, lsplit_len
  */
   __pyx_tuple__154 = PyTuple_Pack(6, __pyx_n_s_feature_vec, __pyx_n_s_node, __pyx_n_s_vec_len, __pyx_n_s_lsplit_len, __pyx_n_s_fs_array, __pyx_n_s_mask_vec); if (unlikely(!__pyx_tuple__154)) __PYX_ERR(0, 1073, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__154);
   __Pyx_GIVEREF(__pyx_tuple__154);
   __pyx_codeobj__63 = (PyObject*)__Pyx_PyCode_New(2, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__154, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_pyx, __pyx_n_s_get_node_response_graphical_int, 1073, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__63)) __PYX_ERR(0, 1073, __pyx_L1_error)
 
@@ -50252,15 +50201,15 @@
   __Pyx_GIVEREF(__pyx_tuple__162);
   __pyx_codeobj__71 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__162, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_pyx, __pyx_n_s_ridge_points_to_edge_set, 1159, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__71)) __PYX_ERR(0, 1159, __pyx_L1_error)
 
   /* "structureboost/structure_dt.pyx":1165
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def map_to_nn_point_index(double[:,:] core_pts, double[:,:] query_pts,             # <<<<<<<<<<<<<<
- *                           np.ndarray[np.int_t] out_mat, long num_core_pts,
+ *                           np.ndarray[np.int32_t] out_mat, long num_core_pts,
  *                           long num_query_pts, long ndim):
  */
   __pyx_tuple__163 = PyTuple_Pack(13, __pyx_n_s_core_pts, __pyx_n_s_query_pts, __pyx_n_s_out_mat, __pyx_n_s_num_core_pts, __pyx_n_s_num_query_pts, __pyx_n_s_ndim, __pyx_n_s_curr_dist, __pyx_n_s_tnum, __pyx_n_s_best_dist, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_best_j, __pyx_n_s_k); if (unlikely(!__pyx_tuple__163)) __PYX_ERR(0, 1165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__163);
   __Pyx_GIVEREF(__pyx_tuple__163);
   __pyx_codeobj__72 = (PyObject*)__Pyx_PyCode_New(6, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__163, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_pyx, __pyx_n_s_map_to_nn_point_index, 1165, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__72)) __PYX_ERR(0, 1165, __pyx_L1_error)
 
@@ -51218,15 +51167,15 @@
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_evaluate_feature_onehot, __pyx_t_3) < 0) __PYX_ERR(0, 740, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "structureboost/structure_dt.pyx":767
  * 
  * 
  *     def get_prediction(self, tree_node, X_te, dict col_to_int_dict):             # <<<<<<<<<<<<<<
- *         cdef np.ndarray[np.int_t] ind_subset_left, ind_subset_right
+ *         cdef np.ndarray[np.int32_t] ind_subset_left, ind_subset_right
  *         cdef long vec_len, lsize
  */
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_14structureboost_12structure_dt_21StructureDecisionTree_61get_prediction, 0, __pyx_n_s_StructureDecisionTree_get_predic, NULL, __pyx_n_s_structureboost_structure_dt, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 767, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_1, __pyx_n_s_get_prediction, __pyx_t_3) < 0) __PYX_ERR(0, 767, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
@@ -51352,15 +51301,15 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_best_vals, __pyx_t_2) < 0) __PYX_ERR(0, 888, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "structureboost/structure_dt.pyx":898
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def get_bin_sums_c(np.ndarray[double, ndim=2] g_h_mat,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] bin_result_vec, long out_vec_size):
+ *                    np.ndarray[np.int32_t] bin_result_vec, long out_vec_size):
  *     cdef int i
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_12structure_dt_15get_bin_sums_c, NULL, __pyx_n_s_structureboost_structure_dt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 898, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_bin_sums_c, __pyx_t_2) < 0) __PYX_ERR(0, 898, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
@@ -51447,15 +51396,15 @@
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_voronoi_obj, __pyx_t_2) < 0) __PYX_ERR(0, 965, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "structureboost/structure_dt.pyx":975
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_g_h_feature_sum_arrays(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ * def get_g_h_feature_sum_arrays(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
  *                                np.ndarray[double, ndim=2] g_h_train_node,
  *                                np.ndarray[double, ndim=2] g_h_val_arr):
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_12structure_dt_31get_g_h_feature_sum_arrays, NULL, __pyx_n_s_structureboost_structure_dt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 975, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_g_h_feature_sum_arrays, __pyx_t_2) < 0) __PYX_ERR(0, 975, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -51495,40 +51444,40 @@
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_mask, __pyx_t_2) < 0) __PYX_ERR(0, 1039, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "structureboost/structure_dt.pyx":1045
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_mask_int_c(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] left_split,
+ * def get_mask_int_c(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ *                    np.ndarray[np.int32_t] left_split,
  *                    long vec_len, long lsplit_len,
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_12structure_dt_39get_mask_int_c, NULL, __pyx_n_s_structureboost_structure_dt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1045, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_mask_int_c, __pyx_t_2) < 0) __PYX_ERR(0, 1045, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "structureboost/structure_dt.pyx":1060
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
- * def separate_indices(np.ndarray[np.int_t] a, np.ndarray[np.int_t] b,             # <<<<<<<<<<<<<<
- *                      np.ndarray[np.int_t] c, long vec_len):
+ * def separate_indices(np.ndarray[np.int32_t] a, np.ndarray[np.int32_t] b,             # <<<<<<<<<<<<<<
+ *                      np.ndarray[np.int32_t] c, long vec_len):
  *     cdef long ind_a = 0, ind_b = 0, i
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_12structure_dt_41separate_indices, NULL, __pyx_n_s_structureboost_structure_dt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1060, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_separate_indices, __pyx_t_2) < 0) __PYX_ERR(0, 1060, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "structureboost/structure_dt.pyx":1073
  * 
  * 
  * def get_node_response_graphical_int(feature_vec, node):             # <<<<<<<<<<<<<<
- *     # fs_array = np.array(list(node['left_split'])).astype(np.int_)
+ *     # fs_array = np.array(list(node['left_split'])).astype(np.int32)
  *     cdef int vec_len, lsplit_len
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_12structure_dt_43get_node_response_graphical_int, NULL, __pyx_n_s_structureboost_structure_dt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1073, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_node_response_graphical_int, __pyx_t_2) < 0) __PYX_ERR(0, 1073, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
@@ -51628,15 +51577,15 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ridge_points_to_edge_set, __pyx_t_2) < 0) __PYX_ERR(0, 1159, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "structureboost/structure_dt.pyx":1165
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def map_to_nn_point_index(double[:,:] core_pts, double[:,:] query_pts,             # <<<<<<<<<<<<<<
- *                           np.ndarray[np.int_t] out_mat, long num_core_pts,
+ *                           np.ndarray[np.int32_t] out_mat, long num_core_pts,
  *                           long num_query_pts, long ndim):
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_12structure_dt_61map_to_nn_point_index, NULL, __pyx_n_s_structureboost_structure_dt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_map_to_nn_point_index, __pyx_t_2) < 0) __PYX_ERR(0, 1165, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
```

### Comparing `structureboost-0.4.2/structureboost/structure_dt_multi.c` & `structureboost-0.4.3/structureboost/structure_dt_multi.c`

 * *Files 1% similar despite different names*

```diff
@@ -2220,15 +2220,15 @@
 static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'structureboost.structure_dt_multi' */
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int_t = { "int_t", NULL, sizeof(__pyx_t_5numpy_int_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int_t), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t = { "int32_t", NULL, sizeof(__pyx_t_5numpy_int32_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int32_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int32_t), 0 };
 #define __Pyx_MODULE_NAME "structureboost.structure_dt_multi"
 extern int __pyx_module_is_main_structureboost__structure_dt_multi;
 int __pyx_module_is_main_structureboost__structure_dt_multi = 0;
 
 /* Implementation of 'structureboost.structure_dt_multi' */
 static PyObject *__pyx_builtin_super;
 static PyObject *__pyx_builtin_range;
@@ -2238,15 +2238,14 @@
 static const char __pyx_k_m[] = "m";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_pd[] = "pd";
 static const char __pyx_k_sp[] = "sp";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_ind[] = "ind";
 static const char __pyx_k_inf[] = "inf";
-static const char __pyx_k_int[] = "int_";
 static const char __pyx_k_lni[] = "lni";
 static const char __pyx_k_lvi[] = "lvi";
 static const char __pyx_k_sum[] = "sum";
 static const char __pyx_k_tol[] = "tol";
 static const char __pyx_k_X_te[] = "X_te";
 static const char __pyx_k_axis[] = "axis";
 static const char __pyx_k_copy[] = "copy";
@@ -2261,14 +2260,15 @@
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_empty[] = "empty";
 static const char __pyx_k_g_sum[] = "g_sum";
 static const char __pyx_k_g_vec[] = "g_vec";
 static const char __pyx_k_gamma[] = "gamma";
 static const char __pyx_k_h_sum[] = "h_sum";
 static const char __pyx_k_h_vec[] = "h_vec";
+static const char __pyx_k_int32[] = "int32";
 static const char __pyx_k_isnan[] = "isnan";
 static const char __pyx_k_limit[] = "limit";
 static const char __pyx_k_lsize[] = "lsize";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_right[] = "right";
 static const char __pyx_k_scipy[] = "scipy";
@@ -2483,15 +2483,15 @@
 static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_ind;
 static PyObject *__pyx_n_s_ind_subset_left;
 static PyObject *__pyx_n_s_ind_subset_right;
 static PyObject *__pyx_n_s_inf;
 static PyObject *__pyx_n_s_init;
-static PyObject *__pyx_n_s_int;
+static PyObject *__pyx_n_s_int32;
 static PyObject *__pyx_n_s_isnan;
 static PyObject *__pyx_n_s_j;
 static PyObject *__pyx_n_u_leaf;
 static PyObject *__pyx_n_s_leaf_vertex_ind;
 static PyObject *__pyx_n_u_left_child;
 static PyObject *__pyx_n_s_left_feat_values;
 static PyObject *__pyx_n_s_limit;
@@ -3391,75 +3391,75 @@
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_dt_multi.pyx":51
  * 
  *         has_na_vals = np.isnan(split_vec[-1])
  *         bin_result_vec = np.searchsorted(split_vec,             # <<<<<<<<<<<<<<
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_searchsorted); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "structureboost/structure_dt_multi.pyx":52
  *         has_na_vals = np.isnan(split_vec[-1])
  *         bin_result_vec = np.searchsorted(split_vec,
  *                                          feature_vec,             # <<<<<<<<<<<<<<
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  *         g_sum_bins, h_sum_bins = get_bin_sums_c_mc(g_h_mat,
  */
   __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_split_vec);
   __Pyx_GIVEREF(__pyx_v_split_vec);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_split_vec);
   __Pyx_INCREF(__pyx_v_feature_vec);
   __Pyx_GIVEREF(__pyx_v_feature_vec);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_feature_vec);
 
   /* "structureboost/structure_dt_multi.pyx":53
  *         bin_result_vec = np.searchsorted(split_vec,
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)             # <<<<<<<<<<<<<<
+ *                                          side='right').astype(np.int32)             # <<<<<<<<<<<<<<
  *         g_sum_bins, h_sum_bins = get_bin_sums_c_mc(g_h_mat,
  *                                                 bin_result_vec,
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_side, __pyx_n_u_right) < 0) __PYX_ERR(0, 53, __pyx_L1_error)
 
   /* "structureboost/structure_dt_multi.pyx":51
  * 
  *         has_na_vals = np.isnan(split_vec[-1])
  *         bin_result_vec = np.searchsorted(split_vec,             # <<<<<<<<<<<<<<
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  */
   __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "structureboost/structure_dt_multi.pyx":53
  *         bin_result_vec = np.searchsorted(split_vec,
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)             # <<<<<<<<<<<<<<
+ *                                          side='right').astype(np.int32)             # <<<<<<<<<<<<<<
  *         g_sum_bins, h_sum_bins = get_bin_sums_c_mc(g_h_mat,
  *                                                 bin_result_vec,
  */
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -3475,15 +3475,15 @@
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_bin_result_vec = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_dt_multi.pyx":54
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  *         g_sum_bins, h_sum_bins = get_bin_sums_c_mc(g_h_mat,             # <<<<<<<<<<<<<<
  *                                                 bin_result_vec,
  *                                                 len(split_vec)+1, self.num_classes)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_get_bin_sums_c_mc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
@@ -3599,15 +3599,15 @@
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
     __PYX_ERR(0, 54, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
 
   /* "structureboost/structure_dt_multi.pyx":54
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  *         g_sum_bins, h_sum_bins = get_bin_sums_c_mc(g_h_mat,             # <<<<<<<<<<<<<<
  *                                                 bin_result_vec,
  *                                                 len(split_vec)+1, self.num_classes)
  */
   __pyx_v_g_sum_bins = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_v_h_sum_bins = __pyx_t_8;
@@ -4587,15 +4587,15 @@
   __Pyx_TraceCall("get_gh_val_mat", __pyx_f[0], 89, 0, __PYX_ERR(0, 89, __pyx_L1_error));
 
   /* "structureboost/structure_dt_multi.pyx":91
  *     def get_gh_val_mat(self, feature_vec_node,g_h_train_node,
  *                        max_num_vertices):
  *         g_h_val_arr = np.zeros((max_num_vertices,2*self.num_classes))             # <<<<<<<<<<<<<<
  *         g_h_val_arr = get_g_h_feature_sum_matrix(
- *                                         feature_vec_node.astype(np.int_),
+ *                                         feature_vec_node.astype(np.int32),
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_num_classes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
@@ -4630,32 +4630,32 @@
   __pyx_v_g_h_val_arr = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_dt_multi.pyx":92
  *                        max_num_vertices):
  *         g_h_val_arr = np.zeros((max_num_vertices,2*self.num_classes))
  *         g_h_val_arr = get_g_h_feature_sum_matrix(             # <<<<<<<<<<<<<<
- *                                         feature_vec_node.astype(np.int_),
+ *                                         feature_vec_node.astype(np.int32),
  *                                         g_h_train_node,
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_get_g_h_feature_sum_matrix); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
   /* "structureboost/structure_dt_multi.pyx":93
  *         g_h_val_arr = np.zeros((max_num_vertices,2*self.num_classes))
  *         g_h_val_arr = get_g_h_feature_sum_matrix(
- *                                         feature_vec_node.astype(np.int_),             # <<<<<<<<<<<<<<
+ *                                         feature_vec_node.astype(np.int32),             # <<<<<<<<<<<<<<
  *                                         g_h_train_node,
  *                                         g_h_val_arr, self.num_classes)
  */
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_feature_vec_node, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -4668,15 +4668,15 @@
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "structureboost/structure_dt_multi.pyx":95
- *                                         feature_vec_node.astype(np.int_),
+ *                                         feature_vec_node.astype(np.int32),
  *                                         g_h_train_node,
  *                                         g_h_val_arr, self.num_classes)             # <<<<<<<<<<<<<<
  *         return g_h_val_arr
  * 
  */
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_num_classes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
@@ -6050,15 +6050,15 @@
   return __pyx_r;
 }
 
 /* "structureboost/structure_dt_multi.pyx":142
  * 
  * 
  *     def get_prediction(self, tree_node, X_te, dict col_to_int_dict):             # <<<<<<<<<<<<<<
- *         cdef np.ndarray[np.int_t] ind_subset_left, ind_subset_right
+ *         cdef np.ndarray[np.int32_t] ind_subset_left, ind_subset_right
  *         cdef long vec_len, lsize
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_18structure_dt_multi_26StructureDecisionTreeMulti_17get_prediction(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_18structure_dt_multi_26StructureDecisionTreeMulti_17get_prediction = {"get_prediction", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_18structure_dt_multi_26StructureDecisionTreeMulti_17get_prediction, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_18structure_dt_multi_26StructureDecisionTreeMulti_17get_prediction(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -6357,25 +6357,25 @@
     __pyx_t_1 = 0;
 
     /* "structureboost/structure_dt_multi.pyx":151
  *         else:
  *             split_bool = stdt.get_node_response_df_val(X_te, tree_node, col_to_int_dict)
  *             vec_len = len(split_bool)             # <<<<<<<<<<<<<<
  *             next_vec = np.zeros((vec_len,self.num_classes))
- *             ind_subset_left = np.empty(vec_len, dtype=np.int_)
+ *             ind_subset_left = np.empty(vec_len, dtype=np.int32)
  */
     __pyx_t_8 = PyObject_Length(__pyx_v_split_bool); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 151, __pyx_L1_error)
     __pyx_v_vec_len = __pyx_t_8;
 
     /* "structureboost/structure_dt_multi.pyx":152
  *             split_bool = stdt.get_node_response_df_val(X_te, tree_node, col_to_int_dict)
  *             vec_len = len(split_bool)
  *             next_vec = np.zeros((vec_len,self.num_classes))             # <<<<<<<<<<<<<<
- *             ind_subset_left = np.empty(vec_len, dtype=np.int_)
- *             ind_subset_right = np.empty(vec_len, dtype=np.int_)
+ *             ind_subset_left = np.empty(vec_len, dtype=np.int32)
+ *             ind_subset_right = np.empty(vec_len, dtype=np.int32)
  */
     __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 152, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_v_vec_len); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
@@ -6428,16 +6428,16 @@
     __pyx_t_9 = 0;
     __pyx_v_next_vec = ((PyArrayObject *)__pyx_t_1);
     __pyx_t_1 = 0;
 
     /* "structureboost/structure_dt_multi.pyx":153
  *             vec_len = len(split_bool)
  *             next_vec = np.zeros((vec_len,self.num_classes))
- *             ind_subset_left = np.empty(vec_len, dtype=np.int_)             # <<<<<<<<<<<<<<
- *             ind_subset_right = np.empty(vec_len, dtype=np.int_)
+ *             ind_subset_left = np.empty(vec_len, dtype=np.int32)             # <<<<<<<<<<<<<<
+ *             ind_subset_right = np.empty(vec_len, dtype=np.int32)
  *             ind_subset_left, ind_subset_right, lsize = stdt.separate_indices(
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 153, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -6448,33 +6448,33 @@
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
     __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 153, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 153, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 153, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 153, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (!(likely(((__pyx_t_7) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_7, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 153, __pyx_L1_error)
     __pyx_t_13 = ((PyArrayObject *)__pyx_t_7);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer);
-      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_12, &__pyx_t_11, &__pyx_t_10);
-        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_left, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_left, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_10);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_12, __pyx_t_11, __pyx_t_10);
         }
         __pyx_t_12 = __pyx_t_11 = __pyx_t_10 = 0;
       }
@@ -6483,16 +6483,16 @@
     }
     __pyx_t_13 = 0;
     __pyx_v_ind_subset_left = ((PyArrayObject *)__pyx_t_7);
     __pyx_t_7 = 0;
 
     /* "structureboost/structure_dt_multi.pyx":154
  *             next_vec = np.zeros((vec_len,self.num_classes))
- *             ind_subset_left = np.empty(vec_len, dtype=np.int_)
- *             ind_subset_right = np.empty(vec_len, dtype=np.int_)             # <<<<<<<<<<<<<<
+ *             ind_subset_left = np.empty(vec_len, dtype=np.int32)
+ *             ind_subset_right = np.empty(vec_len, dtype=np.int32)             # <<<<<<<<<<<<<<
  *             ind_subset_left, ind_subset_right, lsize = stdt.separate_indices(
  *                                                     ind_subset_left,
  */
     __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 154, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
@@ -6504,33 +6504,33 @@
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_7);
     __pyx_t_7 = 0;
     __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 154, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 154, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 154, __pyx_L1_error)
     __pyx_t_13 = ((PyArrayObject *)__pyx_t_4);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer);
-      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
-        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_right, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_right, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_10); Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_12);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_10, __pyx_t_11, __pyx_t_12);
         }
         __pyx_t_10 = __pyx_t_11 = __pyx_t_12 = 0;
       }
@@ -6538,38 +6538,38 @@
       if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 154, __pyx_L1_error)
     }
     __pyx_t_13 = 0;
     __pyx_v_ind_subset_right = ((PyArrayObject *)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "structureboost/structure_dt_multi.pyx":155
- *             ind_subset_left = np.empty(vec_len, dtype=np.int_)
- *             ind_subset_right = np.empty(vec_len, dtype=np.int_)
+ *             ind_subset_left = np.empty(vec_len, dtype=np.int32)
+ *             ind_subset_right = np.empty(vec_len, dtype=np.int32)
  *             ind_subset_left, ind_subset_right, lsize = stdt.separate_indices(             # <<<<<<<<<<<<<<
  *                                                     ind_subset_left,
  *                                                     ind_subset_right,
  */
     __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_stdt); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 155, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_separate_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
     /* "structureboost/structure_dt_multi.pyx":158
  *                                                     ind_subset_left,
  *                                                     ind_subset_right,
- *                                                     split_bool.astype(np.int_),             # <<<<<<<<<<<<<<
+ *                                                     split_bool.astype(np.int32),             # <<<<<<<<<<<<<<
  *                                                     vec_len)
  *             ind_subset_left = ind_subset_left[:lsize]
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_split_bool, __pyx_n_s_astype); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_14);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -6583,15 +6583,15 @@
     __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
     if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 158, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "structureboost/structure_dt_multi.pyx":159
  *                                                     ind_subset_right,
- *                                                     split_bool.astype(np.int_),
+ *                                                     split_bool.astype(np.int32),
  *                                                     vec_len)             # <<<<<<<<<<<<<<
  *             ind_subset_left = ind_subset_left[:lsize]
  *             ind_subset_right = ind_subset_right[:(vec_len-lsize)]
  */
     __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_vec_len); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_14 = NULL;
@@ -6700,32 +6700,32 @@
       __pyx_t_15 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
       __PYX_ERR(0, 155, __pyx_L1_error)
       __pyx_L5_unpacking_done:;
     }
 
     /* "structureboost/structure_dt_multi.pyx":155
- *             ind_subset_left = np.empty(vec_len, dtype=np.int_)
- *             ind_subset_right = np.empty(vec_len, dtype=np.int_)
+ *             ind_subset_left = np.empty(vec_len, dtype=np.int32)
+ *             ind_subset_right = np.empty(vec_len, dtype=np.int32)
  *             ind_subset_left, ind_subset_right, lsize = stdt.separate_indices(             # <<<<<<<<<<<<<<
  *                                                     ind_subset_left,
  *                                                     ind_subset_right,
  */
     if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 155, __pyx_L1_error)
     if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 155, __pyx_L1_error)
     __pyx_t_16 = __Pyx_PyInt_As_long(__pyx_t_1); if (unlikely((__pyx_t_16 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 155, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_13 = ((PyArrayObject *)__pyx_t_3);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer);
-      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_12, &__pyx_t_11, &__pyx_t_10);
-        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_left, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_left, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_10);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_12, __pyx_t_11, __pyx_t_10);
         }
         __pyx_t_12 = __pyx_t_11 = __pyx_t_10 = 0;
       }
@@ -6735,18 +6735,18 @@
     __pyx_t_13 = 0;
     __Pyx_DECREF_SET(__pyx_v_ind_subset_left, ((PyArrayObject *)__pyx_t_3));
     __pyx_t_3 = 0;
     __pyx_t_13 = ((PyArrayObject *)__pyx_t_5);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer);
-      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
-        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_right, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_right, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_10); Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_12);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_10, __pyx_t_11, __pyx_t_12);
         }
         __pyx_t_10 = __pyx_t_11 = __pyx_t_12 = 0;
       }
@@ -6755,15 +6755,15 @@
     }
     __pyx_t_13 = 0;
     __Pyx_DECREF_SET(__pyx_v_ind_subset_right, ((PyArrayObject *)__pyx_t_5));
     __pyx_t_5 = 0;
     __pyx_v_lsize = __pyx_t_16;
 
     /* "structureboost/structure_dt_multi.pyx":160
- *                                                     split_bool.astype(np.int_),
+ *                                                     split_bool.astype(np.int32),
  *                                                     vec_len)
  *             ind_subset_left = ind_subset_left[:lsize]             # <<<<<<<<<<<<<<
  *             ind_subset_right = ind_subset_right[:(vec_len-lsize)]
  * 
  */
     __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_v_lsize); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 160, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
@@ -6774,18 +6774,18 @@
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 160, __pyx_L1_error)
     __pyx_t_13 = ((PyArrayObject *)__pyx_t_4);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer);
-      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_12, &__pyx_t_11, &__pyx_t_10);
-        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_left, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_left.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_left, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_12); Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_10);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_12, __pyx_t_11, __pyx_t_10);
         }
         __pyx_t_12 = __pyx_t_11 = __pyx_t_10 = 0;
       }
@@ -6812,18 +6812,18 @@
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 161, __pyx_L1_error)
     __pyx_t_13 = ((PyArrayObject *)__pyx_t_4);
     {
       __Pyx_BufFmt_StackElem __pyx_stack[1];
       __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer);
-      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+      __pyx_t_6 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
       if (unlikely(__pyx_t_6 < 0)) {
         PyErr_Fetch(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
-        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_right, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+        if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ind_subset_right.rcbuffer->pybuffer, (PyObject*)__pyx_v_ind_subset_right, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
           Py_XDECREF(__pyx_t_10); Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_12);
           __Pyx_RaiseBufferFallbackError();
         } else {
           PyErr_Restore(__pyx_t_10, __pyx_t_11, __pyx_t_12);
         }
         __pyx_t_10 = __pyx_t_11 = __pyx_t_12 = 0;
       }
@@ -7113,15 +7113,15 @@
     goto __pyx_L0;
   }
 
   /* "structureboost/structure_dt_multi.pyx":142
  * 
  * 
  *     def get_prediction(self, tree_node, X_te, dict col_to_int_dict):             # <<<<<<<<<<<<<<
- *         cdef np.ndarray[np.int_t] ind_subset_left, ind_subset_right
+ *         cdef np.ndarray[np.int32_t] ind_subset_left, ind_subset_right
  *         cdef long vec_len, lsize
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
@@ -7154,15 +7154,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "structureboost/structure_dt_multi.pyx":179
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_g_h_feature_sum_matrix(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ * def get_g_h_feature_sum_matrix(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
  *                                np.ndarray[double, ndim=2] g_h_train_node,
  *                                np.ndarray[double, ndim=2] g_h_val_arr,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_18structure_dt_multi_1get_g_h_feature_sum_matrix(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_18structure_dt_multi_1get_g_h_feature_sum_matrix = {"get_g_h_feature_sum_matrix", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_18structure_dt_multi_1get_g_h_feature_sum_matrix, METH_VARARGS|METH_KEYWORDS, 0};
@@ -7298,15 +7298,15 @@
   __pyx_pybuffernd_g_h_train_node.rcbuffer = &__pyx_pybuffer_g_h_train_node;
   __pyx_pybuffer_g_h_val_arr.pybuffer.buf = NULL;
   __pyx_pybuffer_g_h_val_arr.refcount = 0;
   __pyx_pybuffernd_g_h_val_arr.data = NULL;
   __pyx_pybuffernd_g_h_val_arr.rcbuffer = &__pyx_pybuffer_g_h_val_arr;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer, (PyObject*)__pyx_v_feature_vec_node, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 179, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer, (PyObject*)__pyx_v_feature_vec_node, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 179, __pyx_L1_error)
   }
   __pyx_pybuffernd_feature_vec_node.diminfo[0].strides = __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_feature_vec_node.diminfo[0].shape = __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_g_h_train_node.rcbuffer->pybuffer, (PyObject*)__pyx_v_g_h_train_node, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 179, __pyx_L1_error)
   }
   __pyx_pybuffernd_g_h_train_node.diminfo[0].strides = __pyx_pybuffernd_g_h_train_node.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_g_h_train_node.diminfo[0].shape = __pyx_pybuffernd_g_h_train_node.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_g_h_train_node.diminfo[1].strides = __pyx_pybuffernd_g_h_train_node.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_g_h_train_node.diminfo[1].shape = __pyx_pybuffernd_g_h_train_node.rcbuffer->pybuffer.shape[1];
@@ -7354,15 +7354,15 @@
  *     for i in range(array_size):
  *         for j in range(2*num_classes):
  *             ind = feature_vec_node[i]             # <<<<<<<<<<<<<<
  *             g_h_val_arr[ind,j] += g_h_train_node[i,j]
  *     return g_h_val_arr
  */
       __pyx_t_8 = __pyx_v_i;
-      __pyx_v_ind = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_feature_vec_node.diminfo[0].strides));
+      __pyx_v_ind = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_feature_vec_node.diminfo[0].strides));
 
       /* "structureboost/structure_dt_multi.pyx":188
  *         for j in range(2*num_classes):
  *             ind = feature_vec_node[i]
  *             g_h_val_arr[ind,j] += g_h_train_node[i,j]             # <<<<<<<<<<<<<<
  *     return g_h_val_arr
  * 
@@ -7386,15 +7386,15 @@
   __Pyx_INCREF(((PyObject *)__pyx_v_g_h_val_arr));
   __pyx_r = ((PyObject *)__pyx_v_g_h_val_arr);
   goto __pyx_L0;
 
   /* "structureboost/structure_dt_multi.pyx":179
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_g_h_feature_sum_matrix(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ * def get_g_h_feature_sum_matrix(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
  *                                np.ndarray[double, ndim=2] g_h_train_node,
  *                                np.ndarray[double, ndim=2] g_h_val_arr,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
@@ -8287,15 +8287,15 @@
   return __pyx_r;
 }
 
 /* "structureboost/structure_dt_multi.pyx":219
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def get_bin_sums_c_mc(np.ndarray[double, ndim=2] g_h_mat,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] bin_result_vec,
+ *                    np.ndarray[np.int32_t] bin_result_vec,
  *                    long out_vec_size, long num_classes):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_18structure_dt_multi_7get_bin_sums_c_mc(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_18structure_dt_multi_7get_bin_sums_c_mc = {"get_bin_sums_c_mc", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_18structure_dt_multi_7get_bin_sums_c_mc, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_18structure_dt_multi_7get_bin_sums_c_mc(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -8448,15 +8448,15 @@
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_g_h_mat.rcbuffer->pybuffer, (PyObject*)__pyx_v_g_h_mat, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 219, __pyx_L1_error)
   }
   __pyx_pybuffernd_g_h_mat.diminfo[0].strides = __pyx_pybuffernd_g_h_mat.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_g_h_mat.diminfo[0].shape = __pyx_pybuffernd_g_h_mat.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_g_h_mat.diminfo[1].strides = __pyx_pybuffernd_g_h_mat.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_g_h_mat.diminfo[1].shape = __pyx_pybuffernd_g_h_mat.rcbuffer->pybuffer.shape[1];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_bin_result_vec, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 219, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_bin_result_vec, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 219, __pyx_L1_error)
   }
   __pyx_pybuffernd_bin_result_vec.diminfo[0].strides = __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_bin_result_vec.diminfo[0].shape = __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.shape[0];
 
   /* "structureboost/structure_dt_multi.pyx":223
  *                    long out_vec_size, long num_classes):
  *     cdef int i,j
  *     cdef int m = bin_result_vec.shape[0]             # <<<<<<<<<<<<<<
@@ -8603,29 +8603,29 @@
  *             g_sum_bins[bin_result_vec[i],j] += g_h_mat[i,j]             # <<<<<<<<<<<<<<
  *             h_sum_bins[bin_result_vec[i],j] += g_h_mat[i,num_classes+j]
  *     return g_sum_bins, h_sum_bins
  */
       __pyx_t_14 = __pyx_v_i;
       __pyx_t_15 = __pyx_v_j;
       __pyx_t_16 = __pyx_v_i;
-      __pyx_t_17 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_bin_result_vec.diminfo[0].strides));
+      __pyx_t_17 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_bin_result_vec.diminfo[0].strides));
       __pyx_t_18 = __pyx_v_j;
       *__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_g_sum_bins.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_g_sum_bins.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_g_sum_bins.diminfo[1].strides) += (*__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_g_h_mat.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_g_h_mat.diminfo[0].strides, __pyx_t_15, __pyx_pybuffernd_g_h_mat.diminfo[1].strides));
 
       /* "structureboost/structure_dt_multi.pyx":231
  *         for j in range(num_classes):
  *             g_sum_bins[bin_result_vec[i],j] += g_h_mat[i,j]
  *             h_sum_bins[bin_result_vec[i],j] += g_h_mat[i,num_classes+j]             # <<<<<<<<<<<<<<
  *     return g_sum_bins, h_sum_bins
  * 
  */
       __pyx_t_15 = __pyx_v_i;
       __pyx_t_14 = (__pyx_v_num_classes + __pyx_v_j);
       __pyx_t_16 = __pyx_v_i;
-      __pyx_t_18 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_bin_result_vec.diminfo[0].strides));
+      __pyx_t_18 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_bin_result_vec.diminfo[0].strides));
       __pyx_t_17 = __pyx_v_j;
       *__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_h_sum_bins.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_h_sum_bins.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_h_sum_bins.diminfo[1].strides) += (*__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_g_h_mat.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_g_h_mat.diminfo[0].strides, __pyx_t_14, __pyx_pybuffernd_g_h_mat.diminfo[1].strides));
     }
   }
 
   /* "structureboost/structure_dt_multi.pyx":232
  *             g_sum_bins[bin_result_vec[i],j] += g_h_mat[i,j]
@@ -8647,15 +8647,15 @@
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "structureboost/structure_dt_multi.pyx":219
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def get_bin_sums_c_mc(np.ndarray[double, ndim=2] g_h_mat,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] bin_result_vec,
+ *                    np.ndarray[np.int32_t] bin_result_vec,
  *                    long out_vec_size, long num_classes):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -10089,15 +10089,15 @@
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_ind, __pyx_k_ind, sizeof(__pyx_k_ind), 0, 0, 1, 1},
   {&__pyx_n_s_ind_subset_left, __pyx_k_ind_subset_left, sizeof(__pyx_k_ind_subset_left), 0, 0, 1, 1},
   {&__pyx_n_s_ind_subset_right, __pyx_k_ind_subset_right, sizeof(__pyx_k_ind_subset_right), 0, 0, 1, 1},
   {&__pyx_n_s_inf, __pyx_k_inf, sizeof(__pyx_k_inf), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
-  {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
+  {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
   {&__pyx_n_s_isnan, __pyx_k_isnan, sizeof(__pyx_k_isnan), 0, 0, 1, 1},
   {&__pyx_n_s_j, __pyx_k_j, sizeof(__pyx_k_j), 0, 0, 1, 1},
   {&__pyx_n_u_leaf, __pyx_k_leaf, sizeof(__pyx_k_leaf), 0, 1, 0, 1},
   {&__pyx_n_s_leaf_vertex_ind, __pyx_k_leaf_vertex_ind, sizeof(__pyx_k_leaf_vertex_ind), 0, 0, 1, 1},
   {&__pyx_n_u_left_child, __pyx_k_left_child, sizeof(__pyx_k_left_child), 0, 1, 0, 1},
   {&__pyx_n_s_left_feat_values, __pyx_k_left_feat_values, sizeof(__pyx_k_left_feat_values), 0, 0, 1, 1},
   {&__pyx_n_s_limit, __pyx_k_limit, sizeof(__pyx_k_limit), 0, 0, 1, 1},
@@ -10326,26 +10326,26 @@
   __Pyx_GIVEREF(__pyx_tuple__29);
   __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_multi_pyx, __pyx_n_s_predict, 135, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 135, __pyx_L1_error)
 
   /* "structureboost/structure_dt_multi.pyx":142
  * 
  * 
  *     def get_prediction(self, tree_node, X_te, dict col_to_int_dict):             # <<<<<<<<<<<<<<
- *         cdef np.ndarray[np.int_t] ind_subset_left, ind_subset_right
+ *         cdef np.ndarray[np.int32_t] ind_subset_left, ind_subset_right
  *         cdef long vec_len, lsize
  */
   __pyx_tuple__30 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_tree_node, __pyx_n_s_X_te, __pyx_n_s_col_to_int_dict, __pyx_n_s_ind_subset_left, __pyx_n_s_ind_subset_right, __pyx_n_s_vec_len, __pyx_n_s_lsize, __pyx_n_s_next_vec, __pyx_n_s_split_bool); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__30);
   __Pyx_GIVEREF(__pyx_tuple__30);
   __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(4, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_multi_pyx, __pyx_n_s_get_prediction, 142, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 142, __pyx_L1_error)
 
   /* "structureboost/structure_dt_multi.pyx":179
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_g_h_feature_sum_matrix(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ * def get_g_h_feature_sum_matrix(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
  *                                np.ndarray[double, ndim=2] g_h_train_node,
  *                                np.ndarray[double, ndim=2] g_h_val_arr,
  */
   __pyx_tuple__31 = PyTuple_Pack(8, __pyx_n_s_feature_vec_node, __pyx_n_s_g_h_train_node, __pyx_n_s_g_h_val_arr, __pyx_n_s_num_classes, __pyx_n_s_i, __pyx_n_s_ind, __pyx_n_s_array_size, __pyx_n_s_j); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
   __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(4, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_multi_pyx, __pyx_n_s_get_g_h_feature_sum_matrix, 179, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 179, __pyx_L1_error)
@@ -10374,15 +10374,15 @@
   __Pyx_GIVEREF(__pyx_tuple__33);
   __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(6, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_multi_pyx, __pyx_n_s_get_gh_score_array_mc, 206, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 206, __pyx_L1_error)
 
   /* "structureboost/structure_dt_multi.pyx":219
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def get_bin_sums_c_mc(np.ndarray[double, ndim=2] g_h_mat,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] bin_result_vec,
+ *                    np.ndarray[np.int32_t] bin_result_vec,
  *                    long out_vec_size, long num_classes):
  */
   __pyx_tuple__34 = PyTuple_Pack(9, __pyx_n_s_g_h_mat, __pyx_n_s_bin_result_vec, __pyx_n_s_out_vec_size, __pyx_n_s_num_classes, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_m, __pyx_n_s_g_sum_bins, __pyx_n_s_h_sum_bins); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__34);
   __Pyx_GIVEREF(__pyx_tuple__34);
   __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(4, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_dt_multi_pyx, __pyx_n_s_get_bin_sums_c_mc, 219, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 219, __pyx_L1_error)
 
@@ -10978,15 +10978,15 @@
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_predict, __pyx_t_5) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "structureboost/structure_dt_multi.pyx":142
  * 
  * 
  *     def get_prediction(self, tree_node, X_te, dict col_to_int_dict):             # <<<<<<<<<<<<<<
- *         cdef np.ndarray[np.int_t] ind_subset_left, ind_subset_right
+ *         cdef np.ndarray[np.int32_t] ind_subset_left, ind_subset_right
  *         cdef long vec_len, lsize
  */
   __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_14structureboost_18structure_dt_multi_26StructureDecisionTreeMulti_17get_prediction, 0, __pyx_n_s_StructureDecisionTreeMulti_get_p, NULL, __pyx_n_s_structureboost_structure_dt_mult, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_get_prediction, __pyx_t_5) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
@@ -11006,15 +11006,15 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_dt_multi.pyx":179
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_g_h_feature_sum_matrix(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ * def get_g_h_feature_sum_matrix(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
  *                                np.ndarray[double, ndim=2] g_h_train_node,
  *                                np.ndarray[double, ndim=2] g_h_val_arr,
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_18structure_dt_multi_1get_g_h_feature_sum_matrix, NULL, __pyx_n_s_structureboost_structure_dt_mult); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_g_h_feature_sum_matrix, __pyx_t_1) < 0) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -11043,15 +11043,15 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_gh_score_array_mc, __pyx_t_1) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_dt_multi.pyx":219
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def get_bin_sums_c_mc(np.ndarray[double, ndim=2] g_h_mat,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] bin_result_vec,
+ *                    np.ndarray[np.int32_t] bin_result_vec,
  *                    long out_vec_size, long num_classes):
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_18structure_dt_multi_7get_bin_sums_c_mc, NULL, __pyx_n_s_structureboost_structure_dt_mult); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_bin_sums_c_mc, __pyx_t_1) < 0) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `structureboost-0.4.2/structureboost/structure_gb.c` & `structureboost-0.4.3/structureboost/structure_gb.c`

 * *Files 1% similar despite different names*

```diff
@@ -2679,14 +2679,17 @@
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_Py_intptr_t(Py_intptr_t value);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_npy_int32(npy_int32 value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
@@ -2793,15 +2796,15 @@
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *, int, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_long = { "long", NULL, sizeof(long), { 0 }, 0, IS_UNSIGNED(long) ? 'U' : 'I', IS_UNSIGNED(long), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t = { "int32_t", NULL, sizeof(__pyx_t_5numpy_int32_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int32_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int32_t), 0 };
 #define __Pyx_MODULE_NAME "structureboost.structure_gb"
 extern int __pyx_module_is_main_structureboost__structure_gb;
 int __pyx_module_is_main_structureboost__structure_gb = 0;
 
 /* Implementation of 'structureboost.structure_gb' */
 static PyObject *__pyx_builtin_object;
 static PyObject *__pyx_builtin_print;
@@ -2839,15 +2842,14 @@
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_dtm[] = "dtm";
 static const char __pyx_k_eps[] = "eps";
 static const char __pyx_k_exp[] = "exp";
 static const char __pyx_k_fit[] = "fit";
 static const char __pyx_k_i_2[] = "i={}";
 static const char __pyx_k_ind[] = "ind";
-static const char __pyx_k_int[] = "int_";
 static const char __pyx_k_log[] = "log";
 static const char __pyx_k_max[] = "max";
 static const char __pyx_k_mse[] = "mse";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_phi[] = "phi";
 static const char __pyx_k_sum[] = "sum";
@@ -2893,14 +2895,15 @@
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_floor[] = "floor";
 static const char __pyx_k_gamma[] = "gamma";
 static const char __pyx_k_graph[] = "graph";
 static const char __pyx_k_index[] = "index";
+static const char __pyx_k_int32[] = "int32";
 static const char __pyx_k_isnan[] = "isnan";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_nfeat[] = "nfeat";
 static const char __pyx_k_nrows[] = "nrows";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_print[] = "print";
 static const char __pyx_k_range[] = "range";
@@ -3548,15 +3551,15 @@
 static PyObject *__pyx_n_s_index;
 static PyObject *__pyx_n_s_indexes;
 static PyObject *__pyx_n_s_init;
 static PyObject *__pyx_n_s_init_eval_set_info;
 static PyObject *__pyx_n_s_initial_model;
 static PyObject *__pyx_n_s_initial_pred;
 static PyObject *__pyx_n_s_initialize_uv_dict;
-static PyObject *__pyx_n_s_int;
+static PyObject *__pyx_n_s_int32;
 static PyObject *__pyx_n_u_interior;
 static PyObject *__pyx_n_s_inv_cti;
 static PyObject *__pyx_n_s_is_connected;
 static PyObject *__pyx_n_s_isnan;
 static PyObject *__pyx_n_s_isnan_array;
 static PyObject *__pyx_n_s_items;
 static PyObject *__pyx_n_s_itemsize;
@@ -17252,27 +17255,27 @@
     __pyx_t_1 = 0;
 
     /* "structureboost/structure_gb.pyx":746
  *         if self.optimizable:
  *             cat_size = np.max(np.array([dt.get_max_split_size() for dt in self.dec_tree_list]))
  *             num_dt = len(self.dec_tree_list)             # <<<<<<<<<<<<<<
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dec_tree_list); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 746, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_9 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 746, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_num_dt = __pyx_t_9;
 
     /* "structureboost/structure_gb.pyx":747
  *             cat_size = np.max(np.array([dt.get_max_split_size() for dt in self.dec_tree_list]))
  *             num_dt = len(self.dec_tree_list)
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))             # <<<<<<<<<<<<<<
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, 3))
  */
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 747, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_max); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 747, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
@@ -17375,15 +17378,15 @@
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_max_nodes = __pyx_t_1;
     __pyx_t_1 = 0;
 
     /* "structureboost/structure_gb.pyx":748
  *             num_dt = len(self.dec_tree_list)
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1             # <<<<<<<<<<<<<<
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1             # <<<<<<<<<<<<<<
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, 3))
  *             for i in range(num_dt):
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 748, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 748, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
@@ -17408,15 +17411,15 @@
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 748, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 748, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 748, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 748, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 748, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 748, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -17426,15 +17429,15 @@
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int, __pyx_t_5) < 0) __PYX_ERR(0, 748, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
     /* "structureboost/structure_gb.pyx":749
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, 3))             # <<<<<<<<<<<<<<
  *             for i in range(num_dt):
  *                 self.convert_dt_to_matrix(i)
  */
     __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 749, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 749, __pyx_L1_error)
@@ -17469,15 +17472,15 @@
     if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 749, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_float, __pyx_t_5) < 0) __PYX_ERR(0, 749, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
     /* "structureboost/structure_gb.pyx":750
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, 3))
  *             for i in range(num_dt):             # <<<<<<<<<<<<<<
  *                 self.convert_dt_to_matrix(i)
  *             self.optimized=True
  */
     __pyx_t_9 = __pyx_v_num_dt;
     __pyx_t_13 = __pyx_t_9;
@@ -17863,16 +17866,17 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
-  int __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_8;
+  PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__33)
   __Pyx_RefNannySetupContext("convert_subtree", 0);
   __Pyx_TraceCall("convert_subtree", __pyx_f[0], 760, 0, __PYX_ERR(0, 760, __pyx_L1_error));
 
@@ -18098,213 +18102,220 @@
     }
 
     /* "structureboost/structure_gb.pyx":771
  *                 self.pred_tens_float[dt_num, ni, 0] = node['split_val']
  *                 self.pred_tens_int[dt_num, ni, 0]= 1
  *             elif node['feature_type']=='categorical_int':             # <<<<<<<<<<<<<<
  *                 setlen = len(node['left_split'])
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  */
     __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_feature_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 771, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_categorical_int, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 771, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_2) {
 
       /* "structureboost/structure_gb.pyx":772
  *                 self.pred_tens_int[dt_num, ni, 0]= 1
  *             elif node['feature_type']=='categorical_int':
  *                 setlen = len(node['left_split'])             # <<<<<<<<<<<<<<
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  *                 self.pred_tens_int[dt_num, ni, 0]= 2
  */
       __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_split); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 772, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_5 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 772, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 772, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_v_setlen = __pyx_t_1;
       __pyx_t_1 = 0;
 
       /* "structureboost/structure_gb.pyx":773
  *             elif node['feature_type']=='categorical_int':
  *                 setlen = len(node['left_split'])
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)             # <<<<<<<<<<<<<<
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)             # <<<<<<<<<<<<<<
  *                 self.pred_tens_int[dt_num, ni, 0]= 2
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen
  */
       __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 773, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_fromiter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 773, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_split); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 773, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 773, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_int32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 773, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = NULL;
-      __pyx_t_7 = 0;
+      __pyx_t_8 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
-          __pyx_t_7 = 1;
+          __pyx_t_8 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_4)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_3, ((PyObject *)(&PyInt_Type)), __pyx_v_setlen};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 773, __pyx_L1_error)
+        PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_3, __pyx_t_7, __pyx_v_setlen};
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 773, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_3, ((PyObject *)(&PyInt_Type)), __pyx_v_setlen};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 773, __pyx_L1_error)
+        PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_3, __pyx_t_7, __pyx_v_setlen};
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 773, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       {
-        __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 773, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_8);
+        __pyx_t_9 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 773, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_9);
         if (__pyx_t_6) {
-          __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
+          __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_6); __pyx_t_6 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_3);
-        PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
-        __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
-        __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
-        PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, ((PyObject *)(&PyInt_Type)));
+        PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_3);
+        __Pyx_GIVEREF(__pyx_t_7);
+        PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_t_7);
         __Pyx_INCREF(__pyx_v_setlen);
         __Pyx_GIVEREF(__pyx_v_setlen);
-        PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_7, __pyx_v_setlen);
+        PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_v_setlen);
         __pyx_t_3 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 773, __pyx_L1_error)
+        __pyx_t_7 = 0;
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 773, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 773, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_8 = __Pyx_PyInt_AddCObj(__pyx_int_6, __pyx_v_setlen, 6, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 773, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_3 = PySlice_New(__pyx_int_6, __pyx_t_8, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 773, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 773, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_9 = __Pyx_PyInt_AddCObj(__pyx_int_6, __pyx_v_setlen, 6, 0, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 773, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __pyx_t_7 = PySlice_New(__pyx_int_6, __pyx_t_9, Py_None); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 773, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 773, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
-      PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_dt_num);
+      PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_dt_num);
       __Pyx_INCREF(__pyx_v_ni);
       __Pyx_GIVEREF(__pyx_v_ni);
-      PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_ni);
-      __Pyx_GIVEREF(__pyx_t_3);
-      PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_3);
-      __pyx_t_3 = 0;
-      if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_8, __pyx_t_1) < 0)) __PYX_ERR(0, 773, __pyx_L1_error)
+      PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_ni);
+      __Pyx_GIVEREF(__pyx_t_7);
+      PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_t_7);
+      __pyx_t_7 = 0;
+      if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_9, __pyx_t_1) < 0)) __PYX_ERR(0, 773, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
       /* "structureboost/structure_gb.pyx":774
  *                 setlen = len(node['left_split'])
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  *                 self.pred_tens_int[dt_num, ni, 0]= 2             # <<<<<<<<<<<<<<
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]
  */
       __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 774, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 774, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 774, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
-      PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_dt_num);
+      PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_dt_num);
       __Pyx_INCREF(__pyx_v_ni);
       __Pyx_GIVEREF(__pyx_v_ni);
-      PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_ni);
+      PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_ni);
       __Pyx_INCREF(__pyx_int_0);
       __Pyx_GIVEREF(__pyx_int_0);
-      PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_int_0);
-      if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_8, __pyx_int_2) < 0)) __PYX_ERR(0, 774, __pyx_L1_error)
+      PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_int_0);
+      if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_9, __pyx_int_2) < 0)) __PYX_ERR(0, 774, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
       /* "structureboost/structure_gb.pyx":775
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  *                 self.pred_tens_int[dt_num, ni, 0]= 2
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen             # <<<<<<<<<<<<<<
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']
  */
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 775, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 775, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 775, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
       PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_dt_num);
       __Pyx_INCREF(__pyx_v_ni);
       __Pyx_GIVEREF(__pyx_v_ni);
       PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_ni);
       __Pyx_INCREF(__pyx_int_5);
       __Pyx_GIVEREF(__pyx_int_5);
       PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_int_5);
-      if (unlikely(PyObject_SetItem(__pyx_t_8, __pyx_t_1, __pyx_v_setlen) < 0)) __PYX_ERR(0, 775, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      if (unlikely(PyObject_SetItem(__pyx_t_9, __pyx_t_1, __pyx_v_setlen) < 0)) __PYX_ERR(0, 775, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
       /* "structureboost/structure_gb.pyx":771
  *                 self.pred_tens_float[dt_num, ni, 0] = node['split_val']
  *                 self.pred_tens_int[dt_num, ni, 0]= 1
  *             elif node['feature_type']=='categorical_int':             # <<<<<<<<<<<<<<
  *                 setlen = len(node['left_split'])
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  */
     }
     __pyx_L4:;
 
     /* "structureboost/structure_gb.pyx":776
  *                 self.pred_tens_int[dt_num, ni, 0]= 2
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]             # <<<<<<<<<<<<<<
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 3]=node['right_child']['node_index']
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_column_to_int_dict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_split_feature); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 776, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 776, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_split_feature); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 776, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 776, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 776, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 776, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_dt_num);
     __Pyx_GIVEREF(__pyx_v_dt_num);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_dt_num);
     __Pyx_INCREF(__pyx_v_ni);
     __Pyx_GIVEREF(__pyx_v_ni);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_ni);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_int_1);
-    if (unlikely(PyObject_SetItem(__pyx_t_8, __pyx_t_1, __pyx_t_4) < 0)) __PYX_ERR(0, 776, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (unlikely(PyObject_SetItem(__pyx_t_9, __pyx_t_1, __pyx_t_4) < 0)) __PYX_ERR(0, 776, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "structureboost/structure_gb.pyx":777
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']             # <<<<<<<<<<<<<<
@@ -18314,206 +18325,206 @@
     __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_child); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 777, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_n_u_node_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 777, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 777, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 777, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 777, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_INCREF(__pyx_v_dt_num);
     __Pyx_GIVEREF(__pyx_v_dt_num);
-    PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_dt_num);
+    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_dt_num);
     __Pyx_INCREF(__pyx_v_ni);
     __Pyx_GIVEREF(__pyx_v_ni);
-    PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_ni);
+    PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_ni);
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_GIVEREF(__pyx_int_2);
-    PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_int_2);
-    if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_8, __pyx_t_1) < 0)) __PYX_ERR(0, 777, __pyx_L1_error)
+    PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_int_2);
+    if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_9, __pyx_t_1) < 0)) __PYX_ERR(0, 777, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "structureboost/structure_gb.pyx":778
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 3]=node['right_child']['node_index']             # <<<<<<<<<<<<<<
  *             self.pred_tens_int[dt_num, ni, 4]=node['na_left']
  *             self.convert_subtree(node['left_child'], dt_num)
  */
     __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_right_child); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 778, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_node_index); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 778, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_node_index); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 778, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 778, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 778, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_dt_num);
     __Pyx_GIVEREF(__pyx_v_dt_num);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_dt_num);
     __Pyx_INCREF(__pyx_v_ni);
     __Pyx_GIVEREF(__pyx_v_ni);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_ni);
     __Pyx_INCREF(__pyx_int_3);
     __Pyx_GIVEREF(__pyx_int_3);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_int_3);
-    if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_4, __pyx_t_8) < 0)) __PYX_ERR(0, 778, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_4, __pyx_t_9) < 0)) __PYX_ERR(0, 778, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
     /* "structureboost/structure_gb.pyx":779
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 3]=node['right_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 4]=node['na_left']             # <<<<<<<<<<<<<<
  *             self.convert_subtree(node['left_child'], dt_num)
  *             self.convert_subtree(node['right_child'], dt_num)
  */
-    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_na_left); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 779, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_na_left); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 779, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_dt_num);
     __Pyx_GIVEREF(__pyx_v_dt_num);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_dt_num);
     __Pyx_INCREF(__pyx_v_ni);
     __Pyx_GIVEREF(__pyx_v_ni);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_ni);
     __Pyx_INCREF(__pyx_int_4);
     __Pyx_GIVEREF(__pyx_int_4);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_int_4);
-    if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_1, __pyx_t_8) < 0)) __PYX_ERR(0, 779, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_1, __pyx_t_9) < 0)) __PYX_ERR(0, 779, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
     /* "structureboost/structure_gb.pyx":780
  *             self.pred_tens_int[dt_num, ni, 3]=node['right_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 4]=node['na_left']
  *             self.convert_subtree(node['left_child'], dt_num)             # <<<<<<<<<<<<<<
  *             self.convert_subtree(node['right_child'], dt_num)
  * 
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_convert_subtree); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 780, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_child); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 780, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = NULL;
-    __pyx_t_7 = 0;
+    __pyx_t_7 = NULL;
+    __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_3)) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
-        __pyx_t_7 = 1;
+        __pyx_t_8 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_4, __pyx_v_dt_num};
-      __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 780, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
+      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_4, __pyx_v_dt_num};
+      __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 780, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_4, __pyx_v_dt_num};
-      __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 780, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
+      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_4, __pyx_v_dt_num};
+      __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 780, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     {
-      __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 780, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      if (__pyx_t_3) {
-        __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3); __pyx_t_3 = NULL;
+      __pyx_t_3 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 780, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      if (__pyx_t_7) {
+        __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_7); __pyx_t_7 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
-      PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_7, __pyx_t_4);
+      PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_8, __pyx_t_4);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
-      PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_7, __pyx_v_dt_num);
+      PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_8, __pyx_v_dt_num);
       __pyx_t_4 = 0;
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 780, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 780, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
     /* "structureboost/structure_gb.pyx":781
  *             self.pred_tens_int[dt_num, ni, 4]=node['na_left']
  *             self.convert_subtree(node['left_child'], dt_num)
  *             self.convert_subtree(node['right_child'], dt_num)             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_convert_subtree); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 781, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_right_child); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 781, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_right_child); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 781, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
-    __pyx_t_7 = 0;
+    __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
-        __pyx_t_7 = 1;
+        __pyx_t_8 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_6, __pyx_v_dt_num};
-      __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 781, __pyx_L1_error)
+      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_3, __pyx_v_dt_num};
+      __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 781, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_6, __pyx_v_dt_num};
-      __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 781, __pyx_L1_error)
+      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_3, __pyx_v_dt_num};
+      __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 781, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else
     #endif
     {
-      __pyx_t_3 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 781, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_7 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 781, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       if (__pyx_t_4) {
-        __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4); __pyx_t_4 = NULL;
+        __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
-      __Pyx_GIVEREF(__pyx_t_6);
-      PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_7, __pyx_t_6);
+      __Pyx_GIVEREF(__pyx_t_3);
+      PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_8, __pyx_t_3);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
-      PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_7, __pyx_v_dt_num);
-      __pyx_t_6 = 0;
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 781, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_8, __pyx_v_dt_num);
+      __pyx_t_3 = 0;
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 781, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __pyx_L3:;
 
   /* "structureboost/structure_gb.pyx":760
  *         self.convert_subtree(curr_node, dt_num)
  * 
  *     def convert_subtree(self, node, dt_num):             # <<<<<<<<<<<<<<
@@ -18525,15 +18536,16 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("structureboost.structure_gb.StructureBoost.convert_subtree", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ni);
   __Pyx_XDECREF(__pyx_v_setlen);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
@@ -21049,15 +21061,15 @@
   return __pyx_r;
 }
 
 /* "structureboost/structure_gb.pyx":877
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[long, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_12structure_gb_21predict_with_tensor_c(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_12structure_gb_21predict_with_tensor_c = {"predict_with_tensor_c", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_12structure_gb_21predict_with_tensor_c, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_12structure_gb_21predict_with_tensor_c(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -21193,15 +21205,15 @@
   long __pyx_t_13;
   int __pyx_t_14;
   Py_ssize_t __pyx_t_15;
   Py_ssize_t __pyx_t_16;
   Py_ssize_t __pyx_t_17;
   Py_ssize_t __pyx_t_18;
   Py_ssize_t __pyx_t_19;
-  long __pyx_t_20;
+  __pyx_t_5numpy_int32_t __pyx_t_20;
   Py_ssize_t __pyx_t_21;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__44)
   __Pyx_RefNannySetupContext("predict_with_tensor_c", 0);
   __Pyx_TraceCall("predict_with_tensor_c", __pyx_f[0], 877, 0, __PYX_ERR(0, 877, __pyx_L1_error));
@@ -21228,15 +21240,15 @@
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm_float.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm_float, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 877, __pyx_L1_error)
   }
   __pyx_pybuffernd_dtm_float.diminfo[0].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_dtm_float.diminfo[0].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_dtm_float.diminfo[1].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_dtm_float.diminfo[1].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_dtm_float.diminfo[2].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_dtm_float.diminfo[2].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[2];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 877, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 877, __pyx_L1_error)
   }
   __pyx_pybuffernd_dtm.diminfo[0].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_dtm.diminfo[0].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_dtm.diminfo[1].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_dtm.diminfo[1].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_dtm.diminfo[2].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_dtm.diminfo[2].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[2];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feat_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_feat_array, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 877, __pyx_L1_error)
   }
   __pyx_pybuffernd_feat_array.diminfo[0].strides = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_feat_array.diminfo[0].shape = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_feat_array.diminfo[1].strides = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_feat_array.diminfo[1].shape = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.shape[1];
@@ -21294,15 +21306,15 @@
   __pyx_t_6 = 0;
   __pyx_v_res_mat = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb.pyx":886
  *     cdef double curr_val, ind_doub
  *     cdef bint at_leaf, found_val
- *     cdef np.ndarray[long, ndim=2] isnan_array = np.isnan(feat_array).astype(int)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.int32_t, ndim=2] isnan_array = np.isnan(feat_array).astype(np.int32)             # <<<<<<<<<<<<<<
  * 
  *     # These are in dtm_float
  */
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 886, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_isnan); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 886, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
@@ -21321,34 +21333,40 @@
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 886, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 886, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 886, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 886, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, ((PyObject *)(&PyInt_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_4, ((PyObject *)(&PyInt_Type)));
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 886, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 886, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_isnan_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_isnan_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_isnan_array = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 886, __pyx_L1_error)
     } else {__pyx_pybuffernd_isnan_array.diminfo[0].strides = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_isnan_array.diminfo[0].shape = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_isnan_array.diminfo[1].strides = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_isnan_array.diminfo[1].shape = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_isnan_array = ((PyArrayObject *)__pyx_t_1);
@@ -21530,15 +21548,15 @@
  *                 if dtm[k,cn, NODE_TYPE]==LEAF:             # <<<<<<<<<<<<<<
  *                     at_leaf = 1
  *                     res_mat[ri,k] = dtm_float[k,cn, NODE_VALUE]
  */
         __pyx_t_15 = __pyx_v_k;
         __pyx_t_16 = __pyx_v_cn;
         __pyx_t_17 = __pyx_v_NODE_TYPE;
-        __pyx_t_14 = (((*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_LEAF) != 0);
+        __pyx_t_14 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_LEAF) != 0);
         if (__pyx_t_14) {
 
           /* "structureboost/structure_gb.pyx":914
  *                 cn = int(cn)
  *                 if dtm[k,cn, NODE_TYPE]==LEAF:
  *                     at_leaf = 1             # <<<<<<<<<<<<<<
  *                     res_mat[ri,k] = dtm_float[k,cn, NODE_VALUE]
@@ -21576,61 +21594,61 @@
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:             # <<<<<<<<<<<<<<
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:
  */
         __pyx_t_15 = __pyx_v_k;
         __pyx_t_16 = __pyx_v_cn;
         __pyx_t_17 = __pyx_v_NODE_TYPE;
-        __pyx_t_14 = (((*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_NUMER) != 0);
+        __pyx_t_14 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_NUMER) != 0);
         if (__pyx_t_14) {
 
           /* "structureboost/structure_gb.pyx":917
  *                     res_mat[ri,k] = dtm_float[k,cn, NODE_VALUE]
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]             # <<<<<<<<<<<<<<
  *                     if isnan_array[ri,ind]:
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]
  */
           __pyx_t_17 = __pyx_v_k;
           __pyx_t_16 = __pyx_v_cn;
           __pyx_t_15 = __pyx_v_FEATURE_COL;
-          __pyx_v_ind = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides));
+          __pyx_v_ind = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides));
 
           /* "structureboost/structure_gb.pyx":918
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:             # <<<<<<<<<<<<<<
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]
  *                     else:
  */
           __pyx_t_15 = __pyx_v_ri;
           __pyx_t_16 = __pyx_v_ind;
-          __pyx_t_14 = ((*__Pyx_BufPtrStrided2d(long *, __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_isnan_array.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_isnan_array.diminfo[1].strides)) != 0);
+          __pyx_t_14 = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_isnan_array.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_isnan_array.diminfo[1].strides)) != 0);
           if (__pyx_t_14) {
 
             /* "structureboost/structure_gb.pyx":919
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]             # <<<<<<<<<<<<<<
  *                     else:
  *                         curr_val = feat_array[ri,ind]
  */
             __pyx_t_16 = __pyx_v_k;
             __pyx_t_15 = __pyx_v_cn;
             __pyx_t_17 = __pyx_v_NA_LEFT;
-            if (((*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides)) != 0)) {
+            if (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides)) != 0)) {
               __pyx_t_19 = __pyx_v_k;
               __pyx_t_18 = __pyx_v_cn;
               __pyx_t_21 = __pyx_v_LEFT_CHILD;
-              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[2].strides));
             } else {
               __pyx_t_21 = __pyx_v_k;
               __pyx_t_18 = __pyx_v_cn;
               __pyx_t_19 = __pyx_v_RIGHT_CHILD;
-              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[2].strides));
             }
             __pyx_v_cn = __pyx_t_20;
 
             /* "structureboost/structure_gb.pyx":918
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:             # <<<<<<<<<<<<<<
@@ -21662,20 +21680,20 @@
             __pyx_t_15 = __pyx_v_k;
             __pyx_t_17 = __pyx_v_cn;
             __pyx_t_16 = __pyx_v_THRESH;
             if (((__pyx_v_curr_val < (*__Pyx_BufPtrStrided3d(double *, __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm_float.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm_float.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm_float.diminfo[2].strides))) != 0)) {
               __pyx_t_19 = __pyx_v_k;
               __pyx_t_18 = __pyx_v_cn;
               __pyx_t_21 = __pyx_v_LEFT_CHILD;
-              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[2].strides));
             } else {
               __pyx_t_21 = __pyx_v_k;
               __pyx_t_18 = __pyx_v_cn;
               __pyx_t_19 = __pyx_v_RIGHT_CHILD;
-              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[2].strides));
             }
             __pyx_v_cn = __pyx_t_20;
           }
           __pyx_L10:;
 
           /* "structureboost/structure_gb.pyx":916
  *                     at_leaf = 1
@@ -21693,29 +21711,29 @@
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:             # <<<<<<<<<<<<<<
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]
  *                     found_val = 0
  */
         __pyx_t_16 = __pyx_v_k;
         __pyx_t_17 = __pyx_v_cn;
         __pyx_t_15 = __pyx_v_NODE_TYPE;
-        __pyx_t_14 = (((*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_CATEG) != 0);
+        __pyx_t_14 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_CATEG) != 0);
         if (__pyx_t_14) {
 
           /* "structureboost/structure_gb.pyx":924
  *                         cn = dtm[k,cn, LEFT_CHILD] if curr_val<dtm_float[k,cn, THRESH] else dtm[k,cn, RIGHT_CHILD]
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]             # <<<<<<<<<<<<<<
  *                     found_val = 0
  *                     j = CAT_VALS_START
  */
           __pyx_t_15 = __pyx_v_k;
           __pyx_t_17 = __pyx_v_cn;
           __pyx_t_16 = __pyx_v_FEATURE_COL;
           __pyx_t_19 = __pyx_v_ri;
-          __pyx_t_18 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
+          __pyx_t_18 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
           __pyx_v_curr_val = (*__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_feat_array.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_feat_array.diminfo[1].strides));
 
           /* "structureboost/structure_gb.pyx":925
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]
  *                     found_val = 0             # <<<<<<<<<<<<<<
  *                     j = CAT_VALS_START
@@ -21738,15 +21756,15 @@
  *                     cat_vals_end = CAT_VALS_START + dtm[k, cn, NUM_CAT_VALS]             # <<<<<<<<<<<<<<
  *                     while ((not found_val) & (j<cat_vals_end)):
  *                         if curr_val==dtm[k,cn, j]:
  */
           __pyx_t_16 = __pyx_v_k;
           __pyx_t_17 = __pyx_v_cn;
           __pyx_t_15 = __pyx_v_NUM_CAT_VALS;
-          __pyx_v_cat_vals_end = (__pyx_v_CAT_VALS_START + (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides)));
+          __pyx_v_cat_vals_end = (__pyx_v_CAT_VALS_START + (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides)));
 
           /* "structureboost/structure_gb.pyx":928
  *                     j = CAT_VALS_START
  *                     cat_vals_end = CAT_VALS_START + dtm[k, cn, NUM_CAT_VALS]
  *                     while ((not found_val) & (j<cat_vals_end)):             # <<<<<<<<<<<<<<
  *                         if curr_val==dtm[k,cn, j]:
  *                             found_val=1
@@ -21761,15 +21779,15 @@
  *                         if curr_val==dtm[k,cn, j]:             # <<<<<<<<<<<<<<
  *                             found_val=1
  *                         else:
  */
             __pyx_t_15 = __pyx_v_k;
             __pyx_t_17 = __pyx_v_cn;
             __pyx_t_16 = __pyx_v_j;
-            __pyx_t_14 = ((__pyx_v_curr_val == (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides))) != 0);
+            __pyx_t_14 = ((__pyx_v_curr_val == (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides))) != 0);
             if (__pyx_t_14) {
 
               /* "structureboost/structure_gb.pyx":930
  *                     while ((not found_val) & (j<cat_vals_end)):
  *                         if curr_val==dtm[k,cn, j]:
  *                             found_val=1             # <<<<<<<<<<<<<<
  *                         else:
@@ -21807,20 +21825,20 @@
  *     return(res_mat)
  * 
  */
           if ((__pyx_v_found_val != 0)) {
             __pyx_t_16 = __pyx_v_k;
             __pyx_t_17 = __pyx_v_cn;
             __pyx_t_15 = __pyx_v_LEFT_CHILD;
-            __pyx_t_20 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides));
+            __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides));
           } else {
             __pyx_t_15 = __pyx_v_k;
             __pyx_t_17 = __pyx_v_cn;
             __pyx_t_16 = __pyx_v_RIGHT_CHILD;
-            __pyx_t_20 = (*__Pyx_BufPtrStrided3d(long *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
+            __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
           }
           __pyx_v_cn = __pyx_t_20;
 
           /* "structureboost/structure_gb.pyx":923
  *                         curr_val = feat_array[ri,ind]
  *                         cn = dtm[k,cn, LEFT_CHILD] if curr_val<dtm_float[k,cn, THRESH] else dtm[k,cn, RIGHT_CHILD]
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:             # <<<<<<<<<<<<<<
@@ -21845,15 +21863,15 @@
   __pyx_r = ((PyObject *)__pyx_v_res_mat);
   goto __pyx_L0;
 
   /* "structureboost/structure_gb.pyx":877
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[long, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -21887,15 +21905,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "structureboost/structure_gb.pyx":946
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * @cython.cdivision(True)
- * cdef extend_path(np.ndarray[long] feature_indexes,             # <<<<<<<<<<<<<<
+ * cdef extend_path(np.ndarray[np.int32_t] feature_indexes,             # <<<<<<<<<<<<<<
  *                 np.ndarray[double] zero_fractions,
  *                 np.ndarray[double] one_fractions,
  */
 
 static PyObject *__pyx_f_14structureboost_12structure_gb_extend_path(PyArrayObject *__pyx_v_feature_indexes, PyArrayObject *__pyx_v_zero_fractions, PyArrayObject *__pyx_v_one_fractions, PyArrayObject *__pyx_v_pweights, long __pyx_v_unique_depth, double __pyx_v_zero_fraction, double __pyx_v_one_fraction, long __pyx_v_feature_index) {
   long __pyx_v_i;
   __Pyx_LocalBuf_ND __pyx_pybuffernd_feature_indexes;
@@ -21932,15 +21950,15 @@
   __pyx_pybuffernd_one_fractions.rcbuffer = &__pyx_pybuffer_one_fractions;
   __pyx_pybuffer_pweights.pybuffer.buf = NULL;
   __pyx_pybuffer_pweights.refcount = 0;
   __pyx_pybuffernd_pweights.data = NULL;
   __pyx_pybuffernd_pweights.rcbuffer = &__pyx_pybuffer_pweights;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer, (PyObject*)__pyx_v_feature_indexes, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 946, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer, (PyObject*)__pyx_v_feature_indexes, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 946, __pyx_L1_error)
   }
   __pyx_pybuffernd_feature_indexes.diminfo[0].strides = __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_feature_indexes.diminfo[0].shape = __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zero_fractions.rcbuffer->pybuffer, (PyObject*)__pyx_v_zero_fractions, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 946, __pyx_L1_error)
   }
   __pyx_pybuffernd_zero_fractions.diminfo[0].strides = __pyx_pybuffernd_zero_fractions.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_zero_fractions.diminfo[0].shape = __pyx_pybuffernd_zero_fractions.rcbuffer->pybuffer.shape[0];
@@ -21959,15 +21977,15 @@
  *     cdef long i
  * 
  *     feature_indexes[unique_depth] = feature_index             # <<<<<<<<<<<<<<
  *     zero_fractions[unique_depth] = zero_fraction
  *     one_fractions[unique_depth] = one_fraction
  */
   __pyx_t_1 = __pyx_v_unique_depth;
-  *__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_feature_indexes.diminfo[0].strides) = __pyx_v_feature_index;
+  *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_feature_indexes.diminfo[0].strides) = __pyx_v_feature_index;
 
   /* "structureboost/structure_gb.pyx":956
  * 
  *     feature_indexes[unique_depth] = feature_index
  *     zero_fractions[unique_depth] = zero_fraction             # <<<<<<<<<<<<<<
  *     one_fractions[unique_depth] = one_fraction
  *     if unique_depth == 0:
@@ -22060,15 +22078,15 @@
     __pyx_t_4 = __pyx_v_i;
     *__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_pweights.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_pweights.diminfo[0].strides) = (((__pyx_v_zero_fraction * (*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_pweights.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_pweights.diminfo[0].strides))) * (__pyx_v_unique_depth - __pyx_v_i)) / ((double)(__pyx_v_unique_depth + 1)));
   }
 
   /* "structureboost/structure_gb.pyx":946
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * @cython.cdivision(True)
- * cdef extend_path(np.ndarray[long] feature_indexes,             # <<<<<<<<<<<<<<
+ * cdef extend_path(np.ndarray[np.int32_t] feature_indexes,             # <<<<<<<<<<<<<<
  *                 np.ndarray[double] zero_fractions,
  *                 np.ndarray[double] one_fractions,
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
@@ -22096,15 +22114,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "structureboost/structure_gb.pyx":972
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * @cython.cdivision(True)
- * cdef unwind_path(np.ndarray[long] feature_indexes,             # <<<<<<<<<<<<<<
+ * cdef unwind_path(np.ndarray[np.int32_t] feature_indexes,             # <<<<<<<<<<<<<<
  *                 np.ndarray[double] zero_fractions,
  *                 np.ndarray[double] one_fractions,
  */
 
 static PyObject *__pyx_f_14structureboost_12structure_gb_unwind_path(PyArrayObject *__pyx_v_feature_indexes, PyArrayObject *__pyx_v_zero_fractions, PyArrayObject *__pyx_v_one_fractions, PyArrayObject *__pyx_v_pweights, long __pyx_v_unique_depth, long __pyx_v_path_index) {
   double __pyx_v_one_fraction;
   double __pyx_v_zero_fraction;
@@ -22147,15 +22165,15 @@
   __pyx_pybuffernd_one_fractions.rcbuffer = &__pyx_pybuffer_one_fractions;
   __pyx_pybuffer_pweights.pybuffer.buf = NULL;
   __pyx_pybuffer_pweights.refcount = 0;
   __pyx_pybuffernd_pweights.data = NULL;
   __pyx_pybuffernd_pweights.rcbuffer = &__pyx_pybuffer_pweights;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer, (PyObject*)__pyx_v_feature_indexes, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 972, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer, (PyObject*)__pyx_v_feature_indexes, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 972, __pyx_L1_error)
   }
   __pyx_pybuffernd_feature_indexes.diminfo[0].strides = __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_feature_indexes.diminfo[0].shape = __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zero_fractions.rcbuffer->pybuffer, (PyObject*)__pyx_v_zero_fractions, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 972, __pyx_L1_error)
   }
   __pyx_pybuffernd_zero_fractions.diminfo[0].strides = __pyx_pybuffernd_zero_fractions.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_zero_fractions.diminfo[0].shape = __pyx_pybuffernd_zero_fractions.rcbuffer->pybuffer.shape[0];
@@ -22292,15 +22310,15 @@
  *     for i in range(path_index, unique_depth):
  *         feature_indexes[i] = feature_indexes[i+1]             # <<<<<<<<<<<<<<
  *         zero_fractions[i] = zero_fractions[i+1]
  *         one_fractions[i] = one_fractions[i+1]
  */
     __pyx_t_1 = (__pyx_v_i + 1);
     __pyx_t_4 = __pyx_v_i;
-    *__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_feature_indexes.diminfo[0].strides) = (*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_feature_indexes.diminfo[0].strides));
+    *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_feature_indexes.diminfo[0].strides) = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_feature_indexes.diminfo[0].strides));
 
     /* "structureboost/structure_gb.pyx":995
  *     for i in range(path_index, unique_depth):
  *         feature_indexes[i] = feature_indexes[i+1]
  *         zero_fractions[i] = zero_fractions[i+1]             # <<<<<<<<<<<<<<
  *         one_fractions[i] = one_fractions[i+1]
  * 
@@ -22320,15 +22338,15 @@
     __pyx_t_4 = __pyx_v_i;
     *__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_one_fractions.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_one_fractions.diminfo[0].strides) = (*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_one_fractions.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_one_fractions.diminfo[0].strides));
   }
 
   /* "structureboost/structure_gb.pyx":972
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * @cython.cdivision(True)
- * cdef unwind_path(np.ndarray[long] feature_indexes,             # <<<<<<<<<<<<<<
+ * cdef unwind_path(np.ndarray[np.int32_t] feature_indexes,             # <<<<<<<<<<<<<<
  *                 np.ndarray[double] zero_fractions,
  *                 np.ndarray[double] one_fractions,
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
@@ -22356,15 +22374,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "structureboost/structure_gb.pyx":1002
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * cdef double unwound_path_sum(np.ndarray[long] feature_indexes,             # <<<<<<<<<<<<<<
+ * cdef double unwound_path_sum(np.ndarray[np.int32_t] feature_indexes,             # <<<<<<<<<<<<<<
  *                      np.ndarray[double] zero_fractions,
  *                      np.ndarray[double] one_fractions,
  */
 
 static double __pyx_f_14structureboost_12structure_gb_unwound_path_sum(CYTHON_UNUSED PyArrayObject *__pyx_v_feature_indexes, PyArrayObject *__pyx_v_zero_fractions, PyArrayObject *__pyx_v_one_fractions, PyArrayObject *__pyx_v_pweights, long __pyx_v_unique_depth, long __pyx_v_path_index) {
   double __pyx_v_one_fraction;
   double __pyx_v_zero_fraction;
@@ -22410,15 +22428,15 @@
   __pyx_pybuffernd_one_fractions.rcbuffer = &__pyx_pybuffer_one_fractions;
   __pyx_pybuffer_pweights.pybuffer.buf = NULL;
   __pyx_pybuffer_pweights.refcount = 0;
   __pyx_pybuffernd_pweights.data = NULL;
   __pyx_pybuffernd_pweights.rcbuffer = &__pyx_pybuffer_pweights;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer, (PyObject*)__pyx_v_feature_indexes, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1002, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer, (PyObject*)__pyx_v_feature_indexes, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1002, __pyx_L1_error)
   }
   __pyx_pybuffernd_feature_indexes.diminfo[0].strides = __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_feature_indexes.diminfo[0].shape = __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zero_fractions.rcbuffer->pybuffer, (PyObject*)__pyx_v_zero_fractions, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1002, __pyx_L1_error)
   }
   __pyx_pybuffernd_zero_fractions.diminfo[0].strides = __pyx_pybuffernd_zero_fractions.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_zero_fractions.diminfo[0].shape = __pyx_pybuffernd_zero_fractions.rcbuffer->pybuffer.shape[0];
@@ -22616,15 +22634,15 @@
  */
   __pyx_r = __pyx_v_total;
   goto __pyx_L0;
 
   /* "structureboost/structure_gb.pyx":1002
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * cdef double unwound_path_sum(np.ndarray[long] feature_indexes,             # <<<<<<<<<<<<<<
+ * cdef double unwound_path_sum(np.ndarray[np.int32_t] feature_indexes,             # <<<<<<<<<<<<<<
  *                      np.ndarray[double] zero_fractions,
  *                      np.ndarray[double] one_fractions,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_8);
@@ -22648,17 +22666,17 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "structureboost/structure_gb.pyx":1032
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * @cython.cdivision(True)
- * cdef tree_shap_recursive(np.ndarray[long] children_left,             # <<<<<<<<<<<<<<
- *                         np.ndarray[long] children_right,
- *                         np.ndarray[long] children_default,
+ * cdef tree_shap_recursive(np.ndarray[np.int32_t] children_left,             # <<<<<<<<<<<<<<
+ *                         np.ndarray[np.int32_t] children_right,
+ *                         np.ndarray[np.int32_t] children_default,
  */
 
 static PyObject *__pyx_f_14structureboost_12structure_gb_tree_shap_recursive(PyArrayObject *__pyx_v_children_left, PyArrayObject *__pyx_v_children_right, PyArrayObject *__pyx_v_children_default, PyArrayObject *__pyx_v_features, PyArrayObject *__pyx_v_node_type_vec, PyArrayObject *__pyx_v_num_cat_vals_vec, PyArrayObject *__pyx_v_cat_vals_mat, PyArrayObject *__pyx_v_thresholds, PyArrayObject *__pyx_v_values, PyArrayObject *__pyx_v_node_sample_weight, PyArrayObject *__pyx_v_x, PyArrayObject *__pyx_v_x_missing, PyArrayObject *__pyx_v_phi, long __pyx_v_node_index, long __pyx_v_unique_depth, PyArrayObject *__pyx_v_parent_feature_indexes, PyArrayObject *__pyx_v_parent_zero_fractions, PyArrayObject *__pyx_v_parent_one_fractions, PyArrayObject *__pyx_v_parent_pweights, double __pyx_v_parent_zero_fraction, double __pyx_v_parent_one_fraction, long __pyx_v_parent_feature_index, long __pyx_v_condition, long __pyx_v_condition_feature, double __pyx_v_condition_fraction) {
   long __pyx_v_pfi_len;
   PyArrayObject *__pyx_v_feature_indexes = 0;
   PyArrayObject *__pyx_v_zero_fractions = 0;
   PyArrayObject *__pyx_v_one_fractions = 0;
@@ -22740,14 +22758,16 @@
   long __pyx_t_14;
   Py_ssize_t __pyx_t_15;
   Py_ssize_t __pyx_t_16;
   int __pyx_t_17;
   Py_ssize_t __pyx_t_18;
   Py_ssize_t __pyx_t_19;
   Py_ssize_t __pyx_t_20;
+  __pyx_t_5numpy_int32_t __pyx_t_21;
+  __pyx_t_5numpy_int32_t __pyx_t_22;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("tree_shap_recursive", 0);
   __Pyx_TraceCall("tree_shap_recursive", __pyx_f[0], 1032, 0, __PYX_ERR(0, 1032, __pyx_L1_error));
   __pyx_pybuffer_feature_indexes.pybuffer.buf = NULL;
   __pyx_pybuffer_feature_indexes.refcount = 0;
@@ -22831,45 +22851,45 @@
   __pyx_pybuffernd_parent_one_fractions.rcbuffer = &__pyx_pybuffer_parent_one_fractions;
   __pyx_pybuffer_parent_pweights.pybuffer.buf = NULL;
   __pyx_pybuffer_parent_pweights.refcount = 0;
   __pyx_pybuffernd_parent_pweights.data = NULL;
   __pyx_pybuffernd_parent_pweights.rcbuffer = &__pyx_pybuffer_parent_pweights;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_children_left.rcbuffer->pybuffer, (PyObject*)__pyx_v_children_left, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_children_left.rcbuffer->pybuffer, (PyObject*)__pyx_v_children_left, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
   }
   __pyx_pybuffernd_children_left.diminfo[0].strides = __pyx_pybuffernd_children_left.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_children_left.diminfo[0].shape = __pyx_pybuffernd_children_left.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_children_right.rcbuffer->pybuffer, (PyObject*)__pyx_v_children_right, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_children_right.rcbuffer->pybuffer, (PyObject*)__pyx_v_children_right, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
   }
   __pyx_pybuffernd_children_right.diminfo[0].strides = __pyx_pybuffernd_children_right.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_children_right.diminfo[0].shape = __pyx_pybuffernd_children_right.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_children_default.rcbuffer->pybuffer, (PyObject*)__pyx_v_children_default, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_children_default.rcbuffer->pybuffer, (PyObject*)__pyx_v_children_default, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
   }
   __pyx_pybuffernd_children_default.diminfo[0].strides = __pyx_pybuffernd_children_default.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_children_default.diminfo[0].shape = __pyx_pybuffernd_children_default.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_features.rcbuffer->pybuffer, (PyObject*)__pyx_v_features, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_features.rcbuffer->pybuffer, (PyObject*)__pyx_v_features, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
   }
   __pyx_pybuffernd_features.diminfo[0].strides = __pyx_pybuffernd_features.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_features.diminfo[0].shape = __pyx_pybuffernd_features.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_node_type_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_node_type_vec, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_node_type_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_node_type_vec, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
   }
   __pyx_pybuffernd_node_type_vec.diminfo[0].strides = __pyx_pybuffernd_node_type_vec.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_node_type_vec.diminfo[0].shape = __pyx_pybuffernd_node_type_vec.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_num_cat_vals_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_num_cat_vals_vec, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_num_cat_vals_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_num_cat_vals_vec, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
   }
   __pyx_pybuffernd_num_cat_vals_vec.diminfo[0].strides = __pyx_pybuffernd_num_cat_vals_vec.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_num_cat_vals_vec.diminfo[0].shape = __pyx_pybuffernd_num_cat_vals_vec.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cat_vals_mat.rcbuffer->pybuffer, (PyObject*)__pyx_v_cat_vals_mat, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_cat_vals_mat.rcbuffer->pybuffer, (PyObject*)__pyx_v_cat_vals_mat, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
   }
   __pyx_pybuffernd_cat_vals_mat.diminfo[0].strides = __pyx_pybuffernd_cat_vals_mat.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_cat_vals_mat.diminfo[0].shape = __pyx_pybuffernd_cat_vals_mat.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_cat_vals_mat.diminfo[1].strides = __pyx_pybuffernd_cat_vals_mat.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_cat_vals_mat.diminfo[1].shape = __pyx_pybuffernd_cat_vals_mat.rcbuffer->pybuffer.shape[1];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_thresholds.rcbuffer->pybuffer, (PyObject*)__pyx_v_thresholds, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
   }
   __pyx_pybuffernd_thresholds.diminfo[0].strides = __pyx_pybuffernd_thresholds.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_thresholds.diminfo[0].shape = __pyx_pybuffernd_thresholds.rcbuffer->pybuffer.shape[0];
@@ -22886,25 +22906,25 @@
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x.rcbuffer->pybuffer, (PyObject*)__pyx_v_x, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
   }
   __pyx_pybuffernd_x.diminfo[0].strides = __pyx_pybuffernd_x.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_x.diminfo[0].shape = __pyx_pybuffernd_x.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_missing.rcbuffer->pybuffer, (PyObject*)__pyx_v_x_missing, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_missing.rcbuffer->pybuffer, (PyObject*)__pyx_v_x_missing, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
   }
   __pyx_pybuffernd_x_missing.diminfo[0].strides = __pyx_pybuffernd_x_missing.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_x_missing.diminfo[0].shape = __pyx_pybuffernd_x_missing.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_phi.rcbuffer->pybuffer, (PyObject*)__pyx_v_phi, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
   }
   __pyx_pybuffernd_phi.diminfo[0].strides = __pyx_pybuffernd_phi.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_phi.diminfo[0].shape = __pyx_pybuffernd_phi.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parent_feature_indexes.rcbuffer->pybuffer, (PyObject*)__pyx_v_parent_feature_indexes, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parent_feature_indexes.rcbuffer->pybuffer, (PyObject*)__pyx_v_parent_feature_indexes, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
   }
   __pyx_pybuffernd_parent_feature_indexes.diminfo[0].strides = __pyx_pybuffernd_parent_feature_indexes.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_parent_feature_indexes.diminfo[0].shape = __pyx_pybuffernd_parent_feature_indexes.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_parent_zero_fractions.rcbuffer->pybuffer, (PyObject*)__pyx_v_parent_zero_fractions, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 1032, __pyx_L1_error)
   }
   __pyx_pybuffernd_parent_zero_fractions.diminfo[0].strides = __pyx_pybuffernd_parent_zero_fractions.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_parent_zero_fractions.diminfo[0].shape = __pyx_pybuffernd_parent_zero_fractions.rcbuffer->pybuffer.shape[0];
@@ -22919,24 +22939,24 @@
   }
   __pyx_pybuffernd_parent_pweights.diminfo[0].strides = __pyx_pybuffernd_parent_pweights.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_parent_pweights.diminfo[0].shape = __pyx_pybuffernd_parent_pweights.rcbuffer->pybuffer.shape[0];
 
   /* "structureboost/structure_gb.pyx":1058
  *                         double condition_fraction):
  * 
  *     cdef long pfi_len = len(parent_feature_indexes)             # <<<<<<<<<<<<<<
- *     cdef np.ndarray[long] feature_indexes = np.zeros(pfi_len, dtype=np.int_)
+ *     cdef np.ndarray[np.int32_t] feature_indexes = np.zeros(pfi_len, dtype=np.int32)
  *     cdef np.ndarray[double] zero_fractions = np.zeros(pfi_len, dtype=np.float64)
  */
   __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_parent_feature_indexes)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1058, __pyx_L1_error)
   __pyx_v_pfi_len = __pyx_t_1;
 
   /* "structureboost/structure_gb.pyx":1059
  * 
  *     cdef long pfi_len = len(parent_feature_indexes)
- *     cdef np.ndarray[long] feature_indexes = np.zeros(pfi_len, dtype=np.int_)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.int32_t] feature_indexes = np.zeros(pfi_len, dtype=np.int32)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[double] zero_fractions = np.zeros(pfi_len, dtype=np.float64)
  *     cdef np.ndarray[double] one_fractions = np.zeros(pfi_len, dtype=np.float64)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1059, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1059, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
@@ -22948,41 +22968,41 @@
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1059, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1059, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1059, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1059, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 1059, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1059, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1059, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_feature_indexes = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 1059, __pyx_L1_error)
     } else {__pyx_pybuffernd_feature_indexes.diminfo[0].strides = __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_feature_indexes.diminfo[0].shape = __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_feature_indexes = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
   /* "structureboost/structure_gb.pyx":1060
  *     cdef long pfi_len = len(parent_feature_indexes)
- *     cdef np.ndarray[long] feature_indexes = np.zeros(pfi_len, dtype=np.int_)
+ *     cdef np.ndarray[np.int32_t] feature_indexes = np.zeros(pfi_len, dtype=np.int32)
  *     cdef np.ndarray[double] zero_fractions = np.zeros(pfi_len, dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[double] one_fractions = np.zeros(pfi_len, dtype=np.float64)
  *     cdef np.ndarray[double] pweights = np.zeros(pfi_len, dtype=np.float64)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1060, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1060, __pyx_L1_error)
@@ -23020,15 +23040,15 @@
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_zero_fractions = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
   /* "structureboost/structure_gb.pyx":1061
- *     cdef np.ndarray[long] feature_indexes = np.zeros(pfi_len, dtype=np.int_)
+ *     cdef np.ndarray[np.int32_t] feature_indexes = np.zeros(pfi_len, dtype=np.int32)
  *     cdef np.ndarray[double] zero_fractions = np.zeros(pfi_len, dtype=np.float64)
  *     cdef np.ndarray[double] one_fractions = np.zeros(pfi_len, dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[double] pweights = np.zeros(pfi_len, dtype=np.float64)
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1061, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
@@ -23173,15 +23193,15 @@
  *     for i in range((unique_depth + 1),pfi_len):
  *         feature_indexes[j] = parent_feature_indexes[i]             # <<<<<<<<<<<<<<
  *         zero_fractions[j] = parent_zero_fractions[i]
  *         one_fractions[j] = parent_one_fractions[i]
  */
     __pyx_t_15 = __pyx_v_i;
     __pyx_t_16 = __pyx_v_j;
-    *__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_feature_indexes.diminfo[0].strides) = (*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_parent_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_parent_feature_indexes.diminfo[0].strides));
+    *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_feature_indexes.diminfo[0].strides) = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_parent_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_parent_feature_indexes.diminfo[0].strides));
 
     /* "structureboost/structure_gb.pyx":1090
  *     for i in range((unique_depth + 1),pfi_len):
  *         feature_indexes[j] = parent_feature_indexes[i]
  *         zero_fractions[j] = parent_zero_fractions[i]             # <<<<<<<<<<<<<<
  *         one_fractions[j] = parent_one_fractions[i]
  *         pweights[j] = parent_pweights[i]
@@ -23239,15 +23259,15 @@
  *     for i in range(unique_depth+1):
  *         feature_indexes[i] = parent_feature_indexes[i]             # <<<<<<<<<<<<<<
  *         zero_fractions[i] = parent_zero_fractions[i]
  *         one_fractions[i] = parent_one_fractions[i]
  */
     __pyx_t_15 = __pyx_v_i;
     __pyx_t_16 = __pyx_v_i;
-    *__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_feature_indexes.diminfo[0].strides) = (*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_parent_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_parent_feature_indexes.diminfo[0].strides));
+    *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_feature_indexes.diminfo[0].strides) = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_parent_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_parent_feature_indexes.diminfo[0].strides));
 
     /* "structureboost/structure_gb.pyx":1096
  *     for i in range(unique_depth+1):
  *         feature_indexes[i] = parent_feature_indexes[i]
  *         zero_fractions[i] = parent_zero_fractions[i]             # <<<<<<<<<<<<<<
  *         one_fractions[i] = parent_one_fractions[i]
  *         pweights[i] = parent_pweights[i]
@@ -23321,25 +23341,25 @@
  *         )
  * 
  *     split_index = features[node_index]             # <<<<<<<<<<<<<<
  * 
  *     # leaf node
  */
   __pyx_t_15 = __pyx_v_node_index;
-  __pyx_v_split_index = (*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_features.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_features.diminfo[0].strides));
+  __pyx_v_split_index = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_features.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_features.diminfo[0].strides));
 
   /* "structureboost/structure_gb.pyx":1109
  * 
  *     # leaf node
  *     if children_right[node_index] == -1:             # <<<<<<<<<<<<<<
  *         for i in range(1, unique_depth+1):
  *             w = unwound_path_sum(feature_indexes, zero_fractions, one_fractions, pweights, unique_depth, i)
  */
   __pyx_t_15 = __pyx_v_node_index;
-  __pyx_t_11 = (((*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_children_right.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_children_right.diminfo[0].strides)) == -1L) != 0);
+  __pyx_t_11 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_children_right.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_children_right.diminfo[0].strides)) == -1L) != 0);
   if (__pyx_t_11) {
 
     /* "structureboost/structure_gb.pyx":1110
  *     # leaf node
  *     if children_right[node_index] == -1:
  *         for i in range(1, unique_depth+1):             # <<<<<<<<<<<<<<
  *             w = unwound_path_sum(feature_indexes, zero_fractions, one_fractions, pweights, unique_depth, i)
@@ -23366,15 +23386,15 @@
  *     # internal node
  *     else:
  */
       __pyx_t_15 = __pyx_v_i;
       __pyx_t_16 = __pyx_v_i;
       __pyx_t_18 = __pyx_v_node_index;
       __pyx_t_19 = __pyx_v_i;
-      __pyx_t_20 = (*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_feature_indexes.diminfo[0].strides));
+      __pyx_t_20 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_feature_indexes.diminfo[0].strides));
       *__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_phi.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_phi.diminfo[0].strides) += (((__pyx_v_w * ((*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_one_fractions.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_one_fractions.diminfo[0].strides)) - (*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_zero_fractions.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_zero_fractions.diminfo[0].strides)))) * (*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_values.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_values.diminfo[0].strides))) * __pyx_v_condition_fraction);
     }
 
     /* "structureboost/structure_gb.pyx":1109
  * 
  *     # leaf node
  *     if children_right[node_index] == -1:             # <<<<<<<<<<<<<<
@@ -23398,46 +23418,46 @@
  *         # find which branch is "hot" (meaning x would follow it)
  *         hot_index = 0
  *         cleft = children_left[node_index]             # <<<<<<<<<<<<<<
  *         cright = children_right[node_index]
  *         if x_missing[split_index] == 1:
  */
     __pyx_t_18 = __pyx_v_node_index;
-    __pyx_v_cleft = (*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_children_left.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_children_left.diminfo[0].strides));
+    __pyx_v_cleft = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_children_left.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_children_left.diminfo[0].strides));
 
     /* "structureboost/structure_gb.pyx":1118
  *         hot_index = 0
  *         cleft = children_left[node_index]
  *         cright = children_right[node_index]             # <<<<<<<<<<<<<<
  *         if x_missing[split_index] == 1:
  *             hot_index = children_default[node_index]
  */
     __pyx_t_18 = __pyx_v_node_index;
-    __pyx_v_cright = (*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_children_right.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_children_right.diminfo[0].strides));
+    __pyx_v_cright = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_children_right.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_children_right.diminfo[0].strides));
 
     /* "structureboost/structure_gb.pyx":1119
  *         cleft = children_left[node_index]
  *         cright = children_right[node_index]
  *         if x_missing[split_index] == 1:             # <<<<<<<<<<<<<<
  *             hot_index = children_default[node_index]
  *         elif (node_type_vec[node_index]==1) and (x[split_index] < thresholds[node_index]): # (node_type_vec[node_index]==1) and
  */
     __pyx_t_18 = __pyx_v_split_index;
-    __pyx_t_11 = (((*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_x_missing.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_x_missing.diminfo[0].strides)) == 1) != 0);
+    __pyx_t_11 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_x_missing.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_x_missing.diminfo[0].strides)) == 1) != 0);
     if (__pyx_t_11) {
 
       /* "structureboost/structure_gb.pyx":1120
  *         cright = children_right[node_index]
  *         if x_missing[split_index] == 1:
  *             hot_index = children_default[node_index]             # <<<<<<<<<<<<<<
  *         elif (node_type_vec[node_index]==1) and (x[split_index] < thresholds[node_index]): # (node_type_vec[node_index]==1) and
  *             hot_index = cleft
  */
       __pyx_t_18 = __pyx_v_node_index;
-      __pyx_v_hot_index = (*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_children_default.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_children_default.diminfo[0].strides));
+      __pyx_v_hot_index = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_children_default.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_children_default.diminfo[0].strides));
 
       /* "structureboost/structure_gb.pyx":1119
  *         cleft = children_left[node_index]
  *         cright = children_right[node_index]
  *         if x_missing[split_index] == 1:             # <<<<<<<<<<<<<<
  *             hot_index = children_default[node_index]
  *         elif (node_type_vec[node_index]==1) and (x[split_index] < thresholds[node_index]): # (node_type_vec[node_index]==1) and
@@ -23449,15 +23469,15 @@
  *         if x_missing[split_index] == 1:
  *             hot_index = children_default[node_index]
  *         elif (node_type_vec[node_index]==1) and (x[split_index] < thresholds[node_index]): # (node_type_vec[node_index]==1) and             # <<<<<<<<<<<<<<
  *             hot_index = cleft
  *         elif (node_type_vec[node_index]==2):
  */
     __pyx_t_18 = __pyx_v_node_index;
-    __pyx_t_17 = (((*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_node_type_vec.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_node_type_vec.diminfo[0].strides)) == 1) != 0);
+    __pyx_t_17 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_node_type_vec.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_node_type_vec.diminfo[0].strides)) == 1) != 0);
     if (__pyx_t_17) {
     } else {
       __pyx_t_11 = __pyx_t_17;
       goto __pyx_L15_bool_binop_done;
     }
     __pyx_t_18 = __pyx_v_split_index;
     __pyx_t_16 = __pyx_v_node_index;
@@ -23489,15 +23509,15 @@
  *         elif (node_type_vec[node_index]==1) and (x[split_index] < thresholds[node_index]): # (node_type_vec[node_index]==1) and
  *             hot_index = cleft
  *         elif (node_type_vec[node_index]==2):             # <<<<<<<<<<<<<<
  *             hot_index = cright
  *             for k in range(num_cat_vals_vec[node_index]):
  */
     __pyx_t_16 = __pyx_v_node_index;
-    __pyx_t_11 = (((*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_node_type_vec.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_node_type_vec.diminfo[0].strides)) == 2) != 0);
+    __pyx_t_11 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_node_type_vec.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_node_type_vec.diminfo[0].strides)) == 2) != 0);
     if (__pyx_t_11) {
 
       /* "structureboost/structure_gb.pyx":1124
  *             hot_index = cleft
  *         elif (node_type_vec[node_index]==2):
  *             hot_index = cright             # <<<<<<<<<<<<<<
  *             for k in range(num_cat_vals_vec[node_index]):
@@ -23509,30 +23529,30 @@
  *         elif (node_type_vec[node_index]==2):
  *             hot_index = cright
  *             for k in range(num_cat_vals_vec[node_index]):             # <<<<<<<<<<<<<<
  *                 if x[split_index]==cat_vals_mat[node_index,k]:
  *                     hot_index = cleft
  */
       __pyx_t_16 = __pyx_v_node_index;
-      __pyx_t_12 = (*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_num_cat_vals_vec.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_num_cat_vals_vec.diminfo[0].strides));
-      __pyx_t_13 = __pyx_t_12;
-      for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_13; __pyx_t_14+=1) {
-        __pyx_v_k = __pyx_t_14;
+      __pyx_t_21 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_num_cat_vals_vec.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_num_cat_vals_vec.diminfo[0].strides));
+      __pyx_t_22 = __pyx_t_21;
+      for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_22; __pyx_t_12+=1) {
+        __pyx_v_k = __pyx_t_12;
 
         /* "structureboost/structure_gb.pyx":1126
  *             hot_index = cright
  *             for k in range(num_cat_vals_vec[node_index]):
  *                 if x[split_index]==cat_vals_mat[node_index,k]:             # <<<<<<<<<<<<<<
  *                     hot_index = cleft
  *                     break
  */
         __pyx_t_16 = __pyx_v_split_index;
         __pyx_t_18 = __pyx_v_node_index;
         __pyx_t_15 = __pyx_v_k;
-        __pyx_t_11 = (((*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_x.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_x.diminfo[0].strides)) == (*__Pyx_BufPtrStrided2d(long *, __pyx_pybuffernd_cat_vals_mat.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_cat_vals_mat.diminfo[0].strides, __pyx_t_15, __pyx_pybuffernd_cat_vals_mat.diminfo[1].strides))) != 0);
+        __pyx_t_11 = (((*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_x.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_x.diminfo[0].strides)) == (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_cat_vals_mat.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_cat_vals_mat.diminfo[0].strides, __pyx_t_15, __pyx_pybuffernd_cat_vals_mat.diminfo[1].strides))) != 0);
         if (__pyx_t_11) {
 
           /* "structureboost/structure_gb.pyx":1127
  *             for k in range(num_cat_vals_vec[node_index]):
  *                 if x[split_index]==cat_vals_mat[node_index,k]:
  *                     hot_index = cleft             # <<<<<<<<<<<<<<
  *                     break
@@ -23668,15 +23688,15 @@
  *         path_index = 0
  *         while (path_index <= unique_depth):
  *             if feature_indexes[path_index] == split_index:             # <<<<<<<<<<<<<<
  *                 break
  *             path_index += 1
  */
       __pyx_t_15 = __pyx_v_path_index;
-      __pyx_t_11 = (((*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_feature_indexes.diminfo[0].strides)) == __pyx_v_split_index) != 0);
+      __pyx_t_11 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_feature_indexes.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_feature_indexes.diminfo[0].strides)) == __pyx_v_split_index) != 0);
       if (__pyx_t_11) {
 
         /* "structureboost/structure_gb.pyx":1143
  *         while (path_index <= unique_depth):
  *             if feature_indexes[path_index] == split_index:
  *                 break             # <<<<<<<<<<<<<<
  *             path_index += 1
@@ -23905,17 +23925,17 @@
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L11:;
 
   /* "structureboost/structure_gb.pyx":1032
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * @cython.cdivision(True)
- * cdef tree_shap_recursive(np.ndarray[long] children_left,             # <<<<<<<<<<<<<<
- *                         np.ndarray[long] children_right,
- *                         np.ndarray[long] children_default,
+ * cdef tree_shap_recursive(np.ndarray[np.int32_t] children_left,             # <<<<<<<<<<<<<<
+ *                         np.ndarray[np.int32_t] children_right,
+ *                         np.ndarray[np.int32_t] children_default,
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -23986,15 +24006,15 @@
 }
 
 /* "structureboost/structure_gb.pyx":1183
  *         )
  * 
  * def tree_shap_single_pt(dt_mat_int, dt_mat_float,  dt_max_depth, X_in, condition=0, condition_feature=0):             # <<<<<<<<<<<<<<
  * 
- *     x_missing = np.isnan(X_in).astype(int)
+ *     x_missing = np.isnan(X_in).astype(np.int32)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_12structure_gb_23tree_shap_single_pt(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_12structure_gb_23tree_shap_single_pt = {"tree_shap_single_pt", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_12structure_gb_23tree_shap_single_pt, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_12structure_gb_23tree_shap_single_pt(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_dt_mat_int = 0;
@@ -24146,15 +24166,15 @@
   __Pyx_TraceFrameInit(__pyx_codeobj__46)
   __Pyx_RefNannySetupContext("tree_shap_single_pt", 0);
   __Pyx_TraceCall("tree_shap_single_pt", __pyx_f[0], 1183, 0, __PYX_ERR(0, 1183, __pyx_L1_error));
 
   /* "structureboost/structure_gb.pyx":1185
  * def tree_shap_single_pt(dt_mat_int, dt_mat_float,  dt_max_depth, X_in, condition=0, condition_feature=0):
  * 
- *     x_missing = np.isnan(X_in).astype(int)             # <<<<<<<<<<<<<<
+ *     x_missing = np.isnan(X_in).astype(np.int32)             # <<<<<<<<<<<<<<
  *     # Extract tree info from the matrix/tensor representation
  *     dt_thresholds = dt_mat_float[:,0]
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_isnan); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
@@ -24173,34 +24193,40 @@
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1185, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1185, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, ((PyObject *)(&PyInt_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_4, ((PyObject *)(&PyInt_Type)));
+  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1185, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_x_missing = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb.pyx":1187
- *     x_missing = np.isnan(X_in).astype(int)
+ *     x_missing = np.isnan(X_in).astype(np.int32)
  *     # Extract tree info from the matrix/tensor representation
  *     dt_thresholds = dt_mat_float[:,0]             # <<<<<<<<<<<<<<
  *     dt_node_weights = dt_mat_float[:,1]
  *     dt_node_vals = dt_mat_float[:,2] # for a single valued output
  */
   __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_dt_mat_float, __pyx_tuple__47); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -24268,193 +24294,217 @@
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb.pyx":1194
  *     dt_features = dt_mat_int[:,1]
  *     dt_left_children = dt_mat_int[:,2]
  *     dt_right_children = dt_mat_int[:,3]             # <<<<<<<<<<<<<<
  *     dt_na_left = dt_mat_int[:,4]
- *     dt_default_children = dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children
+ *     dt_default_children = (dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children).astype(np.int32)
  */
   __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_dt_mat_int, __pyx_tuple__49); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_dt_right_children = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb.pyx":1195
  *     dt_left_children = dt_mat_int[:,2]
  *     dt_right_children = dt_mat_int[:,3]
  *     dt_na_left = dt_mat_int[:,4]             # <<<<<<<<<<<<<<
- *     dt_default_children = dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children
+ *     dt_default_children = (dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children).astype(np.int32)
  *     dt_num_cat_vals = dt_mat_int[:,5]
  */
   __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_dt_mat_int, __pyx_tuple__50); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_dt_na_left = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb.pyx":1196
  *     dt_right_children = dt_mat_int[:,3]
  *     dt_na_left = dt_mat_int[:,4]
- *     dt_default_children = dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children             # <<<<<<<<<<<<<<
+ *     dt_default_children = (dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children).astype(np.int32)             # <<<<<<<<<<<<<<
  *     dt_num_cat_vals = dt_mat_int[:,5]
  *     dt_cat_vals_mat = dt_mat_int[:,6:]
  */
-  __pyx_t_1 = PyNumber_Multiply(__pyx_v_dt_na_left, __pyx_v_dt_left_children); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1196, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyInt_SubtractCObj(__pyx_int_1, __pyx_v_dt_na_left, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1196, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Multiply(__pyx_v_dt_na_left, __pyx_v_dt_left_children); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_4, __pyx_v_dt_right_children); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1196, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_SubtractCObj(__pyx_int_1, __pyx_v_dt_na_left, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = PyNumber_Multiply(__pyx_t_3, __pyx_v_dt_right_children); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyNumber_Add(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1196, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1196, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v_dt_default_children = __pyx_t_4;
-  __pyx_t_4 = 0;
+  __pyx_v_dt_default_children = __pyx_t_1;
+  __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb.pyx":1197
  *     dt_na_left = dt_mat_int[:,4]
- *     dt_default_children = dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children
+ *     dt_default_children = (dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children).astype(np.int32)
  *     dt_num_cat_vals = dt_mat_int[:,5]             # <<<<<<<<<<<<<<
  *     dt_cat_vals_mat = dt_mat_int[:,6:]
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_dt_mat_int, __pyx_tuple__51); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1197, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_v_dt_num_cat_vals = __pyx_t_4;
-  __pyx_t_4 = 0;
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_dt_mat_int, __pyx_tuple__51); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1197, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_dt_num_cat_vals = __pyx_t_1;
+  __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb.pyx":1198
- *     dt_default_children = dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children
+ *     dt_default_children = (dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children).astype(np.int32)
  *     dt_num_cat_vals = dt_mat_int[:,5]
  *     dt_cat_vals_mat = dt_mat_int[:,6:]             # <<<<<<<<<<<<<<
  * 
  *     # Initialize tracking vectors
  */
-  __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_dt_mat_int, __pyx_tuple__53); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1198, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_v_dt_cat_vals_mat = __pyx_t_4;
-  __pyx_t_4 = 0;
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_dt_mat_int, __pyx_tuple__53); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1198, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_dt_cat_vals_mat = __pyx_t_1;
+  __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb.pyx":1201
  * 
  *     # Initialize tracking vectors
  *     s = (dt_max_depth+2)*(dt_max_depth+1)             # <<<<<<<<<<<<<<
- *     feature_indexes = np.zeros(s, dtype=np.int_)
+ *     feature_indexes = np.zeros(s, dtype=np.int32)
  *     zero_fractions = np.zeros(s, dtype=np.float64)
  */
-  __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_v_dt_max_depth, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1201, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_dt_max_depth, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1201, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_v_dt_max_depth, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyNumber_Multiply(__pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1201, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1201, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v_s = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_v_s = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "structureboost/structure_gb.pyx":1202
  *     # Initialize tracking vectors
  *     s = (dt_max_depth+2)*(dt_max_depth+1)
- *     feature_indexes = np.zeros(s, dtype=np.int_)             # <<<<<<<<<<<<<<
+ *     feature_indexes = np.zeros(s, dtype=np.int32)             # <<<<<<<<<<<<<<
  *     zero_fractions = np.zeros(s, dtype=np.float64)
  *     one_fractions = np.zeros(s, dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1202, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1202, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1202, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1202, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1202, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_v_s);
   __Pyx_GIVEREF(__pyx_v_s);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_s);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1202, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_s);
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1202, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1202, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1202, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1202, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1202, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_feature_indexes = __pyx_t_5;
   __pyx_t_5 = 0;
 
   /* "structureboost/structure_gb.pyx":1203
  *     s = (dt_max_depth+2)*(dt_max_depth+1)
- *     feature_indexes = np.zeros(s, dtype=np.int_)
+ *     feature_indexes = np.zeros(s, dtype=np.int32)
  *     zero_fractions = np.zeros(s, dtype=np.float64)             # <<<<<<<<<<<<<<
  *     one_fractions = np.zeros(s, dtype=np.float64)
  *     pweights = np.zeros(s, dtype=np.float64)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1203, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1203, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_s);
   __Pyx_GIVEREF(__pyx_v_s);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_s);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1203, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1203, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 1203, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 1203, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1203, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_zero_fractions = __pyx_t_3;
   __pyx_t_3 = 0;
 
   /* "structureboost/structure_gb.pyx":1204
- *     feature_indexes = np.zeros(s, dtype=np.int_)
+ *     feature_indexes = np.zeros(s, dtype=np.int32)
  *     zero_fractions = np.zeros(s, dtype=np.float64)
  *     one_fractions = np.zeros(s, dtype=np.float64)             # <<<<<<<<<<<<<<
  *     pweights = np.zeros(s, dtype=np.float64)
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1204, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1204, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_s);
   __Pyx_GIVEREF(__pyx_v_s);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_s);
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1204, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1204, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1204, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1204, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_one_fractions = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "structureboost/structure_gb.pyx":1205
  *     zero_fractions = np.zeros(s, dtype=np.float64)
@@ -24471,28 +24521,28 @@
   __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_s);
   __Pyx_GIVEREF(__pyx_v_s);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_s);
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1205, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1205, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 1205, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1205, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1205, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 1205, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1205, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_pweights = __pyx_t_4;
-  __pyx_t_4 = 0;
+  __pyx_v_pweights = __pyx_t_1;
+  __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb.pyx":1207
  *     pweights = np.zeros(s, dtype=np.float64)
  * 
  *     phi = np.zeros(len(X_in)+1) # Assuming single value output             # <<<<<<<<<<<<<<
  *     root_val = (np.sum((dt_node_type==0) * (dt_node_weights) * dt_node_vals) /
  *                 np.sum((dt_node_type==0) * (dt_node_weights)) )
@@ -24511,22 +24561,22 @@
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
+  __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1207, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1207, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v_phi = __pyx_t_4;
-  __pyx_t_4 = 0;
+  __pyx_v_phi = __pyx_t_1;
+  __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb.pyx":1208
  * 
  *     phi = np.zeros(len(X_in)+1) # Assuming single value output
  *     root_val = (np.sum((dt_node_type==0) * (dt_node_weights) * dt_node_vals) /             # <<<<<<<<<<<<<<
  *                 np.sum((dt_node_type==0) * (dt_node_weights)) )
  *     # update the bias term, which is the last index in phi
@@ -24550,19 +24600,19 @@
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
-  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
+  __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1208, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1208, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "structureboost/structure_gb.pyx":1209
  *     phi = np.zeros(len(X_in)+1) # Assuming single value output
  *     root_val = (np.sum((dt_node_type==0) * (dt_node_weights) * dt_node_vals) /
  *                 np.sum((dt_node_type==0) * (dt_node_weights)) )             # <<<<<<<<<<<<<<
  *     # update the bias term, which is the last index in phi
@@ -24571,44 +24621,44 @@
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_sum); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyInt_EqObjC(__pyx_v_dt_node_type, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyNumber_Multiply(__pyx_t_2, __pyx_v_dt_node_weights); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1209, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = PyNumber_Multiply(__pyx_t_2, __pyx_v_dt_node_weights); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1209, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_2, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_1);
+  __pyx_t_3 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "structureboost/structure_gb.pyx":1208
  * 
  *     phi = np.zeros(len(X_in)+1) # Assuming single value output
  *     root_val = (np.sum((dt_node_type==0) * (dt_node_weights) * dt_node_vals) /             # <<<<<<<<<<<<<<
  *                 np.sum((dt_node_type==0) * (dt_node_weights)) )
  *     # update the bias term, which is the last index in phi
  */
-  __pyx_t_5 = __Pyx_PyNumber_Divide(__pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1208, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyNumber_Divide(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1208, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_root_val = __pyx_t_5;
   __pyx_t_5 = 0;
 
   /* "structureboost/structure_gb.pyx":1212
  *     # update the bias term, which is the last index in phi
  *     # (note the paper has this as phi_0 instead of phi_M)
@@ -24730,15 +24780,15 @@
   goto __pyx_L0;
 
   /* "structureboost/structure_gb.pyx":1183
  *         )
  * 
  * def tree_shap_single_pt(dt_mat_int, dt_mat_float,  dt_max_depth, X_in, condition=0, condition_feature=0):             # <<<<<<<<<<<<<<
  * 
- *     x_missing = np.isnan(X_in).astype(int)
+ *     x_missing = np.isnan(X_in).astype(np.int32)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -41351,15 +41401,15 @@
   {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
   {&__pyx_n_s_indexes, __pyx_k_indexes, sizeof(__pyx_k_indexes), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
   {&__pyx_n_s_init_eval_set_info, __pyx_k_init_eval_set_info, sizeof(__pyx_k_init_eval_set_info), 0, 0, 1, 1},
   {&__pyx_n_s_initial_model, __pyx_k_initial_model, sizeof(__pyx_k_initial_model), 0, 0, 1, 1},
   {&__pyx_n_s_initial_pred, __pyx_k_initial_pred, sizeof(__pyx_k_initial_pred), 0, 0, 1, 1},
   {&__pyx_n_s_initialize_uv_dict, __pyx_k_initialize_uv_dict, sizeof(__pyx_k_initialize_uv_dict), 0, 0, 1, 1},
-  {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
+  {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
   {&__pyx_n_u_interior, __pyx_k_interior, sizeof(__pyx_k_interior), 0, 1, 0, 1},
   {&__pyx_n_s_inv_cti, __pyx_k_inv_cti, sizeof(__pyx_k_inv_cti), 0, 0, 1, 1},
   {&__pyx_n_s_is_connected, __pyx_k_is_connected, sizeof(__pyx_k_is_connected), 0, 0, 1, 1},
   {&__pyx_n_s_isnan, __pyx_k_isnan, sizeof(__pyx_k_isnan), 0, 0, 1, 1},
   {&__pyx_n_s_isnan_array, __pyx_k_isnan_array, sizeof(__pyx_k_isnan_array), 0, 0, 1, 1},
   {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
@@ -41642,15 +41692,15 @@
  *                 total += (pweights[i] / zero_fraction) / ((unique_depth - i) / (unique_depth + 1))
  */
   __pyx_tuple__45 = PyTuple_Pack(1, __pyx_kp_u_Warning_zero_fraction_is_0); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 1022, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__45);
   __Pyx_GIVEREF(__pyx_tuple__45);
 
   /* "structureboost/structure_gb.pyx":1187
- *     x_missing = np.isnan(X_in).astype(int)
+ *     x_missing = np.isnan(X_in).astype(np.int32)
  *     # Extract tree info from the matrix/tensor representation
  *     dt_thresholds = dt_mat_float[:,0]             # <<<<<<<<<<<<<<
  *     dt_node_weights = dt_mat_float[:,1]
  *     dt_node_vals = dt_mat_float[:,2] # for a single valued output
  */
   __pyx_tuple__47 = PyTuple_Pack(2, __pyx_slice__5, __pyx_int_0); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 1187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__47);
@@ -41668,44 +41718,44 @@
   __Pyx_GIVEREF(__pyx_tuple__48);
 
   /* "structureboost/structure_gb.pyx":1194
  *     dt_features = dt_mat_int[:,1]
  *     dt_left_children = dt_mat_int[:,2]
  *     dt_right_children = dt_mat_int[:,3]             # <<<<<<<<<<<<<<
  *     dt_na_left = dt_mat_int[:,4]
- *     dt_default_children = dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children
+ *     dt_default_children = (dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children).astype(np.int32)
  */
   __pyx_tuple__49 = PyTuple_Pack(2, __pyx_slice__5, __pyx_int_3); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 1194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__49);
   __Pyx_GIVEREF(__pyx_tuple__49);
 
   /* "structureboost/structure_gb.pyx":1195
  *     dt_left_children = dt_mat_int[:,2]
  *     dt_right_children = dt_mat_int[:,3]
  *     dt_na_left = dt_mat_int[:,4]             # <<<<<<<<<<<<<<
- *     dt_default_children = dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children
+ *     dt_default_children = (dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children).astype(np.int32)
  *     dt_num_cat_vals = dt_mat_int[:,5]
  */
   __pyx_tuple__50 = PyTuple_Pack(2, __pyx_slice__5, __pyx_int_4); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 1195, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__50);
   __Pyx_GIVEREF(__pyx_tuple__50);
 
   /* "structureboost/structure_gb.pyx":1197
  *     dt_na_left = dt_mat_int[:,4]
- *     dt_default_children = dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children
+ *     dt_default_children = (dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children).astype(np.int32)
  *     dt_num_cat_vals = dt_mat_int[:,5]             # <<<<<<<<<<<<<<
  *     dt_cat_vals_mat = dt_mat_int[:,6:]
  * 
  */
   __pyx_tuple__51 = PyTuple_Pack(2, __pyx_slice__5, __pyx_int_5); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 1197, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__51);
   __Pyx_GIVEREF(__pyx_tuple__51);
 
   /* "structureboost/structure_gb.pyx":1198
- *     dt_default_children = dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children
+ *     dt_default_children = (dt_na_left*dt_left_children + (1-dt_na_left)*dt_right_children).astype(np.int32)
  *     dt_num_cat_vals = dt_mat_int[:,5]
  *     dt_cat_vals_mat = dt_mat_int[:,6:]             # <<<<<<<<<<<<<<
  * 
  *     # Initialize tracking vectors
  */
   __pyx_slice__52 = PySlice_New(__pyx_int_6, Py_None, Py_None); if (unlikely(!__pyx_slice__52)) __PYX_ERR(0, 1198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__52);
@@ -42393,28 +42443,28 @@
   __Pyx_GIVEREF(__pyx_tuple__118);
   __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(2, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__118, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_gb_pyx, __pyx_n_s_c_entropy_link_der_2, 858, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(0, 858, __pyx_L1_error)
 
   /* "structureboost/structure_gb.pyx":877
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[long, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array):
  */
   __pyx_tuple__119 = PyTuple_Pack(28, __pyx_n_s_dtm_float, __pyx_n_s_dtm, __pyx_n_s_feat_array, __pyx_n_s_cat_vals_end, __pyx_n_s_res_mat, __pyx_n_s_cn, __pyx_n_s_ri, __pyx_n_s_ind, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_curr_val, __pyx_n_s_ind_doub, __pyx_n_s_at_leaf, __pyx_n_s_found_val, __pyx_n_s_isnan_array, __pyx_n_s_THRESH, __pyx_n_s_NODE_WEIGHT, __pyx_n_s_NODE_VALUE, __pyx_n_s_NODE_TYPE, __pyx_n_s_FEATURE_COL, __pyx_n_s_LEFT_CHILD, __pyx_n_s_RIGHT_CHILD, __pyx_n_s_NA_LEFT, __pyx_n_s_NUM_CAT_VALS, __pyx_n_s_CAT_VALS_START, __pyx_n_s_LEAF, __pyx_n_s_NUMER, __pyx_n_s_CATEG); if (unlikely(!__pyx_tuple__119)) __PYX_ERR(0, 877, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__119);
   __Pyx_GIVEREF(__pyx_tuple__119);
   __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(3, 0, 28, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__119, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_gb_pyx, __pyx_n_s_predict_with_tensor_c, 877, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 877, __pyx_L1_error)
 
   /* "structureboost/structure_gb.pyx":1183
  *         )
  * 
  * def tree_shap_single_pt(dt_mat_int, dt_mat_float,  dt_max_depth, X_in, condition=0, condition_feature=0):             # <<<<<<<<<<<<<<
  * 
- *     x_missing = np.isnan(X_in).astype(int)
+ *     x_missing = np.isnan(X_in).astype(np.int32)
  */
   __pyx_tuple__120 = PyTuple_Pack(25, __pyx_n_s_dt_mat_int, __pyx_n_s_dt_mat_float, __pyx_n_s_dt_max_depth, __pyx_n_s_X_in, __pyx_n_s_condition, __pyx_n_s_condition_feature, __pyx_n_s_x_missing, __pyx_n_s_dt_thresholds, __pyx_n_s_dt_node_weights, __pyx_n_s_dt_node_vals, __pyx_n_s_dt_node_type, __pyx_n_s_dt_features, __pyx_n_s_dt_left_children, __pyx_n_s_dt_right_children, __pyx_n_s_dt_na_left, __pyx_n_s_dt_default_children, __pyx_n_s_dt_num_cat_vals, __pyx_n_s_dt_cat_vals_mat, __pyx_n_s_s, __pyx_n_s_feature_indexes, __pyx_n_s_zero_fractions, __pyx_n_s_one_fractions, __pyx_n_s_pweights, __pyx_n_s_phi, __pyx_n_s_root_val); if (unlikely(!__pyx_tuple__120)) __PYX_ERR(0, 1183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__120);
   __Pyx_GIVEREF(__pyx_tuple__120);
   __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(6, 0, 25, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__120, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_gb_pyx, __pyx_n_s_tree_shap_single_pt, 1183, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 1183, __pyx_L1_error)
 
   /* "structureboost/structure_gb.pyx":1226
@@ -43557,28 +43607,28 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_c_entropy_link_der_2, __pyx_t_1) < 0) __PYX_ERR(0, 858, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb.pyx":877
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[long, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array):
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_12structure_gb_21predict_with_tensor_c, NULL, __pyx_n_s_structureboost_structure_gb); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 877, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_predict_with_tensor_c, __pyx_t_1) < 0) __PYX_ERR(0, 877, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb.pyx":1183
  *         )
  * 
  * def tree_shap_single_pt(dt_mat_int, dt_mat_float,  dt_max_depth, X_in, condition=0, condition_feature=0):             # <<<<<<<<<<<<<<
  * 
- *     x_missing = np.isnan(X_in).astype(int)
+ *     x_missing = np.isnan(X_in).astype(np.int32)
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_12structure_gb_23tree_shap_single_pt, NULL, __pyx_n_s_structureboost_structure_gb); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_tree_shap_single_pt, __pyx_t_1) < 0) __PYX_ERR(0, 1183, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb.pyx":1226
@@ -49787,14 +49837,52 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(Py_intptr_t),
                                      little, !is_unsigned);
     }
 }
 
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_npy_int32(npy_int32 value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const npy_int32 neg_one = (npy_int32) -1, const_zero = (npy_int32) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(npy_int32) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(npy_int32) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(npy_int32) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(npy_int32) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(npy_int32) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(npy_int32),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
   static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const char neg_one = (char) -1, const_zero = (char) 0;
```

### Comparing `structureboost-0.4.2/structureboost/structure_gb_multi.c` & `structureboost-0.4.3/structureboost/structure_gb_multi.c`

 * *Files 0% similar despite different names*

```diff
@@ -2487,15 +2487,15 @@
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_double(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_double(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsdsds_long(PyObject *, int writable_flag);
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsdsds_nn___pyx_t_5numpy_int32_t(PyObject *, int writable_flag);
 
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_double(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_double(const char *itemp, PyObject *obj);
 
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
@@ -2723,16 +2723,15 @@
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *, int, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int_t = { "int_t", NULL, sizeof(__pyx_t_5numpy_int_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int_t), 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_long = { "long", NULL, sizeof(long), { 0 }, 0, IS_UNSIGNED(long) ? 'U' : 'I', IS_UNSIGNED(long), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t = { "int32_t", NULL, sizeof(__pyx_t_5numpy_int32_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int32_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int32_t), 0 };
 #define __Pyx_MODULE_NAME "structureboost.structure_gb_multi"
 extern int __pyx_module_is_main_structureboost__structure_gb_multi;
 int __pyx_module_is_main_structureboost__structure_gb_multi = 0;
 
 /* Implementation of 'structureboost.structure_gb_multi' */
 static PyObject *__pyx_builtin_super;
 static PyObject *__pyx_builtin_print;
@@ -2772,15 +2771,14 @@
 static const char __pyx_k_all[] = "all";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_dtm[] = "dtm";
 static const char __pyx_k_eps[] = "eps";
 static const char __pyx_k_exp[] = "exp";
 static const char __pyx_k_fit[] = "fit";
 static const char __pyx_k_ind[] = "ind";
-static const char __pyx_k_int[] = "int_";
 static const char __pyx_k_log[] = "log";
 static const char __pyx_k_max[] = "max";
 static const char __pyx_k_min[] = "min";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_qqq[] = "qqq";
 static const char __pyx_k_rpt[] = "rpt";
@@ -2819,14 +2817,15 @@
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_fixed[] = "fixed";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_gamma[] = "gamma";
 static const char __pyx_k_index[] = "index";
+static const char __pyx_k_int32[] = "int32";
 static const char __pyx_k_isnan[] = "isnan";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_print[] = "print";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_super[] = "super";
@@ -3300,15 +3299,15 @@
 static PyObject *__pyx_n_s_ind;
 static PyObject *__pyx_n_s_ind_doub;
 static PyObject *__pyx_n_s_index;
 static PyObject *__pyx_n_s_init;
 static PyObject *__pyx_n_s_initial_model;
 static PyObject *__pyx_n_s_initial_pred;
 static PyObject *__pyx_kp_u_instead_of_1_May_cause_unexpect;
-static PyObject *__pyx_n_s_int;
+static PyObject *__pyx_n_s_int32;
 static PyObject *__pyx_n_u_interior;
 static PyObject *__pyx_n_s_isnan;
 static PyObject *__pyx_n_s_isnan_array;
 static PyObject *__pyx_n_s_itemsize;
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
 static PyObject *__pyx_n_s_j;
 static PyObject *__pyx_n_s_jk;
@@ -6836,24 +6835,24 @@
   __Pyx_TraceCall("_create_rpt_from_list", __pyx_f[0], 251, 0, __PYX_ERR(0, 251, __pyx_L1_error));
 
   /* "structureboost/structure_gb_multi.pyx":252
  * 
  *     def _create_rpt_from_list(self, partition_list):
  *         num_part = len(partition_list)             # <<<<<<<<<<<<<<
  *         max_part_size = np.max(np.array([len(qq) for qq in partition_list]))
- *         rpt = np.zeros((num_part, max_part_size, self.num_classes), dtype=np.int_)
+ *         rpt = np.zeros((num_part, max_part_size, self.num_classes), dtype=np.int32)
  */
   __pyx_t_1 = PyObject_Length(__pyx_v_partition_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 252, __pyx_L1_error)
   __pyx_v_num_part = __pyx_t_1;
 
   /* "structureboost/structure_gb_multi.pyx":253
  *     def _create_rpt_from_list(self, partition_list):
  *         num_part = len(partition_list)
  *         max_part_size = np.max(np.array([len(qq) for qq in partition_list]))             # <<<<<<<<<<<<<<
- *         rpt = np.zeros((num_part, max_part_size, self.num_classes), dtype=np.int_)
+ *         rpt = np.zeros((num_part, max_part_size, self.num_classes), dtype=np.int32)
  *         flat_list = [j for sl in partition_list for i in sl for j in i]
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_max); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -6954,15 +6953,15 @@
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_max_part_size = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "structureboost/structure_gb_multi.pyx":254
  *         num_part = len(partition_list)
  *         max_part_size = np.max(np.array([len(qq) for qq in partition_list]))
- *         rpt = np.zeros((num_part, max_part_size, self.num_classes), dtype=np.int_)             # <<<<<<<<<<<<<<
+ *         rpt = np.zeros((num_part, max_part_size, self.num_classes), dtype=np.int32)             # <<<<<<<<<<<<<<
  *         flat_list = [j for sl in partition_list for i in sl for j in i]
  *         min_val, max_val = np.min(flat_list), np.max(flat_list)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
@@ -6987,30 +6986,30 @@
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6);
   __pyx_t_6 = 0;
   __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 254, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_rpt = __pyx_t_5;
   __pyx_t_5 = 0;
 
   /* "structureboost/structure_gb_multi.pyx":255
  *         max_part_size = np.max(np.array([len(qq) for qq in partition_list]))
- *         rpt = np.zeros((num_part, max_part_size, self.num_classes), dtype=np.int_)
+ *         rpt = np.zeros((num_part, max_part_size, self.num_classes), dtype=np.int32)
  *         flat_list = [j for sl in partition_list for i in sl for j in i]             # <<<<<<<<<<<<<<
  *         min_val, max_val = np.min(flat_list), np.max(flat_list)
  *         if (min_val<0) or (max_val>self.num_classes-1):
  */
   { /* enter inner scope */
     __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 255, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_5);
@@ -7155,15 +7154,15 @@
     goto __pyx_L1_error;
     __pyx_L18_exit_scope:;
   } /* exit inner scope */
   __pyx_v_flat_list = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
   /* "structureboost/structure_gb_multi.pyx":256
- *         rpt = np.zeros((num_part, max_part_size, self.num_classes), dtype=np.int_)
+ *         rpt = np.zeros((num_part, max_part_size, self.num_classes), dtype=np.int32)
  *         flat_list = [j for sl in partition_list for i in sl for j in i]
  *         min_val, max_val = np.min(flat_list), np.max(flat_list)             # <<<<<<<<<<<<<<
  *         if (min_val<0) or (max_val>self.num_classes-1):
  *             w_str = "Elements of partition must be >=0 and <=(num_classes-1). "
  */
   __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
@@ -7467,15 +7466,15 @@
 }
 
 /* "structureboost/structure_gb_multi.pyx":267
  *         return(rpt)
  * 
  *     def _process_y_data(self, y_data):             # <<<<<<<<<<<<<<
  *         if type(y_data) == pd.Series:
- *             y_data = y_data.to_numpy().astype(np.int_)
+ *             y_data = y_data.to_numpy().astype(np.int32)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_18structure_gb_multi_19StructureBoostMulti_17_process_y_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_18structure_gb_multi_19StructureBoostMulti_17_process_y_data = {"_process_y_data", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_18structure_gb_multi_19StructureBoostMulti_17_process_y_data, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_18structure_gb_multi_19StructureBoostMulti_17_process_y_data(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_self = 0;
@@ -7556,15 +7555,15 @@
   __Pyx_TraceCall("_process_y_data", __pyx_f[0], 267, 0, __PYX_ERR(0, 267, __pyx_L1_error));
   __Pyx_INCREF(__pyx_v_y_data);
 
   /* "structureboost/structure_gb_multi.pyx":268
  * 
  *     def _process_y_data(self, y_data):
  *         if type(y_data) == pd.Series:             # <<<<<<<<<<<<<<
- *             y_data = y_data.to_numpy().astype(np.int_)
+ *             y_data = y_data.to_numpy().astype(np.int32)
  *         elif type(y_data) == np.ndarray:
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pd); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_Series); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -7573,17 +7572,17 @@
   __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_3) {
 
     /* "structureboost/structure_gb_multi.pyx":269
  *     def _process_y_data(self, y_data):
  *         if type(y_data) == pd.Series:
- *             y_data = y_data.to_numpy().astype(np.int_)             # <<<<<<<<<<<<<<
+ *             y_data = y_data.to_numpy().astype(np.int32)             # <<<<<<<<<<<<<<
  *         elif type(y_data) == np.ndarray:
- *             y_data = y_data.astype(np.int_)
+ *             y_data = y_data.astype(np.int32)
  */
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_y_data, __pyx_n_s_to_numpy); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 269, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
@@ -7599,15 +7598,15 @@
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 269, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 269, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 269, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -7625,44 +7624,44 @@
     __Pyx_DECREF_SET(__pyx_v_y_data, __pyx_t_1);
     __pyx_t_1 = 0;
 
     /* "structureboost/structure_gb_multi.pyx":268
  * 
  *     def _process_y_data(self, y_data):
  *         if type(y_data) == pd.Series:             # <<<<<<<<<<<<<<
- *             y_data = y_data.to_numpy().astype(np.int_)
+ *             y_data = y_data.to_numpy().astype(np.int32)
  *         elif type(y_data) == np.ndarray:
  */
     goto __pyx_L3;
   }
 
   /* "structureboost/structure_gb_multi.pyx":270
  *         if type(y_data) == pd.Series:
- *             y_data = y_data.to_numpy().astype(np.int_)
+ *             y_data = y_data.to_numpy().astype(np.int32)
  *         elif type(y_data) == np.ndarray:             # <<<<<<<<<<<<<<
- *             y_data = y_data.astype(np.int_)
+ *             y_data = y_data.astype(np.int32)
  *         #y_data = get_one_hot_mat(y_data, self.num_classes)
  */
   __pyx_t_1 = PyObject_RichCompare(((PyObject *)Py_TYPE(__pyx_v_y_data)), ((PyObject *)__pyx_ptype_5numpy_ndarray), Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
   __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_3) {
 
     /* "structureboost/structure_gb_multi.pyx":271
- *             y_data = y_data.to_numpy().astype(np.int_)
+ *             y_data = y_data.to_numpy().astype(np.int32)
  *         elif type(y_data) == np.ndarray:
- *             y_data = y_data.astype(np.int_)             # <<<<<<<<<<<<<<
+ *             y_data = y_data.astype(np.int32)             # <<<<<<<<<<<<<<
  *         #y_data = get_one_hot_mat(y_data, self.num_classes)
  *         return(y_data)
  */
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_y_data, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 271, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 271, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 271, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -7678,24 +7677,24 @@
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_y_data, __pyx_t_1);
     __pyx_t_1 = 0;
 
     /* "structureboost/structure_gb_multi.pyx":270
  *         if type(y_data) == pd.Series:
- *             y_data = y_data.to_numpy().astype(np.int_)
+ *             y_data = y_data.to_numpy().astype(np.int32)
  *         elif type(y_data) == np.ndarray:             # <<<<<<<<<<<<<<
- *             y_data = y_data.astype(np.int_)
+ *             y_data = y_data.astype(np.int32)
  *         #y_data = get_one_hot_mat(y_data, self.num_classes)
  */
   }
   __pyx_L3:;
 
   /* "structureboost/structure_gb_multi.pyx":273
- *             y_data = y_data.astype(np.int_)
+ *             y_data = y_data.astype(np.int32)
  *         #y_data = get_one_hot_mat(y_data, self.num_classes)
  *         return(y_data)             # <<<<<<<<<<<<<<
  * 
  *     def _get_initial_pred(self, X_train, y_train):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_y_data);
@@ -7703,15 +7702,15 @@
   goto __pyx_L0;
 
   /* "structureboost/structure_gb_multi.pyx":267
  *         return(rpt)
  * 
  *     def _process_y_data(self, y_data):             # <<<<<<<<<<<<<<
  *         if type(y_data) == pd.Series:
- *             y_data = y_data.to_numpy().astype(np.int_)
+ *             y_data = y_data.to_numpy().astype(np.int32)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
@@ -11377,27 +11376,27 @@
     __pyx_t_1 = 0;
 
     /* "structureboost/structure_gb_multi.pyx":416
  *         if self.optimizable:
  *             cat_size = np.max(np.array([dt.get_max_split_size() for dt in self.dec_tree_list]))
  *             num_dt = len(self.dec_tree_list)             # <<<<<<<<<<<<<<
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dec_tree_list); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_9 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_num_dt = __pyx_t_9;
 
     /* "structureboost/structure_gb_multi.pyx":417
  *             cat_size = np.max(np.array([dt.get_max_split_size() for dt in self.dec_tree_list]))
  *             num_dt = len(self.dec_tree_list)
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))             # <<<<<<<<<<<<<<
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, self.num_classes+2))
  */
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_max); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
@@ -11500,15 +11499,15 @@
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_max_nodes = __pyx_t_1;
     __pyx_t_1 = 0;
 
     /* "structureboost/structure_gb_multi.pyx":418
  *             num_dt = len(self.dec_tree_list)
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1             # <<<<<<<<<<<<<<
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1             # <<<<<<<<<<<<<<
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, self.num_classes+2))
  *             for i in range(num_dt):
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
@@ -11533,15 +11532,15 @@
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 418, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -11551,15 +11550,15 @@
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int, __pyx_t_5) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
     /* "structureboost/structure_gb_multi.pyx":419
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, self.num_classes+2))             # <<<<<<<<<<<<<<
  *             for i in range(num_dt):
  *                 self.convert_dt_to_matrix(i)
  */
     __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 419, __pyx_L1_error)
@@ -11599,15 +11598,15 @@
     if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_float, __pyx_t_5) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
     /* "structureboost/structure_gb_multi.pyx":420
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, self.num_classes+2))
  *             for i in range(num_dt):             # <<<<<<<<<<<<<<
  *                 self.convert_dt_to_matrix(i)
  *             self.optimized=True
  */
     __pyx_t_9 = __pyx_v_num_dt;
     __pyx_t_13 = __pyx_t_9;
@@ -11993,16 +11992,17 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
-  int __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_8;
+  PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__28)
   __Pyx_RefNannySetupContext("convert_subtree", 0);
   __Pyx_TraceCall("convert_subtree", __pyx_f[0], 451, 0, __PYX_ERR(0, 451, __pyx_L1_error));
 
@@ -12236,213 +12236,220 @@
     }
 
     /* "structureboost/structure_gb_multi.pyx":462
  *                 self.pred_tens_float[dt_num, ni, 0] = node['split_val']
  *                 self.pred_tens_int[dt_num, ni, 0]= 1
  *             elif node['feature_type']=='categorical_int':             # <<<<<<<<<<<<<<
  *                 setlen = len(node['left_split'])
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  */
     __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_feature_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_categorical_int, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_2) {
 
       /* "structureboost/structure_gb_multi.pyx":463
  *                 self.pred_tens_int[dt_num, ni, 0]= 1
  *             elif node['feature_type']=='categorical_int':
  *                 setlen = len(node['left_split'])             # <<<<<<<<<<<<<<
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  *                 self.pred_tens_int[dt_num, ni, 0]= 2
  */
       __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_split); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 463, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_6 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 463, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 463, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_v_setlen = __pyx_t_1;
       __pyx_t_1 = 0;
 
       /* "structureboost/structure_gb_multi.pyx":464
  *             elif node['feature_type']=='categorical_int':
  *                 setlen = len(node['left_split'])
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)             # <<<<<<<<<<<<<<
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)             # <<<<<<<<<<<<<<
  *                 self.pred_tens_int[dt_num, ni, 0]= 2
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen
  */
       __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 464, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_fromiter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 464, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_split); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 464, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 464, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = NULL;
-      __pyx_t_7 = 0;
+      __pyx_t_8 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
-          __pyx_t_7 = 1;
+          __pyx_t_8 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_4)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_3, __pyx_t_5, ((PyObject *)(&PyInt_Type)), __pyx_v_setlen};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
+        PyObject *__pyx_temp[4] = {__pyx_t_3, __pyx_t_5, __pyx_t_7, __pyx_v_setlen};
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_3, __pyx_t_5, ((PyObject *)(&PyInt_Type)), __pyx_v_setlen};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
+        PyObject *__pyx_temp[4] = {__pyx_t_3, __pyx_t_5, __pyx_t_7, __pyx_v_setlen};
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       {
-        __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 464, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_8);
+        __pyx_t_9 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 464, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_9);
         if (__pyx_t_3) {
-          __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_3); __pyx_t_3 = NULL;
+          __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_3); __pyx_t_3 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_5);
-        PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_5);
-        __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
-        __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
-        PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, ((PyObject *)(&PyInt_Type)));
+        PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_5);
+        __Pyx_GIVEREF(__pyx_t_7);
+        PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_t_7);
         __Pyx_INCREF(__pyx_v_setlen);
         __Pyx_GIVEREF(__pyx_v_setlen);
-        PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_7, __pyx_v_setlen);
+        PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_v_setlen);
         __pyx_t_5 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
+        __pyx_t_7 = 0;
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 464, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_8 = __Pyx_PyInt_AddCObj(__pyx_int_6, __pyx_v_setlen, 6, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 464, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_5 = PySlice_New(__pyx_int_6, __pyx_t_8, Py_None); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 464, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 464, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_9 = __Pyx_PyInt_AddCObj(__pyx_int_6, __pyx_v_setlen, 6, 0, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 464, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __pyx_t_7 = PySlice_New(__pyx_int_6, __pyx_t_9, Py_None); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 464, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 464, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
-      PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_dt_num);
+      PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_dt_num);
       __Pyx_INCREF(__pyx_v_ni);
       __Pyx_GIVEREF(__pyx_v_ni);
-      PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_ni);
-      __Pyx_GIVEREF(__pyx_t_5);
-      PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_5);
-      __pyx_t_5 = 0;
-      if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_8, __pyx_t_1) < 0)) __PYX_ERR(0, 464, __pyx_L1_error)
+      PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_ni);
+      __Pyx_GIVEREF(__pyx_t_7);
+      PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_t_7);
+      __pyx_t_7 = 0;
+      if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_9, __pyx_t_1) < 0)) __PYX_ERR(0, 464, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
       /* "structureboost/structure_gb_multi.pyx":465
  *                 setlen = len(node['left_split'])
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  *                 self.pred_tens_int[dt_num, ni, 0]= 2             # <<<<<<<<<<<<<<
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]
  */
       __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 465, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 465, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 465, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
-      PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_dt_num);
+      PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_dt_num);
       __Pyx_INCREF(__pyx_v_ni);
       __Pyx_GIVEREF(__pyx_v_ni);
-      PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_ni);
+      PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_ni);
       __Pyx_INCREF(__pyx_int_0);
       __Pyx_GIVEREF(__pyx_int_0);
-      PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_int_0);
-      if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_8, __pyx_int_2) < 0)) __PYX_ERR(0, 465, __pyx_L1_error)
+      PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_int_0);
+      if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_9, __pyx_int_2) < 0)) __PYX_ERR(0, 465, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
       /* "structureboost/structure_gb_multi.pyx":466
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  *                 self.pred_tens_int[dt_num, ni, 0]= 2
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen             # <<<<<<<<<<<<<<
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']
  */
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 466, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 466, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 466, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
       PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_dt_num);
       __Pyx_INCREF(__pyx_v_ni);
       __Pyx_GIVEREF(__pyx_v_ni);
       PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_ni);
       __Pyx_INCREF(__pyx_int_5);
       __Pyx_GIVEREF(__pyx_int_5);
       PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_int_5);
-      if (unlikely(PyObject_SetItem(__pyx_t_8, __pyx_t_1, __pyx_v_setlen) < 0)) __PYX_ERR(0, 466, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      if (unlikely(PyObject_SetItem(__pyx_t_9, __pyx_t_1, __pyx_v_setlen) < 0)) __PYX_ERR(0, 466, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
       /* "structureboost/structure_gb_multi.pyx":462
  *                 self.pred_tens_float[dt_num, ni, 0] = node['split_val']
  *                 self.pred_tens_int[dt_num, ni, 0]= 1
  *             elif node['feature_type']=='categorical_int':             # <<<<<<<<<<<<<<
  *                 setlen = len(node['left_split'])
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  */
     }
     __pyx_L4:;
 
     /* "structureboost/structure_gb_multi.pyx":467
  *                 self.pred_tens_int[dt_num, ni, 0]= 2
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]             # <<<<<<<<<<<<<<
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 3]=node['right_child']['node_index']
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_column_to_int_dict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 467, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_split_feature); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 467, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 467, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_split_feature); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 467, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 467, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 467, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 467, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 467, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_dt_num);
     __Pyx_GIVEREF(__pyx_v_dt_num);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_dt_num);
     __Pyx_INCREF(__pyx_v_ni);
     __Pyx_GIVEREF(__pyx_v_ni);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_ni);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_int_1);
-    if (unlikely(PyObject_SetItem(__pyx_t_8, __pyx_t_1, __pyx_t_4) < 0)) __PYX_ERR(0, 467, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (unlikely(PyObject_SetItem(__pyx_t_9, __pyx_t_1, __pyx_t_4) < 0)) __PYX_ERR(0, 467, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "structureboost/structure_gb_multi.pyx":468
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']             # <<<<<<<<<<<<<<
@@ -12452,206 +12459,206 @@
     __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_child); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_n_u_node_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 468, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 468, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_INCREF(__pyx_v_dt_num);
     __Pyx_GIVEREF(__pyx_v_dt_num);
-    PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_dt_num);
+    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_dt_num);
     __Pyx_INCREF(__pyx_v_ni);
     __Pyx_GIVEREF(__pyx_v_ni);
-    PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_ni);
+    PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_ni);
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_GIVEREF(__pyx_int_2);
-    PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_int_2);
-    if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_8, __pyx_t_1) < 0)) __PYX_ERR(0, 468, __pyx_L1_error)
+    PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_int_2);
+    if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_9, __pyx_t_1) < 0)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "structureboost/structure_gb_multi.pyx":469
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 3]=node['right_child']['node_index']             # <<<<<<<<<<<<<<
  *             self.pred_tens_int[dt_num, ni, 4]=node['na_left']
  *             self.convert_subtree(node['left_child'], dt_num)
  */
     __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_right_child); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_node_index); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 469, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_node_index); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_dt_num);
     __Pyx_GIVEREF(__pyx_v_dt_num);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_dt_num);
     __Pyx_INCREF(__pyx_v_ni);
     __Pyx_GIVEREF(__pyx_v_ni);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_ni);
     __Pyx_INCREF(__pyx_int_3);
     __Pyx_GIVEREF(__pyx_int_3);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_int_3);
-    if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_4, __pyx_t_8) < 0)) __PYX_ERR(0, 469, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_4, __pyx_t_9) < 0)) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
     /* "structureboost/structure_gb_multi.pyx":470
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 3]=node['right_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 4]=node['na_left']             # <<<<<<<<<<<<<<
  *             self.convert_subtree(node['left_child'], dt_num)
  *             self.convert_subtree(node['right_child'], dt_num)
  */
-    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_na_left); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 470, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_na_left); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 470, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_dt_num);
     __Pyx_GIVEREF(__pyx_v_dt_num);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_dt_num);
     __Pyx_INCREF(__pyx_v_ni);
     __Pyx_GIVEREF(__pyx_v_ni);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_ni);
     __Pyx_INCREF(__pyx_int_4);
     __Pyx_GIVEREF(__pyx_int_4);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_int_4);
-    if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_1, __pyx_t_8) < 0)) __PYX_ERR(0, 470, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_1, __pyx_t_9) < 0)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
     /* "structureboost/structure_gb_multi.pyx":471
  *             self.pred_tens_int[dt_num, ni, 3]=node['right_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 4]=node['na_left']
  *             self.convert_subtree(node['left_child'], dt_num)             # <<<<<<<<<<<<<<
  *             self.convert_subtree(node['right_child'], dt_num)
  * 
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_convert_subtree); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 471, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_child); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 471, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = NULL;
-    __pyx_t_7 = 0;
+    __pyx_t_7 = NULL;
+    __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_5)) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
-        __pyx_t_7 = 1;
+        __pyx_t_8 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_4, __pyx_v_dt_num};
-      __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 471, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
+      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_4, __pyx_v_dt_num};
+      __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 471, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_4, __pyx_v_dt_num};
-      __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 471, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
+      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_4, __pyx_v_dt_num};
+      __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 471, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     {
-      __pyx_t_3 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 471, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      if (__pyx_t_5) {
-        __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5); __pyx_t_5 = NULL;
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 471, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      if (__pyx_t_7) {
+        __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7); __pyx_t_7 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
-      PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_7, __pyx_t_4);
+      PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_8, __pyx_t_4);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
-      PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_7, __pyx_v_dt_num);
+      PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_8, __pyx_v_dt_num);
       __pyx_t_4 = 0;
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 471, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 471, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
     /* "structureboost/structure_gb_multi.pyx":472
  *             self.pred_tens_int[dt_num, ni, 4]=node['na_left']
  *             self.convert_subtree(node['left_child'], dt_num)
  *             self.convert_subtree(node['right_child'], dt_num)             # <<<<<<<<<<<<<<
  * 
  * @cython.boundscheck(False)
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_convert_subtree); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 472, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_right_child); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 472, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_right_child); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 472, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_4 = NULL;
-    __pyx_t_7 = 0;
+    __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
-        __pyx_t_7 = 1;
+        __pyx_t_8 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_3, __pyx_v_dt_num};
-      __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 472, __pyx_L1_error)
+      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_5, __pyx_v_dt_num};
+      __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 472, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_3, __pyx_v_dt_num};
-      __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 472, __pyx_L1_error)
+      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_5, __pyx_v_dt_num};
+      __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 472, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 472, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_7 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 472, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       if (__pyx_t_4) {
-        __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4); __pyx_t_4 = NULL;
+        __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
-      __Pyx_GIVEREF(__pyx_t_3);
-      PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_7, __pyx_t_3);
+      __Pyx_GIVEREF(__pyx_t_5);
+      PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_8, __pyx_t_5);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
-      PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_7, __pyx_v_dt_num);
-      __pyx_t_3 = 0;
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 472, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_8, __pyx_v_dt_num);
+      __pyx_t_5 = 0;
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 472, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __pyx_L3:;
 
   /* "structureboost/structure_gb_multi.pyx":451
  *         self.convert_subtree(curr_node, dt_num)
  * 
  *     def convert_subtree(self, node, dt_num):             # <<<<<<<<<<<<<<
@@ -12663,15 +12670,16 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("structureboost.structure_gb_multi.StructureBoostMulti.convert_subtree", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ni);
   __Pyx_XDECREF(__pyx_v_setlen);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
@@ -12679,15 +12687,15 @@
   return __pyx_r;
 }
 
 /* "structureboost/structure_gb_multi.pyx":476
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[np.int_t, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_18structure_gb_multi_1predict_with_tensor_c_mc(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_18structure_gb_multi_1predict_with_tensor_c_mc = {"predict_with_tensor_c_mc", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_18structure_gb_multi_1predict_with_tensor_c_mc, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_18structure_gb_multi_1predict_with_tensor_c_mc(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -12840,15 +12848,15 @@
   Py_ssize_t __pyx_t_18;
   long __pyx_t_19;
   long __pyx_t_20;
   long __pyx_t_21;
   Py_ssize_t __pyx_t_22;
   Py_ssize_t __pyx_t_23;
   Py_ssize_t __pyx_t_24;
-  __pyx_t_5numpy_int_t __pyx_t_25;
+  __pyx_t_5numpy_int32_t __pyx_t_25;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__29)
   __Pyx_RefNannySetupContext("predict_with_tensor_c_mc", 0);
   __Pyx_TraceCall("predict_with_tensor_c_mc", __pyx_f[0], 476, 0, __PYX_ERR(0, 476, __pyx_L1_error));
   __pyx_pybuffer_res_tens.pybuffer.buf = NULL;
@@ -12874,15 +12882,15 @@
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm_float.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm_float, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 476, __pyx_L1_error)
   }
   __pyx_pybuffernd_dtm_float.diminfo[0].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_dtm_float.diminfo[0].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_dtm_float.diminfo[1].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_dtm_float.diminfo[1].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_dtm_float.diminfo[2].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_dtm_float.diminfo[2].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[2];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 476, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 476, __pyx_L1_error)
   }
   __pyx_pybuffernd_dtm.diminfo[0].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_dtm.diminfo[0].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_dtm.diminfo[1].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_dtm.diminfo[1].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_dtm.diminfo[2].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_dtm.diminfo[2].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[2];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feat_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_feat_array, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 476, __pyx_L1_error)
   }
   __pyx_pybuffernd_feat_array.diminfo[0].strides = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_feat_array.diminfo[0].shape = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_feat_array.diminfo[1].strides = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_feat_array.diminfo[1].shape = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.shape[1];
@@ -12961,15 +12969,15 @@
   __pyx_t_7 = 0;
   __pyx_v_res_tens = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb_multi.pyx":487
  *     cdef double curr_val, ind_doub
  *     cdef bint at_leaf, found_val
- *     cdef np.ndarray[np.int_t, ndim=2] isnan_array = np.isnan(feat_array).astype(int)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.int32_t, ndim=2] isnan_array = np.isnan(feat_array).astype(np.int32)             # <<<<<<<<<<<<<<
  * 
  *     # These are in dtm_float
  */
   __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_isnan); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
@@ -12988,34 +12996,40 @@
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 487, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_int32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 487, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, ((PyObject *)(&PyInt_Type))) : __Pyx_PyObject_CallOneArg(__pyx_t_5, ((PyObject *)(&PyInt_Type)));
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 487, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_isnan_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_isnan_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_isnan_array = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 487, __pyx_L1_error)
     } else {__pyx_pybuffernd_isnan_array.diminfo[0].strides = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_isnan_array.diminfo[0].shape = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_isnan_array.diminfo[1].strides = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_isnan_array.diminfo[1].shape = __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_isnan_array = ((PyArrayObject *)__pyx_t_1);
@@ -13197,15 +13211,15 @@
  *                 if dtm[k,cn, NODE_TYPE]==LEAF:             # <<<<<<<<<<<<<<
  *                     at_leaf = 1
  *                     for q in range(num_classes):
  */
         __pyx_t_16 = __pyx_v_k;
         __pyx_t_17 = __pyx_v_cn;
         __pyx_t_18 = __pyx_v_NODE_TYPE;
-        __pyx_t_15 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_LEAF) != 0);
+        __pyx_t_15 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_LEAF) != 0);
         if (__pyx_t_15) {
 
           /* "structureboost/structure_gb_multi.pyx":515
  *                 cn = int(cn)
  *                 if dtm[k,cn, NODE_TYPE]==LEAF:
  *                     at_leaf = 1             # <<<<<<<<<<<<<<
  *                     for q in range(num_classes):
@@ -13257,61 +13271,61 @@
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:             # <<<<<<<<<<<<<<
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:
  */
         __pyx_t_16 = __pyx_v_k;
         __pyx_t_17 = __pyx_v_cn;
         __pyx_t_18 = __pyx_v_NODE_TYPE;
-        __pyx_t_15 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_NUMER) != 0);
+        __pyx_t_15 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_NUMER) != 0);
         if (__pyx_t_15) {
 
           /* "structureboost/structure_gb_multi.pyx":519
  *                         res_tens[ri,k,q] = dtm_float[k,cn,NODE_VALUE_START+q]
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]             # <<<<<<<<<<<<<<
  *                     if isnan_array[ri,ind]:
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]
  */
           __pyx_t_18 = __pyx_v_k;
           __pyx_t_17 = __pyx_v_cn;
           __pyx_t_16 = __pyx_v_FEATURE_COL;
-          __pyx_v_ind = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
+          __pyx_v_ind = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
 
           /* "structureboost/structure_gb_multi.pyx":520
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:             # <<<<<<<<<<<<<<
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]
  *                     else:
  */
           __pyx_t_16 = __pyx_v_ri;
           __pyx_t_17 = __pyx_v_ind;
-          __pyx_t_15 = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_isnan_array.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_isnan_array.diminfo[1].strides)) != 0);
+          __pyx_t_15 = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_isnan_array.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_isnan_array.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_isnan_array.diminfo[1].strides)) != 0);
           if (__pyx_t_15) {
 
             /* "structureboost/structure_gb_multi.pyx":521
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]             # <<<<<<<<<<<<<<
  *                     else:
  *                         curr_val = feat_array[ri,ind]
  */
             __pyx_t_17 = __pyx_v_k;
             __pyx_t_16 = __pyx_v_cn;
             __pyx_t_18 = __pyx_v_NA_LEFT;
-            if (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) != 0)) {
+            if (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[2].strides)) != 0)) {
               __pyx_t_24 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_22 = __pyx_v_LEFT_CHILD;
-              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
             } else {
               __pyx_t_22 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_24 = __pyx_v_RIGHT_CHILD;
-              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
             }
             __pyx_v_cn = __pyx_t_25;
 
             /* "structureboost/structure_gb_multi.pyx":520
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:             # <<<<<<<<<<<<<<
@@ -13343,20 +13357,20 @@
             __pyx_t_16 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_17 = __pyx_v_THRESH;
             if (((__pyx_v_curr_val < (*__Pyx_BufPtrStrided3d(double *, __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm_float.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm_float.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm_float.diminfo[2].strides))) != 0)) {
               __pyx_t_24 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_22 = __pyx_v_LEFT_CHILD;
-              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[2].strides));
             } else {
               __pyx_t_22 = __pyx_v_k;
               __pyx_t_23 = __pyx_v_cn;
               __pyx_t_24 = __pyx_v_RIGHT_CHILD;
-              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_24, __pyx_pybuffernd_dtm.diminfo[2].strides));
             }
             __pyx_v_cn = __pyx_t_25;
           }
           __pyx_L12:;
 
           /* "structureboost/structure_gb_multi.pyx":518
  *                     for q in range(num_classes):
@@ -13374,29 +13388,29 @@
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:             # <<<<<<<<<<<<<<
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]
  *                     found_val = 0
  */
         __pyx_t_17 = __pyx_v_k;
         __pyx_t_18 = __pyx_v_cn;
         __pyx_t_16 = __pyx_v_NODE_TYPE;
-        __pyx_t_15 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_CATEG) != 0);
+        __pyx_t_15 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_CATEG) != 0);
         if (__pyx_t_15) {
 
           /* "structureboost/structure_gb_multi.pyx":526
  *                         cn = dtm[k,cn, LEFT_CHILD] if curr_val<dtm_float[k,cn, THRESH] else dtm[k,cn, RIGHT_CHILD]
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]             # <<<<<<<<<<<<<<
  *                     found_val = 0
  *                     j = CAT_VALS_START
  */
           __pyx_t_16 = __pyx_v_k;
           __pyx_t_18 = __pyx_v_cn;
           __pyx_t_17 = __pyx_v_FEATURE_COL;
           __pyx_t_24 = __pyx_v_ri;
-          __pyx_t_23 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
+          __pyx_t_23 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
           __pyx_v_curr_val = (*__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_feat_array.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_feat_array.diminfo[1].strides));
 
           /* "structureboost/structure_gb_multi.pyx":527
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]
  *                     found_val = 0             # <<<<<<<<<<<<<<
  *                     j = CAT_VALS_START
@@ -13419,15 +13433,15 @@
  *                     cat_vals_end = CAT_VALS_START + dtm[k, cn, NUM_CAT_VALS]             # <<<<<<<<<<<<<<
  *                     while ((not found_val) & (j<cat_vals_end)):
  *                         if curr_val==dtm[k,cn, j]:
  */
           __pyx_t_17 = __pyx_v_k;
           __pyx_t_18 = __pyx_v_cn;
           __pyx_t_16 = __pyx_v_NUM_CAT_VALS;
-          __pyx_v_cat_vals_end = (__pyx_v_CAT_VALS_START + (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides)));
+          __pyx_v_cat_vals_end = (__pyx_v_CAT_VALS_START + (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides)));
 
           /* "structureboost/structure_gb_multi.pyx":530
  *                     j = CAT_VALS_START
  *                     cat_vals_end = CAT_VALS_START + dtm[k, cn, NUM_CAT_VALS]
  *                     while ((not found_val) & (j<cat_vals_end)):             # <<<<<<<<<<<<<<
  *                         if curr_val==dtm[k,cn, j]:
  *                             found_val=1
@@ -13442,15 +13456,15 @@
  *                         if curr_val==dtm[k,cn, j]:             # <<<<<<<<<<<<<<
  *                             found_val=1
  *                         else:
  */
             __pyx_t_16 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_17 = __pyx_v_j;
-            __pyx_t_15 = ((__pyx_v_curr_val == (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides))) != 0);
+            __pyx_t_15 = ((__pyx_v_curr_val == (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides))) != 0);
             if (__pyx_t_15) {
 
               /* "structureboost/structure_gb_multi.pyx":532
  *                     while ((not found_val) & (j<cat_vals_end)):
  *                         if curr_val==dtm[k,cn, j]:
  *                             found_val=1             # <<<<<<<<<<<<<<
  *                         else:
@@ -13488,20 +13502,20 @@
  *     return(res_tens)
  * 
  */
           if ((__pyx_v_found_val != 0)) {
             __pyx_t_17 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_16 = __pyx_v_LEFT_CHILD;
-            __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
+            __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
           } else {
             __pyx_t_16 = __pyx_v_k;
             __pyx_t_18 = __pyx_v_cn;
             __pyx_t_17 = __pyx_v_RIGHT_CHILD;
-            __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
+            __pyx_t_25 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides));
           }
           __pyx_v_cn = __pyx_t_25;
 
           /* "structureboost/structure_gb_multi.pyx":525
  *                         curr_val = feat_array[ri,ind]
  *                         cn = dtm[k,cn, LEFT_CHILD] if curr_val<dtm_float[k,cn, THRESH] else dtm[k,cn, RIGHT_CHILD]
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:             # <<<<<<<<<<<<<<
@@ -13526,15 +13540,15 @@
   __pyx_r = ((PyObject *)__pyx_v_res_tens);
   goto __pyx_L0;
 
   /* "structureboost/structure_gb_multi.pyx":476
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[np.int_t, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -13569,15 +13583,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "structureboost/structure_gb_multi.pyx":543
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
- * def c_entropy_link_der_12_vec_sp(np.ndarray[np.int_t] y_true,             # <<<<<<<<<<<<<<
+ * def c_entropy_link_der_12_vec_sp(np.ndarray[np.int32_t] y_true,             # <<<<<<<<<<<<<<
  *                          double[:,:] exp_phi_pred,
  *                          double[:] exp_phi_sum_vec):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_18structure_gb_multi_3c_entropy_link_der_12_vec_sp(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static char __pyx_doc_14structureboost_18structure_gb_multi_2c_entropy_link_der_12_vec_sp[] = "In this variant, y_true is just a vector of correct classes (not one hot)";
@@ -13702,15 +13716,15 @@
   __Pyx_TraceCall("c_entropy_link_der_12_vec_sp", __pyx_f[0], 543, 0, __PYX_ERR(0, 543, __pyx_L1_error));
   __pyx_pybuffer_y_true.pybuffer.buf = NULL;
   __pyx_pybuffer_y_true.refcount = 0;
   __pyx_pybuffernd_y_true.data = NULL;
   __pyx_pybuffernd_y_true.rcbuffer = &__pyx_pybuffer_y_true;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_true.rcbuffer->pybuffer, (PyObject*)__pyx_v_y_true, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 543, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_true.rcbuffer->pybuffer, (PyObject*)__pyx_v_y_true, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 543, __pyx_L1_error)
   }
   __pyx_pybuffernd_y_true.diminfo[0].strides = __pyx_pybuffernd_y_true.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_y_true.diminfo[0].shape = __pyx_pybuffernd_y_true.rcbuffer->pybuffer.shape[0];
 
   /* "structureboost/structure_gb_multi.pyx":547
  *                          double[:] exp_phi_sum_vec):
  *     """In this variant, y_true is just a vector of correct classes (not one hot)"""
  *     cdef long N = len(y_true)             # <<<<<<<<<<<<<<
@@ -13803,15 +13817,15 @@
  *     for i in range(N):
  *         for j in range(m):
  *             if y_true[i]==j:             # <<<<<<<<<<<<<<
  *                 Y[i,j]=(exp_phi_pred[i,j]/exp_phi_sum_vec[i])-1
  *             else:
  */
       __pyx_t_14 = __pyx_v_i;
-      __pyx_t_15 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_y_true.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_y_true.diminfo[0].strides)) == __pyx_v_j) != 0);
+      __pyx_t_15 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_y_true.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_y_true.diminfo[0].strides)) == __pyx_v_j) != 0);
       if (__pyx_t_15) {
 
         /* "structureboost/structure_gb_multi.pyx":555
  *         for j in range(m):
  *             if y_true[i]==j:
  *                 Y[i,j]=(exp_phi_pred[i,j]/exp_phi_sum_vec[i])-1             # <<<<<<<<<<<<<<
  *             else:
@@ -13921,15 +13935,15 @@
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "structureboost/structure_gb_multi.pyx":543
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
- * def c_entropy_link_der_12_vec_sp(np.ndarray[np.int_t] y_true,             # <<<<<<<<<<<<<<
+ * def c_entropy_link_der_12_vec_sp(np.ndarray[np.int32_t] y_true,             # <<<<<<<<<<<<<<
  *                          double[:,:] exp_phi_pred,
  *                          double[:] exp_phi_sum_vec):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -13958,15 +13972,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "structureboost/structure_gb_multi.pyx":566
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
- * def c_str_entropy_link_der_12_vec_sp(np.ndarray[np.int_t] y_true,             # <<<<<<<<<<<<<<
+ * def c_str_entropy_link_der_12_vec_sp(np.ndarray[np.int32_t] y_true,             # <<<<<<<<<<<<<<
  *                                  double[:,:] exp_phi_pred,
  *                                  double[:] exp_phi_sum_vec,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_18structure_gb_multi_5c_str_entropy_link_der_12_vec_sp(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_18structure_gb_multi_5c_str_entropy_link_der_12_vec_sp = {"c_str_entropy_link_der_12_vec_sp", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_18structure_gb_multi_5c_str_entropy_link_der_12_vec_sp, METH_VARARGS|METH_KEYWORDS, 0};
@@ -14044,15 +14058,15 @@
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
     }
     __pyx_v_y_true = ((PyArrayObject *)values[0]);
     __pyx_v_exp_phi_pred = __Pyx_PyObject_to_MemoryviewSlice_dsds_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_exp_phi_pred.memview)) __PYX_ERR(0, 567, __pyx_L3_error)
     __pyx_v_exp_phi_sum_vec = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_exp_phi_sum_vec.memview)) __PYX_ERR(0, 568, __pyx_L3_error)
     __pyx_v_weight_vec = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_weight_vec.memview)) __PYX_ERR(0, 569, __pyx_L3_error)
-    __pyx_v_rp_tensor = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_long(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_rp_tensor.memview)) __PYX_ERR(0, 570, __pyx_L3_error)
+    __pyx_v_rp_tensor = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_nn___pyx_t_5numpy_int32_t(values[4], PyBUF_WRITABLE); if (unlikely(!__pyx_v_rp_tensor.memview)) __PYX_ERR(0, 570, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("c_str_entropy_link_der_12_vec_sp", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 566, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("structureboost.structure_gb_multi.c_str_entropy_link_der_12_vec_sp", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
@@ -14123,30 +14137,30 @@
   __Pyx_TraceCall("c_str_entropy_link_der_12_vec_sp", __pyx_f[0], 566, 0, __PYX_ERR(0, 566, __pyx_L1_error));
   __pyx_pybuffer_y_true.pybuffer.buf = NULL;
   __pyx_pybuffer_y_true.refcount = 0;
   __pyx_pybuffernd_y_true.data = NULL;
   __pyx_pybuffernd_y_true.rcbuffer = &__pyx_pybuffer_y_true;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_true.rcbuffer->pybuffer, (PyObject*)__pyx_v_y_true, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 566, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_true.rcbuffer->pybuffer, (PyObject*)__pyx_v_y_true, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 566, __pyx_L1_error)
   }
   __pyx_pybuffernd_y_true.diminfo[0].strides = __pyx_pybuffernd_y_true.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_y_true.diminfo[0].shape = __pyx_pybuffernd_y_true.rcbuffer->pybuffer.shape[0];
 
   /* "structureboost/structure_gb_multi.pyx":571
  *                                  double[:] weight_vec,
- *                                  long[:,:,:] rp_tensor):
+ *                                  np.int32_t[:,:,:] rp_tensor):
  *     cdef long N = len(y_true)             # <<<<<<<<<<<<<<
  *     cdef long m = exp_phi_pred.shape[1]
  *     cdef long ind = 0
  */
   __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_y_true)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 571, __pyx_L1_error)
   __pyx_v_N = __pyx_t_1;
 
   /* "structureboost/structure_gb_multi.pyx":572
- *                                  long[:,:,:] rp_tensor):
+ *                                  np.int32_t[:,:,:] rp_tensor):
  *     cdef long N = len(y_true)
  *     cdef long m = exp_phi_pred.shape[1]             # <<<<<<<<<<<<<<
  *     cdef long ind = 0
  *     cdef long qqq, xyz
  */
   __pyx_v_m = (__pyx_v_exp_phi_pred.shape[1]);
 
@@ -14288,28 +14302,28 @@
  *             xyz=0
  *             # get y_true value from y_true onehot (passed in)
  *             yval = y_true[i]             # <<<<<<<<<<<<<<
  *             while (rp_tensor[qqq,xyz,yval]==0):
  *                 xyz+=1
  */
       __pyx_t_11 = __pyx_v_i;
-      __pyx_v_yval = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_y_true.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_y_true.diminfo[0].strides));
+      __pyx_v_yval = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_y_true.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_y_true.diminfo[0].strides));
 
       /* "structureboost/structure_gb_multi.pyx":590
  *             # get y_true value from y_true onehot (passed in)
  *             yval = y_true[i]
  *             while (rp_tensor[qqq,xyz,yval]==0):             # <<<<<<<<<<<<<<
  *                 xyz+=1
  *             set_sum = 0
  */
       while (1) {
         __pyx_t_11 = __pyx_v_qqq;
         __pyx_t_15 = __pyx_v_xyz;
         __pyx_t_16 = __pyx_v_yval;
-        __pyx_t_17 = (((*((long *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rp_tensor.data + __pyx_t_11 * __pyx_v_rp_tensor.strides[0]) ) + __pyx_t_15 * __pyx_v_rp_tensor.strides[1]) ) + __pyx_t_16 * __pyx_v_rp_tensor.strides[2]) ))) == 0) != 0);
+        __pyx_t_17 = (((*((__pyx_t_5numpy_int32_t *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rp_tensor.data + __pyx_t_11 * __pyx_v_rp_tensor.strides[0]) ) + __pyx_t_15 * __pyx_v_rp_tensor.strides[1]) ) + __pyx_t_16 * __pyx_v_rp_tensor.strides[2]) ))) == 0) != 0);
         if (!__pyx_t_17) break;
 
         /* "structureboost/structure_gb_multi.pyx":591
  *             yval = y_true[i]
  *             while (rp_tensor[qqq,xyz,yval]==0):
  *                 xyz+=1             # <<<<<<<<<<<<<<
  *             set_sum = 0
@@ -14345,15 +14359,15 @@
  *                 if (rp_tensor[qqq,xyz,t]==1):             # <<<<<<<<<<<<<<
  *                     set_sum+=exp_phi_pred[i,t]
  *             for j in range(m):
  */
         __pyx_t_16 = __pyx_v_qqq;
         __pyx_t_15 = __pyx_v_xyz;
         __pyx_t_11 = __pyx_v_t;
-        __pyx_t_17 = (((*((long *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rp_tensor.data + __pyx_t_16 * __pyx_v_rp_tensor.strides[0]) ) + __pyx_t_15 * __pyx_v_rp_tensor.strides[1]) ) + __pyx_t_11 * __pyx_v_rp_tensor.strides[2]) ))) == 1) != 0);
+        __pyx_t_17 = (((*((__pyx_t_5numpy_int32_t *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rp_tensor.data + __pyx_t_16 * __pyx_v_rp_tensor.strides[0]) ) + __pyx_t_15 * __pyx_v_rp_tensor.strides[1]) ) + __pyx_t_11 * __pyx_v_rp_tensor.strides[2]) ))) == 1) != 0);
         if (__pyx_t_17) {
 
           /* "structureboost/structure_gb_multi.pyx":595
  *             for t in range(m):
  *                 if (rp_tensor[qqq,xyz,t]==1):
  *                     set_sum+=exp_phi_pred[i,t]             # <<<<<<<<<<<<<<
  *             for j in range(m):
@@ -14414,15 +14428,15 @@
  *                 if (rp_tensor[qqq,xyz,j]==1):             # <<<<<<<<<<<<<<
  *                     #Y[i,j]+= value when j in T * weight
  *                     Y[i,j]+=(-curr_wt * (exp_phi_pred[i,j]*(exp_phi_sum_vec[i]-set_sum)/
  */
         __pyx_t_16 = __pyx_v_qqq;
         __pyx_t_15 = __pyx_v_xyz;
         __pyx_t_11 = __pyx_v_j;
-        __pyx_t_17 = (((*((long *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rp_tensor.data + __pyx_t_16 * __pyx_v_rp_tensor.strides[0]) ) + __pyx_t_15 * __pyx_v_rp_tensor.strides[1]) ) + __pyx_t_11 * __pyx_v_rp_tensor.strides[2]) ))) == 1) != 0);
+        __pyx_t_17 = (((*((__pyx_t_5numpy_int32_t *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rp_tensor.data + __pyx_t_16 * __pyx_v_rp_tensor.strides[0]) ) + __pyx_t_15 * __pyx_v_rp_tensor.strides[1]) ) + __pyx_t_11 * __pyx_v_rp_tensor.strides[2]) ))) == 1) != 0);
         if (__pyx_t_17) {
 
           /* "structureboost/structure_gb_multi.pyx":602
  *                 if (rp_tensor[qqq,xyz,j]==1):
  *                     #Y[i,j]+= value when j in T * weight
  *                     Y[i,j]+=(-curr_wt * (exp_phi_pred[i,j]*(exp_phi_sum_vec[i]-set_sum)/             # <<<<<<<<<<<<<<
  *                                         (set_sum*exp_phi_sum_vec[i])))
@@ -14538,15 +14552,15 @@
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "structureboost/structure_gb_multi.pyx":566
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
- * def c_str_entropy_link_der_12_vec_sp(np.ndarray[np.int_t] y_true,             # <<<<<<<<<<<<<<
+ * def c_str_entropy_link_der_12_vec_sp(np.ndarray[np.int32_t] y_true,             # <<<<<<<<<<<<<<
  *                                  double[:,:] exp_phi_pred,
  *                                  double[:] exp_phi_sum_vec,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -14577,15 +14591,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "structureboost/structure_gb_multi.pyx":616
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
- * def get_one_hot_mat(np.ndarray[np.int_t] y_true,             # <<<<<<<<<<<<<<
+ * def get_one_hot_mat(np.ndarray[np.int32_t] y_true,             # <<<<<<<<<<<<<<
  *                          int num_classes):
  *     cdef int N = y_true.shape[0]
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_18structure_gb_multi_7get_one_hot_mat(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_18structure_gb_multi_7get_one_hot_mat = {"get_one_hot_mat", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_18structure_gb_multi_7get_one_hot_mat, METH_VARARGS|METH_KEYWORDS, 0};
@@ -14691,31 +14705,31 @@
   __pyx_pybuffernd_Y.rcbuffer = &__pyx_pybuffer_Y;
   __pyx_pybuffer_y_true.pybuffer.buf = NULL;
   __pyx_pybuffer_y_true.refcount = 0;
   __pyx_pybuffernd_y_true.data = NULL;
   __pyx_pybuffernd_y_true.rcbuffer = &__pyx_pybuffer_y_true;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_true.rcbuffer->pybuffer, (PyObject*)__pyx_v_y_true, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 616, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_true.rcbuffer->pybuffer, (PyObject*)__pyx_v_y_true, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 616, __pyx_L1_error)
   }
   __pyx_pybuffernd_y_true.diminfo[0].strides = __pyx_pybuffernd_y_true.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_y_true.diminfo[0].shape = __pyx_pybuffernd_y_true.rcbuffer->pybuffer.shape[0];
 
   /* "structureboost/structure_gb_multi.pyx":618
- * def get_one_hot_mat(np.ndarray[np.int_t] y_true,
+ * def get_one_hot_mat(np.ndarray[np.int32_t] y_true,
  *                          int num_classes):
  *     cdef int N = y_true.shape[0]             # <<<<<<<<<<<<<<
- *     cdef np.ndarray[np.int_t, ndim=2] Y = np.zeros((N,num_classes), dtype=np.int_)
+ *     cdef np.ndarray[np.int32_t, ndim=2] Y = np.zeros((N,num_classes), dtype=np.int32)
  * 
  */
   __pyx_v_N = (__pyx_v_y_true->dimensions[0]);
 
   /* "structureboost/structure_gb_multi.pyx":619
  *                          int num_classes):
  *     cdef int N = y_true.shape[0]
- *     cdef np.ndarray[np.int_t, ndim=2] Y = np.zeros((N,num_classes), dtype=np.int_)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray[np.int32_t, ndim=2] Y = np.zeros((N,num_classes), dtype=np.int32)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(N):
  */
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -14737,40 +14751,40 @@
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 619, __pyx_L1_error)
   __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_Y.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_Y.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_Y = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_Y.rcbuffer->pybuffer.buf = NULL;
       __PYX_ERR(0, 619, __pyx_L1_error)
     } else {__pyx_pybuffernd_Y.diminfo[0].strides = __pyx_pybuffernd_Y.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_Y.diminfo[0].shape = __pyx_pybuffernd_Y.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_Y.diminfo[1].strides = __pyx_pybuffernd_Y.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_Y.diminfo[1].shape = __pyx_pybuffernd_Y.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_6 = 0;
   __pyx_v_Y = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
   /* "structureboost/structure_gb_multi.pyx":621
- *     cdef np.ndarray[np.int_t, ndim=2] Y = np.zeros((N,num_classes), dtype=np.int_)
+ *     cdef np.ndarray[np.int32_t, ndim=2] Y = np.zeros((N,num_classes), dtype=np.int32)
  * 
  *     for i in range(N):             # <<<<<<<<<<<<<<
  *         Y[i,y_true[i]]= 1
  *     return(Y)
  */
   __pyx_t_7 = __pyx_v_N;
   __pyx_t_8 = __pyx_t_7;
@@ -14782,16 +14796,16 @@
  *     for i in range(N):
  *         Y[i,y_true[i]]= 1             # <<<<<<<<<<<<<<
  *     return(Y)
  * 
  */
     __pyx_t_10 = __pyx_v_i;
     __pyx_t_11 = __pyx_v_i;
-    __pyx_t_12 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_y_true.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_y_true.diminfo[0].strides));
-    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_Y.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_Y.diminfo[0].strides, __pyx_t_12, __pyx_pybuffernd_Y.diminfo[1].strides) = 1;
+    __pyx_t_12 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_y_true.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_y_true.diminfo[0].strides));
+    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_Y.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_Y.diminfo[0].strides, __pyx_t_12, __pyx_pybuffernd_Y.diminfo[1].strides) = 1;
   }
 
   /* "structureboost/structure_gb_multi.pyx":623
  *     for i in range(N):
  *         Y[i,y_true[i]]= 1
  *     return(Y)             # <<<<<<<<<<<<<<
  * 
@@ -14801,15 +14815,15 @@
   __Pyx_INCREF(((PyObject *)__pyx_v_Y));
   __pyx_r = ((PyObject *)__pyx_v_Y);
   goto __pyx_L0;
 
   /* "structureboost/structure_gb_multi.pyx":616
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
- * def get_one_hot_mat(np.ndarray[np.int_t] y_true,             # <<<<<<<<<<<<<<
+ * def get_one_hot_mat(np.ndarray[np.int32_t] y_true,             # <<<<<<<<<<<<<<
  *                          int num_classes):
  *     cdef int N = y_true.shape[0]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -31474,15 +31488,15 @@
   {&__pyx_n_s_ind, __pyx_k_ind, sizeof(__pyx_k_ind), 0, 0, 1, 1},
   {&__pyx_n_s_ind_doub, __pyx_k_ind_doub, sizeof(__pyx_k_ind_doub), 0, 0, 1, 1},
   {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
   {&__pyx_n_s_initial_model, __pyx_k_initial_model, sizeof(__pyx_k_initial_model), 0, 0, 1, 1},
   {&__pyx_n_s_initial_pred, __pyx_k_initial_pred, sizeof(__pyx_k_initial_pred), 0, 0, 1, 1},
   {&__pyx_kp_u_instead_of_1_May_cause_unexpect, __pyx_k_instead_of_1_May_cause_unexpect, sizeof(__pyx_k_instead_of_1_May_cause_unexpect), 0, 1, 0, 0},
-  {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
+  {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
   {&__pyx_n_u_interior, __pyx_k_interior, sizeof(__pyx_k_interior), 0, 1, 0, 1},
   {&__pyx_n_s_isnan, __pyx_k_isnan, sizeof(__pyx_k_isnan), 0, 0, 1, 1},
   {&__pyx_n_s_isnan_array, __pyx_k_isnan_array, sizeof(__pyx_k_isnan_array), 0, 0, 1, 1},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
   {&__pyx_n_s_j, __pyx_k_j, sizeof(__pyx_k_j), 0, 0, 1, 1},
   {&__pyx_n_s_jk, __pyx_k_jk, sizeof(__pyx_k_jk), 0, 0, 1, 1},
@@ -32091,15 +32105,15 @@
   __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(2, 0, 16, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_gb_multi_pyx, __pyx_n_s_create_rpt_from_list, 251, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 251, __pyx_L1_error)
 
   /* "structureboost/structure_gb_multi.pyx":267
  *         return(rpt)
  * 
  *     def _process_y_data(self, y_data):             # <<<<<<<<<<<<<<
  *         if type(y_data) == pd.Series:
- *             y_data = y_data.to_numpy().astype(np.int_)
+ *             y_data = y_data.to_numpy().astype(np.int32)
  */
   __pyx_tuple__67 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_y_data); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__67);
   __Pyx_GIVEREF(__pyx_tuple__67);
   __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_gb_multi_pyx, __pyx_n_s_process_y_data, 267, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 267, __pyx_L1_error)
 
   /* "structureboost/structure_gb_multi.pyx":275
@@ -32246,50 +32260,50 @@
   __Pyx_GIVEREF(__pyx_tuple__79);
   __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__79, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_gb_multi_pyx, __pyx_n_s_convert_subtree, 451, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 451, __pyx_L1_error)
 
   /* "structureboost/structure_gb_multi.pyx":476
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[np.int_t, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
   __pyx_tuple__80 = PyTuple_Pack(30, __pyx_n_s_dtm_float, __pyx_n_s_dtm, __pyx_n_s_feat_array, __pyx_n_s_num_classes, __pyx_n_s_cat_vals_end, __pyx_n_s_res_tens, __pyx_n_s_cn, __pyx_n_s_ri, __pyx_n_s_ind, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_q, __pyx_n_s_curr_val, __pyx_n_s_ind_doub, __pyx_n_s_at_leaf, __pyx_n_s_found_val, __pyx_n_s_isnan_array, __pyx_n_s_THRESH, __pyx_n_s_NODE_WEIGHT, __pyx_n_s_NODE_VALUE_START, __pyx_n_s_NODE_TYPE, __pyx_n_s_FEATURE_COL, __pyx_n_s_LEFT_CHILD, __pyx_n_s_RIGHT_CHILD, __pyx_n_s_NA_LEFT, __pyx_n_s_NUM_CAT_VALS, __pyx_n_s_CAT_VALS_START, __pyx_n_s_LEAF, __pyx_n_s_NUMER, __pyx_n_s_CATEG); if (unlikely(!__pyx_tuple__80)) __PYX_ERR(0, 476, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__80);
   __Pyx_GIVEREF(__pyx_tuple__80);
   __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(4, 0, 30, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__80, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_gb_multi_pyx, __pyx_n_s_predict_with_tensor_c_mc, 476, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 476, __pyx_L1_error)
 
   /* "structureboost/structure_gb_multi.pyx":543
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
- * def c_entropy_link_der_12_vec_sp(np.ndarray[np.int_t] y_true,             # <<<<<<<<<<<<<<
+ * def c_entropy_link_der_12_vec_sp(np.ndarray[np.int32_t] y_true,             # <<<<<<<<<<<<<<
  *                          double[:,:] exp_phi_pred,
  *                          double[:] exp_phi_sum_vec):
  */
   __pyx_tuple__81 = PyTuple_Pack(9, __pyx_n_s_y_true, __pyx_n_s_exp_phi_pred, __pyx_n_s_exp_phi_sum_vec, __pyx_n_s_N, __pyx_n_s_m, __pyx_n_s_Y, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k); if (unlikely(!__pyx_tuple__81)) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__81);
   __Pyx_GIVEREF(__pyx_tuple__81);
   __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__81, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_gb_multi_pyx, __pyx_n_s_c_entropy_link_der_12_vec_sp, 543, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 543, __pyx_L1_error)
 
   /* "structureboost/structure_gb_multi.pyx":566
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
- * def c_str_entropy_link_der_12_vec_sp(np.ndarray[np.int_t] y_true,             # <<<<<<<<<<<<<<
+ * def c_str_entropy_link_der_12_vec_sp(np.ndarray[np.int32_t] y_true,             # <<<<<<<<<<<<<<
  *                                  double[:,:] exp_phi_pred,
  *                                  double[:] exp_phi_sum_vec,
  */
   __pyx_tuple__82 = PyTuple_Pack(22, __pyx_n_s_y_true, __pyx_n_s_exp_phi_pred, __pyx_n_s_exp_phi_sum_vec, __pyx_n_s_weight_vec, __pyx_n_s_rp_tensor, __pyx_n_s_N, __pyx_n_s_m, __pyx_n_s_ind, __pyx_n_s_qqq, __pyx_n_s_xyz, __pyx_n_s_yval, __pyx_n_s_curr_wt, __pyx_n_s_Y, __pyx_n_s_all_sum, __pyx_n_s_set_sum, __pyx_n_s_num_part, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_t, __pyx_n_s_jt, __pyx_n_s_jk); if (unlikely(!__pyx_tuple__82)) __PYX_ERR(0, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__82);
   __Pyx_GIVEREF(__pyx_tuple__82);
   __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(5, 0, 22, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__82, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_gb_multi_pyx, __pyx_n_s_c_str_entropy_link_der_12_vec_sp, 566, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 566, __pyx_L1_error)
 
   /* "structureboost/structure_gb_multi.pyx":616
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
- * def get_one_hot_mat(np.ndarray[np.int_t] y_true,             # <<<<<<<<<<<<<<
+ * def get_one_hot_mat(np.ndarray[np.int32_t] y_true,             # <<<<<<<<<<<<<<
  *                          int num_classes):
  *     cdef int N = y_true.shape[0]
  */
   __pyx_tuple__83 = PyTuple_Pack(5, __pyx_n_s_y_true, __pyx_n_s_num_classes, __pyx_n_s_N, __pyx_n_s_Y, __pyx_n_s_i); if (unlikely(!__pyx_tuple__83)) __PYX_ERR(0, 616, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__83);
   __Pyx_GIVEREF(__pyx_tuple__83);
   __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_gb_multi_pyx, __pyx_n_s_get_one_hot_mat, 616, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 616, __pyx_L1_error)
@@ -33079,15 +33093,15 @@
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "structureboost/structure_gb_multi.pyx":267
  *         return(rpt)
  * 
  *     def _process_y_data(self, y_data):             # <<<<<<<<<<<<<<
  *         if type(y_data) == pd.Series:
- *             y_data = y_data.to_numpy().astype(np.int_)
+ *             y_data = y_data.to_numpy().astype(np.int32)
  */
   __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_14structureboost_18structure_gb_multi_19StructureBoostMulti_17_process_y_data, 0, __pyx_n_s_StructureBoostMulti__process_y_d, NULL, __pyx_n_s_structureboost_structure_gb_mult, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_process_y_data, __pyx_t_5) < 0) __PYX_ERR(0, 267, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "structureboost/structure_gb_multi.pyx":275
@@ -33278,50 +33292,50 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb_multi.pyx":476
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c_mc(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[np.int_t, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array,
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_18structure_gb_multi_1predict_with_tensor_c_mc, NULL, __pyx_n_s_structureboost_structure_gb_mult); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 476, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_predict_with_tensor_c_mc, __pyx_t_1) < 0) __PYX_ERR(0, 476, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb_multi.pyx":543
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
- * def c_entropy_link_der_12_vec_sp(np.ndarray[np.int_t] y_true,             # <<<<<<<<<<<<<<
+ * def c_entropy_link_der_12_vec_sp(np.ndarray[np.int32_t] y_true,             # <<<<<<<<<<<<<<
  *                          double[:,:] exp_phi_pred,
  *                          double[:] exp_phi_sum_vec):
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_18structure_gb_multi_3c_entropy_link_der_12_vec_sp, NULL, __pyx_n_s_structureboost_structure_gb_mult); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_c_entropy_link_der_12_vec_sp, __pyx_t_1) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb_multi.pyx":566
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
- * def c_str_entropy_link_der_12_vec_sp(np.ndarray[np.int_t] y_true,             # <<<<<<<<<<<<<<
+ * def c_str_entropy_link_der_12_vec_sp(np.ndarray[np.int32_t] y_true,             # <<<<<<<<<<<<<<
  *                                  double[:,:] exp_phi_pred,
  *                                  double[:] exp_phi_sum_vec,
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_18structure_gb_multi_5c_str_entropy_link_der_12_vec_sp, NULL, __pyx_n_s_structureboost_structure_gb_mult); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_c_str_entropy_link_der_12_vec_sp, __pyx_t_1) < 0) __PYX_ERR(0, 566, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_gb_multi.pyx":616
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
- * def get_one_hot_mat(np.ndarray[np.int_t] y_true,             # <<<<<<<<<<<<<<
+ * def get_one_hot_mat(np.ndarray[np.int32_t] y_true,             # <<<<<<<<<<<<<<
  *                          int num_classes):
  *     cdef int N = y_true.shape[0]
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_18structure_gb_multi_7get_one_hot_mat, NULL, __pyx_n_s_structureboost_structure_gb_mult); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 616, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_one_hot_mat, __pyx_t_1) < 0) __PYX_ERR(0, 616, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -38296,26 +38310,26 @@
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
 /* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsdsds_long(PyObject *obj, int writable_flag) {
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsdsds_nn___pyx_t_5numpy_int32_t(PyObject *obj, int writable_flag) {
     __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
     __Pyx_BufFmt_StackElem stack[1];
     int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
     int retcode;
     if (obj == Py_None) {
         result.memview = (struct __pyx_memoryview_obj *) Py_None;
         return result;
     }
     retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
                                                  PyBUF_RECORDS_RO | writable_flag, 3,
-                                                 &__Pyx_TypeInfo_long, stack,
+                                                 &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, stack,
                                                  &result, obj);
     if (unlikely(retcode == -1))
         goto __pyx_fail;
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
```

### Comparing `structureboost-0.4.2/structureboost/structure_rf.c` & `structureboost-0.4.3/structureboost/structure_rf.c`

 * *Files 0% similar despite different names*

```diff
@@ -2354,15 +2354,15 @@
 static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'structureboost.structure_rf' */
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int_t = { "int_t", NULL, sizeof(__pyx_t_5numpy_int_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int_t), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t = { "int32_t", NULL, sizeof(__pyx_t_5numpy_int32_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int32_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int32_t), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_long = { "long", NULL, sizeof(long), { 0 }, 0, IS_UNSIGNED(long) ? 'U' : 'I', IS_UNSIGNED(long), 0 };
 #define __Pyx_MODULE_NAME "structureboost.structure_rf"
 extern int __pyx_module_is_main_structureboost__structure_rf;
 int __pyx_module_is_main_structureboost__structure_rf = 0;
 
 /* Implementation of 'structureboost.structure_rf' */
 static PyObject *__pyx_builtin_object;
@@ -2384,15 +2384,14 @@
 static const char __pyx_k_ri[] = "ri";
 static const char __pyx_k_rw[] = "rw";
 static const char __pyx_k_all[] = "all";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_dtm[] = "dtm";
 static const char __pyx_k_fit[] = "fit";
 static const char __pyx_k_ind[] = "ind";
-static const char __pyx_k_int[] = "int_";
 static const char __pyx_k_max[] = "max";
 static const char __pyx_k_LEAF[] = "LEAF";
 static const char __pyx_k_axis[] = "axis";
 static const char __pyx_k_ceil[] = "ceil";
 static const char __pyx_k_iloc[] = "iloc";
 static const char __pyx_k_init[] = "__init__";
 static const char __pyx_k_keys[] = "keys";
@@ -2408,14 +2407,15 @@
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_warn[] = "warn";
 static const char __pyx_k_CATEG[] = "CATEG";
 static const char __pyx_k_NUMER[] = "NUMER";
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_graph[] = "graph";
+static const char __pyx_k_int32[] = "int32";
 static const char __pyx_k_isnan[] = "isnan";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_print[] = "print";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_zeros[] = "zeros";
@@ -2675,15 +2675,15 @@
 static PyObject *__pyx_n_s_graphs;
 static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_iloc;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_ind;
 static PyObject *__pyx_n_s_ind_doub;
 static PyObject *__pyx_n_s_init;
-static PyObject *__pyx_n_s_int;
+static PyObject *__pyx_n_s_int32;
 static PyObject *__pyx_n_u_interior;
 static PyObject *__pyx_n_s_interval;
 static PyObject *__pyx_n_s_inv_cti;
 static PyObject *__pyx_n_s_isnan;
 static PyObject *__pyx_n_s_isnan_array;
 static PyObject *__pyx_n_s_items;
 static PyObject *__pyx_n_s_j;
@@ -7625,27 +7625,27 @@
     __pyx_t_1 = 0;
 
     /* "structureboost/structure_rf.pyx":372
  *         if self.optimizable:
  *             cat_size = np.max(np.array([dt.get_max_split_size() for dt in self.dec_tree_list]))
  *             num_dt = len(self.dec_tree_list)             # <<<<<<<<<<<<<<
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_dec_tree_list); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_9 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_num_dt = __pyx_t_9;
 
     /* "structureboost/structure_rf.pyx":373
  *             cat_size = np.max(np.array([dt.get_max_split_size() for dt in self.dec_tree_list]))
  *             num_dt = len(self.dec_tree_list)
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))             # <<<<<<<<<<<<<<
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, 3))
  */
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 373, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_max); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 373, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
@@ -7748,15 +7748,15 @@
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_max_nodes = __pyx_t_1;
     __pyx_t_1 = 0;
 
     /* "structureboost/structure_rf.pyx":374
  *             num_dt = len(self.dec_tree_list)
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1             # <<<<<<<<<<<<<<
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1             # <<<<<<<<<<<<<<
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, 3))
  *             for i in range(num_dt):
  */
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
@@ -7781,15 +7781,15 @@
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 374, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -7799,15 +7799,15 @@
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int, __pyx_t_5) < 0) __PYX_ERR(0, 374, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
     /* "structureboost/structure_rf.pyx":375
  *             max_nodes = np.max(np.array([dt.num_nodes for dt in self.dec_tree_list]))
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, 3))             # <<<<<<<<<<<<<<
  *             for i in range(num_dt):
  *                 self.convert_dt_to_matrix(i)
  */
     __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 375, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 375, __pyx_L1_error)
@@ -7842,15 +7842,15 @@
     if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 375, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_float, __pyx_t_5) < 0) __PYX_ERR(0, 375, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
     /* "structureboost/structure_rf.pyx":376
- *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int_)-1
+ *             self.pred_tens_int = np.zeros((num_dt, max_nodes, cat_size+6), dtype=np.int32)-1
  *             self.pred_tens_float = np.zeros((num_dt, max_nodes, 3))
  *             for i in range(num_dt):             # <<<<<<<<<<<<<<
  *                 self.convert_dt_to_matrix(i)
  *             self.optimized=True
  */
     __pyx_t_9 = __pyx_v_num_dt;
     __pyx_t_13 = __pyx_t_9;
@@ -8236,16 +8236,17 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
-  int __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_8;
+  PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__14)
   __Pyx_RefNannySetupContext("convert_subtree", 0);
   __Pyx_TraceCall("convert_subtree", __pyx_f[0], 406, 0, __PYX_ERR(0, 406, __pyx_L1_error));
 
@@ -8471,213 +8472,220 @@
     }
 
     /* "structureboost/structure_rf.pyx":417
  *                 self.pred_tens_float[dt_num, ni, 0] = node['split_val']
  *                 self.pred_tens_int[dt_num, ni, 0]= 1
  *             elif node['feature_type']=='categorical_int':             # <<<<<<<<<<<<<<
  *                 setlen = len(node['left_split'])
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  */
     __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_feature_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_categorical_int, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_2) {
 
       /* "structureboost/structure_rf.pyx":418
  *                 self.pred_tens_int[dt_num, ni, 0]= 1
  *             elif node['feature_type']=='categorical_int':
  *                 setlen = len(node['left_split'])             # <<<<<<<<<<<<<<
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  *                 self.pred_tens_int[dt_num, ni, 0]= 2
  */
       __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_split); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_5 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_v_setlen = __pyx_t_1;
       __pyx_t_1 = 0;
 
       /* "structureboost/structure_rf.pyx":419
  *             elif node['feature_type']=='categorical_int':
  *                 setlen = len(node['left_split'])
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)             # <<<<<<<<<<<<<<
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)             # <<<<<<<<<<<<<<
  *                 self.pred_tens_int[dt_num, ni, 0]= 2
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen
  */
       __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_fromiter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 419, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_split); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 419, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_int32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 419, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = NULL;
-      __pyx_t_7 = 0;
+      __pyx_t_8 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
-          __pyx_t_7 = 1;
+          __pyx_t_8 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_4)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_3, ((PyObject *)(&PyInt_Type)), __pyx_v_setlen};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
+        PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_3, __pyx_t_7, __pyx_v_setlen};
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_3, ((PyObject *)(&PyInt_Type)), __pyx_v_setlen};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
+        PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_3, __pyx_t_7, __pyx_v_setlen};
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       {
-        __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 419, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_8);
+        __pyx_t_9 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 419, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_9);
         if (__pyx_t_6) {
-          __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
+          __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_6); __pyx_t_6 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_3);
-        PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
-        __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
-        __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
-        PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, ((PyObject *)(&PyInt_Type)));
+        PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_3);
+        __Pyx_GIVEREF(__pyx_t_7);
+        PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_t_7);
         __Pyx_INCREF(__pyx_v_setlen);
         __Pyx_GIVEREF(__pyx_v_setlen);
-        PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_7, __pyx_v_setlen);
+        PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_v_setlen);
         __pyx_t_3 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
+        __pyx_t_7 = 0;
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 419, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_8 = __Pyx_PyInt_AddCObj(__pyx_int_6, __pyx_v_setlen, 6, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 419, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_3 = PySlice_New(__pyx_int_6, __pyx_t_8, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 419, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_9 = __Pyx_PyInt_AddCObj(__pyx_int_6, __pyx_v_setlen, 6, 0, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 419, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __pyx_t_7 = PySlice_New(__pyx_int_6, __pyx_t_9, Py_None); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 419, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 419, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
-      PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_dt_num);
+      PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_dt_num);
       __Pyx_INCREF(__pyx_v_ni);
       __Pyx_GIVEREF(__pyx_v_ni);
-      PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_ni);
-      __Pyx_GIVEREF(__pyx_t_3);
-      PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_3);
-      __pyx_t_3 = 0;
-      if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_8, __pyx_t_1) < 0)) __PYX_ERR(0, 419, __pyx_L1_error)
+      PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_ni);
+      __Pyx_GIVEREF(__pyx_t_7);
+      PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_t_7);
+      __pyx_t_7 = 0;
+      if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_9, __pyx_t_1) < 0)) __PYX_ERR(0, 419, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
       /* "structureboost/structure_rf.pyx":420
  *                 setlen = len(node['left_split'])
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  *                 self.pred_tens_int[dt_num, ni, 0]= 2             # <<<<<<<<<<<<<<
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]
  */
       __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 420, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 420, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 420, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
-      PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_dt_num);
+      PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_dt_num);
       __Pyx_INCREF(__pyx_v_ni);
       __Pyx_GIVEREF(__pyx_v_ni);
-      PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_ni);
+      PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_ni);
       __Pyx_INCREF(__pyx_int_0);
       __Pyx_GIVEREF(__pyx_int_0);
-      PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_int_0);
-      if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_8, __pyx_int_2) < 0)) __PYX_ERR(0, 420, __pyx_L1_error)
+      PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_int_0);
+      if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_9, __pyx_int_2) < 0)) __PYX_ERR(0, 420, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
       /* "structureboost/structure_rf.pyx":421
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  *                 self.pred_tens_int[dt_num, ni, 0]= 2
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen             # <<<<<<<<<<<<<<
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']
  */
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 421, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 421, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 421, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
       PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_dt_num);
       __Pyx_INCREF(__pyx_v_ni);
       __Pyx_GIVEREF(__pyx_v_ni);
       PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_ni);
       __Pyx_INCREF(__pyx_int_5);
       __Pyx_GIVEREF(__pyx_int_5);
       PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_int_5);
-      if (unlikely(PyObject_SetItem(__pyx_t_8, __pyx_t_1, __pyx_v_setlen) < 0)) __PYX_ERR(0, 421, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      if (unlikely(PyObject_SetItem(__pyx_t_9, __pyx_t_1, __pyx_v_setlen) < 0)) __PYX_ERR(0, 421, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
       /* "structureboost/structure_rf.pyx":417
  *                 self.pred_tens_float[dt_num, ni, 0] = node['split_val']
  *                 self.pred_tens_int[dt_num, ni, 0]= 1
  *             elif node['feature_type']=='categorical_int':             # <<<<<<<<<<<<<<
  *                 setlen = len(node['left_split'])
- *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], int, setlen)
+ *                 self.pred_tens_int[dt_num, ni, 6:6+setlen] = np.fromiter(node['left_split'], np.int32, setlen)
  */
     }
     __pyx_L4:;
 
     /* "structureboost/structure_rf.pyx":422
  *                 self.pred_tens_int[dt_num, ni, 0]= 2
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]             # <<<<<<<<<<<<<<
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 3]=node['right_child']['node_index']
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_column_to_int_dict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_split_feature); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 422, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 422, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_split_feature); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 422, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 422, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 422, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_dt_num);
     __Pyx_GIVEREF(__pyx_v_dt_num);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_dt_num);
     __Pyx_INCREF(__pyx_v_ni);
     __Pyx_GIVEREF(__pyx_v_ni);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_ni);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_int_1);
-    if (unlikely(PyObject_SetItem(__pyx_t_8, __pyx_t_1, __pyx_t_4) < 0)) __PYX_ERR(0, 422, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (unlikely(PyObject_SetItem(__pyx_t_9, __pyx_t_1, __pyx_t_4) < 0)) __PYX_ERR(0, 422, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "structureboost/structure_rf.pyx":423
  *                 self.pred_tens_int[dt_num, ni, 5]= setlen
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']             # <<<<<<<<<<<<<<
@@ -8687,206 +8695,206 @@
     __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_child); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 423, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_n_u_node_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 423, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 423, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 423, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 423, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_INCREF(__pyx_v_dt_num);
     __Pyx_GIVEREF(__pyx_v_dt_num);
-    PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_dt_num);
+    PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_dt_num);
     __Pyx_INCREF(__pyx_v_ni);
     __Pyx_GIVEREF(__pyx_v_ni);
-    PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_ni);
+    PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_v_ni);
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_GIVEREF(__pyx_int_2);
-    PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_int_2);
-    if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_8, __pyx_t_1) < 0)) __PYX_ERR(0, 423, __pyx_L1_error)
+    PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_int_2);
+    if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_9, __pyx_t_1) < 0)) __PYX_ERR(0, 423, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "structureboost/structure_rf.pyx":424
  *             self.pred_tens_int[dt_num, ni, 1]=self.column_to_int_dict[node['split_feature']]
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 3]=node['right_child']['node_index']             # <<<<<<<<<<<<<<
  *             self.pred_tens_int[dt_num, ni, 4]=node['na_left']
  *             self.convert_subtree(node['left_child'], dt_num)
  */
     __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_right_child); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 424, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_node_index); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 424, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_node_index); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 424, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 424, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 424, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_dt_num);
     __Pyx_GIVEREF(__pyx_v_dt_num);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_dt_num);
     __Pyx_INCREF(__pyx_v_ni);
     __Pyx_GIVEREF(__pyx_v_ni);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_ni);
     __Pyx_INCREF(__pyx_int_3);
     __Pyx_GIVEREF(__pyx_int_3);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_int_3);
-    if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_4, __pyx_t_8) < 0)) __PYX_ERR(0, 424, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_t_4, __pyx_t_9) < 0)) __PYX_ERR(0, 424, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
     /* "structureboost/structure_rf.pyx":425
  *             self.pred_tens_int[dt_num, ni, 2]=node['left_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 3]=node['right_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 4]=node['na_left']             # <<<<<<<<<<<<<<
  *             self.convert_subtree(node['left_child'], dt_num)
  *             self.convert_subtree(node['right_child'], dt_num)
  */
-    __pyx_t_8 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_na_left); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 425, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_na_left); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 425, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pred_tens_int); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 425, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 425, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_dt_num);
     __Pyx_GIVEREF(__pyx_v_dt_num);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_dt_num);
     __Pyx_INCREF(__pyx_v_ni);
     __Pyx_GIVEREF(__pyx_v_ni);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_ni);
     __Pyx_INCREF(__pyx_int_4);
     __Pyx_GIVEREF(__pyx_int_4);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_int_4);
-    if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_1, __pyx_t_8) < 0)) __PYX_ERR(0, 425, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_t_4, __pyx_t_1, __pyx_t_9) < 0)) __PYX_ERR(0, 425, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
     /* "structureboost/structure_rf.pyx":426
  *             self.pred_tens_int[dt_num, ni, 3]=node['right_child']['node_index']
  *             self.pred_tens_int[dt_num, ni, 4]=node['na_left']
  *             self.convert_subtree(node['left_child'], dt_num)             # <<<<<<<<<<<<<<
  *             self.convert_subtree(node['right_child'], dt_num)
  * 
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_convert_subtree); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 426, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_left_child); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 426, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = NULL;
-    __pyx_t_7 = 0;
+    __pyx_t_7 = NULL;
+    __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_3)) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_3);
+        __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
-        __pyx_t_7 = 1;
+        __pyx_t_8 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_4, __pyx_v_dt_num};
-      __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 426, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
+      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_4, __pyx_v_dt_num};
+      __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 426, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_t_4, __pyx_v_dt_num};
-      __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 426, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
+      PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_4, __pyx_v_dt_num};
+      __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 426, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     {
-      __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 426, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      if (__pyx_t_3) {
-        __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3); __pyx_t_3 = NULL;
+      __pyx_t_3 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 426, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      if (__pyx_t_7) {
+        __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_7); __pyx_t_7 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_4);
-      PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_7, __pyx_t_4);
+      PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_8, __pyx_t_4);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
-      PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_7, __pyx_v_dt_num);
+      PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_8, __pyx_v_dt_num);
       __pyx_t_4 = 0;
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 426, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 426, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
     /* "structureboost/structure_rf.pyx":427
  *             self.pred_tens_int[dt_num, ni, 4]=node['na_left']
  *             self.convert_subtree(node['left_child'], dt_num)
  *             self.convert_subtree(node['right_child'], dt_num)             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_convert_subtree); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_right_child); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_v_node, __pyx_n_u_right_child); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 427, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
-    __pyx_t_7 = 0;
+    __pyx_t_8 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
-        __pyx_t_7 = 1;
+        __pyx_t_8 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_6, __pyx_v_dt_num};
-      __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 427, __pyx_L1_error)
+      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_3, __pyx_v_dt_num};
+      __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 427, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_6, __pyx_v_dt_num};
-      __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 427, __pyx_L1_error)
+      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_3, __pyx_v_dt_num};
+      __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 427, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else
     #endif
     {
-      __pyx_t_3 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 427, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_7 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 427, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       if (__pyx_t_4) {
-        __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4); __pyx_t_4 = NULL;
+        __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
-      __Pyx_GIVEREF(__pyx_t_6);
-      PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_7, __pyx_t_6);
+      __Pyx_GIVEREF(__pyx_t_3);
+      PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_8, __pyx_t_3);
       __Pyx_INCREF(__pyx_v_dt_num);
       __Pyx_GIVEREF(__pyx_v_dt_num);
-      PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_7, __pyx_v_dt_num);
-      __pyx_t_6 = 0;
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 427, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_8, __pyx_v_dt_num);
+      __pyx_t_3 = 0;
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 427, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __pyx_L3:;
 
   /* "structureboost/structure_rf.pyx":406
  *         self.convert_subtree(curr_node, dt_num)
  * 
  *     def convert_subtree(self, node, dt_num):             # <<<<<<<<<<<<<<
@@ -8898,15 +8906,16 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("structureboost.structure_rf.StructureRF.convert_subtree", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ni);
   __Pyx_XDECREF(__pyx_v_setlen);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
@@ -9647,15 +9656,15 @@
   return __pyx_r;
 }
 
 /* "structureboost/structure_rf.pyx":457
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[np.int_t, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_12structure_rf_5predict_with_tensor_c(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_12structure_rf_5predict_with_tensor_c = {"predict_with_tensor_c", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_12structure_rf_5predict_with_tensor_c, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_12structure_rf_5predict_with_tensor_c(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -9790,15 +9799,15 @@
   long __pyx_t_13;
   int __pyx_t_14;
   Py_ssize_t __pyx_t_15;
   Py_ssize_t __pyx_t_16;
   Py_ssize_t __pyx_t_17;
   Py_ssize_t __pyx_t_18;
   Py_ssize_t __pyx_t_19;
-  __pyx_t_5numpy_int_t __pyx_t_20;
+  __pyx_t_5numpy_int32_t __pyx_t_20;
   Py_ssize_t __pyx_t_21;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceFrameInit(__pyx_codeobj__17)
   __Pyx_RefNannySetupContext("predict_with_tensor_c", 0);
   __Pyx_TraceCall("predict_with_tensor_c", __pyx_f[0], 457, 0, __PYX_ERR(0, 457, __pyx_L1_error));
@@ -9825,15 +9834,15 @@
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm_float.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm_float, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 457, __pyx_L1_error)
   }
   __pyx_pybuffernd_dtm_float.diminfo[0].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_dtm_float.diminfo[0].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_dtm_float.diminfo[1].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_dtm_float.diminfo[1].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_dtm_float.diminfo[2].strides = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_dtm_float.diminfo[2].shape = __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.shape[2];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 457, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_dtm.rcbuffer->pybuffer, (PyObject*)__pyx_v_dtm, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) __PYX_ERR(0, 457, __pyx_L1_error)
   }
   __pyx_pybuffernd_dtm.diminfo[0].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_dtm.diminfo[0].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_dtm.diminfo[1].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_dtm.diminfo[1].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_dtm.diminfo[2].strides = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_dtm.diminfo[2].shape = __pyx_pybuffernd_dtm.rcbuffer->pybuffer.shape[2];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feat_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_feat_array, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 457, __pyx_L1_error)
   }
   __pyx_pybuffernd_feat_array.diminfo[0].strides = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_feat_array.diminfo[0].shape = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_feat_array.diminfo[1].strides = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_feat_array.diminfo[1].shape = __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.shape[1];
@@ -10118,15 +10127,15 @@
  *                 if dtm[k,cn, NODE_TYPE]==LEAF:             # <<<<<<<<<<<<<<
  *                     at_leaf = 1
  *                     res_mat[ri,k] = dtm_float[k,cn, NODE_VALUE]
  */
         __pyx_t_15 = __pyx_v_k;
         __pyx_t_16 = __pyx_v_cn;
         __pyx_t_17 = __pyx_v_NODE_TYPE;
-        __pyx_t_14 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_LEAF) != 0);
+        __pyx_t_14 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_LEAF) != 0);
         if (__pyx_t_14) {
 
           /* "structureboost/structure_rf.pyx":493
  *                 cn = int(cn)
  *                 if dtm[k,cn, NODE_TYPE]==LEAF:
  *                     at_leaf = 1             # <<<<<<<<<<<<<<
  *                     res_mat[ri,k] = dtm_float[k,cn, NODE_VALUE]
@@ -10164,28 +10173,28 @@
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:             # <<<<<<<<<<<<<<
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:
  */
         __pyx_t_15 = __pyx_v_k;
         __pyx_t_16 = __pyx_v_cn;
         __pyx_t_17 = __pyx_v_NODE_TYPE;
-        __pyx_t_14 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_NUMER) != 0);
+        __pyx_t_14 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_NUMER) != 0);
         if (__pyx_t_14) {
 
           /* "structureboost/structure_rf.pyx":496
  *                     res_mat[ri,k] = dtm_float[k,cn, NODE_VALUE]
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]             # <<<<<<<<<<<<<<
  *                     if isnan_array[ri,ind]:
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]
  */
           __pyx_t_17 = __pyx_v_k;
           __pyx_t_16 = __pyx_v_cn;
           __pyx_t_15 = __pyx_v_FEATURE_COL;
-          __pyx_v_ind = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides));
+          __pyx_v_ind = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides));
 
           /* "structureboost/structure_rf.pyx":497
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:             # <<<<<<<<<<<<<<
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]
  *                     else:
@@ -10201,24 +10210,24 @@
  *                         cn = dtm[k,cn, LEFT_CHILD] if dtm[k,cn, NA_LEFT] else dtm[k,cn, RIGHT_CHILD]             # <<<<<<<<<<<<<<
  *                     else:
  *                         curr_val = feat_array[ri,ind]
  */
             __pyx_t_16 = __pyx_v_k;
             __pyx_t_15 = __pyx_v_cn;
             __pyx_t_17 = __pyx_v_NA_LEFT;
-            if (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides)) != 0)) {
+            if (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[2].strides)) != 0)) {
               __pyx_t_19 = __pyx_v_k;
               __pyx_t_18 = __pyx_v_cn;
               __pyx_t_21 = __pyx_v_LEFT_CHILD;
-              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[2].strides));
             } else {
               __pyx_t_21 = __pyx_v_k;
               __pyx_t_18 = __pyx_v_cn;
               __pyx_t_19 = __pyx_v_RIGHT_CHILD;
-              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[2].strides));
             }
             __pyx_v_cn = __pyx_t_20;
 
             /* "structureboost/structure_rf.pyx":497
  *                 elif dtm[k,cn, NODE_TYPE]==NUMER:
  *                     ind = dtm[k,cn, FEATURE_COL]
  *                     if isnan_array[ri,ind]:             # <<<<<<<<<<<<<<
@@ -10250,20 +10259,20 @@
             __pyx_t_15 = __pyx_v_k;
             __pyx_t_17 = __pyx_v_cn;
             __pyx_t_16 = __pyx_v_THRESH;
             if (((__pyx_v_curr_val < (*__Pyx_BufPtrStrided3d(double *, __pyx_pybuffernd_dtm_float.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm_float.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm_float.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm_float.diminfo[2].strides))) != 0)) {
               __pyx_t_19 = __pyx_v_k;
               __pyx_t_18 = __pyx_v_cn;
               __pyx_t_21 = __pyx_v_LEFT_CHILD;
-              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[2].strides));
             } else {
               __pyx_t_21 = __pyx_v_k;
               __pyx_t_18 = __pyx_v_cn;
               __pyx_t_19 = __pyx_v_RIGHT_CHILD;
-              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[2].strides));
+              __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_19, __pyx_pybuffernd_dtm.diminfo[2].strides));
             }
             __pyx_v_cn = __pyx_t_20;
           }
           __pyx_L10:;
 
           /* "structureboost/structure_rf.pyx":495
  *                     at_leaf = 1
@@ -10281,29 +10290,29 @@
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:             # <<<<<<<<<<<<<<
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]
  *                     found_val = 0
  */
         __pyx_t_16 = __pyx_v_k;
         __pyx_t_17 = __pyx_v_cn;
         __pyx_t_15 = __pyx_v_NODE_TYPE;
-        __pyx_t_14 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_CATEG) != 0);
+        __pyx_t_14 = (((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides)) == __pyx_v_CATEG) != 0);
         if (__pyx_t_14) {
 
           /* "structureboost/structure_rf.pyx":503
  *                         cn = dtm[k,cn, LEFT_CHILD] if curr_val<dtm_float[k,cn, THRESH] else dtm[k,cn, RIGHT_CHILD]
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]             # <<<<<<<<<<<<<<
  *                     found_val = 0
  *                     j = CAT_VALS_START
  */
           __pyx_t_15 = __pyx_v_k;
           __pyx_t_17 = __pyx_v_cn;
           __pyx_t_16 = __pyx_v_FEATURE_COL;
           __pyx_t_19 = __pyx_v_ri;
-          __pyx_t_18 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
+          __pyx_t_18 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
           __pyx_v_curr_val = (*__Pyx_BufPtrStrided2d(double *, __pyx_pybuffernd_feat_array.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_feat_array.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_feat_array.diminfo[1].strides));
 
           /* "structureboost/structure_rf.pyx":504
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:
  *                     curr_val = feat_array[ri,dtm[k,cn, FEATURE_COL]]
  *                     found_val = 0             # <<<<<<<<<<<<<<
  *                     j = CAT_VALS_START
@@ -10326,15 +10335,15 @@
  *                     cat_vals_end = CAT_VALS_START + dtm[k, cn, NUM_CAT_VALS]             # <<<<<<<<<<<<<<
  *                     while ((not found_val) & (j<cat_vals_end)):
  *                         if curr_val==dtm[k,cn, j]:
  */
           __pyx_t_16 = __pyx_v_k;
           __pyx_t_17 = __pyx_v_cn;
           __pyx_t_15 = __pyx_v_NUM_CAT_VALS;
-          __pyx_v_cat_vals_end = (__pyx_v_CAT_VALS_START + (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides)));
+          __pyx_v_cat_vals_end = (__pyx_v_CAT_VALS_START + (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides)));
 
           /* "structureboost/structure_rf.pyx":507
  *                     j = CAT_VALS_START
  *                     cat_vals_end = CAT_VALS_START + dtm[k, cn, NUM_CAT_VALS]
  *                     while ((not found_val) & (j<cat_vals_end)):             # <<<<<<<<<<<<<<
  *                         if curr_val==dtm[k,cn, j]:
  *                             found_val=1
@@ -10349,15 +10358,15 @@
  *                         if curr_val==dtm[k,cn, j]:             # <<<<<<<<<<<<<<
  *                             found_val=1
  *                         else:
  */
             __pyx_t_15 = __pyx_v_k;
             __pyx_t_17 = __pyx_v_cn;
             __pyx_t_16 = __pyx_v_j;
-            __pyx_t_14 = ((__pyx_v_curr_val == (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides))) != 0);
+            __pyx_t_14 = ((__pyx_v_curr_val == (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides))) != 0);
             if (__pyx_t_14) {
 
               /* "structureboost/structure_rf.pyx":509
  *                     while ((not found_val) & (j<cat_vals_end)):
  *                         if curr_val==dtm[k,cn, j]:
  *                             found_val=1             # <<<<<<<<<<<<<<
  *                         else:
@@ -10394,20 +10403,20 @@
  *                     cn = dtm[k,cn, LEFT_CHILD] if found_val else dtm[k,cn, RIGHT_CHILD]             # <<<<<<<<<<<<<<
  *     return(res_mat)
  */
           if ((__pyx_v_found_val != 0)) {
             __pyx_t_16 = __pyx_v_k;
             __pyx_t_17 = __pyx_v_cn;
             __pyx_t_15 = __pyx_v_LEFT_CHILD;
-            __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides));
+            __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[2].strides));
           } else {
             __pyx_t_15 = __pyx_v_k;
             __pyx_t_17 = __pyx_v_cn;
             __pyx_t_16 = __pyx_v_RIGHT_CHILD;
-            __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
+            __pyx_t_20 = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_dtm.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_dtm.diminfo[0].strides, __pyx_t_17, __pyx_pybuffernd_dtm.diminfo[1].strides, __pyx_t_16, __pyx_pybuffernd_dtm.diminfo[2].strides));
           }
           __pyx_v_cn = __pyx_t_20;
 
           /* "structureboost/structure_rf.pyx":502
  *                         curr_val = feat_array[ri,ind]
  *                         cn = dtm[k,cn, LEFT_CHILD] if curr_val<dtm_float[k,cn, THRESH] else dtm[k,cn, RIGHT_CHILD]
  *                 elif dtm[k,cn, NODE_TYPE]==CATEG:             # <<<<<<<<<<<<<<
@@ -10430,15 +10439,15 @@
   __pyx_r = ((PyObject *)__pyx_v_res_mat);
   goto __pyx_L0;
 
   /* "structureboost/structure_rf.pyx":457
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[np.int_t, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -11729,15 +11738,15 @@
   {&__pyx_n_s_graphs, __pyx_k_graphs, sizeof(__pyx_k_graphs), 0, 0, 1, 1},
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_iloc, __pyx_k_iloc, sizeof(__pyx_k_iloc), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_ind, __pyx_k_ind, sizeof(__pyx_k_ind), 0, 0, 1, 1},
   {&__pyx_n_s_ind_doub, __pyx_k_ind_doub, sizeof(__pyx_k_ind_doub), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
-  {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
+  {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
   {&__pyx_n_u_interior, __pyx_k_interior, sizeof(__pyx_k_interior), 0, 1, 0, 1},
   {&__pyx_n_s_interval, __pyx_k_interval, sizeof(__pyx_k_interval), 0, 0, 1, 1},
   {&__pyx_n_s_inv_cti, __pyx_k_inv_cti, sizeof(__pyx_k_inv_cti), 0, 0, 1, 1},
   {&__pyx_n_s_isnan, __pyx_k_isnan, sizeof(__pyx_k_isnan), 0, 0, 1, 1},
   {&__pyx_n_s_isnan_array, __pyx_k_isnan_array, sizeof(__pyx_k_isnan_array), 0, 0, 1, 1},
   {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
   {&__pyx_n_s_j, __pyx_k_j, sizeof(__pyx_k_j), 0, 0, 1, 1},
@@ -12086,15 +12095,15 @@
   __Pyx_GIVEREF(__pyx_tuple__35);
   __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_rf_pyx, __pyx_n_s_randomize_node_na_dir_weighted, 442, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 442, __pyx_L1_error)
 
   /* "structureboost/structure_rf.pyx":457
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[np.int_t, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array):
  */
   __pyx_tuple__36 = PyTuple_Pack(27, __pyx_n_s_dtm_float, __pyx_n_s_dtm, __pyx_n_s_feat_array, __pyx_n_s_cat_vals_end, __pyx_n_s_res_mat, __pyx_n_s_cn, __pyx_n_s_ri, __pyx_n_s_ind, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_curr_val, __pyx_n_s_ind_doub, __pyx_n_s_at_leaf, __pyx_n_s_found_val, __pyx_n_s_isnan_array, __pyx_n_s_THRESH, __pyx_n_s_NODE_VALUE, __pyx_n_s_NODE_TYPE, __pyx_n_s_FEATURE_COL, __pyx_n_s_LEFT_CHILD, __pyx_n_s_RIGHT_CHILD, __pyx_n_s_NA_LEFT, __pyx_n_s_NUM_CAT_VALS, __pyx_n_s_CAT_VALS_START, __pyx_n_s_LEAF, __pyx_n_s_NUMER, __pyx_n_s_CATEG); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__36);
   __Pyx_GIVEREF(__pyx_tuple__36);
   __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 27, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_rf_pyx, __pyx_n_s_predict_with_tensor_c, 457, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
@@ -12738,15 +12747,15 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_randomize_node_na_dir_weighted, __pyx_t_1) < 0) __PYX_ERR(0, 442, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_rf.pyx":457
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def predict_with_tensor_c(np.ndarray[double, ndim=3] dtm_float,             # <<<<<<<<<<<<<<
- *                       np.ndarray[np.int_t, ndim=3] dtm,
+ *                       np.ndarray[np.int32_t, ndim=3] dtm,
  *                       np.ndarray[double, ndim=2] feat_array):
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_12structure_rf_5predict_with_tensor_c, NULL, __pyx_n_s_structureboost_structure_rf); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_predict_with_tensor_c, __pyx_t_1) < 0) __PYX_ERR(0, 457, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `structureboost-0.4.2/structureboost/structure_rfdt.c` & `structureboost-0.4.3/structureboost/structure_rfdt.c`

 * *Files 0% similar despite different names*

```diff
@@ -2231,15 +2231,15 @@
 static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
 /* Module declarations from 'cython' */
 
 /* Module declarations from 'structureboost.structure_rfdt' */
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
-static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int_t = { "int_t", NULL, sizeof(__pyx_t_5numpy_int_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int_t), 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t = { "int32_t", NULL, sizeof(__pyx_t_5numpy_int32_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int32_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int32_t), 0 };
 #define __Pyx_MODULE_NAME "structureboost.structure_rfdt"
 extern int __pyx_module_is_main_structureboost__structure_rfdt;
 int __pyx_module_is_main_structureboost__structure_rfdt = 0;
 
 /* Implementation of 'structureboost.structure_rfdt' */
 static PyObject *__pyx_builtin_super;
 static PyObject *__pyx_builtin_range;
@@ -2254,15 +2254,14 @@
 static const char __pyx_k_sp[] = "sp";
 static const char __pyx_k_cbl[] = "cbl";
 static const char __pyx_k_cbr[] = "cbr";
 static const char __pyx_k_cbt[] = "cbt";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_eps[] = "eps";
 static const char __pyx_k_inf[] = "inf";
-static const char __pyx_k_int[] = "int_";
 static const char __pyx_k_log[] = "log";
 static const char __pyx_k_mls[] = "mls";
 static const char __pyx_k_sum[] = "sum";
 static const char __pyx_k_ysl[] = "ysl";
 static const char __pyx_k_ysr[] = "ysr";
 static const char __pyx_k_yst[] = "yst";
 static const char __pyx_k_axis[] = "axis";
@@ -2280,14 +2279,15 @@
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_side[] = "side";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_depth[] = "depth";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_gamma[] = "gamma";
+static const char __pyx_k_int32[] = "int32";
 static const char __pyx_k_isnan[] = "isnan";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_right[] = "right";
 static const char __pyx_k_scipy[] = "scipy";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_super[] = "super";
@@ -2492,15 +2492,15 @@
 static PyObject *__pyx_n_u_graphical_voronoi;
 static PyObject *__pyx_n_s_graphs;
 static PyObject *__pyx_n_s_has_na_vals;
 static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_inf;
 static PyObject *__pyx_n_s_init;
-static PyObject *__pyx_n_s_int;
+static PyObject *__pyx_n_s_int32;
 static PyObject *__pyx_n_s_isnan;
 static PyObject *__pyx_n_s_j;
 static PyObject *__pyx_n_s_leaf_vertex_ind;
 static PyObject *__pyx_n_s_left_feat_values;
 static PyObject *__pyx_n_s_left_mean;
 static PyObject *__pyx_n_s_left_split;
 static PyObject *__pyx_n_s_log;
@@ -3669,75 +3669,75 @@
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_rfdt.pyx":65
  * 
  *         has_na_vals = np.isnan(split_vec[-1])
  *         bin_result_vec = np.searchsorted(split_vec,             # <<<<<<<<<<<<<<
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_searchsorted); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "structureboost/structure_rfdt.pyx":66
  *         has_na_vals = np.isnan(split_vec[-1])
  *         bin_result_vec = np.searchsorted(split_vec,
  *                                          feature_vec,             # <<<<<<<<<<<<<<
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  *         y_sum_bins, count_in_bins = get_bin_sums_c_rfbin(y_c_mat[:,0],
  */
   __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_split_vec);
   __Pyx_GIVEREF(__pyx_v_split_vec);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_split_vec);
   __Pyx_INCREF(__pyx_v_feature_vec);
   __Pyx_GIVEREF(__pyx_v_feature_vec);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_feature_vec);
 
   /* "structureboost/structure_rfdt.pyx":67
  *         bin_result_vec = np.searchsorted(split_vec,
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)             # <<<<<<<<<<<<<<
+ *                                          side='right').astype(np.int32)             # <<<<<<<<<<<<<<
  *         y_sum_bins, count_in_bins = get_bin_sums_c_rfbin(y_c_mat[:,0],
  *                                                 bin_result_vec,
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_side, __pyx_n_u_right) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
 
   /* "structureboost/structure_rfdt.pyx":65
  * 
  *         has_na_vals = np.isnan(split_vec[-1])
  *         bin_result_vec = np.searchsorted(split_vec,             # <<<<<<<<<<<<<<
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  */
   __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "structureboost/structure_rfdt.pyx":67
  *         bin_result_vec = np.searchsorted(split_vec,
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)             # <<<<<<<<<<<<<<
+ *                                          side='right').astype(np.int32)             # <<<<<<<<<<<<<<
  *         y_sum_bins, count_in_bins = get_bin_sums_c_rfbin(y_c_mat[:,0],
  *                                                 bin_result_vec,
  */
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -3753,15 +3753,15 @@
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_bin_result_vec = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "structureboost/structure_rfdt.pyx":68
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  *         y_sum_bins, count_in_bins = get_bin_sums_c_rfbin(y_c_mat[:,0],             # <<<<<<<<<<<<<<
  *                                                 bin_result_vec,
  *                                                 len(split_vec)+1)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_get_bin_sums_c_rfbin); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_y_c_mat, __pyx_tuple__4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
@@ -3874,15 +3874,15 @@
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
     __PYX_ERR(0, 68, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
 
   /* "structureboost/structure_rfdt.pyx":68
  *                                          feature_vec,
- *                                          side='right').astype(np.int_)
+ *                                          side='right').astype(np.int32)
  *         y_sum_bins, count_in_bins = get_bin_sums_c_rfbin(y_c_mat[:,0],             # <<<<<<<<<<<<<<
  *                                                 bin_result_vec,
  *                                                 len(split_vec)+1)
  */
   __pyx_v_y_sum_bins = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_v_count_in_bins = __pyx_t_8;
@@ -5730,15 +5730,15 @@
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
       /* "structureboost/structure_rfdt.pyx":137
  *                                             y_c_sum[0]-y_left,
  *                                             c_left, y_c_sum[1]-c_left,
  *                                             float(self.min_leaf_size))             # <<<<<<<<<<<<<<
  *             elif feature_type in ['categorical_int','graphical_voronoi']:
- *                 fs_array = np.fromiter(left_feat_values, int,
+ *                 fs_array = np.fromiter(left_feat_values, np.int32,
  */
       __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_min_leaf_size); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 137, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_4 = __Pyx_PyNumber_Float(__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 137, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_t_9 = NULL;
@@ -5822,16 +5822,16 @@
       goto __pyx_L4;
     }
 
     /* "structureboost/structure_rfdt.pyx":138
  *                                             c_left, y_c_sum[1]-c_left,
  *                                             float(self.min_leaf_size))
  *             elif feature_type in ['categorical_int','graphical_voronoi']:             # <<<<<<<<<<<<<<
- *                 fs_array = np.fromiter(left_feat_values, int,
- *                 len(left_feat_values)).astype(np.int_)
+ *                 fs_array = np.fromiter(left_feat_values, np.int32,
+ *                 len(left_feat_values)).astype(np.int32)
  */
     __Pyx_INCREF(__pyx_v_feature_type);
     __pyx_t_1 = __pyx_v_feature_type;
     __pyx_t_11 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_categorical_int, Py_EQ)); if (unlikely(__pyx_t_11 < 0)) __PYX_ERR(0, 138, __pyx_L1_error)
     if (!__pyx_t_11) {
     } else {
       __pyx_t_3 = __pyx_t_11;
@@ -5843,214 +5843,221 @@
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_11 = (__pyx_t_3 != 0);
     if (__pyx_t_11) {
 
       /* "structureboost/structure_rfdt.pyx":139
  *                                             float(self.min_leaf_size))
  *             elif feature_type in ['categorical_int','graphical_voronoi']:
- *                 fs_array = np.fromiter(left_feat_values, int,             # <<<<<<<<<<<<<<
- *                 len(left_feat_values)).astype(np.int_)
+ *                 fs_array = np.fromiter(left_feat_values, np.int32,             # <<<<<<<<<<<<<<
+ *                 len(left_feat_values)).astype(np.int32)
  *                 vec_len = len(feature_vec_node)
  */
       __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_fromiter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 139, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 139, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 139, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
       /* "structureboost/structure_rfdt.pyx":140
  *             elif feature_type in ['categorical_int','graphical_voronoi']:
- *                 fs_array = np.fromiter(left_feat_values, int,
- *                 len(left_feat_values)).astype(np.int_)             # <<<<<<<<<<<<<<
+ *                 fs_array = np.fromiter(left_feat_values, np.int32,
+ *                 len(left_feat_values)).astype(np.int32)             # <<<<<<<<<<<<<<
  *                 vec_len = len(feature_vec_node)
  *                 lsplit_len = len(fs_array)
  */
       __pyx_t_12 = PyObject_Length(__pyx_v_left_feat_values); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1))) __PYX_ERR(0, 140, __pyx_L1_error)
       __pyx_t_10 = PyInt_FromSsize_t(__pyx_t_12); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 140, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_5 = NULL;
+      __pyx_t_6 = NULL;
       __pyx_t_8 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
-        if (likely(__pyx_t_5)) {
+        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-          __Pyx_INCREF(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
           __pyx_t_8 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_4)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_v_left_feat_values, ((PyObject *)(&PyInt_Type)), __pyx_t_10};
+        PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_v_left_feat_values, __pyx_t_5, __pyx_t_10};
         __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-        PyObject *__pyx_temp[4] = {__pyx_t_5, __pyx_v_left_feat_values, ((PyObject *)(&PyInt_Type)), __pyx_t_10};
+        PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_v_left_feat_values, __pyx_t_5, __pyx_t_10};
         __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
-        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       } else
       #endif
       {
-        __pyx_t_6 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 139, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        if (__pyx_t_5) {
-          __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5); __pyx_t_5 = NULL;
+        __pyx_t_7 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 139, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        if (__pyx_t_6) {
+          __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_6); __pyx_t_6 = NULL;
         }
         __Pyx_INCREF(__pyx_v_left_feat_values);
         __Pyx_GIVEREF(__pyx_v_left_feat_values);
-        PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_8, __pyx_v_left_feat_values);
-        __Pyx_INCREF(((PyObject *)(&PyInt_Type)));
-        __Pyx_GIVEREF(((PyObject *)(&PyInt_Type)));
-        PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_8, ((PyObject *)(&PyInt_Type)));
+        PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_8, __pyx_v_left_feat_values);
+        __Pyx_GIVEREF(__pyx_t_5);
+        PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_8, __pyx_t_5);
         __Pyx_GIVEREF(__pyx_t_10);
-        PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_8, __pyx_t_10);
+        PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_8, __pyx_t_10);
+        __pyx_t_5 = 0;
         __pyx_t_10 = 0;
-        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 140, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 140, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_2 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_2)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_2);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
-      __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6);
+      __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_7);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_v_fs_array = __pyx_t_1;
       __pyx_t_1 = 0;
 
       /* "structureboost/structure_rfdt.pyx":141
- *                 fs_array = np.fromiter(left_feat_values, int,
- *                 len(left_feat_values)).astype(np.int_)
+ *                 fs_array = np.fromiter(left_feat_values, np.int32,
+ *                 len(left_feat_values)).astype(np.int32)
  *                 vec_len = len(feature_vec_node)             # <<<<<<<<<<<<<<
  *                 lsplit_len = len(fs_array)
- *                 mask = np.zeros(vec_len, dtype=np.int_)
+ *                 mask = np.zeros(vec_len, dtype=np.int32)
  */
       __pyx_t_12 = PyObject_Length(__pyx_v_feature_vec_node); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1))) __PYX_ERR(0, 141, __pyx_L1_error)
       __pyx_v_vec_len = __pyx_t_12;
 
       /* "structureboost/structure_rfdt.pyx":142
- *                 len(left_feat_values)).astype(np.int_)
+ *                 len(left_feat_values)).astype(np.int32)
  *                 vec_len = len(feature_vec_node)
  *                 lsplit_len = len(fs_array)             # <<<<<<<<<<<<<<
- *                 mask = np.zeros(vec_len, dtype=np.int_)
- *                 mask = get_mask_int_c(feature_vec_node.astype(np.int_),
+ *                 mask = np.zeros(vec_len, dtype=np.int32)
+ *                 mask = get_mask_int_c(feature_vec_node.astype(np.int32),
  */
       __pyx_t_12 = PyObject_Length(__pyx_v_fs_array); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1))) __PYX_ERR(0, 142, __pyx_L1_error)
       __pyx_v_lsplit_len = __pyx_t_12;
 
       /* "structureboost/structure_rfdt.pyx":143
  *                 vec_len = len(feature_vec_node)
  *                 lsplit_len = len(fs_array)
- *                 mask = np.zeros(vec_len, dtype=np.int_)             # <<<<<<<<<<<<<<
- *                 mask = get_mask_int_c(feature_vec_node.astype(np.int_),
+ *                 mask = np.zeros(vec_len, dtype=np.int32)             # <<<<<<<<<<<<<<
+ *                 mask = get_mask_int_c(feature_vec_node.astype(np.int32),
  *                                fs_array, vec_len, lsplit_len,
  */
       __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_vec_len); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 143, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 143, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_1);
-      PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
+      PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_1);
       __pyx_t_1 = 0;
       __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 143, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_10) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 143, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_v_mask = __pyx_t_10;
       __pyx_t_10 = 0;
 
       /* "structureboost/structure_rfdt.pyx":144
  *                 lsplit_len = len(fs_array)
- *                 mask = np.zeros(vec_len, dtype=np.int_)
- *                 mask = get_mask_int_c(feature_vec_node.astype(np.int_),             # <<<<<<<<<<<<<<
+ *                 mask = np.zeros(vec_len, dtype=np.int32)
+ *                 mask = get_mask_int_c(feature_vec_node.astype(np.int32),             # <<<<<<<<<<<<<<
  *                                fs_array, vec_len, lsplit_len,
  *                                mask)
  */
       __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_mask_int_c); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_feature_vec_node, __pyx_n_s_astype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 144, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 144, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 144, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_2 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_2)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_2);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
-      __pyx_t_6 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
+      __pyx_t_7 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 144, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 144, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
       /* "structureboost/structure_rfdt.pyx":145
- *                 mask = np.zeros(vec_len, dtype=np.int_)
- *                 mask = get_mask_int_c(feature_vec_node.astype(np.int_),
+ *                 mask = np.zeros(vec_len, dtype=np.int32)
+ *                 mask = get_mask_int_c(feature_vec_node.astype(np.int32),
  *                                fs_array, vec_len, lsplit_len,             # <<<<<<<<<<<<<<
  *                                mask)
  * 
  */
       __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_vec_len); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_lsplit_len); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 145, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
 
       /* "structureboost/structure_rfdt.pyx":146
- *                 mask = get_mask_int_c(feature_vec_node.astype(np.int_),
+ *                 mask = get_mask_int_c(feature_vec_node.astype(np.int32),
  *                                fs_array, vec_len, lsplit_len,
  *                                mask)             # <<<<<<<<<<<<<<
  * 
  *                 curr_loss = _get_mse_mask(y_c_mat[:,0], mask, y_left,
  */
       __pyx_t_2 = NULL;
       __pyx_t_8 = 0;
@@ -6062,74 +6069,74 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
           __pyx_t_8 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_1)) {
-        PyObject *__pyx_temp[6] = {__pyx_t_2, __pyx_t_6, __pyx_v_fs_array, __pyx_t_4, __pyx_t_5, __pyx_v_mask};
+        PyObject *__pyx_temp[6] = {__pyx_t_2, __pyx_t_7, __pyx_v_fs_array, __pyx_t_4, __pyx_t_5, __pyx_v_mask};
         __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 5+__pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 144, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_GOTREF(__pyx_t_10);
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-        PyObject *__pyx_temp[6] = {__pyx_t_2, __pyx_t_6, __pyx_v_fs_array, __pyx_t_4, __pyx_t_5, __pyx_v_mask};
+        PyObject *__pyx_temp[6] = {__pyx_t_2, __pyx_t_7, __pyx_v_fs_array, __pyx_t_4, __pyx_t_5, __pyx_v_mask};
         __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 5+__pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 144, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_GOTREF(__pyx_t_10);
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       } else
       #endif
       {
-        __pyx_t_7 = PyTuple_New(5+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 144, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
+        __pyx_t_6 = PyTuple_New(5+__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 144, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_6);
         if (__pyx_t_2) {
-          __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_2); __pyx_t_2 = NULL;
+          __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_2); __pyx_t_2 = NULL;
         }
-        __Pyx_GIVEREF(__pyx_t_6);
-        PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_8, __pyx_t_6);
+        __Pyx_GIVEREF(__pyx_t_7);
+        PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_8, __pyx_t_7);
         __Pyx_INCREF(__pyx_v_fs_array);
         __Pyx_GIVEREF(__pyx_v_fs_array);
-        PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_8, __pyx_v_fs_array);
+        PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_8, __pyx_v_fs_array);
         __Pyx_GIVEREF(__pyx_t_4);
-        PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_8, __pyx_t_4);
+        PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_8, __pyx_t_4);
         __Pyx_GIVEREF(__pyx_t_5);
-        PyTuple_SET_ITEM(__pyx_t_7, 3+__pyx_t_8, __pyx_t_5);
+        PyTuple_SET_ITEM(__pyx_t_6, 3+__pyx_t_8, __pyx_t_5);
         __Pyx_INCREF(__pyx_v_mask);
         __Pyx_GIVEREF(__pyx_v_mask);
-        PyTuple_SET_ITEM(__pyx_t_7, 4+__pyx_t_8, __pyx_v_mask);
-        __pyx_t_6 = 0;
+        PyTuple_SET_ITEM(__pyx_t_6, 4+__pyx_t_8, __pyx_v_mask);
+        __pyx_t_7 = 0;
         __pyx_t_4 = 0;
         __pyx_t_5 = 0;
-        __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_7, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 144, __pyx_L1_error)
+        __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 144, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
-        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF_SET(__pyx_v_mask, __pyx_t_10);
       __pyx_t_10 = 0;
 
       /* "structureboost/structure_rfdt.pyx":148
  *                                mask)
  * 
  *                 curr_loss = _get_mse_mask(y_c_mat[:,0], mask, y_left,             # <<<<<<<<<<<<<<
  *                                             y_c_sum[0]-y_left,
  *                                             c_left, y_c_sum[1]-c_left,
  */
       __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_get_mse_mask); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_y_c_mat, __pyx_tuple__4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 148, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_y_c_mat, __pyx_tuple__4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 148, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
 
       /* "structureboost/structure_rfdt.pyx":149
  * 
  *                 curr_loss = _get_mse_mask(y_c_mat[:,0], mask, y_left,
  *                                             y_c_sum[0]-y_left,             # <<<<<<<<<<<<<<
  *                                             c_left, y_c_sum[1]-c_left,
  *                                             float(self.min_leaf_size))
@@ -6145,16 +6152,16 @@
  *                                             y_c_sum[0]-y_left,
  *                                             c_left, y_c_sum[1]-c_left,             # <<<<<<<<<<<<<<
  *                                             float(self.min_leaf_size))
  *         return(curr_loss)
  */
       __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_y_c_sum, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 150, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = PyNumber_Subtract(__pyx_t_5, __pyx_v_c_left); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 150, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_7 = PyNumber_Subtract(__pyx_t_5, __pyx_v_c_left); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 150, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
       /* "structureboost/structure_rfdt.pyx":151
  *                                             y_c_sum[0]-y_left,
  *                                             c_left, y_c_sum[1]-c_left,
  *                                             float(self.min_leaf_size))             # <<<<<<<<<<<<<<
  *         return(curr_loss)
@@ -6175,77 +6182,77 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
           __pyx_t_8 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_1)) {
-        PyObject *__pyx_temp[8] = {__pyx_t_5, __pyx_t_7, __pyx_v_mask, __pyx_v_y_left, __pyx_t_4, __pyx_v_c_left, __pyx_t_6, __pyx_t_2};
+        PyObject *__pyx_temp[8] = {__pyx_t_5, __pyx_t_6, __pyx_v_mask, __pyx_v_y_left, __pyx_t_4, __pyx_v_c_left, __pyx_t_7, __pyx_t_2};
         __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 7+__pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 148, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_GOTREF(__pyx_t_10);
-        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-        PyObject *__pyx_temp[8] = {__pyx_t_5, __pyx_t_7, __pyx_v_mask, __pyx_v_y_left, __pyx_t_4, __pyx_v_c_left, __pyx_t_6, __pyx_t_2};
+        PyObject *__pyx_temp[8] = {__pyx_t_5, __pyx_t_6, __pyx_v_mask, __pyx_v_y_left, __pyx_t_4, __pyx_v_c_left, __pyx_t_7, __pyx_t_2};
         __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_8, 7+__pyx_t_8); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 148, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_GOTREF(__pyx_t_10);
-        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       } else
       #endif
       {
         __pyx_t_9 = PyTuple_New(7+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 148, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         if (__pyx_t_5) {
           __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_5); __pyx_t_5 = NULL;
         }
-        __Pyx_GIVEREF(__pyx_t_7);
-        PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_7);
+        __Pyx_GIVEREF(__pyx_t_6);
+        PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_6);
         __Pyx_INCREF(__pyx_v_mask);
         __Pyx_GIVEREF(__pyx_v_mask);
         PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_mask);
         __Pyx_INCREF(__pyx_v_y_left);
         __Pyx_GIVEREF(__pyx_v_y_left);
         PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_8, __pyx_v_y_left);
         __Pyx_GIVEREF(__pyx_t_4);
         PyTuple_SET_ITEM(__pyx_t_9, 3+__pyx_t_8, __pyx_t_4);
         __Pyx_INCREF(__pyx_v_c_left);
         __Pyx_GIVEREF(__pyx_v_c_left);
         PyTuple_SET_ITEM(__pyx_t_9, 4+__pyx_t_8, __pyx_v_c_left);
-        __Pyx_GIVEREF(__pyx_t_6);
-        PyTuple_SET_ITEM(__pyx_t_9, 5+__pyx_t_8, __pyx_t_6);
+        __Pyx_GIVEREF(__pyx_t_7);
+        PyTuple_SET_ITEM(__pyx_t_9, 5+__pyx_t_8, __pyx_t_7);
         __Pyx_GIVEREF(__pyx_t_2);
         PyTuple_SET_ITEM(__pyx_t_9, 6+__pyx_t_8, __pyx_t_2);
-        __pyx_t_7 = 0;
-        __pyx_t_4 = 0;
         __pyx_t_6 = 0;
+        __pyx_t_4 = 0;
+        __pyx_t_7 = 0;
         __pyx_t_2 = 0;
         __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_9, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 148, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_v_curr_loss = __pyx_t_10;
       __pyx_t_10 = 0;
 
       /* "structureboost/structure_rfdt.pyx":138
  *                                             c_left, y_c_sum[1]-c_left,
  *                                             float(self.min_leaf_size))
  *             elif feature_type in ['categorical_int','graphical_voronoi']:             # <<<<<<<<<<<<<<
- *                 fs_array = np.fromiter(left_feat_values, int,
- *                 len(left_feat_values)).astype(np.int_)
+ *                 fs_array = np.fromiter(left_feat_values, np.int32,
+ *                 len(left_feat_values)).astype(np.int32)
  */
     }
     __pyx_L4:;
 
     /* "structureboost/structure_rfdt.pyx":131
  *                                                         float(self.min_leaf_size))
  * 
@@ -6806,15 +6813,15 @@
   return __pyx_r;
 }
 
 /* "structureboost/structure_rfdt.pyx":175
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def get_bin_sums_c_rfbin(np.ndarray[double] y_vec,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] bin_result_vec, long out_vec_size):
+ *                    np.ndarray[np.int32_t] bin_result_vec, long out_vec_size):
  *     cdef int i
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_14structure_rfdt_1get_bin_sums_c_rfbin(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_14structure_rfdt_1get_bin_sums_c_rfbin = {"get_bin_sums_c_rfbin", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_14structure_rfdt_1get_bin_sums_c_rfbin, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_14structure_rfdt_1get_bin_sums_c_rfbin(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -6949,20 +6956,20 @@
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_y_vec, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 175, __pyx_L1_error)
   }
   __pyx_pybuffernd_y_vec.diminfo[0].strides = __pyx_pybuffernd_y_vec.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_y_vec.diminfo[0].shape = __pyx_pybuffernd_y_vec.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_bin_result_vec, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 175, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_bin_result_vec, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 175, __pyx_L1_error)
   }
   __pyx_pybuffernd_bin_result_vec.diminfo[0].strides = __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_bin_result_vec.diminfo[0].shape = __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.shape[0];
 
   /* "structureboost/structure_rfdt.pyx":178
- *                    np.ndarray[np.int_t] bin_result_vec, long out_vec_size):
+ *                    np.ndarray[np.int32_t] bin_result_vec, long out_vec_size):
  *     cdef int i
  *     cdef int m = bin_result_vec.shape[0]             # <<<<<<<<<<<<<<
  * 
  *     cdef np.ndarray[double] y_sum_bins = np.zeros(out_vec_size)
  */
   __pyx_v_m = (__pyx_v_bin_result_vec->dimensions[0]);
 
@@ -7071,26 +7078,26 @@
  *     for i in range(m):
  *         y_sum_bins[bin_result_vec[i]] += y_vec[i]             # <<<<<<<<<<<<<<
  *         count_in_bins[bin_result_vec[i]] += 1
  *     return y_sum_bins, count_in_bins
  */
     __pyx_t_10 = __pyx_v_i;
     __pyx_t_11 = __pyx_v_i;
-    __pyx_t_12 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_bin_result_vec.diminfo[0].strides));
+    __pyx_t_12 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_bin_result_vec.diminfo[0].strides));
     *__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_y_sum_bins.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_y_sum_bins.diminfo[0].strides) += (*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_y_vec.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_y_vec.diminfo[0].strides));
 
     /* "structureboost/structure_rfdt.pyx":185
  *     for i in range(m):
  *         y_sum_bins[bin_result_vec[i]] += y_vec[i]
  *         count_in_bins[bin_result_vec[i]] += 1             # <<<<<<<<<<<<<<
  *     return y_sum_bins, count_in_bins
  * 
  */
     __pyx_t_10 = __pyx_v_i;
-    __pyx_t_11 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_bin_result_vec.diminfo[0].strides));
+    __pyx_t_11 = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_bin_result_vec.diminfo[0].strides));
     *__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_count_in_bins.rcbuffer->pybuffer.buf, __pyx_t_11, __pyx_pybuffernd_count_in_bins.diminfo[0].strides) += 1.0;
   }
 
   /* "structureboost/structure_rfdt.pyx":186
  *         y_sum_bins[bin_result_vec[i]] += y_vec[i]
  *         count_in_bins[bin_result_vec[i]] += 1
  *     return y_sum_bins, count_in_bins             # <<<<<<<<<<<<<<
@@ -7110,15 +7117,15 @@
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "structureboost/structure_rfdt.pyx":175
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def get_bin_sums_c_rfbin(np.ndarray[double] y_vec,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] bin_result_vec, long out_vec_size):
+ *                    np.ndarray[np.int32_t] bin_result_vec, long out_vec_size):
  *     cdef int i
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -8704,15 +8711,15 @@
   return __pyx_r;
 }
 
 /* "structureboost/structure_rfdt.pyx":252
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
  * def _get_score_array_mse(np.ndarray[double] y_vec,             # <<<<<<<<<<<<<<
- *                         np.ndarray[np.int_t] bin_result_vec,
+ *                         np.ndarray[np.int32_t] bin_result_vec,
  *                         np.ndarray[double] ysl,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_14structure_rfdt_9_get_score_array_mse(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_14structure_rfdt_9_get_score_array_mse = {"_get_score_array_mse", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_14structure_rfdt_9_get_score_array_mse, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_14structure_rfdt_9_get_score_array_mse(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -8932,15 +8939,15 @@
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_y_vec, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 252, __pyx_L1_error)
   }
   __pyx_pybuffernd_y_vec.diminfo[0].strides = __pyx_pybuffernd_y_vec.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_y_vec.diminfo[0].shape = __pyx_pybuffernd_y_vec.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_bin_result_vec, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 252, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_bin_result_vec, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 252, __pyx_L1_error)
   }
   __pyx_pybuffernd_bin_result_vec.diminfo[0].strides = __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_bin_result_vec.diminfo[0].shape = __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ysl.rcbuffer->pybuffer, (PyObject*)__pyx_v_ysl, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 252, __pyx_L1_error)
   }
   __pyx_pybuffernd_ysl.diminfo[0].strides = __pyx_pybuffernd_ysl.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_ysl.diminfo[0].shape = __pyx_pybuffernd_ysl.rcbuffer->pybuffer.shape[0];
@@ -9100,15 +9107,15 @@
  *         right_mean = ysr[i]/(cbr[i]+eps)
  *         for j in range(len(y_vec)):
  *             if bin_result_vec[j]<=i:             # <<<<<<<<<<<<<<
  *                 adj_y_vec[j] = y_vec[j] - left_mean
  *             else:
  */
       __pyx_t_10 = __pyx_v_j;
-      __pyx_t_15 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_bin_result_vec.diminfo[0].strides)) <= __pyx_v_i) != 0);
+      __pyx_t_15 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_bin_result_vec.rcbuffer->pybuffer.buf, __pyx_t_10, __pyx_pybuffernd_bin_result_vec.diminfo[0].strides)) <= __pyx_v_i) != 0);
       if (__pyx_t_15) {
 
         /* "structureboost/structure_rfdt.pyx":269
  *         for j in range(len(y_vec)):
  *             if bin_result_vec[j]<=i:
  *                 adj_y_vec[j] = y_vec[j] - left_mean             # <<<<<<<<<<<<<<
  *             else:
@@ -9191,15 +9198,15 @@
   __pyx_r = ((PyObject *)__pyx_v_score_vec);
   goto __pyx_L0;
 
   /* "structureboost/structure_rfdt.pyx":252
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
  * def _get_score_array_mse(np.ndarray[double] y_vec,             # <<<<<<<<<<<<<<
- *                         np.ndarray[np.int_t] bin_result_vec,
+ *                         np.ndarray[np.int32_t] bin_result_vec,
  *                         np.ndarray[double] ysl,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -9636,16 +9643,16 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "structureboost/structure_rfdt.pyx":314
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_mask_int_c(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] left_split,
+ * def get_mask_int_c(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ *                    np.ndarray[np.int32_t] left_split,
  *                    long vec_len, long lsplit_len,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_14structureboost_14structure_rfdt_15get_mask_int_c(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_14structureboost_14structure_rfdt_15get_mask_int_c = {"get_mask_int_c", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_14structureboost_14structure_rfdt_15get_mask_int_c, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_14structureboost_14structure_rfdt_15get_mask_int_c(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
@@ -9790,30 +9797,30 @@
   __pyx_pybuffernd_left_split.rcbuffer = &__pyx_pybuffer_left_split;
   __pyx_pybuffer_mask_vec.pybuffer.buf = NULL;
   __pyx_pybuffer_mask_vec.refcount = 0;
   __pyx_pybuffernd_mask_vec.data = NULL;
   __pyx_pybuffernd_mask_vec.rcbuffer = &__pyx_pybuffer_mask_vec;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer, (PyObject*)__pyx_v_feature_vec_node, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 314, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer, (PyObject*)__pyx_v_feature_vec_node, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 314, __pyx_L1_error)
   }
   __pyx_pybuffernd_feature_vec_node.diminfo[0].strides = __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_feature_vec_node.diminfo[0].shape = __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_left_split.rcbuffer->pybuffer, (PyObject*)__pyx_v_left_split, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 314, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_left_split.rcbuffer->pybuffer, (PyObject*)__pyx_v_left_split, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 314, __pyx_L1_error)
   }
   __pyx_pybuffernd_left_split.diminfo[0].strides = __pyx_pybuffernd_left_split.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_left_split.diminfo[0].shape = __pyx_pybuffernd_left_split.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mask_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_mask_vec, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 314, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mask_vec.rcbuffer->pybuffer, (PyObject*)__pyx_v_mask_vec, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 314, __pyx_L1_error)
   }
   __pyx_pybuffernd_mask_vec.diminfo[0].strides = __pyx_pybuffernd_mask_vec.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mask_vec.diminfo[0].shape = __pyx_pybuffernd_mask_vec.rcbuffer->pybuffer.shape[0];
 
   /* "structureboost/structure_rfdt.pyx":319
- *                    np.ndarray[np.int_t] mask_vec):
+ *                    np.ndarray[np.int32_t] mask_vec):
  *     cdef int i, j
  *     for i in range(vec_len):             # <<<<<<<<<<<<<<
  *         for j in range(lsplit_len):
  *             if feature_vec_node[i] == left_split[j]:
  */
   __pyx_t_1 = __pyx_v_vec_len;
   __pyx_t_2 = __pyx_t_1;
@@ -9837,26 +9844,26 @@
  *         for j in range(lsplit_len):
  *             if feature_vec_node[i] == left_split[j]:             # <<<<<<<<<<<<<<
  *                 mask_vec[i] = 1
  *                 break
  */
       __pyx_t_7 = __pyx_v_i;
       __pyx_t_8 = __pyx_v_j;
-      __pyx_t_9 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.buf, __pyx_t_7, __pyx_pybuffernd_feature_vec_node.diminfo[0].strides)) == (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_left_split.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_left_split.diminfo[0].strides))) != 0);
+      __pyx_t_9 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_feature_vec_node.rcbuffer->pybuffer.buf, __pyx_t_7, __pyx_pybuffernd_feature_vec_node.diminfo[0].strides)) == (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_left_split.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_left_split.diminfo[0].strides))) != 0);
       if (__pyx_t_9) {
 
         /* "structureboost/structure_rfdt.pyx":322
  *         for j in range(lsplit_len):
  *             if feature_vec_node[i] == left_split[j]:
  *                 mask_vec[i] = 1             # <<<<<<<<<<<<<<
  *                 break
  *     return mask_vec.astype(bool)
  */
         __pyx_t_8 = __pyx_v_i;
-        *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_mask_vec.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_mask_vec.diminfo[0].strides) = 1;
+        *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int32_t *, __pyx_pybuffernd_mask_vec.rcbuffer->pybuffer.buf, __pyx_t_8, __pyx_pybuffernd_mask_vec.diminfo[0].strides) = 1;
 
         /* "structureboost/structure_rfdt.pyx":323
  *             if feature_vec_node[i] == left_split[j]:
  *                 mask_vec[i] = 1
  *                 break             # <<<<<<<<<<<<<<
  *     return mask_vec.astype(bool)
  * 
@@ -9903,16 +9910,16 @@
   __pyx_r = __pyx_t_10;
   __pyx_t_10 = 0;
   goto __pyx_L0;
 
   /* "structureboost/structure_rfdt.pyx":314
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_mask_int_c(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] left_split,
+ * def get_mask_int_c(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ *                    np.ndarray[np.int32_t] left_split,
  *                    long vec_len, long lsplit_len,
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
@@ -11587,15 +11594,15 @@
   {&__pyx_n_u_graphical_voronoi, __pyx_k_graphical_voronoi, sizeof(__pyx_k_graphical_voronoi), 0, 1, 0, 1},
   {&__pyx_n_s_graphs, __pyx_k_graphs, sizeof(__pyx_k_graphs), 0, 0, 1, 1},
   {&__pyx_n_s_has_na_vals, __pyx_k_has_na_vals, sizeof(__pyx_k_has_na_vals), 0, 0, 1, 1},
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_inf, __pyx_k_inf, sizeof(__pyx_k_inf), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
-  {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
+  {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
   {&__pyx_n_s_isnan, __pyx_k_isnan, sizeof(__pyx_k_isnan), 0, 0, 1, 1},
   {&__pyx_n_s_j, __pyx_k_j, sizeof(__pyx_k_j), 0, 0, 1, 1},
   {&__pyx_n_s_leaf_vertex_ind, __pyx_k_leaf_vertex_ind, sizeof(__pyx_k_leaf_vertex_ind), 0, 0, 1, 1},
   {&__pyx_n_s_left_feat_values, __pyx_k_left_feat_values, sizeof(__pyx_k_left_feat_values), 0, 0, 1, 1},
   {&__pyx_n_s_left_mean, __pyx_k_left_mean, sizeof(__pyx_k_left_mean), 0, 0, 1, 1},
   {&__pyx_n_s_left_split, __pyx_k_left_split, sizeof(__pyx_k_left_split), 0, 0, 1, 1},
   {&__pyx_n_s_log, __pyx_k_log, sizeof(__pyx_k_log), 0, 0, 1, 1},
@@ -11831,15 +11838,15 @@
   __Pyx_GIVEREF(__pyx_tuple__29);
   __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(4, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_rfdt_pyx, __pyx_n_s_get_score_of_split, 155, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 155, __pyx_L1_error)
 
   /* "structureboost/structure_rfdt.pyx":175
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def get_bin_sums_c_rfbin(np.ndarray[double] y_vec,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] bin_result_vec, long out_vec_size):
+ *                    np.ndarray[np.int32_t] bin_result_vec, long out_vec_size):
  *     cdef int i
  */
   __pyx_tuple__30 = PyTuple_Pack(7, __pyx_n_s_y_vec, __pyx_n_s_bin_result_vec, __pyx_n_s_out_vec_size, __pyx_n_s_i, __pyx_n_s_m, __pyx_n_s_y_sum_bins, __pyx_n_s_count_in_bins); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__30);
   __Pyx_GIVEREF(__pyx_tuple__30);
   __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_rfdt_pyx, __pyx_n_s_get_bin_sums_c_rfbin, 175, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 175, __pyx_L1_error)
 
@@ -11879,15 +11886,15 @@
   __Pyx_GIVEREF(__pyx_tuple__33);
   __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(6, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_rfdt_pyx, __pyx_n_s_get_score_binary_entropy, 225, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 225, __pyx_L1_error)
 
   /* "structureboost/structure_rfdt.pyx":252
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
  * def _get_score_array_mse(np.ndarray[double] y_vec,             # <<<<<<<<<<<<<<
- *                         np.ndarray[np.int_t] bin_result_vec,
+ *                         np.ndarray[np.int32_t] bin_result_vec,
  *                         np.ndarray[double] ysl,
  */
   __pyx_tuple__34 = PyTuple_Pack(13, __pyx_n_s_y_vec, __pyx_n_s_bin_result_vec, __pyx_n_s_ysl, __pyx_n_s_ysr, __pyx_n_s_cbl, __pyx_n_s_cbr, __pyx_n_s_eps, __pyx_n_s_score_vec, __pyx_n_s_adj_y_vec, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_left_mean, __pyx_n_s_right_mean); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__34);
   __Pyx_GIVEREF(__pyx_tuple__34);
   __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(7, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_rfdt_pyx, __pyx_n_s_get_score_array_mse, 252, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 252, __pyx_L1_error)
 
@@ -11914,16 +11921,16 @@
   __Pyx_GOTREF(__pyx_tuple__36);
   __Pyx_GIVEREF(__pyx_tuple__36);
   __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_rfdt_pyx, __pyx_n_s_get_mask, 309, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 309, __pyx_L1_error)
 
   /* "structureboost/structure_rfdt.pyx":314
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_mask_int_c(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] left_split,
+ * def get_mask_int_c(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ *                    np.ndarray[np.int32_t] left_split,
  *                    long vec_len, long lsplit_len,
  */
   __pyx_tuple__37 = PyTuple_Pack(7, __pyx_n_s_feature_vec_node, __pyx_n_s_left_split, __pyx_n_s_vec_len, __pyx_n_s_lsplit_len, __pyx_n_s_mask_vec, __pyx_n_s_i, __pyx_n_s_j); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__37);
   __Pyx_GIVEREF(__pyx_tuple__37);
   __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(5, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_structure_rfdt_pyx, __pyx_n_s_get_mask_int_c, 314, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 314, __pyx_L1_error)
 
@@ -12513,15 +12520,15 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_rfdt.pyx":175
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
  * def get_bin_sums_c_rfbin(np.ndarray[double] y_vec,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] bin_result_vec, long out_vec_size):
+ *                    np.ndarray[np.int32_t] bin_result_vec, long out_vec_size):
  *     cdef int i
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_14structure_rfdt_1get_bin_sums_c_rfbin, NULL, __pyx_n_s_structureboost_structure_rfdt); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_bin_sums_c_rfbin, __pyx_t_1) < 0) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
@@ -12561,15 +12568,15 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_score_binary_entropy, __pyx_t_1) < 0) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_rfdt.pyx":252
  * @cython.nonecheck(False)
  * @cython.cdivision(True)
  * def _get_score_array_mse(np.ndarray[double] y_vec,             # <<<<<<<<<<<<<<
- *                         np.ndarray[np.int_t] bin_result_vec,
+ *                         np.ndarray[np.int32_t] bin_result_vec,
  *                         np.ndarray[double] ysl,
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_14structure_rfdt_9_get_score_array_mse, NULL, __pyx_n_s_structureboost_structure_rfdt); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_score_array_mse, __pyx_t_1) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
@@ -12596,16 +12603,16 @@
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_mask, __pyx_t_1) < 0) __PYX_ERR(0, 309, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "structureboost/structure_rfdt.pyx":314
  * @cython.boundscheck(False)  # Deactivate bounds checking
  * @cython.wraparound(False)   # Deactivate negative indexing.
- * def get_mask_int_c(np.ndarray[np.int_t] feature_vec_node,             # <<<<<<<<<<<<<<
- *                    np.ndarray[np.int_t] left_split,
+ * def get_mask_int_c(np.ndarray[np.int32_t] feature_vec_node,             # <<<<<<<<<<<<<<
+ *                    np.ndarray[np.int32_t] left_split,
  *                    long vec_len, long lsplit_len,
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_14structureboost_14structure_rfdt_15get_mask_int_c, NULL, __pyx_n_s_structureboost_structure_rfdt); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_mask_int_c, __pyx_t_1) < 0) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `structureboost-0.4.2/structureboost/utils.py` & `structureboost-0.4.3/structureboost/utils.py`

 * *Files identical despite different names*

### Comparing `structureboost-0.4.2/structureboost.egg-info/PKG-INFO` & `structureboost-0.4.3/structureboost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structureboost
-Version: 0.4.2
+Version: 0.4.3
 Summary: StructureBoost is a Python package for gradient boosting using categorical structure.  See documentation at: https://structureboost.readthedocs.io/
 Home-page: https://github.com/numeristical/structureboost
 Author: Brian Lucena
 Author-email: brianlucena@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `structureboost-0.4.2/structureboost.egg-info/SOURCES.txt` & `structureboost-0.4.3/structureboost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

