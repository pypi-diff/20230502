# Comparing `tmp/secure_pickle-0.0.3.tar.gz` & `tmp/secure_pickle-0.0.4.tar.gz`

## Comparing `secure_pickle-0.0.3.tar` & `secure_pickle-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/src/securepickle/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/src/securepickle/securepickle.py
--rw-r--r--   0        0        0 11179058 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/tests/test.pickle
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/tests/test.py
--rw-r--r--   0        0        0   264426 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/tests/winequality-white.csv
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/LICENSE
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/src/securepickle/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/src/securepickle/securepickle.py
+-rw-r--r--   0        0        0 11179058 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/tests/test.pickle
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/tests/test.py
+-rw-r--r--   0        0        0   264426 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/tests/winequality-white.csv
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/README.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/PKG-INFO
```

### Comparing `secure_pickle-0.0.3/src/securepickle/securepickle.py` & `secure_pickle-0.0.4/src/securepickle/securepickle.py`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.3/tests/test.pickle` & `secure_pickle-0.0.4/tests/test.pickle`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.3/tests/test.py` & `secure_pickle-0.0.4/tests/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-sys.path.insert(0, '../src/picklesecure')
+sys.path.insert(0, '../src/securepickle')
 from securepickle import securedump, secureload
 
 import pandas
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import train_test_split
 import sklearn.metrics
```

### Comparing `secure_pickle-0.0.3/tests/winequality-white.csv` & `secure_pickle-0.0.4/tests/winequality-white.csv`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.3/LICENSE` & `secure_pickle-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.3/pyproject.toml` & `secure_pickle-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "secure-pickle"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Ethan Dowalter", email="edowalte@uwyo.edu" },
 ]
 description = "A small package which can add HMACs to pickle files for integrity checks upon unpickling"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `secure_pickle-0.0.3/PKG-INFO` & `secure_pickle-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-pickle
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small package which can add HMACs to pickle files for integrity checks upon unpickling
 Project-URL: Homepage, https://github.com/Ethan-Dowalter/secure-pickle-files
 Project-URL: Bug Tracker, https://github.com/Ethan-Dowalter/secure-pickle-files/issues
 Author-email: Ethan Dowalter <edowalte@uwyo.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,7 +14,22 @@
 
 # secure-pickle-files
 The "pickle" package in python enables users to export almost any type of object containing data to an external file. This file can then be simply loaded into memory whenever the need for the object arises, as opposed to regenerating the object each time. The main application of this package is for objects which are computationally expensive to generate, such as machine learning models. This repo contains a python package which streamlines the process of ensuring the integrity of a pickle file by attaching a hash-based message authentication code (HMAC) with it.
 
 ## Usage
 
 To use this package simply run the command 'pip3 install secure-pickle' and 
+
+The package contains two functions which are based on the Python 'pickle' module: 
+
+securedump(obj, file, SECRETKEY)
+    desc: Writes bytedata of 'obj' and an HMAC generated with 'obj' and 'SECRETKEY' to 'file'
+    params: obj - Any python object that you wish to write out to a pickle file
+            file - A file object which must be in 'wb' mode
+            SECRETKEY - A string or bytearray which must be at least 64 bytes to ensure security
+    returns: nothing
+
+secureload(file, SECRETKEY)
+    desc: Loads bytedata from 'file' and verifies its integrity using the HMAC in the file and the bytedata and 'SECRETKEY'
+    params: file - A file object which must be in 'rb' mode
+            SECRETKEY - A string or bytearray which will be used to verify the HMAC
+    returns: the object loaded from pickle file, assuming integrity check passes
```

