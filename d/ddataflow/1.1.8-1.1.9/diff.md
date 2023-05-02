# Comparing `tmp/ddataflow-1.1.8.tar.gz` & `tmp/ddataflow-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddataflow-1.1.8.tar", max compression
+gzip compressed data, was "ddataflow-1.1.9.tar", max compression
```

## Comparing `ddataflow-1.1.8.tar` & `ddataflow-1.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2022-10-01 09:22:40.621071 ddataflow-1.1.8/LICENSE.txt
--rw-r--r--   0        0        0       98 2022-10-01 09:22:40.621348 ddataflow-1.1.8/ddataflow/__init__.py
--rw-r--r--   0        0        0     4121 2022-10-11 14:50:00.074077 ddataflow-1.1.8/ddataflow/data_source.py
--rw-r--r--   0        0        0     1274 2022-10-11 14:50:00.074235 ddataflow-1.1.8/ddataflow/data_sources.py
--rw-r--r--   0        0        0    13869 2022-10-20 11:11:20.695944 ddataflow-1.1.8/ddataflow/ddataflow.py
--rw-r--r--   0        0        0     2104 2022-10-12 13:24:20.515140 ddataflow-1.1.8/ddataflow/downloader.py
--rw-r--r--   0        0        0      723 2022-10-01 09:22:40.621844 ddataflow-1.1.8/ddataflow/exceptions.py
--rw-r--r--   0        0        0        0 2022-10-11 14:50:00.074905 ddataflow-1.1.8/ddataflow/sampling/__init__.py
--rw-r--r--   0        0        0     1748 2022-10-12 14:09:25.040491 ddataflow-1.1.8/ddataflow/sampling/default.py
--rw-r--r--   0        0        0     3466 2022-10-12 13:24:20.529199 ddataflow-1.1.8/ddataflow/sampling/sampler.py
--rw-r--r--   0        0        0     1187 2022-10-12 13:29:59.177496 ddataflow-1.1.8/ddataflow/setup/__init__.py
--rw-r--r--   0        0        0     1337 2022-10-12 14:01:33.731861 ddataflow-1.1.8/ddataflow/setup/ddataflow_config.py
--rw-r--r--   0        0        0      318 2022-10-12 13:40:39.184793 ddataflow-1.1.8/ddataflow/setup/setup_project.py
--rw-r--r--   0        0        0      973 2022-10-11 14:50:00.075667 ddataflow-1.1.8/ddataflow/utils.py
--rw-r--r--   0        0        0      718 2022-10-31 14:15:01.393468 ddataflow-1.1.8/pyproject.toml
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 ddataflow-1.1.8/setup.py
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 ddataflow-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-10-01 09:22:40.621071 ddataflow-1.1.9/LICENSE.txt
+-rw-r--r--   0        0        0       98 2022-10-01 09:22:40.621348 ddataflow-1.1.9/ddataflow/__init__.py
+-rw-r--r--   0        0        0     4121 2022-10-11 14:50:00.074077 ddataflow-1.1.9/ddataflow/data_source.py
+-rw-r--r--   0        0        0     1274 2022-10-11 14:50:00.074235 ddataflow-1.1.9/ddataflow/data_sources.py
+-rw-r--r--   0        0        0    13869 2022-10-31 14:18:15.812426 ddataflow-1.1.9/ddataflow/ddataflow.py
+-rw-r--r--   0        0        0     2104 2022-10-12 13:24:20.515140 ddataflow-1.1.9/ddataflow/downloader.py
+-rw-r--r--   0        0        0      723 2022-10-01 09:22:40.621844 ddataflow-1.1.9/ddataflow/exceptions.py
+-rw-r--r--   0        0        0        0 2022-10-11 14:50:00.074905 ddataflow-1.1.9/ddataflow/sampling/__init__.py
+-rw-r--r--   0        0        0     1748 2022-10-31 14:18:15.813264 ddataflow-1.1.9/ddataflow/sampling/default.py
+-rw-r--r--   0        0        0     3466 2022-10-12 13:24:20.529199 ddataflow-1.1.9/ddataflow/sampling/sampler.py
+-rw-r--r--   0        0        0     1187 2022-10-12 13:29:59.177496 ddataflow-1.1.9/ddataflow/setup/__init__.py
+-rw-r--r--   0        0        0     1337 2022-10-31 14:18:15.813537 ddataflow-1.1.9/ddataflow/setup/ddataflow_config.py
+-rw-r--r--   0        0        0      318 2022-10-12 13:40:39.184793 ddataflow-1.1.9/ddataflow/setup/setup_project.py
+-rw-r--r--   0        0        0      973 2022-10-11 14:50:00.075667 ddataflow-1.1.9/ddataflow/utils.py
+-rw-r--r--   0        0        0      720 2022-11-07 16:17:25.800163 ddataflow-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 ddataflow-1.1.9/setup.py
+-rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 ddataflow-1.1.9/PKG-INFO
```

### Comparing `ddataflow-1.1.8/LICENSE.txt` & `ddataflow-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ddataflow-1.1.8/ddataflow/data_source.py` & `ddataflow-1.1.9/ddataflow/data_source.py`

 * *Files identical despite different names*

### Comparing `ddataflow-1.1.8/ddataflow/data_sources.py` & `ddataflow-1.1.9/ddataflow/data_sources.py`

 * *Files identical despite different names*

### Comparing `ddataflow-1.1.8/ddataflow/ddataflow.py` & `ddataflow-1.1.9/ddataflow/ddataflow.py`

 * *Files identical despite different names*

### Comparing `ddataflow-1.1.8/ddataflow/downloader.py` & `ddataflow-1.1.9/ddataflow/downloader.py`

 * *Files identical despite different names*

### Comparing `ddataflow-1.1.8/ddataflow/exceptions.py` & `ddataflow-1.1.9/ddataflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `ddataflow-1.1.8/ddataflow/sampling/default.py` & `ddataflow-1.1.9/ddataflow/sampling/default.py`

 * *Files identical despite different names*

