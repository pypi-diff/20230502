# Comparing `tmp/strictly_typed_pandas-0.1.6.tar.gz` & `tmp/strictly_typed_pandas-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strictly_typed_pandas-0.1.6.tar", last modified: Sun Apr  9 07:53:39 2023, max compression
+gzip compressed data, was "strictly_typed_pandas-0.1.8.tar", last modified: Tue May  2 18:22:52 2023, max compression
```

## Comparing `strictly_typed_pandas-0.1.6.tar` & `strictly_typed_pandas-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:53:39.909392 strictly_typed_pandas-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-09 07:53:39.909392 strictly_typed_pandas-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 07:53:39.909392 strictly_typed_pandas-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:53:39.909392 strictly_typed_pandas-0.1.6/strictly_typed_pandas/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/create_empty_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/immutable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/pandas_types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/typeguard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-09 07:53:23.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas/validate_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:53:39.909392 strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-09 07:53:39.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-09 07:53:39.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:53:39.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-09 07:53:39.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 07:53:39.000000 strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:22:52.874759 strictly_typed_pandas-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-02 18:22:41.000000 strictly_typed_pandas-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-02 18:22:52.874759 strictly_typed_pandas-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-02 18:22:41.000000 strictly_typed_pandas-0.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 18:22:52.874759 strictly_typed_pandas-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-02 18:22:41.000000 strictly_typed_pandas-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:22:52.874759 strictly_typed_pandas-0.1.8/strictly_typed_pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-02 18:22:41.000000 strictly_typed_pandas-0.1.8/strictly_typed_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-02 18:22:41.000000 strictly_typed_pandas-0.1.8/strictly_typed_pandas/create_empty_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-05-02 18:22:41.000000 strictly_typed_pandas-0.1.8/strictly_typed_pandas/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-02 18:22:41.000000 strictly_typed_pandas-0.1.8/strictly_typed_pandas/immutable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-02 18:22:41.000000 strictly_typed_pandas-0.1.8/strictly_typed_pandas/pandas_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 18:22:41.000000 strictly_typed_pandas-0.1.8/strictly_typed_pandas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-02 18:22:41.000000 strictly_typed_pandas-0.1.8/strictly_typed_pandas/typeguard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-02 18:22:41.000000 strictly_typed_pandas-0.1.8/strictly_typed_pandas/validate_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:22:52.874759 strictly_typed_pandas-0.1.8/strictly_typed_pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-02 18:22:52.000000 strictly_typed_pandas-0.1.8/strictly_typed_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-02 18:22:52.000000 strictly_typed_pandas-0.1.8/strictly_typed_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:22:52.000000 strictly_typed_pandas-0.1.8/strictly_typed_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 18:22:52.000000 strictly_typed_pandas-0.1.8/strictly_typed_pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 18:22:52.000000 strictly_typed_pandas-0.1.8/strictly_typed_pandas.egg-info/top_level.txt
```

### Comparing `strictly_typed_pandas-0.1.6/LICENSE` & `strictly_typed_pandas-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.6/PKG-INFO` & `strictly_typed_pandas-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strictly_typed_pandas
-Version: 0.1.6
+Version: 0.1.8
 Summary: Static type checking of pandas DataFrames
 Home-page: https://github.com/nanne-aben/strictly_typed_pandas
 Author: Nanne Aben
 Author-email: nanne.aben@gmail.com
 License: MIT
 Keywords: typing type checking pandas mypy linting
 Classifier: Typing :: Typed
```

### Comparing `strictly_typed_pandas-0.1.6/README.rst` & `strictly_typed_pandas-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.6/setup.py` & `strictly_typed_pandas-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.6/strictly_typed_pandas/create_empty_dataframe.py` & `strictly_typed_pandas-0.1.8/strictly_typed_pandas/create_empty_dataframe.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.6/strictly_typed_pandas/dataset.py` & `strictly_typed_pandas-0.1.8/strictly_typed_pandas/dataset.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.6/strictly_typed_pandas/immutable.py` & `strictly_typed_pandas-0.1.8/strictly_typed_pandas/immutable.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.6/strictly_typed_pandas/pandas_types.py` & `strictly_typed_pandas-0.1.8/strictly_typed_pandas/pandas_types.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.6/strictly_typed_pandas/typeguard.py` & `strictly_typed_pandas-0.1.8/strictly_typed_pandas/typeguard.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.6/strictly_typed_pandas/validate_schema.py` & `strictly_typed_pandas-0.1.8/strictly_typed_pandas/validate_schema.py`

 * *Files identical despite different names*

### Comparing `strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/PKG-INFO` & `strictly_typed_pandas-0.1.8/strictly_typed_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strictly-typed-pandas
-Version: 0.1.6
+Version: 0.1.8
 Summary: Static type checking of pandas DataFrames
 Home-page: https://github.com/nanne-aben/strictly_typed_pandas
 Author: Nanne Aben
 Author-email: nanne.aben@gmail.com
 License: MIT
 Keywords: typing type checking pandas mypy linting
 Classifier: Typing :: Typed
```

### Comparing `strictly_typed_pandas-0.1.6/strictly_typed_pandas.egg-info/SOURCES.txt` & `strictly_typed_pandas-0.1.8/strictly_typed_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

