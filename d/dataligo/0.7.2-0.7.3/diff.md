# Comparing `tmp/dataligo-0.7.2.tar.gz` & `tmp/dataligo-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/alchemist/Desktop/OpenSource/dataligo/dist/.tmp-q0swwcn3/dataligo-0.7.2.tar", last modified: Thu Apr 27 17:35:37 2023, max compression
+gzip compressed data, was "/home/alchemist/Desktop/OpenSource/hifxit/dataligo/dist/.tmp-eplkdmcp/dataligo-0.7.3.tar", last modified: Tue May  2 07:52:39 2023, max compression
```

## Comparing `dataligo-0.7.2.tar` & `dataligo-0.7.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 17:35:37.000000 dataligo-0.7.2/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11338 2023-04-15 19:19:37.000000 dataligo-0.7.2/LICENSE
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    19517 2023-04-27 17:35:37.000000 dataligo-0.7.2/PKG-INFO
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     5942 2023-04-26 05:05:28.000000 dataligo-0.7.2/README.md
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 17:35:37.000000 dataligo-0.7.2/dataligo/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      189 2023-04-27 17:34:24.000000 dataligo-0.7.2/dataligo/__init__.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     4068 2023-04-27 17:20:51.000000 dataligo-0.7.2/dataligo/core.py
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 17:35:37.000000 dataligo-0.7.2/dataligo/databases/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-04-15 19:19:37.000000 dataligo-0.7.2/dataligo/databases/__init__.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11633 2023-04-22 06:58:51.000000 dataligo-0.7.2/dataligo/databases/database.py
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 17:35:37.000000 dataligo-0.7.2/dataligo/datalakes/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-04-15 19:19:37.000000 dataligo-0.7.2/dataligo/datalakes/__init__.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    20814 2023-04-26 05:01:07.000000 dataligo-0.7.2/dataligo/datalakes/datalake.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    10320 2023-04-22 09:57:28.000000 dataligo-0.7.2/dataligo/datalakes/utils.py
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 17:35:37.000000 dataligo-0.7.2/dataligo/datawarehouses/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-04-15 19:19:37.000000 dataligo-0.7.2/dataligo/datawarehouses/__init__.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    12643 2023-04-23 15:01:59.000000 dataligo-0.7.2/dataligo/datawarehouses/datawarehouse.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1796 2023-04-18 17:25:36.000000 dataligo-0.7.2/dataligo/datawarehouses/utils.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      544 2023-04-22 06:09:11.000000 dataligo-0.7.2/dataligo/exceptions.py
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 17:35:37.000000 dataligo-0.7.2/dataligo/nosql/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-04-15 19:19:37.000000 dataligo-0.7.2/dataligo/nosql/__init__.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     8175 2023-04-22 12:10:42.000000 dataligo-0.7.2/dataligo/nosql/nosql.py
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      249 2023-04-21 06:38:04.000000 dataligo-0.7.2/dataligo/utils.py
-drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-04-27 17:35:37.000000 dataligo-0.7.2/dataligo.egg-info/
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    19517 2023-04-27 17:35:37.000000 dataligo-0.7.2/dataligo.egg-info/PKG-INFO
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      583 2023-04-27 17:35:37.000000 dataligo-0.7.2/dataligo.egg-info/SOURCES.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        1 2023-04-27 17:35:37.000000 dataligo-0.7.2/dataligo.egg-info/dependency_links.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      358 2023-04-27 17:35:37.000000 dataligo-0.7.2/dataligo.egg-info/requires.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        9 2023-04-27 17:35:37.000000 dataligo-0.7.2/dataligo.egg-info/top_level.txt
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1718 2023-04-27 17:34:24.000000 dataligo-0.7.2/pyproject.toml
--rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       38 2023-04-27 17:35:37.000000 dataligo-0.7.2/setup.cfg
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-05-02 07:52:39.000000 dataligo-0.7.3/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11338 2023-05-02 07:07:17.000000 dataligo-0.7.3/LICENSE
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    19616 2023-05-02 07:52:39.000000 dataligo-0.7.3/PKG-INFO
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     5942 2023-05-02 07:07:17.000000 dataligo-0.7.3/README.md
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-05-02 07:52:39.000000 dataligo-0.7.3/dataligo/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      191 2023-05-02 07:52:12.000000 dataligo-0.7.3/dataligo/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     4068 2023-05-02 07:07:17.000000 dataligo-0.7.3/dataligo/core.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-05-02 07:52:39.000000 dataligo-0.7.3/dataligo/databases/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-05-02 07:07:17.000000 dataligo-0.7.3/dataligo/databases/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    11633 2023-05-02 07:07:17.000000 dataligo-0.7.3/dataligo/databases/database.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-05-02 07:52:39.000000 dataligo-0.7.3/dataligo/datalakes/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-05-02 07:07:17.000000 dataligo-0.7.3/dataligo/datalakes/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    20814 2023-05-02 07:07:17.000000 dataligo-0.7.3/dataligo/datalakes/datalake.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    10320 2023-05-02 07:07:17.000000 dataligo-0.7.3/dataligo/datalakes/utils.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-05-02 07:52:39.000000 dataligo-0.7.3/dataligo/datawarehouses/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-05-02 07:07:17.000000 dataligo-0.7.3/dataligo/datawarehouses/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    12643 2023-05-02 07:07:17.000000 dataligo-0.7.3/dataligo/datawarehouses/datawarehouse.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1796 2023-05-02 07:07:17.000000 dataligo-0.7.3/dataligo/datawarehouses/utils.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      650 2023-05-02 07:27:23.000000 dataligo-0.7.3/dataligo/exceptions.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-05-02 07:52:39.000000 dataligo-0.7.3/dataligo/nosql/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        0 2023-05-02 07:07:17.000000 dataligo-0.7.3/dataligo/nosql/__init__.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     8783 2023-05-02 07:37:25.000000 dataligo-0.7.3/dataligo/nosql/nosql.py
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      249 2023-05-02 07:07:17.000000 dataligo-0.7.3/dataligo/utils.py
+drwxrwxr-x   0 alchemist  (1000) alchemist  (1000)        0 2023-05-02 07:52:39.000000 dataligo-0.7.3/dataligo.egg-info/
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)    19616 2023-05-02 07:52:39.000000 dataligo-0.7.3/dataligo.egg-info/PKG-INFO
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      583 2023-05-02 07:52:39.000000 dataligo-0.7.3/dataligo.egg-info/SOURCES.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        1 2023-05-02 07:52:39.000000 dataligo-0.7.3/dataligo.egg-info/dependency_links.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)      423 2023-05-02 07:52:39.000000 dataligo-0.7.3/dataligo.egg-info/requires.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)        9 2023-05-02 07:52:39.000000 dataligo-0.7.3/dataligo.egg-info/top_level.txt
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)     1705 2023-05-02 07:52:12.000000 dataligo-0.7.3/pyproject.toml
+-rw-rw-r--   0 alchemist  (1000) alchemist  (1000)       38 2023-05-02 07:52:39.000000 dataligo-0.7.3/setup.cfg
```

### Comparing `dataligo-0.7.2/LICENSE` & `dataligo-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dataligo-0.7.2/PKG-INFO` & `dataligo-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataligo
-Version: 0.7.2
+Version: 0.7.3
 Summary: A library to accelerate ML and ETL pipeline by connecting all data sources
 Author-email: Vinish M <vinishuchiha@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,14 +209,18 @@
 Keywords: connectors,datalake reader,datawarehouse reader,dataconnector,nosql connector
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: polars
+Provides-Extra: dynamodb
+Provides-Extra: elasticsearch
+Provides-Extra: mongodb
+Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # DataLigo
```

### Comparing `dataligo-0.7.2/README.md` & `dataligo-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `dataligo-0.7.2/dataligo/core.py` & `dataligo-0.7.3/dataligo/core.py`

 * *Files identical despite different names*

