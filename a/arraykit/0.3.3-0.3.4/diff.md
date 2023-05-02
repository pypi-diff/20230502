# Comparing `tmp/arraykit-0.3.3.tar.gz` & `tmp/arraykit-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraykit-0.3.3.tar", last modified: Tue May  2 01:22:57 2023, max compression
+gzip compressed data, was "arraykit-0.3.4.tar", last modified: Tue May  2 17:47:36 2023, max compression
```

## Comparing `arraykit-0.3.3.tar` & `arraykit-0.3.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:22:57.733880 arraykit-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-05-02 01:22:51.000000 arraykit-0.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-02 01:22:51.000000 arraykit-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-02 01:22:57.729880 arraykit-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-02 01:22:51.000000 arraykit-0.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:22:57.729880 arraykit-0.3.3/arraykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-02 01:22:57.000000 arraykit-0.3.3/arraykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-02 01:22:57.000000 arraykit-0.3.3/arraykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 01:22:57.000000 arraykit-0.3.3/arraykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-02 01:22:57.000000 arraykit-0.3.3/arraykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-02 01:22:57.000000 arraykit-0.3.3/arraykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-02 01:22:57.733880 arraykit-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-05-02 01:22:51.000000 arraykit-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:22:57.729880 arraykit-0.3.3/src/
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-05-02 01:22:51.000000 arraykit-0.3.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   145224 2023-05-02 01:22:51.000000 arraykit-0.3.3/src/_arraykit.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 01:22:57.729880 arraykit-0.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_array_go.py
--rw-r--r--   0 runner    (1001) docker     (122)    49054 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_delimited_to_arrays.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_delimited_to_arrays_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_delimited_to_arrays_property.py
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_pyi.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_split_after_count.py
--rw-r--r--   0 runner    (1001) docker     (122)    28073 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_type_discovery.py
--rw-r--r--   0 runner    (1001) docker     (122)    26066 2023-05-02 01:22:51.000000 arraykit-0.3.3/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 17:47:36.086742 arraykit-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-05-02 17:47:29.000000 arraykit-0.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-02 17:47:29.000000 arraykit-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-02 17:47:36.086742 arraykit-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-02 17:47:29.000000 arraykit-0.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 17:47:36.082742 arraykit-0.3.4/arraykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-02 17:47:35.000000 arraykit-0.3.4/arraykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-02 17:47:36.000000 arraykit-0.3.4/arraykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 17:47:35.000000 arraykit-0.3.4/arraykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-02 17:47:35.000000 arraykit-0.3.4/arraykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-02 17:47:35.000000 arraykit-0.3.4/arraykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-02 17:47:36.086742 arraykit-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-05-02 17:47:29.000000 arraykit-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 17:47:36.082742 arraykit-0.3.4/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-05-02 17:47:29.000000 arraykit-0.3.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   145666 2023-05-02 17:47:29.000000 arraykit-0.3.4/src/_arraykit.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 17:47:36.086742 arraykit-0.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_array_go.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49054 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_delimited_to_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_delimited_to_arrays_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_delimited_to_arrays_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_pyi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_split_after_count.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28073 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_type_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26140 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_util.py
```

### Comparing `arraykit-0.3.3/LICENSE.txt` & `arraykit-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.3/PKG-INFO` & `arraykit-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.3.3
+Version: 0.3.4
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.3.3/README.rst` & `arraykit-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.3/arraykit.egg-info/PKG-INFO` & `arraykit-0.3.4/arraykit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.3.3
+Version: 0.3.4
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.3.3/setup.py` & `arraykit-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import site
 import os
 import typing as tp
 from setuptools import Extension  # type: ignore
 from setuptools import setup
 from pathlib import Path
 