### Comparing `ddataflow-1.1.8/ddataflow/sampling/sampler.py` & `ddataflow-1.1.9/ddataflow/sampling/sampler.py`

 * *Files identical despite different names*

### Comparing `ddataflow-1.1.8/ddataflow/setup/__init__.py` & `ddataflow-1.1.9/ddataflow/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `ddataflow-1.1.8/ddataflow/setup/ddataflow_config.py` & `ddataflow-1.1.9/ddataflow/setup/ddataflow_config.py`

 * *Files identical despite different names*

### Comparing `ddataflow-1.1.8/ddataflow/utils.py` & `ddataflow-1.1.9/ddataflow/utils.py`

 * *Files identical despite different names*

### Comparing `ddataflow-1.1.8/pyproject.toml` & `ddataflow-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "DDataFlow"
-version = "1.1.8"
+version = "1.1.9"
 description = "A tool for end2end data tests"
 authors = ["Data products GYG <engineering.data-products@getyourguide.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 databricks-cli = {version = ">=0.16"}
 pyspark = ">3"
 fire = ">=0.4"
 # this is not a direct dependency of the template, but a dependency of databricks-cli
 # that comes from mlflow, if we dont pin it here we get a lower version that has a security problem
 oauthlib = ">=3.2.1"
-urllib3 = ">=1.23"
+urllib3 = ">=1.24.2"
 
 [tool.poetry.scripts]
 ddataflow = 'ddataflow.ddataflow:main'
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
```

### Comparing `ddataflow-1.1.8/setup.py` & `ddataflow-1.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['databricks-cli>=0.16',
  'fire>=0.4',
  'oauthlib>=3.2.1',
  'pyspark>3',
- 'urllib3>=1.23']
+ 'urllib3>=1.24.2']
 
 entry_points = \
 {'console_scripts': ['ddataflow = ddataflow.ddataflow:main']}
 
 setup_kwargs = {
     'name': 'ddataflow',
-    'version': '1.1.8',
+    'version': '1.1.9',
     'description': 'A tool for end2end data tests',
     'long_description': 'None',
     'author': 'Data products GYG',
     'author_email': 'engineering.data-products@getyourguide.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ddataflow-1.1.8/PKG-INFO` & `ddataflow-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ddataflow
-Version: 1.1.8
+Version: 1.1.9
 Summary: A tool for end2end data tests
 Author: Data products GYG
 Author-email: engineering.data-products@getyourguide.com
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: databricks-cli (>=0.16)
 Requires-Dist: fire (>=0.4)
 Requires-Dist: oauthlib (>=3.2.1)
 Requires-Dist: pyspark (>3)
-Requires-Dist: urllib3 (>=1.23)
+Requires-Dist: urllib3 (>=1.24.2)
```