### Comparing `dataligo-0.7.2/dataligo/databases/database.py` & `dataligo-0.7.3/dataligo/databases/database.py`

 * *Files identical despite different names*

### Comparing `dataligo-0.7.2/dataligo/datalakes/datalake.py` & `dataligo-0.7.3/dataligo/datalakes/datalake.py`

 * *Files identical despite different names*

### Comparing `dataligo-0.7.2/dataligo/datalakes/utils.py` & `dataligo-0.7.3/dataligo/datalakes/utils.py`

 * *Files identical despite different names*

### Comparing `dataligo-0.7.2/dataligo/datawarehouses/datawarehouse.py` & `dataligo-0.7.3/dataligo/datawarehouses/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `dataligo-0.7.2/dataligo/datawarehouses/utils.py` & `dataligo-0.7.3/dataligo/datawarehouses/utils.py`

 * *Files identical despite different names*

### Comparing `dataligo-0.7.2/dataligo/exceptions.py` & `dataligo-0.7.3/dataligo/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,8 +12,12 @@
 
 class UnSupportedDataSourceException(Exception):
     def __init__(self,message):
         self.message = message
 
 class UnSupportedDataFrameException(Exception):
     def __init__(self,message):
+        self.message = message
+
+class ModuleNotFoundException(Exception):
+    def __init__(self,message):
         self.message = message
