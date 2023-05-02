# Comparing `tmp/stream-connect-1.0.7.tar.gz` & `tmp/stream-connect-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stream-connect-1.0.7.tar", last modified: Fri Aug  7 08:11:35 2020, max compression
+gzip compressed data, was "dist/stream-connect-1.0.8.tar", last modified: Tue Aug 18 08:04:20 2020, max compression
```

## Comparing `stream-connect-1.0.7.tar` & `stream-connect-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 devendraratnam   (502) staff       (20)        0 2020-08-07 08:11:35.000000 stream-connect-1.0.7/
--rw-r--r--   0 devendraratnam   (502) staff       (20)      908 2020-08-07 08:11:35.000000 stream-connect-1.0.7/PKG-INFO
-drwxr-xr-x   0 devendraratnam   (502) staff       (20)        0 2020-08-07 08:11:35.000000 stream-connect-1.0.7/stream_connect/
--rw-r--r--   0 devendraratnam   (502) staff       (20)        0 2020-03-13 11:01:36.000000 stream-connect-1.0.7/stream_connect/__init__.py
--rw-r--r--   0 devendraratnam   (502) staff       (20)      731 2020-03-13 11:01:36.000000 stream-connect-1.0.7/stream_connect/test.py
--rw-r--r--   0 devendraratnam   (502) staff       (20)      387 2020-03-13 11:01:36.000000 stream-connect-1.0.7/stream_connect/commons.py
--rw-r--r--   0 devendraratnam   (502) staff       (20)     1156 2020-03-13 13:16:28.000000 stream-connect-1.0.7/stream_connect/connector.py
--rw-r--r--   0 devendraratnam   (502) staff       (20)      143 2020-03-13 11:01:36.000000 stream-connect-1.0.7/stream_connect/errors.py
-drwxr-xr-x   0 devendraratnam   (502) staff       (20)        0 2020-08-07 08:11:35.000000 stream-connect-1.0.7/stream_connect/services/
--rw-r--r--   0 devendraratnam   (502) staff       (20)        0 2020-03-13 11:01:36.000000 stream-connect-1.0.7/stream_connect/services/___init__.py
--rw-r--r--   0 devendraratnam   (502) staff       (20)      128 2020-03-13 11:01:36.000000 stream-connect-1.0.7/stream_connect/services/response.py
--rw-r--r--   0 devendraratnam   (502) staff       (20)     1712 2020-08-07 08:10:47.000000 stream-connect-1.0.7/stream_connect/services/kafka.py
--rw-r--r--   0 devendraratnam   (502) staff       (20)      496 2020-03-13 11:01:36.000000 stream-connect-1.0.7/stream_connect/services/base.py
--rw-r--r--   0 devendraratnam   (502) staff       (20)      230 2020-03-13 11:01:36.000000 stream-connect-1.0.7/README.md
--rw-r--r--   0 devendraratnam   (502) staff       (20)     1104 2020-08-07 08:11:06.000000 stream-connect-1.0.7/setup.py
--rw-r--r--   0 devendraratnam   (502) staff       (20)       79 2020-08-07 08:11:35.000000 stream-connect-1.0.7/setup.cfg
-drwxr-xr-x   0 devendraratnam   (502) staff       (20)        0 2020-08-07 08:11:35.000000 stream-connect-1.0.7/stream_connect.egg-info/
--rw-r--r--   0 devendraratnam   (502) staff       (20)      908 2020-08-07 08:11:35.000000 stream-connect-1.0.7/stream_connect.egg-info/PKG-INFO
--rw-r--r--   0 devendraratnam   (502) staff       (20)      484 2020-08-07 08:11:35.000000 stream-connect-1.0.7/stream_connect.egg-info/SOURCES.txt
--rw-r--r--   0 devendraratnam   (502) staff       (20)       24 2020-08-07 08:11:35.000000 stream-connect-1.0.7/stream_connect.egg-info/requires.txt
--rw-r--r--   0 devendraratnam   (502) staff       (20)       15 2020-08-07 08:11:35.000000 stream-connect-1.0.7/stream_connect.egg-info/top_level.txt
--rw-r--r--   0 devendraratnam   (502) staff       (20)        1 2020-08-07 08:11:35.000000 stream-connect-1.0.7/stream_connect.egg-info/dependency_links.txt
+drwxr-xr-x   0 devendraratnam   (502) staff       (20)        0 2020-08-18 08:04:20.000000 stream-connect-1.0.8/
+-rw-r--r--   0 devendraratnam   (502) staff       (20)      908 2020-08-18 08:04:20.000000 stream-connect-1.0.8/PKG-INFO
+drwxr-xr-x   0 devendraratnam   (502) staff       (20)        0 2020-08-18 08:04:20.000000 stream-connect-1.0.8/stream_connect/
+-rw-r--r--   0 devendraratnam   (502) staff       (20)        0 2020-03-13 11:01:36.000000 stream-connect-1.0.8/stream_connect/__init__.py
+-rw-r--r--   0 devendraratnam   (502) staff       (20)      731 2020-03-13 11:01:36.000000 stream-connect-1.0.8/stream_connect/test.py
+-rw-r--r--   0 devendraratnam   (502) staff       (20)      387 2020-03-13 11:01:36.000000 stream-connect-1.0.8/stream_connect/commons.py
+-rw-r--r--   0 devendraratnam   (502) staff       (20)     1173 2020-08-18 07:59:57.000000 stream-connect-1.0.8/stream_connect/connector.py
+-rw-r--r--   0 devendraratnam   (502) staff       (20)      143 2020-03-13 11:01:36.000000 stream-connect-1.0.8/stream_connect/errors.py
+drwxr-xr-x   0 devendraratnam   (502) staff       (20)        0 2020-08-18 08:04:20.000000 stream-connect-1.0.8/stream_connect/services/
+-rw-r--r--   0 devendraratnam   (502) staff       (20)        0 2020-03-13 11:01:36.000000 stream-connect-1.0.8/stream_connect/services/___init__.py
+-rw-r--r--   0 devendraratnam   (502) staff       (20)      128 2020-03-13 11:01:36.000000 stream-connect-1.0.8/stream_connect/services/response.py
+-rw-r--r--   0 devendraratnam   (502) staff       (20)     1712 2020-08-18 07:49:07.000000 stream-connect-1.0.8/stream_connect/services/kafka.py
+-rw-r--r--   0 devendraratnam   (502) staff       (20)      496 2020-03-13 11:01:36.000000 stream-connect-1.0.8/stream_connect/services/base.py
+-rw-r--r--   0 devendraratnam   (502) staff       (20)      230 2020-03-13 11:01:36.000000 stream-connect-1.0.8/README.md
+-rw-r--r--   0 devendraratnam   (502) staff       (20)     1104 2020-08-18 08:00:35.000000 stream-connect-1.0.8/setup.py
+-rw-r--r--   0 devendraratnam   (502) staff       (20)       79 2020-08-18 08:04:20.000000 stream-connect-1.0.8/setup.cfg
+drwxr-xr-x   0 devendraratnam   (502) staff       (20)        0 2020-08-18 08:04:20.000000 stream-connect-1.0.8/stream_connect.egg-info/
+-rw-r--r--   0 devendraratnam   (502) staff       (20)      908 2020-08-18 08:04:19.000000 stream-connect-1.0.8/stream_connect.egg-info/PKG-INFO
+-rw-r--r--   0 devendraratnam   (502) staff       (20)      484 2020-08-18 08:04:19.000000 stream-connect-1.0.8/stream_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 devendraratnam   (502) staff       (20)       24 2020-08-18 08:04:19.000000 stream-connect-1.0.8/stream_connect.egg-info/requires.txt
+-rw-r--r--   0 devendraratnam   (502) staff       (20)       15 2020-08-18 08:04:19.000000 stream-connect-1.0.8/stream_connect.egg-info/top_level.txt
+-rw-r--r--   0 devendraratnam   (502) staff       (20)        1 2020-08-18 08:04:19.000000 stream-connect-1.0.8/stream_connect.egg-info/dependency_links.txt
```

### Comparing `stream-connect-1.0.7/PKG-INFO` & `stream-connect-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: stream-connect
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python library to connect streaming service
 Home-page: https://github.com/devratnam/stream-connect-py
 Author: Devendra Ratnam
 Author-email: ratnam747@gmail.com
 License: UNKNOWN
 Description: # stream-connect-py