-AK_VERSION = '0.3.3'
+AK_VERSION = '0.3.4'
 
 def get_long_description() -> str:
     return '''The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
 
 Code: https://github.com/static-frame/arraykit
 
 Packages: https://pypi.org/project/arraykit
```

### Comparing `arraykit-0.3.3/src/__init__.py` & `arraykit-0.3.4/src/__init__.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.3/src/_arraykit.c` & `arraykit-0.3.4/src/_arraykit.c`

 * *Files 1% similar despite different names*

```diff
@@ -3766,25 +3766,37 @@
     }
     // NaT - Timedelta
     if (PyArray_IsScalar(element, Timedelta)) {
         return PyBool_FromLong(PyArrayScalar_VAL(element, Timedelta) == NPY_DATETIME_NAT);
     }
     // Try to identify Pandas Timestamp NATs
     if (PyObject_HasAttrString(element, "to_numpy")) {
-        PyObject *to_numpy = PyObject_GetAttrString(element, "to_numpy");
-        if (to_numpy == NULL) {
-            return NULL;
-        }
-        if (!PyCallable_Check(to_numpy)) {
-            Py_RETURN_FALSE;
-        }
-        PyObject* post = PyObject_CallFunction(to_numpy, NULL);
-        Py_DECREF(to_numpy);
-        if (post == NULL) return NULL;
-        return PyBool_FromLong(PyArrayScalar_VAL(post, Datetime) == NPY_DATETIME_NAT);
+        // strcmp returns 0 on match
+        return PyBool_FromLong(strcmp(element->ob_type->tp_name, "NaTType") == 0);
+        // the long way
+        // PyObject *to_numpy = PyObject_GetAttrString(element, "to_numpy");
+        // if (to_numpy == NULL) {
+        //     return NULL;
+        // }
+        // if (!PyCallable_Check(to_numpy)) {
+        //     Py_DECREF(to_numpy);
+        //     Py_RETURN_FALSE;
+        // }
+        // PyObject* scalar = PyObject_CallFunction(to_numpy, NULL);
+        // Py_DECREF(to_numpy);
+        // if (scalar == NULL) {
+        //     return NULL;
+        // }
+        // if (!PyArray_IsScalar(scalar, Datetime)) {
+        //     Py_DECREF(scalar);
+        //     Py_RETURN_FALSE;
+        // }
+        // PyObject* pb = PyBool_FromLong(PyArrayScalar_VAL(scalar, Datetime) == NPY_DATETIME_NAT);
+        // Py_DECREF(scalar);
+        // return pb;
     }
     Py_RETURN_FALSE;
 }
 
 //------------------------------------------------------------------------------
 
 static PyObject *
```

### Comparing `arraykit-0.3.3/test/test_array_go.py` & `arraykit-0.3.4/test/test_array_go.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.3/test/test_delimited_to_arrays.py` & `arraykit-0.3.4/test/test_delimited_to_arrays.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.3/test/test_delimited_to_arrays_integration.py` & `arraykit-0.3.4/test/test_delimited_to_arrays_integration.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.3/test/test_delimited_to_arrays_property.py` & `arraykit-0.3.4/test/test_delimited_to_arrays_property.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.3/test/test_pyi.py` & `arraykit-0.3.4/test/test_pyi.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.3/test/test_split_after_count.py` & `arraykit-0.3.4/test/test_split_after_count.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.3/test/test_type_discovery.py` & `arraykit-0.3.4/test/test_type_discovery.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.3/test/test_util.py` & `arraykit-0.3.4/test/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,21 +347,25 @@
         self.assertFalse(isna_element(None, False))
         self.assertTrue(isna_element(None, True))
 
     def test_isna_element_d(self) -> None:
         ts = pd.Timestamp('nat')
         self.assertTrue(isna_element(ts))
 
+        s1 = pd.Series((0,))
+        self.assertFalse(isna_element(s1))
+
 
     def test_isna_element_e(self) -> None:
         from types import SimpleNamespace
         sn = SimpleNamespace()
         sn.to_numpy = None
         self.assertFalse(isna_element(sn))
 
+
     #---------------------------------------------------------------------------
 
     def test_dtype_from_element_core_dtypes(self) -> None:
         dtypes = [
                 np.longlong,
                 np.int_,
                 np.intc,
```

