# Comparing `tmp/secure_pickle-0.0.6.tar.gz` & `tmp/secure_pickle-0.0.7.tar.gz`

## Comparing `secure_pickle-0.0.6.tar` & `secure_pickle-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 secure_pickle-0.0.6/src/securepickle/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 secure_pickle-0.0.6/src/securepickle/securepickle.py
--rw-r--r--   0        0        0 11179058 2020-02-02 00:00:00.000000 secure_pickle-0.0.6/tests/test.pickle
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 secure_pickle-0.0.6/tests/test.py
--rw-r--r--   0        0        0   264426 2020-02-02 00:00:00.000000 secure_pickle-0.0.6/tests/winequality-white.csv
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 secure_pickle-0.0.6/LICENSE
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 secure_pickle-0.0.6/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 secure_pickle-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 secure_pickle-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/src/securepickle/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/src/securepickle/securepickle.py
+-rw-r--r--   0        0        0 11179058 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/tests/test.pickle
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/tests/test.py
+-rw-r--r--   0        0        0   264426 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/tests/winequality-white.csv
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/README.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 secure_pickle-0.0.7/PKG-INFO
```

### Comparing `secure_pickle-0.0.6/src/securepickle/securepickle.py` & `secure_pickle-0.0.7/src/securepickle/securepickle.py`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.6/tests/test.pickle` & `secure_pickle-0.0.7/tests/test.pickle`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.6/tests/test.py` & `secure_pickle-0.0.7/tests/test.py`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.6/tests/winequality-white.csv` & `secure_pickle-0.0.7/tests/winequality-white.csv`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.6/LICENSE` & `secure_pickle-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.6/README.md` & `secure_pickle-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # secure-pickle-files
 The "pickle" package in python enables users to export almost any type of object containing data to an external file. This file can then be simply loaded into memory whenever the need for the object arises, as opposed to regenerating the object each time. The main application of this package is for objects which are computationally expensive to generate, such as machine learning models. This repo contains a python package which streamlines the process of ensuring the integrity of a pickle file by attaching a hash-based message authentication code (HMAC) with it.
 
 ## Usage
 
-To use this package simply run the command 'pip3 install secure-pickle' and include the line 'from securepickling.src.securepickle import securedump, secureload' at the top of your file and then the two included functions will be callable by their name.
+To use this package simply run the command 'pip3 install secure-pickle' and include the line 
+
+from securepickling.src.securepickle import securedump, secureload
+
+at the top of your file and then the two included functions will be callable by their name.
 
 The package contains two functions which are based on the Python 'pickle' module: 
 
 securedump(obj, file, SECRETKEY)
 
     desc: Writes bytedata of 'obj' and an HMAC generated with 'obj' and 'SECRETKEY' to 'file'
```

### Comparing `secure_pickle-0.0.6/pyproject.toml` & `secure_pickle-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "secure-pickle"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Ethan Dowalter", email="edowalte@uwyo.edu" },
 ]
 description = "A small package which can add HMACs to pickle files for integrity checks upon unpickling"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `secure_pickle-0.0.6/PKG-INFO` & `secure_pickle-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-pickle
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small package which can add HMACs to pickle files for integrity checks upon unpickling
 Project-URL: Homepage, https://github.com/Ethan-Dowalter/secure-pickle-files
 Project-URL: Bug Tracker, https://github.com/Ethan-Dowalter/secure-pickle-files/issues
 Author-email: Ethan Dowalter <edowalte@uwyo.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,19 @@
 Description-Content-Type: text/markdown
 
 # secure-pickle-files
 The "pickle" package in python enables users to export almost any type of object containing data to an external file. This file can then be simply loaded into memory whenever the need for the object arises, as opposed to regenerating the object each time. The main application of this package is for objects which are computationally expensive to generate, such as machine learning models. This repo contains a python package which streamlines the process of ensuring the integrity of a pickle file by attaching a hash-based message authentication code (HMAC) with it.
 
 ## Usage
 
-To use this package simply run the command 'pip3 install secure-pickle' and include the line 'from securepickling.src.securepickle import securedump, secureload' at the top of your file and then the two included functions will be callable by their name.
+To use this package simply run the command 'pip3 install secure-pickle' and include the line 
+
+from securepickling.src.securepickle import securedump, secureload
+
+at the top of your file and then the two included functions will be callable by their name.
 
 The package contains two functions which are based on the Python 'pickle' module: 
 
 securedump(obj, file, SECRETKEY)
 
     desc: Writes bytedata of 'obj' and an HMAC generated with 'obj' and 'SECRETKEY' to 'file'
```

