# Comparing `tmp/secure_pickle-0.0.4.tar.gz` & `tmp/secure_pickle-0.0.5.tar.gz`

## Comparing `secure_pickle-0.0.4.tar` & `secure_pickle-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/src/securepickle/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/src/securepickle/securepickle.py
--rw-r--r--   0        0        0 11179058 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/tests/test.pickle
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/tests/test.py
--rw-r--r--   0        0        0   264426 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/tests/winequality-white.csv
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/LICENSE
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 secure_pickle-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 secure_pickle-0.0.5/src/securepickle/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 secure_pickle-0.0.5/src/securepickle/securepickle.py
+-rw-r--r--   0        0        0 11179058 2020-02-02 00:00:00.000000 secure_pickle-0.0.5/tests/test.pickle
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 secure_pickle-0.0.5/tests/test.py
+-rw-r--r--   0        0        0   264426 2020-02-02 00:00:00.000000 secure_pickle-0.0.5/tests/winequality-white.csv
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 secure_pickle-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 secure_pickle-0.0.5/README.md
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 secure_pickle-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 secure_pickle-0.0.5/PKG-INFO
```

### Comparing `secure_pickle-0.0.4/src/securepickle/securepickle.py` & `secure_pickle-0.0.5/src/securepickle/securepickle.py`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.4/tests/test.pickle` & `secure_pickle-0.0.5/tests/test.pickle`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.4/tests/test.py` & `secure_pickle-0.0.5/tests/test.py`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.4/tests/winequality-white.csv` & `secure_pickle-0.0.5/tests/winequality-white.csv`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.4/LICENSE` & `secure_pickle-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.4/README.md` & `secure_pickle-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `secure_pickle-0.0.4/pyproject.toml` & `secure_pickle-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "secure-pickle"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Ethan Dowalter", email="edowalte@uwyo.edu" },
 ]
 description = "A small package which can add HMACs to pickle files for integrity checks upon unpickling"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `secure_pickle-0.0.4/PKG-INFO` & `secure_pickle-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-pickle
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small package which can add HMACs to pickle files for integrity checks upon unpickling
 Project-URL: Homepage, https://github.com/Ethan-Dowalter/secure-pickle-files
 Project-URL: Bug Tracker, https://github.com/Ethan-Dowalter/secure-pickle-files/issues
 Author-email: Ethan Dowalter <edowalte@uwyo.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