```

### Comparing `dataligo-0.7.2/dataligo/nosql/nosql.py` & `dataligo-0.7.3/dataligo/nosql/nosql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from elasticsearch import Elasticsearch
-from pymongo import MongoClient
 import pandas as pd
-from elasticsearch.helpers import bulk
-from dynamo_pandas.transactions import put_items, get_all_items, get_items
 from typing import List, Dict
 from sqlalchemy import create_engine
 from ..utils import which_dataframe
-from ..exceptions import UnSupportedDataFrameException
+from ..exceptions import UnSupportedDataFrameException, ModuleNotFoundException
 
 class ElasticSearch():
     def __init__(self,config):
         """
         ElasticSearch class create the ligo elasticsearch object, through which you can able to read, write, download data from ElasticSearch.
 
         Args:
             config (dict): Automatically loaded from the config file (yaml)
         """
-        if 'USERNAME' in config and 'PASSWORD' in config:
-            if config['USERNAME'] and config['PASSWORD']:
-                self._es = Elasticsearch([config['HOST']],basic_auth=(config['USERNAME'],config['PASSWORD']))
-        elif 'API_KEY' in config:
-            if config['API_KEY']:
-                self._es = Elasticsearch([config['HOST']],api_key=config['API_KEY'])
-        else:
-            self._es = Elasticsearch([config['HOST']])
+        try:
+            from elasticsearch import Elasticsearch
+            if 'USERNAME' in config and 'PASSWORD' in config:
+                if config['USERNAME'] and config['PASSWORD']:
+                    self._es = Elasticsearch([config['HOST']],basic_auth=(config['USERNAME'],config['PASSWORD']))
+            elif 'API_KEY' in config:
+                if config['API_KEY']:
+                    self._es = Elasticsearch([config['HOST']],api_key=config['API_KEY'])
+            else:
+                self._es = Elasticsearch([config['HOST']])
+        except ImportError:
+            raise ModuleNotFoundException('elasticsearch not found. try `pip install elasticsearch`')
     
     def read_as_dataframe(self,query: str,index: str,return_type='pandas'):
         """
         Takes query and index as arguments and return the dataframe
 
         Args:
             query (str): es query
@@ -51,14 +51,15 @@
     def write_dataframe(self, df, index: str):
         """
         Takes DataFrame, index name as arguments and write the dataframe to ElasticSearch.
         Args:
             df (DataFrame): Dataframe which need to be inserted to es
             index (str): index name
         """
+        from elasticsearch.helpers import bulk
         if which_dataframe(df)=='pandas':
             records = df.to_dict('records')
         elif which_dataframe(df)=='polars':
             records = df.to_dicts()
         else:
             raise UnSupportedDataFrameException(f"Unsupported Dataframe: {which_dataframe(df)}")
         actions = [
@@ -77,15 +78,19 @@
     def __init__(self, config) -> None:
         """
         MongoDB class create the ligo mongodb object, through which you can able to read, write, download data from MongoDB.
 
         Args:
             config (dict): Automatically loaded from the config file (yaml)
         """
-        self._mdb = MongoClient(config['CONN_STRING'])
+        try:
+            from pymongo import MongoClient
+            self._mdb = MongoClient(config['CONN_STRING'])
+        except ImportError:
+            raise ModuleNotFoundException('pymongo not found. try `pip install pymongo`')
 
     def read_as_dataframe(self,database: str,collection: str,filter_query: dict=None,return_type='pandas'):
         """
         Takes database, collections as arguments and return the dataframe
 
         Args:
             database (str): database name
@@ -129,16 +134,20 @@
     def __init__(self, config) -> None:
         """
         DynamoDB class create the ligo dynamodb object, through which you can able to read, write, download data from DynamoDB.
 
         Args:
             config (dict): Automatically loaded from the config file (yaml)
         """
