# Comparing `tmp/flow_helpers_tps-2023.5.1.2100.tar.gz` & `tmp/flow_helpers_tps-2023.5.1.2158.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow_helpers_tps-2023.5.1.2100.tar", max compression
+gzip compressed data, was "flow_helpers_tps-2023.5.1.2158.tar", max compression
```

## Comparing `flow_helpers_tps-2023.5.1.2100.tar` & `flow_helpers_tps-2023.5.1.2158.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1069 2023-05-01 21:00:22.956076 flow_helpers_tps-2023.5.1.2100/LICENSE
--rw-r--r--   0        0        0        0 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/__init__.py
--rw-r--r--   0        0        0     4868 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_bingwmt.py
--rw-r--r--   0        0        0      657 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_covidtracking.py
--rw-r--r--   0        0        0     3895 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_dcm.py
--rw-r--r--   0        0        0     3230 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_facebook.py
--rw-r--r--   0        0        0      488 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_file.py
--rw-r--r--   0        0        0     9315 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_firebasetransform.py
--rw-r--r--   0        0        0    10574 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_funneltransform.py
--rw-r--r--   0        0        0    24475 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_gatransform.py
--rw-r--r--   0        0        0     6953 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_gbq.py
--rw-r--r--   0        0        0     4308 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_gcs.py
--rw-r--r--   0        0        0     2639 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_gdrive.py
--rw-r--r--   0        0        0    11001 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_googleanalytics.py
--rw-r--r--   0        0        0     4408 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_gsc.py
--rw-r--r--   0        0        0      631 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_gsheet.py
--rw-r--r--   0        0        0      981 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_impact.py
--rw-r--r--   0        0        0     7255 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_journera.py
--rw-r--r--   0        0        0     2986 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_listen360.py
--rw-r--r--   0        0        0     6403 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_mssql.py
--rw-r--r--   0        0        0      505 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_s3.py
--rw-r--r--   0        0        0     7919 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_sa360.py
--rw-r--r--   0        0        0    18284 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_salesforce.py
--rw-r--r--   0        0        0     2615 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_scrapinghub.py
--rw-r--r--   0        0        0     6739 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_sftp.py
--rw-r--r--   0        0        0     6113 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_sharepoint.py
--rw-r--r--   0        0        0    11585 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_snowflake.py
--rw-r--r--   0        0        0     2264 2023-05-01 21:00:22.964076 flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_time.py
--rw-r--r--   0        0        0      622 2023-05-01 21:00:59.431510 flow_helpers_tps-2023.5.1.2100/pyproject.toml
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 flow_helpers_tps-2023.5.1.2100/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-01 21:58:05.906715 flow_helpers_tps-2023.5.1.2158/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-01 21:58:05.914715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/__init__.py
+-rw-r--r--   0        0        0     4868 2023-05-01 21:58:05.914715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_bingwmt.py
+-rw-r--r--   0        0        0      657 2023-05-01 21:58:05.914715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_covidtracking.py
+-rw-r--r--   0        0        0     3895 2023-05-01 21:58:05.914715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_dcm.py
+-rw-r--r--   0        0        0     3230 2023-05-01 21:58:05.914715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_facebook.py
+-rw-r--r--   0        0        0      488 2023-05-01 21:58:05.914715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_file.py
+-rw-r--r--   0        0        0     9315 2023-05-01 21:58:05.914715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_firebasetransform.py
+-rw-r--r--   0        0        0    10574 2023-05-01 21:58:05.914715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_funneltransform.py
+-rw-r--r--   0        0        0    24475 2023-05-01 21:58:05.914715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_gatransform.py
+-rw-r--r--   0        0        0     6953 2023-05-01 21:58:05.914715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_gbq.py
+-rw-r--r--   0        0        0     4308 2023-05-01 21:58:05.914715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_gcs.py
+-rw-r--r--   0        0        0     2639 2023-05-01 21:58:05.914715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_gdrive.py
+-rw-r--r--   0        0        0    11001 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_googleanalytics.py
+-rw-r--r--   0        0        0     4408 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_gsc.py
+-rw-r--r--   0        0        0      631 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_gsheet.py
+-rw-r--r--   0        0        0      981 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_impact.py
+-rw-r--r--   0        0        0     7255 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_journera.py
+-rw-r--r--   0        0        0     2986 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_listen360.py
+-rw-r--r--   0        0        0     6403 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_mssql.py
+-rw-r--r--   0        0        0      505 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_s3.py
+-rw-r--r--   0        0        0     7919 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_sa360.py
+-rw-r--r--   0        0        0    18284 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_salesforce.py
+-rw-r--r--   0        0        0     2615 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_scrapinghub.py
+-rw-r--r--   0        0        0     6739 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_sftp.py
+-rw-r--r--   0        0        0     6113 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_sharepoint.py
+-rw-r--r--   0        0        0    11579 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_snowflake.py
+-rw-r--r--   0        0        0     2264 2023-05-01 21:58:05.918715 flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_time.py
+-rw-r--r--   0        0        0      622 2023-05-01 21:58:39.263298 flow_helpers_tps-2023.5.1.2158/pyproject.toml
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 flow_helpers_tps-2023.5.1.2158/PKG-INFO
```

### Comparing `flow_helpers_tps-2023.5.1.2100/LICENSE` & `flow_helpers_tps-2023.5.1.2158/LICENSE`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_bingwmt.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_bingwmt.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_covidtracking.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_covidtracking.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_dcm.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_dcm.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_facebook.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_facebook.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_firebasetransform.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_firebasetransform.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_funneltransform.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_funneltransform.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_gatransform.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_gatransform.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_gbq.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_gbq.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_gcs.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_gcs.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_gdrive.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_gdrive.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_googleanalytics.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_googleanalytics.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_gsc.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_gsc.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_gsheet.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_gsheet.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_impact.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_impact.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_journera.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_journera.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_listen360.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_listen360.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_mssql.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_mssql.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_sa360.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_sa360.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_salesforce.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_salesforce.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_scrapinghub.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_scrapinghub.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_sftp.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_sftp.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_sharepoint.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_sharepoint.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_snowflake.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     def __init__(self, url=None, warehouse=None, db=None, schema=None):
         if url is not None:
             self.url = url
         elif (url is None) and (warehouse is not None) and (db is not None) and (schema is not None):
             self.url = f'{url}/{db}/{schema}?warehouse={warehouse}'
 
-    def read_sqlfile(self, file):
+    def read_sqlfile(file):
         with open(file) as f:
             _sql = f.read()
         return _sql
 
     def execute(self, sql, database_block=None):
         if database_block:
             with database_block as database:
```

### Comparing `flow_helpers_tps-2023.5.1.2100/flow_helpers_tps/_time.py` & `flow_helpers_tps-2023.5.1.2158/flow_helpers_tps/_time.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.5.1.2100/pyproject.toml` & `flow_helpers_tps-2023.5.1.2158/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flow-helpers-tps"
-version = "2023.05.01.2100"
+version = "2023.05.01.2158"
 description = "Handy helpers for ETL and API interfacing."
 authors = [ "joshliu3 <jliu@theparkingspot.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 google-api-python-client = "^2.85.0"
```

### Comparing `flow_helpers_tps-2023.5.1.2100/PKG-INFO` & `flow_helpers_tps-2023.5.1.2158/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flow-helpers-tps
-Version: 2023.5.1.2100
+Version: 2023.5.1.2158
 Summary: Handy helpers for ETL and API interfacing.
 License: MIT
 Author: joshliu3
 Author-email: jliu@theparkingspot.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

