# Comparing `tmp/google_cloud_utilities-0.0.3.tar.gz` & `tmp/google_cloud_utilities-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_cloud_utilities-0.0.3.tar", last modified: Tue Feb 21 19:34:20 2023, max compression
+gzip compressed data, was "google_cloud_utilities-0.0.4.tar", last modified: Tue May  2 18:39:13 2023, max compression
```

## Comparing `google_cloud_utilities-0.0.3.tar` & `google_cloud_utilities-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 johnfoley   (501) staff       (20)        0 2023-02-21 19:34:20.711246 google_cloud_utilities-0.0.3/
--rw-r--r--   0 johnfoley   (501) staff       (20)     1067 2023-02-21 18:52:42.000000 google_cloud_utilities-0.0.3/LICENSE
--rw-r--r--   0 johnfoley   (501) staff       (20)      848 2023-02-21 19:34:20.710819 google_cloud_utilities-0.0.3/PKG-INFO
--rw-r--r--   0 johnfoley   (501) staff       (20)      128 2023-02-21 19:26:51.000000 google_cloud_utilities-0.0.3/README.md
-drwxr-xr-x   0 johnfoley   (501) staff       (20)        0 2023-02-21 19:34:20.707824 google_cloud_utilities-0.0.3/google_cloud_utilities/
--rw-r--r--   0 johnfoley   (501) staff       (20)       41 2023-02-21 19:33:51.000000 google_cloud_utilities-0.0.3/google_cloud_utilities/__init__.py
--rw-r--r--   0 johnfoley   (501) staff       (20)    10509 2023-02-21 18:19:41.000000 google_cloud_utilities-0.0.3/google_cloud_utilities/gcp.py
-drwxr-xr-x   0 johnfoley   (501) staff       (20)        0 2023-02-21 19:34:20.710135 google_cloud_utilities-0.0.3/google_cloud_utilities.egg-info/
--rw-r--r--   0 johnfoley   (501) staff       (20)      848 2023-02-21 19:34:20.000000 google_cloud_utilities-0.0.3/google_cloud_utilities.egg-info/PKG-INFO
--rw-r--r--   0 johnfoley   (501) staff       (20)      320 2023-02-21 19:34:20.000000 google_cloud_utilities-0.0.3/google_cloud_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 johnfoley   (501) staff       (20)        1 2023-02-21 19:34:20.000000 google_cloud_utilities-0.0.3/google_cloud_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 johnfoley   (501) staff       (20)       78 2023-02-21 19:34:20.000000 google_cloud_utilities-0.0.3/google_cloud_utilities.egg-info/requires.txt
--rw-r--r--   0 johnfoley   (501) staff       (20)       23 2023-02-21 19:34:20.000000 google_cloud_utilities-0.0.3/google_cloud_utilities.egg-info/top_level.txt
--rw-r--r--   0 johnfoley   (501) staff       (20)       38 2023-02-21 19:34:20.711430 google_cloud_utilities-0.0.3/setup.cfg
--rw-r--r--   0 johnfoley   (501) staff       (20)     3415 2023-02-21 19:34:15.000000 google_cloud_utilities-0.0.3/setup.py
+drwxr-xr-x   0 johnfoley   (501) staff       (20)        0 2023-05-02 18:39:13.413454 google_cloud_utilities-0.0.4/
+-rw-r--r--   0 johnfoley   (501) staff       (20)     1067 2023-02-21 18:52:42.000000 google_cloud_utilities-0.0.4/LICENSE
+-rw-r--r--   0 johnfoley   (501) staff       (20)      848 2023-05-02 18:39:13.413158 google_cloud_utilities-0.0.4/PKG-INFO
+-rw-r--r--   0 johnfoley   (501) staff       (20)      128 2023-02-21 19:26:51.000000 google_cloud_utilities-0.0.4/README.md
+drwxr-xr-x   0 johnfoley   (501) staff       (20)        0 2023-05-02 18:39:13.410158 google_cloud_utilities-0.0.4/google_cloud_utilities/
+-rw-r--r--   0 johnfoley   (501) staff       (20)       41 2023-02-21 19:33:51.000000 google_cloud_utilities-0.0.4/google_cloud_utilities/__init__.py
+-rw-r--r--   0 johnfoley   (501) staff       (20)    10572 2023-05-02 18:37:41.000000 google_cloud_utilities-0.0.4/google_cloud_utilities/gcp.py
+drwxr-xr-x   0 johnfoley   (501) staff       (20)        0 2023-05-02 18:39:13.412726 google_cloud_utilities-0.0.4/google_cloud_utilities.egg-info/
+-rw-r--r--   0 johnfoley   (501) staff       (20)      848 2023-05-02 18:39:13.000000 google_cloud_utilities-0.0.4/google_cloud_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 johnfoley   (501) staff       (20)      320 2023-05-02 18:39:13.000000 google_cloud_utilities-0.0.4/google_cloud_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 johnfoley   (501) staff       (20)        1 2023-05-02 18:39:13.000000 google_cloud_utilities-0.0.4/google_cloud_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 johnfoley   (501) staff       (20)       78 2023-05-02 18:39:13.000000 google_cloud_utilities-0.0.4/google_cloud_utilities.egg-info/requires.txt
+-rw-r--r--   0 johnfoley   (501) staff       (20)       23 2023-05-02 18:39:13.000000 google_cloud_utilities-0.0.4/google_cloud_utilities.egg-info/top_level.txt
+-rw-r--r--   0 johnfoley   (501) staff       (20)       38 2023-05-02 18:39:13.413568 google_cloud_utilities-0.0.4/setup.cfg
+-rw-r--r--   0 johnfoley   (501) staff       (20)     3415 2023-05-02 18:38:20.000000 google_cloud_utilities-0.0.4/setup.py
```

### Comparing `google_cloud_utilities-0.0.3/LICENSE` & `google_cloud_utilities-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `google_cloud_utilities-0.0.3/PKG-INFO` & `google_cloud_utilities-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google_cloud_utilities
-Version: 0.0.3
+Version: 0.0.4
 Summary: A few handy Python functions for interacting with Google Cloud Platform
 Home-page: https://github.com/johnf1004/google_cloud_utilities
 Author: John Foley
 Author-email: johnf1004@yahoo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `google_cloud_utilities-0.0.3/google_cloud_utilities/gcp.py` & `google_cloud_utilities-0.0.4/google_cloud_utilities/gcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,24 +190,25 @@
     logger.info(
         "Loaded {} rows and {} columns to {}".format(
             table.num_rows, len(table.schema), table_id
         )
     )
 
 
