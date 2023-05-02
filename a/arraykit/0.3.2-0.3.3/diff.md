# Comparing `tmp/arraykit-0.3.2.tar.gz` & `tmp/arraykit-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraykit-0.3.2.tar", last modified: Mon Apr 24 15:28:22 2023, max compression
+gzip compressed data, was "arraykit-0.3.3.tar", last modified: Tue May  2 01:22:57 2023, max compression
```

## Comparing `arraykit-0.3.2.tar` & `arraykit-0.3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:28:22.452730 arraykit-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-04-24 15:28:16.000000 arraykit-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-04-24 15:28:16.000000 arraykit-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-04-24 15:28:22.452730 arraykit-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-04-24 15:28:16.000000 arraykit-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:28:22.452730 arraykit-0.3.2/arraykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-04-24 15:28:22.000000 arraykit-0.3.2/arraykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-04-24 15:28:22.000000 arraykit-0.3.2/arraykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 15:28:22.000000 arraykit-0.3.2/arraykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-24 15:28:22.000000 arraykit-0.3.2/arraykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-24 15:28:22.000000 arraykit-0.3.2/arraykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-24 15:28:22.452730 arraykit-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-04-24 15:28:16.000000 arraykit-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:28:22.452730 arraykit-0.3.2/src/
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-04-24 15:28:16.000000 arraykit-0.3.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   145128 2023-04-24 15:28:16.000000 arraykit-0.3.2/src/_arraykit.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:28:22.452730 arraykit-0.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_array_go.py
--rw-r--r--   0 runner    (1001) docker     (122)    49054 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_delimited_to_arrays.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_delimited_to_arrays_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_delimited_to_arrays_property.py
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_pyi.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_split_after_count.py
--rw-r--r--   0 runner    (1001) docker     (122)    28073 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_type_discovery.py
--rw-r--r--   0 runner    (1001) docker     (122)    26066 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:22:57.733880 arraykit-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-05-02 01:22:51.000000 arraykit-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-02 01:22:51.000000 arraykit-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-02 01:22:57.729880 arraykit-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-02 01:22:51.000000 arraykit-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:22:57.729880 arraykit-0.3.3/arraykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-02 01:22:57.000000 arraykit-0.3.3/arraykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-02 01:22:57.000000 arraykit-0.3.3/arraykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 01:22:57.000000 arraykit-0.3.3/arraykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-02 01:22:57.000000 arraykit-0.3.3/arraykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-02 01:22:57.000000 arraykit-0.3.3/arraykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-02 01:22:57.733880 arraykit-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-05-02 01:22:51.000000 arraykit-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:22:57.729880 arraykit-0.3.3/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-05-02 01:22:51.000000 arraykit-0.3.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   145224 2023-05-02 01:22:51.000000 arraykit-0.3.3/src/_arraykit.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:22:57.729880 arraykit-0.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_array_go.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49054 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_delimited_to_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_delimited_to_arrays_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_delimited_to_arrays_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_pyi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_split_after_count.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28073 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_type_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26066 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_util.py
```

### Comparing `arraykit-0.3.2/LICENSE.txt` & `arraykit-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.2/PKG-INFO` & `arraykit-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.3.2
+Version: 0.3.3
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.3.2/README.rst` & `arraykit-0.3.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -33,18 +33,25 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayKit
 -------------------------
 
+
+0.3.3
+............
+
+Corrected potential memory leak in ``isna_element()``.
+
+
 0.3.2
 ............
 
-Optimization to ``delimited_to_arrays()`` character reading pre line.
+Optimization to ``delimited_to_arrays()`` character reading per line.
 
 
 0.3.1
 ............
 
 Improvements to ``delimited_to_arrays()``, including proper loading of ``float16`` types.
```

### Comparing `arraykit-0.3.2/arraykit.egg-info/PKG-INFO` & `arraykit-0.3.3/arraykit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.3.2
+Version: 0.3.3
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.3.2/setup.py` & `arraykit-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import site
 import os
 import typing as tp
 from setuptools import Extension  # type: ignore
 from setuptools import setup
 from pathlib import Path
 
-AK_VERSION = '0.3.2'
+AK_VERSION = '0.3.3'
 
 def get_long_description() -> str:
     return '''The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
 
 Code: https://github.com/static-frame/arraykit
 
 Packages: https://pypi.org/project/arraykit
```

### Comparing `arraykit-0.3.2/src/__init__.py` & `arraykit-0.3.3/src/__init__.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.2/src/_arraykit.c` & `arraykit-0.3.3/src/_arraykit.c`

 * *Files 0% similar despite different names*

```diff
@@ -3767,18 +3767,22 @@
     // NaT - Timedelta
     if (PyArray_IsScalar(element, Timedelta)) {
         return PyBool_FromLong(PyArrayScalar_VAL(element, Timedelta) == NPY_DATETIME_NAT);
     }
     // Try to identify Pandas Timestamp NATs
     if (PyObject_HasAttrString(element, "to_numpy")) {
         PyObject *to_numpy = PyObject_GetAttrString(element, "to_numpy");
+        if (to_numpy == NULL) {
+            return NULL;
+        }
         if (!PyCallable_Check(to_numpy)) {
             Py_RETURN_FALSE;
         }
         PyObject* post = PyObject_CallFunction(to_numpy, NULL);
+        Py_DECREF(to_numpy);
         if (post == NULL) return NULL;
         return PyBool_FromLong(PyArrayScalar_VAL(post, Datetime) == NPY_DATETIME_NAT);
     }
     Py_RETURN_FALSE;
 }
 
 //------------------------------------------------------------------------------
```

### Comparing `arraykit-0.3.2/test/test_array_go.py` & `arraykit-0.3.3/test/test_array_go.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.2/test/test_delimited_to_arrays.py` & `arraykit-0.3.3/test/test_delimited_to_arrays.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.2/test/test_delimited_to_arrays_integration.py` & `arraykit-0.3.3/test/test_delimited_to_arrays_integration.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.2/test/test_delimited_to_arrays_property.py` & `arraykit-0.3.3/test/test_delimited_to_arrays_property.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.2/test/test_pyi.py` & `arraykit-0.3.3/test/test_pyi.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.2/test/test_split_after_count.py` & `arraykit-0.3.3/test/test_split_after_count.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.2/test/test_type_discovery.py` & `arraykit-0.3.3/test/test_type_discovery.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.2/test/test_util.py` & `arraykit-0.3.3/test/test_util.py`

 * *Files identical despite different names*