```

### Comparing `stream-connect-1.0.7/stream_connect/test.py` & `stream-connect-1.0.8/stream_connect/test.py`

 * *Files identical despite different names*

### Comparing `stream-connect-1.0.7/stream_connect/connector.py` & `stream-connect-1.0.8/stream_connect/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class StreamPublisher(object):
     """
     generic class to publish messages into stream service
     """
 
-    def __init__(self, service, host, topic, configurations={}):
+    def __init__(self, service, host, topic, configurations={}, *args, **kwargs):
         self.service = service
         self.host = host
         self.topic = topic
         self.configurations = configurations
 
     def publish(self, data, *args, **kwargs):
         executable_service = ServiceMap.get_stream_service(
```

### Comparing `stream-connect-1.0.7/stream_connect/services/kafka.py` & `stream-connect-1.0.8/stream_connect/services/kafka.py`

 * *Files identical despite different names*

### Comparing `stream-connect-1.0.7/setup.py` & `stream-connect-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 import sys
 from os.path import join, dirname
 from setuptools import setup, find_packages
 
-VERSION = (1, 0, 7)
+VERSION = (1, 0, 8)
 __version__ = VERSION
 __versionstr__ = '.'.join(map(str, VERSION))
 
 f = open(join(dirname(__file__), 'README.md'))
 long_description = f.read().strip()
 f.close()
```

### Comparing `stream-connect-1.0.7/stream_connect.egg-info/PKG-INFO` & `stream-connect-1.0.8/stream_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: stream-connect
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python library to connect streaming service
 Home-page: https://github.com/devratnam/stream-connect-py
 Author: Devendra Ratnam
 Author-email: ratnam747@gmail.com
 License: UNKNOWN
 Description: # stream-connect-py
```

