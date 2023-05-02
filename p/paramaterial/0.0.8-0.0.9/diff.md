# Comparing `tmp/paramaterial-0.0.8.tar.gz` & `tmp/paramaterial-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paramaterial-0.0.8.tar", last modified: Sat Nov 26 22:21:24 2022, max compression
+gzip compressed data, was "paramaterial-0.0.9.tar", last modified: Sat Nov 26 22:28:30 2022, max compression
```

## Comparing `paramaterial-0.0.8.tar` & `paramaterial-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-11-26 22:21:24.075064 paramaterial-0.0.8/
--rw-rw-rw-   0        0        0     1088 2022-09-15 06:45:20.000000 paramaterial-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3100 2022-11-26 22:21:24.075064 paramaterial-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2182 2022-11-26 22:19:03.000000 paramaterial-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-11-26 22:21:24.043791 paramaterial-0.0.8/paramaterial/
--rw-rw-rw-   0        0        0      178 2022-11-26 22:19:03.000000 paramaterial-0.0.8/paramaterial/__init__.py
--rw-rw-rw-   0        0        0     3056 2022-11-26 22:19:03.000000 paramaterial-0.0.8/paramaterial/example.py
--rw-rw-rw-   0        0        0    18451 2022-11-25 09:30:10.000000 paramaterial-0.0.8/paramaterial/modelling.py
--rw-rw-rw-   0        0        0    15594 2022-11-25 09:30:10.000000 paramaterial-0.0.8/paramaterial/plotting.py
--rw-rw-rw-   0        0        0     9568 2022-11-25 09:30:10.000000 paramaterial-0.0.8/paramaterial/plug.py
--rw-rw-rw-   0        0        0     4653 2022-11-26 22:19:03.000000 paramaterial-0.0.8/paramaterial/preparing.py
--rw-rw-rw-   0        0        0     9404 2022-11-25 09:30:10.000000 paramaterial-0.0.8/paramaterial/processing.py
--rw-rw-rw-   0        0        0     7478 2022-11-09 18:13:21.000000 paramaterial-0.0.8/paramaterial/receipts.py
--rw-rw-rw-   0        0        0     4473 2022-11-25 09:30:10.000000 paramaterial-0.0.8/paramaterial/screening.py
-drwxrwxrwx   0        0        0        0 2022-11-26 22:21:24.075064 paramaterial-0.0.8/paramaterial.egg-info/
--rw-rw-rw-   0        0        0     3100 2022-11-26 22:21:23.000000 paramaterial-0.0.8/paramaterial.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2022-11-26 22:21:23.000000 paramaterial-0.0.8/paramaterial.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-26 22:21:23.000000 paramaterial-0.0.8/paramaterial.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-11-26 22:21:23.000000 paramaterial-0.0.8/paramaterial.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-26 22:21:24.075064 paramaterial-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1340 2022-11-26 22:20:26.000000 paramaterial-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-26 22:28:30.428434 paramaterial-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2022-09-15 06:45:20.000000 paramaterial-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3100 2022-11-26 22:28:30.428434 paramaterial-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2182 2022-11-26 22:19:03.000000 paramaterial-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-11-26 22:28:30.412814 paramaterial-0.0.9/paramaterial/
+-rw-rw-rw-   0        0        0      187 2022-11-26 22:26:45.000000 paramaterial-0.0.9/paramaterial/__init__.py
+-rw-rw-rw-   0        0        0     3056 2022-11-26 22:19:03.000000 paramaterial-0.0.9/paramaterial/example.py
+-rw-rw-rw-   0        0        0    18451 2022-11-25 09:30:10.000000 paramaterial-0.0.9/paramaterial/modelling.py
+-rw-rw-rw-   0        0        0    15594 2022-11-25 09:30:10.000000 paramaterial-0.0.9/paramaterial/plotting.py
+-rw-rw-rw-   0        0        0     9568 2022-11-25 09:30:10.000000 paramaterial-0.0.9/paramaterial/plug.py
+-rw-rw-rw-   0        0        0     4653 2022-11-26 22:19:03.000000 paramaterial-0.0.9/paramaterial/preparing.py
+-rw-rw-rw-   0        0        0     9404 2022-11-25 09:30:10.000000 paramaterial-0.0.9/paramaterial/processing.py
+-rw-rw-rw-   0        0        0     7478 2022-11-09 18:13:21.000000 paramaterial-0.0.9/paramaterial/receipts.py
+-rw-rw-rw-   0        0        0     4473 2022-11-25 09:30:10.000000 paramaterial-0.0.9/paramaterial/screening.py
+drwxrwxrwx   0        0        0        0 2022-11-26 22:28:30.428434 paramaterial-0.0.9/paramaterial.egg-info/
+-rw-rw-rw-   0        0        0     3100 2022-11-26 22:28:29.000000 paramaterial-0.0.9/paramaterial.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2022-11-26 22:28:30.000000 paramaterial-0.0.9/paramaterial.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-26 22:28:29.000000 paramaterial-0.0.9/paramaterial.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2022-11-26 22:28:30.000000 paramaterial-0.0.9/paramaterial.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-11-26 22:28:30.428434 paramaterial-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2022-11-26 22:27:51.000000 paramaterial-0.0.9/setup.py
```

### Comparing `paramaterial-0.0.8/LICENSE` & `paramaterial-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `paramaterial-0.0.8/PKG-INFO` & `paramaterial-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paramaterial
-Version: 0.0.8
+Version: 0.0.9
 Summary: Software toolkit for parameterising materials test data. Easily batch process experimental measurements to determine mechanical properties and material model parameters.
 Home-page: https://github.com/dan-slater/paramaterial
 Author: Daniel Slater
 Author-email: danielgslater@gmail.com
 License: UNKNOWN
 Keywords: python,mechanical testing,materials testing,post-processing,stress-strain,flow stress,yield stress,tensile test,strength,elastic modulus,strain,universal testing machine,fitting constitutive model,material model,solid mechanics,materials science,engineering
 Platform: UNKNOWN
```