-        self._ddb = {'aws_access_key_id':config['AWS_ACCESS_KEY_ID'],
-                     'aws_secret_access_key':config['AWS_SECRET_ACCESS_KEY']}
+        try:
+            import dynamo_pandas
+            self._ddb = {'aws_access_key_id':config['AWS_ACCESS_KEY_ID'],
+                            'aws_secret_access_key':config['AWS_SECRET_ACCESS_KEY']}
+        except ImportError:
+            raise ModuleNotFoundException('dynamo_pandas not found. try `pip install dynamo-pandas`')
 
     def read_as_dataframe(self, table: str, keys=None, attributes=None, dtype=None,return_type='pandas'):
         """
         Takes table name, keys as arguments and return the dataframe
 
         Args:
             table (str): table name
@@ -146,14 +155,15 @@
             attributes (list, optional): fields want to pull from dynamodb. Defaults to None.
             dtype (dict, optional): parse the return field data type. Defaults to None.
             return_type (str, optional): which dataframe you want to return (pandas, polars, dask etc). Defaults to 'pandas'.
 
         Returns:
             DataFrame: Depends on the return_type parameter.
         """
+        from dynamo_pandas.transactions import get_all_items, get_items
         if keys is not None:
             items = get_items(
                 keys=keys, table=table, attributes=attributes, boto3_kwargs=self._ddb
             )
         else:
             items = get_all_items(
                 table=table, attributes=attributes, boto3_kwargs=self._ddb
@@ -174,14 +184,15 @@
         """
         Takes DataFrame, table name as arguments and write the dataframe to DynamoDB.
 
         Args:
             df (DataFrame): Dataframe which need to be inserted to dynamodb
             table (str): table name
         """
+        from dynamo_pandas.transactions import put_items
         if which_dataframe(df)=='pandas':
             records = df.to_dict('records')
         elif which_dataframe(df)=='polars':
             records = df.to_dicts()
         else:
             raise UnSupportedDataFrameException(f"Unsupported Dataframe: {which_dataframe(df)}")
         put_items(items=records, table=table, boto3_kwargs=self._ddb)
```

### Comparing `dataligo-0.7.2/dataligo.egg-info/PKG-INFO` & `dataligo-0.7.3/dataligo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataligo
-Version: 0.7.2
+Version: 0.7.3
 Summary: A library to accelerate ML and ETL pipeline by connecting all data sources
 Author-email: Vinish M <vinishuchiha@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,14 +209,18 @@
 Keywords: connectors,datalake reader,datawarehouse reader,dataconnector,nosql connector
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: polars
+Provides-Extra: dynamodb
+Provides-Extra: elasticsearch
+Provides-Extra: mongodb
+Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # DataLigo
```

### Comparing `dataligo-0.7.2/dataligo.egg-info/SOURCES.txt` & `dataligo-0.7.3/dataligo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataligo-0.7.2/pyproject.toml` & `dataligo-0.7.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataligo"
-version = "0.7.2"
+version = "0.7.3"
 description = "A library to accelerate ML and ETL pipeline by connecting all data sources"
 readme = "README.md"
 authors = [{ name = "Vinish M", email = "vinishuchiha@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -20,38 +20,32 @@
     "google-cloud-storage >= 2.7.0",
     "azure-storage-blob >= 12.15.0",
     "pandas >= 1.0.0",
     "PyYAML",
     "connectorx",
     "snowflake-connector-python[pandas]==3.0.2",
     "mysql-connector-python-rf",
-    "elasticsearch > 8.0.0",
     "sqlalchemy==1.4.46",
-    "pymongo",
-    "dynamo_pandas",
-    "fastparquet",
-    "openpyxl",
-    "xlrd",
-    "xlwt",
     'tomli; python_version < "3.11"',
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 polars = ["polars"]
+dynamodb = ["dynamo-pandas"]
+elasticsearch = ["elasticsearch > 8.0.0"]
+mongodb = ["pymongo"]
+all = ["polars","elasticsearch > 8.0.0","pymongo","dynamo-pandas"]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/VinishUchiha/dataligo"
 
-# [tool.setuptools]
-# py-modules = ["dataligo"]
-
 [tool.bumpver]
-current_version = "0.7.2"
+current_version = "0.7.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