-def generate_feature_bq(sql, table_id, bq_client):
+def generate_feature_bq(sql, table_id, bq_client, labels={}):
     """
     :param sql: Bigquery command to execute
     :param table_id: Name of table to be created; projectname.datasetname.table
     :param bq_client: Bigquery client object
+    :param labels: Additional labels
     :return:
     """
 
     # If table does not already exist, set it up with partitioning
-    job_config = bigquery.QueryJobConfig(destination=table_id, write_disposition='WRITE_APPEND')
+    job_config = bigquery.QueryJobConfig(destination=table_id, write_disposition='WRITE_APPEND', labels=labels)
     try:
         bq_client.get_table(table_id)
     except NotFound:
         job_config.time_partitioning = bigquery.TimePartitioning(
             type_=bigquery.TimePartitioningType.DAY,
             field="event_timestamp")
```

### Comparing `google_cloud_utilities-0.0.3/google_cloud_utilities.egg-info/PKG-INFO` & `google_cloud_utilities-0.0.4/google_cloud_utilities.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-utilities
-Version: 0.0.3
+Version: 0.0.4
 Summary: A few handy Python functions for interacting with Google Cloud Platform
 Home-page: https://github.com/johnf1004/google_cloud_utilities
 Author: John Foley
 Author-email: johnf1004@yahoo.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `google_cloud_utilities-0.0.3/setup.py` & `google_cloud_utilities-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'google_cloud_utilities'
 DESCRIPTION = 'A few handy Python functions for interacting with Google Cloud Platform'
 URL = 'https://github.com/johnf1004/google_cloud_utilities'
 EMAIL = 'johnf1004@yahoo.co.uk'
 AUTHOR = 'John Foley'
 REQUIRES_PYTHON = '>=3.9.7'
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'google-cloud-bigquery==3.4.2', 'google-cloud-secret-manager==2.4.0', 'pandas>=1.5.3',
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
```