### Comparing `paramaterial-0.0.8/README.md` & `paramaterial-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `paramaterial-0.0.8/paramaterial/example.py` & `paramaterial-0.0.9/paramaterial/example.py`

 * *Files identical despite different names*

### Comparing `paramaterial-0.0.8/paramaterial/modelling.py` & `paramaterial-0.0.9/paramaterial/modelling.py`

 * *Files identical despite different names*

### Comparing `paramaterial-0.0.8/paramaterial/plotting.py` & `paramaterial-0.0.9/paramaterial/plotting.py`

 * *Files identical despite different names*

### Comparing `paramaterial-0.0.8/paramaterial/plug.py` & `paramaterial-0.0.9/paramaterial/plug.py`

 * *Files identical despite different names*

### Comparing `paramaterial-0.0.8/paramaterial/preparing.py` & `paramaterial-0.0.9/paramaterial/preparing.py`

 * *Files identical despite different names*

### Comparing `paramaterial-0.0.8/paramaterial/processing.py` & `paramaterial-0.0.9/paramaterial/processing.py`

 * *Files identical despite different names*

### Comparing `paramaterial-0.0.8/paramaterial/receipts.py` & `paramaterial-0.0.9/paramaterial/receipts.py`

 * *Files identical despite different names*

### Comparing `paramaterial-0.0.8/paramaterial/screening.py` & `paramaterial-0.0.9/paramaterial/screening.py`

 * *Files identical despite different names*

### Comparing `paramaterial-0.0.8/paramaterial.egg-info/PKG-INFO` & `paramaterial-0.0.9/paramaterial.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paramaterial
-Version: 0.0.8
+Version: 0.0.9
 Summary: Software toolkit for parameterising materials test data. Easily batch process experimental measurements to determine mechanical properties and material model parameters.
 Home-page: https://github.com/dan-slater/paramaterial
 Author: Daniel Slater
 Author-email: danielgslater@gmail.com
 License: UNKNOWN
 Keywords: python,mechanical testing,materials testing,post-processing,stress-strain,flow stress,yield stress,tensile test,strength,elastic modulus,strain,universal testing machine,fitting constitutive model,material model,solid mechanics,materials science,engineering
 Platform: UNKNOWN
```

### Comparing `paramaterial-0.0.8/setup.py` & `paramaterial-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Software toolkit for parameterising materials test data. ' \
               'Easily batch process experimental measurements to determine mechanical properties and material model ' \
               'parameters.'
 
 
 def readme():
     with open('README.md') as f:
```

