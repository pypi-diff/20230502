# Comparing `tmp/secure_pickle-0.0.7.tar.gz` & `tmp/secure_pickle-0.0.8.tar.gz`

## Comparing `secure_pickle-0.0.7.tar` & `secure_pickle-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/src/securepickle/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/src/securepickle/securepickle.py
--rw-r--r--   0        0        0 11179058 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/tests/test.pickle
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/tests/test.py
--rw-r--r--   0        0        0   264426 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/tests/winequality-white.csv
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/LICENSE
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 secure_pickle-0.0.8/src/securepickle/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 secure_pickle-0.0.8/src/securepickle/securepickle.py
+-rw-r--r--   0        0        0 11179058 2020-02-02 00:00:00.000000 secure_pickle-0.0.8/tests/test.pickle
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 secure_pickle-0.0.8/tests/test.py
+-rw-r--r--   0        0        0   264426 2020-02-02 00:00:00.000000 secure_pickle-0.0.8/tests/winequality-white.csv
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 secure_pickle-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 secure_pickle-0.0.8/README.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 secure_pickle-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 secure_pickle-0.0.8/PKG-INFO
```

### Comparing `secure_pickle-0.0.7/src/securepickle/securepickle.py` & `secure_pickle-0.0.8/src/securepickle/securepickle.py`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.7/tests/test.pickle` & `secure_pickle-0.0.8/tests/test.pickle`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.7/tests/test.py` & `secure_pickle-0.0.8/tests/test.py`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.7/tests/winequality-white.csv` & `secure_pickle-0.0.8/tests/winequality-white.csv`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.7/LICENSE` & `secure_pickle-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.7/README.md` & `secure_pickle-0.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# secure-pickle-files
+# secure-pickle
 The "pickle" package in python enables users to export almost any type of object containing data to an external file. This file can then be simply loaded into memory whenever the need for the object arises, as opposed to regenerating the object each time. The main application of this package is for objects which are computationally expensive to generate, such as machine learning models. This repo contains a python package which streamlines the process of ensuring the integrity of a pickle file by attaching a hash-based message authentication code (HMAC) with it.
 
 ## Usage
 
 To use this package simply run the command 'pip3 install secure-pickle' and include the line 
 
-from securepickling.src.securepickle import securedump, secureload
+`from securepickling.src.securepickle import securedump, secureload`
 
 at the top of your file and then the two included functions will be callable by their name.
 
 The package contains two functions which are based on the Python 'pickle' module: 
 
 securedump(obj, file, SECRETKEY)
 
@@ -24,8 +24,15 @@
 secureload(file, SECRETKEY)
 
     desc: Loads bytedata from 'file' and verifies its integrity using the HMAC in the file and the bytedata and 'SECRETKEY'
 
     params: file - A file object which must be in 'rb' mode
             SECRETKEY - A string or bytearray which will be used to verify the HMAC
 
-    returns: the object loaded from pickle file, assuming integrity check passes
+    returns: the object loaded from pickle file, assuming integrity check passes
+
+
+## Links
+
+https://pypi.org/project/secure-pickle/
+
+https://github.com/Ethan-Dowalter/securepickling
```

### Comparing `secure_pickle-0.0.7/pyproject.toml` & `secure_pickle-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "secure-pickle"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Ethan Dowalter", email="edowalte@uwyo.edu" },
 ]
 description = "A small package which can add HMACs to pickle files for integrity checks upon unpickling"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `secure_pickle-0.0.7/PKG-INFO` & `secure_pickle-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: secure-pickle
-Version: 0.0.7
+Version: 0.0.8
 Summary: A small package which can add HMACs to pickle files for integrity checks upon unpickling
 Project-URL: Homepage, https://github.com/Ethan-Dowalter/secure-pickle-files
 Project-URL: Bug Tracker, https://github.com/Ethan-Dowalter/secure-pickle-files/issues
 Author-email: Ethan Dowalter <edowalte@uwyo.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# secure-pickle-files
+# secure-pickle
 The "pickle" package in python enables users to export almost any type of object containing data to an external file. This file can then be simply loaded into memory whenever the need for the object arises, as opposed to regenerating the object each time. The main application of this package is for objects which are computationally expensive to generate, such as machine learning models. This repo contains a python package which streamlines the process of ensuring the integrity of a pickle file by attaching a hash-based message authentication code (HMAC) with it.
 
 ## Usage
 
 To use this package simply run the command 'pip3 install secure-pickle' and include the line 
 
-from securepickling.src.securepickle import securedump, secureload
+`from securepickling.src.securepickle import securedump, secureload`
 
 at the top of your file and then the two included functions will be callable by their name.
 
 The package contains two functions which are based on the Python 'pickle' module: 
 
 securedump(obj, file, SECRETKEY)
 
@@ -38,8 +38,15 @@
 secureload(file, SECRETKEY)
 
     desc: Loads bytedata from 'file' and verifies its integrity using the HMAC in the file and the bytedata and 'SECRETKEY'
 
     params: file - A file object which must be in 'rb' mode
             SECRETKEY - A string or bytearray which will be used to verify the HMAC
 
-    returns: the object loaded from pickle file, assuming integrity check passes
+    returns: the object loaded from pickle file, assuming integrity check passes
+
+
+## Links
+
+https://pypi.org/project/secure-pickle/
+
+https://github.com/Ethan-Dowalter/securepickling
```

