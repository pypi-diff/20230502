# Comparing `tmp/longalpha_utils-0.42.tar.gz` & `tmp/longalpha_utils-0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.42.tar", last modified: Sun Apr 30 16:06:39 2023, max compression
+gzip compressed data, was "longalpha_utils-0.43.tar", last modified: Tue May  2 00:58:42 2023, max compression
```

## Comparing `longalpha_utils-0.42.tar` & `longalpha_utils-0.43.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:06:39.361355 longalpha_utils-0.42/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-30 16:06:39.361355 longalpha_utils-0.42/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:06:39.357355 longalpha_utils-0.42/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-30 16:06:25.000000 longalpha_utils-0.42/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-30 16:06:25.000000 longalpha_utils-0.42/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-30 16:06:25.000000 longalpha_utils-0.42/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-04-30 16:06:25.000000 longalpha_utils-0.42/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-30 16:06:25.000000 longalpha_utils-0.42/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-30 16:06:25.000000 longalpha_utils-0.42/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:06:39.361355 longalpha_utils-0.42/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-30 16:06:39.000000 longalpha_utils-0.42/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-30 16:06:39.000000 longalpha_utils-0.42/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 16:06:39.000000 longalpha_utils-0.42/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-30 16:06:39.000000 longalpha_utils-0.42/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 16:06:39.000000 longalpha_utils-0.42/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 16:06:39.361355 longalpha_utils-0.42/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-30 16:06:25.000000 longalpha_utils-0.42/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:42.043999 longalpha_utils-0.43/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 00:58:42.043999 longalpha_utils-0.43/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:42.039999 longalpha_utils-0.43/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 00:58:30.000000 longalpha_utils-0.43/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 00:58:30.000000 longalpha_utils-0.43/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-02 00:58:30.000000 longalpha_utils-0.43/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-05-02 00:58:30.000000 longalpha_utils-0.43/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-02 00:58:30.000000 longalpha_utils-0.43/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-02 00:58:30.000000 longalpha_utils-0.43/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:58:42.043999 longalpha_utils-0.43/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 00:58:42.000000 longalpha_utils-0.43/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-02 00:58:42.000000 longalpha_utils-0.43/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:58:42.000000 longalpha_utils-0.43/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-02 00:58:42.000000 longalpha_utils-0.43/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 00:58:42.000000 longalpha_utils-0.43/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 00:58:42.043999 longalpha_utils-0.43/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-02 00:58:30.000000 longalpha_utils-0.43/setup.py
```

### Comparing `longalpha_utils-0.42/longalpha_utils/messenger.py` & `longalpha_utils-0.43/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.42/longalpha_utils/transfers.py` & `longalpha_utils-0.43/longalpha_utils/transfers.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,30 +6,46 @@
 from minio import Minio
 from pyspark.conf import SparkConf
 from pyspark.sql import SparkSession, DataFrame
 from sqlalchemy import Engine
 from sqlalchemy import create_engine
 from sqlalchemy import text
 
-
+from minio.error import S3Error
 class MinioWrapper:
     def __init__(self, minio_url, minio_access_key, minio_secret_key):
         self.minio_client = Minio(
             endpoint=minio_url,
             access_key=minio_access_key,
             secret_key=minio_secret_key,
             secure=False,
         )
 
+    def object_exists(self, bucket_name: str, object_name: str) -> bool:
+        """
+        check if an object exists in the bucket
+        Args:
+            bucket_name: Minio bucket_name
+            object_name: object name in the minio bucket
+
+        Returns: True if the object exists, False otherwise
+
+        """
+        try:
+            self.minio_client.stat_object(bucket_name, object_name)
+            return True
+        except S3Error as e:
+            if e.code == "NoSuchKey":
+                return False
     def fput(
         self,
         file_path,
         bucket_name: str,
         object_name: str,
-    ):
+    )-> None:
         """
         put a file to s3
         Args:
             file_path: path to the file
             bucket_name: Minio bucket_name
             object_name: object name in the minio bucket
```

### Comparing `longalpha_utils-0.42/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.43/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.42/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.43/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.42/setup.py` & `longalpha_utils-0.43/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.42",
+    version="0.43",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

