# Comparing `tmp/airflow-provider-duckdb-0.0.2.tar.gz` & `tmp/airflow-provider-duckdb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-duckdb-0.0.2.tar", last modified: Thu Feb  2 17:27:20 2023, max compression
+gzip compressed data, was "airflow-provider-duckdb-0.1.0.tar", last modified: Tue May  2 14:54:57 2023, max compression
```

## Comparing `airflow-provider-duckdb-0.0.2.tar` & `airflow-provider-duckdb-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-02-02 17:27:20.827721 airflow-provider-duckdb-0.0.2/
--rw-r--r--   0 julian     (502) staff       (20)    11357 2022-10-30 21:15:10.000000 airflow-provider-duckdb-0.0.2/LICENSE
--rw-r--r--   0 julian     (502) staff       (20)     2726 2023-02-02 17:27:20.827577 airflow-provider-duckdb-0.0.2/PKG-INFO
--rw-r--r--   0 julian     (502) staff       (20)     2306 2023-02-02 17:24:37.000000 airflow-provider-duckdb-0.0.2/README.md
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-02-02 17:27:20.826547 airflow-provider-duckdb-0.0.2/airflow_provider_duckdb.egg-info/
--rw-r--r--   0 julian     (502) staff       (20)     2726 2023-02-02 17:27:20.000000 airflow-provider-duckdb-0.0.2/airflow_provider_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 julian     (502) staff       (20)      409 2023-02-02 17:27:20.000000 airflow-provider-duckdb-0.0.2/airflow_provider_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 julian     (502) staff       (20)        1 2023-02-02 17:27:20.000000 airflow-provider-duckdb-0.0.2/airflow_provider_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 julian     (502) staff       (20)       85 2023-02-02 17:27:20.000000 airflow-provider-duckdb-0.0.2/airflow_provider_duckdb.egg-info/entry_points.txt
--rw-r--r--   0 julian     (502) staff       (20)       48 2023-02-02 17:27:20.000000 airflow-provider-duckdb-0.0.2/airflow_provider_duckdb.egg-info/requires.txt
--rw-r--r--   0 julian     (502) staff       (20)       16 2023-02-02 17:27:20.000000 airflow-provider-duckdb-0.0.2/airflow_provider_duckdb.egg-info/top_level.txt
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-02-02 17:27:20.826690 airflow-provider-duckdb-0.0.2/duckdb_provider/
--rw-r--r--   0 julian     (502) staff       (20)      320 2022-10-31 14:16:34.000000 airflow-provider-duckdb-0.0.2/duckdb_provider/__init__.py
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-02-02 17:27:20.827213 airflow-provider-duckdb-0.0.2/duckdb_provider/hooks/
--rw-r--r--   0 julian     (502) staff       (20)        0 2022-10-30 21:28:31.000000 airflow-provider-duckdb-0.0.2/duckdb_provider/hooks/__init__.py
--rw-r--r--   0 julian     (502) staff       (20)     1799 2022-10-31 14:37:54.000000 airflow-provider-duckdb-0.0.2/duckdb_provider/hooks/duckdb_hook.py
--rw-r--r--   0 julian     (502) staff       (20)       38 2023-02-02 17:27:20.827762 airflow-provider-duckdb-0.0.2/setup.cfg
--rw-r--r--   0 julian     (502) staff       (20)      944 2023-02-02 17:26:10.000000 airflow-provider-duckdb-0.0.2/setup.py
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-05-02 14:54:57.291730 airflow-provider-duckdb-0.1.0/
+-rw-r--r--   0 julian     (502) staff       (20)    11357 2022-10-30 21:15:10.000000 airflow-provider-duckdb-0.1.0/LICENSE
+-rw-r--r--   0 julian     (502) staff       (20)     2726 2023-05-02 14:54:57.291531 airflow-provider-duckdb-0.1.0/PKG-INFO
+-rw-r--r--   0 julian     (502) staff       (20)     2306 2023-02-02 17:24:37.000000 airflow-provider-duckdb-0.1.0/README.md
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-05-02 14:54:57.290421 airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/
+-rw-r--r--   0 julian     (502) staff       (20)     2726 2023-05-02 14:54:57.000000 airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 julian     (502) staff       (20)      409 2023-05-02 14:54:57.000000 airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 julian     (502) staff       (20)        1 2023-05-02 14:54:57.000000 airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 julian     (502) staff       (20)       85 2023-05-02 14:54:57.000000 airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/entry_points.txt
+-rw-r--r--   0 julian     (502) staff       (20)       48 2023-05-02 14:54:57.000000 airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/requires.txt
+-rw-r--r--   0 julian     (502) staff       (20)       16 2023-05-02 14:54:57.000000 airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/top_level.txt
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-05-02 14:54:57.290588 airflow-provider-duckdb-0.1.0/duckdb_provider/
+-rw-r--r--   0 julian     (502) staff       (20)      471 2023-05-02 14:52:15.000000 airflow-provider-duckdb-0.1.0/duckdb_provider/__init__.py
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-05-02 14:54:57.291143 airflow-provider-duckdb-0.1.0/duckdb_provider/hooks/
+-rw-r--r--   0 julian     (502) staff       (20)        0 2022-10-30 21:28:31.000000 airflow-provider-duckdb-0.1.0/duckdb_provider/hooks/__init__.py
+-rw-r--r--   0 julian     (502) staff       (20)     1799 2022-10-31 14:37:54.000000 airflow-provider-duckdb-0.1.0/duckdb_provider/hooks/duckdb_hook.py
+-rw-r--r--   0 julian     (502) staff       (20)       38 2023-05-02 14:54:57.291778 airflow-provider-duckdb-0.1.0/setup.cfg
+-rw-r--r--   0 julian     (502) staff       (20)      944 2023-05-02 14:54:30.000000 airflow-provider-duckdb-0.1.0/setup.py
```

### Comparing `airflow-provider-duckdb-0.0.2/LICENSE` & `airflow-provider-duckdb-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-provider-duckdb-0.0.2/PKG-INFO` & `airflow-provider-duckdb-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-duckdb
-Version: 0.0.2
+Version: 0.1.0
 Summary: DuckDB (duckdb.org) provider for Apache Airflow
 Home-page: http://astronomer.io/
 Author: Julian LaNeve
 Author-email: julian@astronomer.io
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
```

### Comparing `airflow-provider-duckdb-0.0.2/README.md` & `airflow-provider-duckdb-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `airflow-provider-duckdb-0.0.2/airflow_provider_duckdb.egg-info/PKG-INFO` & `airflow-provider-duckdb-0.1.0/airflow_provider_duckdb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-duckdb
-Version: 0.0.2
+Version: 0.1.0
 Summary: DuckDB (duckdb.org) provider for Apache Airflow
 Home-page: http://astronomer.io/
 Author: Julian LaNeve
 Author-email: julian@astronomer.io
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
```

### Comparing `airflow-provider-duckdb-0.0.2/duckdb_provider/hooks/duckdb_hook.py` & `airflow-provider-duckdb-0.1.0/duckdb_provider/hooks/duckdb_hook.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-duckdb-0.0.2/setup.py` & `airflow-provider-duckdb-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="airflow-provider-duckdb",
-    version="0.0.2",
+    version="0.1.0",
     description="DuckDB (duckdb.org) provider for Apache Airflow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         "apache_airflow_provider": [
             "provider_info=duckdb_provider.__init__:get_provider_info"
         ]
```

