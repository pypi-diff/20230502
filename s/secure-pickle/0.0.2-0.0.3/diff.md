# Comparing `tmp/secure_pickle-0.0.2.tar.gz` & `tmp/secure_pickle-0.0.3.tar.gz`

## Comparing `secure_pickle-0.0.2.tar` & `secure_pickle-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 secure_pickle-0.0.2/src/picklesecure/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 secure_pickle-0.0.2/src/picklesecure/picklesecure.py
--rw-r--r--   0        0        0 11179058 2020-02-02 00:00:00.000000 secure_pickle-0.0.2/tests/test.pickle
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 secure_pickle-0.0.2/tests/test.py
--rw-r--r--   0        0        0   264426 2020-02-02 00:00:00.000000 secure_pickle-0.0.2/tests/winequality-white.csv
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 secure_pickle-0.0.2/LICENSE
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 secure_pickle-0.0.2/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 secure_pickle-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 secure_pickle-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/src/securepickle/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/src/securepickle/securepickle.py
+-rw-r--r--   0        0        0 11179058 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/tests/test.pickle
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/tests/test.py
+-rw-r--r--   0        0        0   264426 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/tests/winequality-white.csv
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/LICENSE
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/README.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 secure_pickle-0.0.3/PKG-INFO
```

### Comparing `secure_pickle-0.0.2/src/picklesecure/picklesecure.py` & `secure_pickle-0.0.3/src/securepickle/securepickle.py`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.2/tests/test.pickle` & `secure_pickle-0.0.3/tests/test.pickle`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.2/tests/test.py` & `secure_pickle-0.0.3/tests/test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 sys.path.insert(0, '../src/picklesecure')
-from picklesecure import securedump, secureload
+from securepickle import securedump, secureload
 
 import pandas
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import train_test_split
 import sklearn.metrics
 
 data = pandas.read_csv("winequality-white.csv", delimiter=";")
```

### Comparing `secure_pickle-0.0.2/tests/winequality-white.csv` & `secure_pickle-0.0.3/tests/winequality-white.csv`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.2/LICENSE` & `secure_pickle-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.2/README.md` & `secure_pickle-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.2/pyproject.toml` & `secure_pickle-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "secure-pickle"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Ethan Dowalter", email="edowalte@uwyo.edu" },
 ]
 description = "A small package which can add HMACs to pickle files for integrity checks upon unpickling"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `secure_pickle-0.0.2/PKG-INFO` & `secure_pickle-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-pickle
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small package which can add HMACs to pickle files for integrity checks upon unpickling
 Project-URL: Homepage, https://github.com/Ethan-Dowalter/secure-pickle-files
 Project-URL: Bug Tracker, https://github.com/Ethan-Dowalter/secure-pickle-files/issues
 Author-email: Ethan Dowalter <edowalte@uwyo.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

