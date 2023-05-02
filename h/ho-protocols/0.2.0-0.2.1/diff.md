# Comparing `tmp/ho-protocols-0.2.0.tar.gz` & `tmp/ho-protocols-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ho-protocols-0.2.0.tar", last modified: Tue Apr 25 09:45:05 2023, max compression
+gzip compressed data, was "ho-protocols-0.2.1.tar", last modified: Tue May  2 12:05:25 2023, max compression
```

## Comparing `ho-protocols-0.2.0.tar` & `ho-protocols-0.2.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 09:45:05.929158 ho-protocols-0.2.0/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1072 2021-12-17 10:20:38.000000 ho-protocols-0.2.0/LICENCE
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-04-25 09:45:05.925158 ho-protocols-0.2.0/PKG-INFO
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      959 2022-01-14 07:08:59.000000 ho-protocols-0.2.0/README.md
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       38 2023-04-25 09:45:05.929158 ho-protocols-0.2.0/setup.cfg
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1084 2023-04-25 09:43:50.000000 ho-protocols-0.2.0/setup.py
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 09:45:05.917158 ho-protocols-0.2.0/src/
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 09:45:05.921158 ho-protocols-0.2.0/src/ho_protocols/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-17 08:26:26.000000 ho-protocols-0.2.0/src/ho_protocols/__init__.py
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 09:45:05.921158 ho-protocols-0.2.0/src/ho_protocols/alert/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2022-01-12 08:33:24.000000 ho-protocols-0.2.0/src/ho_protocols/alert/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1662 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/alert/alert_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1687 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/alert/alert_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1538 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/alert/bees_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2159 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/alert/bees_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2171 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/alert/system_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3868 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/alert/system_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 09:45:05.925158 ho-protocols-0.2.0/src/ho_protocols/cmd/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-22 12:31:53.000000 ho-protocols-0.2.0/src/ho_protocols/cmd/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3279 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/cmd/cmd_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6358 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/cmd/cmd_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1509 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/common_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1826 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/common_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5246 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/data_in_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    15289 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/data_in_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1563 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/example_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2146 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/example_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 09:45:05.925158 ho-protocols-0.2.0/src/ho_protocols/live/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-16 11:50:20.000000 ho-protocols-0.2.0/src/ho_protocols/live/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3207 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/live/actuators_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6961 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/live/actuators_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2402 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/live/live_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2906 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/live/live_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2573 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/live/models_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5335 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/live/models_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2575 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/live/sensors_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5829 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/live/sensors_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1275 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/live/system_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1273 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/live/system_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 09:45:05.925158 ho-protocols-0.2.0/src/ho_protocols/map/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 09:09:45.000000 ho-protocols-0.2.0/src/ho_protocols/map/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3526 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/map/map_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     8143 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/map/map_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 09:45:05.925158 ho-protocols-0.2.0/src/ho_protocols/query/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-28 10:24:29.000000 ho-protocols-0.2.0/src/ho_protocols/query/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5090 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/query/query_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    13000 2023-04-25 05:45:18.000000 ho-protocols-0.2.0/src/ho_protocols/query/query_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 09:45:05.921158 ho-protocols-0.2.0/src/ho_protocols.egg-info/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-04-25 09:45:05.000000 ho-protocols-0.2.0/src/ho_protocols.egg-info/PKG-INFO
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1421 2023-04-25 09:45:05.000000 ho-protocols-0.2.0/src/ho_protocols.egg-info/SOURCES.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        1 2023-04-25 09:45:05.000000 ho-protocols-0.2.0/src/ho_protocols.egg-info/dependency_links.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       17 2023-04-25 09:45:05.000000 ho-protocols-0.2.0/src/ho_protocols.egg-info/requires.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       13 2023-04-25 09:45:05.000000 ho-protocols-0.2.0/src/ho_protocols.egg-info/top_level.txt
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-04-25 09:45:05.925158 ho-protocols-0.2.0/test/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      625 2021-12-17 12:38:28.000000 ho-protocols-0.2.0/test/test.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.597644 ho-protocols-0.2.1/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1072 2021-12-17 10:20:38.000000 ho-protocols-0.2.1/LICENCE
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-05-02 12:05:25.597644 ho-protocols-0.2.1/PKG-INFO
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      959 2022-01-14 07:08:59.000000 ho-protocols-0.2.1/README.md
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       38 2023-05-02 12:05:25.597644 ho-protocols-0.2.1/setup.cfg
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1084 2023-04-25 09:43:50.000000 ho-protocols-0.2.1/setup.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.581644 ho-protocols-0.2.1/src/
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.593644 ho-protocols-0.2.1/src/ho_protocols/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-17 08:26:26.000000 ho-protocols-0.2.1/src/ho_protocols/__init__.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.593644 ho-protocols-0.2.1/src/ho_protocols/alert/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2022-01-12 08:33:24.000000 ho-protocols-0.2.1/src/ho_protocols/alert/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1662 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/alert/alert_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1687 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/alert/alert_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1538 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/alert/bees_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2159 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/alert/bees_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2171 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/alert/system_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3868 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/alert/system_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.593644 ho-protocols-0.2.1/src/ho_protocols/cmd/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-22 12:31:53.000000 ho-protocols-0.2.1/src/ho_protocols/cmd/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3279 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/cmd/cmd_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6358 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/cmd/cmd_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1509 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/common_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1826 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/common_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5246 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/data_in_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    15289 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/data_in_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1563 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/example_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2146 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/example_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.597644 ho-protocols-0.2.1/src/ho_protocols/live/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-16 11:50:20.000000 ho-protocols-0.2.1/src/ho_protocols/live/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3207 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/actuators_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6961 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/actuators_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2402 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/live_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2906 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/live_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2573 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/models_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5335 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/models_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2575 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/sensors_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5829 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/sensors_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1275 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/system_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1273 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/system_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.597644 ho-protocols-0.2.1/src/ho_protocols/map/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 09:09:45.000000 ho-protocols-0.2.1/src/ho_protocols/map/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     4556 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/map/map_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    10813 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/map/map_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.597644 ho-protocols-0.2.1/src/ho_protocols/query/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-28 10:24:29.000000 ho-protocols-0.2.1/src/ho_protocols/query/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5090 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/query/query_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    13000 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/query/query_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.593644 ho-protocols-0.2.1/src/ho_protocols.egg-info/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-05-02 12:05:25.000000 ho-protocols-0.2.1/src/ho_protocols.egg-info/PKG-INFO
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1421 2023-05-02 12:05:25.000000 ho-protocols-0.2.1/src/ho_protocols.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        1 2023-05-02 12:05:25.000000 ho-protocols-0.2.1/src/ho_protocols.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       17 2023-05-02 12:05:25.000000 ho-protocols-0.2.1/src/ho_protocols.egg-info/requires.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       13 2023-05-02 12:05:25.000000 ho-protocols-0.2.1/src/ho_protocols.egg-info/top_level.txt
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.597644 ho-protocols-0.2.1/test/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      625 2021-12-17 12:38:28.000000 ho-protocols-0.2.1/test/test.py
```

### Comparing `ho-protocols-0.2.0/LICENCE` & `ho-protocols-0.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/PKG-INFO` & `ho-protocols-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ho-protocols
-Version: 0.2.0
+Version: 0.2.1
 Summary: ProtoBuf definitions for HO components
 Home-page: https://github.com/hiveopolis/ho-protocols
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ho-protocols-0.2.0/README.md` & `ho-protocols-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/setup.py` & `ho-protocols-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/alert/alert_pb2.py` & `ho-protocols-0.2.1/src/ho_protocols/alert/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/alert/alert_pb2.pyi` & `ho-protocols-0.2.1/src/ho_protocols/alert/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/alert/bees_pb2.py` & `ho-protocols-0.2.1/src/ho_protocols/alert/bees_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/alert/bees_pb2.pyi` & `ho-protocols-0.2.1/src/ho_protocols/alert/bees_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/alert/system_pb2.py` & `ho-protocols-0.2.1/src/ho_protocols/alert/system_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/alert/system_pb2.pyi` & `ho-protocols-0.2.1/src/ho_protocols/alert/system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/cmd/cmd_pb2.py` & `ho-protocols-0.2.1/src/ho_protocols/cmd/cmd_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/cmd/cmd_pb2.pyi` & `ho-protocols-0.2.1/src/ho_protocols/cmd/cmd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/common_pb2.py` & `ho-protocols-0.2.1/src/ho_protocols/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/common_pb2.pyi` & `ho-protocols-0.2.1/src/ho_protocols/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/data_in_pb2.py` & `ho-protocols-0.2.1/src/ho_protocols/data_in_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/data_in_pb2.pyi` & `ho-protocols-0.2.1/src/ho_protocols/data_in_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/example_pb2.py` & `ho-protocols-0.2.1/src/ho_protocols/example_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/example_pb2.pyi` & `ho-protocols-0.2.1/src/ho_protocols/example_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/live/actuators_pb2.py` & `ho-protocols-0.2.1/src/ho_protocols/live/actuators_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/live/actuators_pb2.pyi` & `ho-protocols-0.2.1/src/ho_protocols/live/actuators_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/live/live_pb2.py` & `ho-protocols-0.2.1/src/ho_protocols/live/live_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/live/live_pb2.pyi` & `ho-protocols-0.2.1/src/ho_protocols/live/live_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/live/models_pb2.py` & `ho-protocols-0.2.1/src/ho_protocols/live/models_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/live/models_pb2.pyi` & `ho-protocols-0.2.1/src/ho_protocols/live/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/live/sensors_pb2.py` & `ho-protocols-0.2.1/src/ho_protocols/live/sensors_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/live/sensors_pb2.pyi` & `ho-protocols-0.2.1/src/ho_protocols/live/sensors_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/live/system_pb2.py` & `ho-protocols-0.2.1/src/ho_protocols/live/system_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/live/system_pb2.pyi` & `ho-protocols-0.2.1/src/ho_protocols/live/system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/map/map_pb2.py` & `ho-protocols-0.2.1/src/ho_protocols/map/map_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,33 +10,41 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from ho_protocols import common_pb2 as ho__protocols_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aho_protocols/map/map.proto\x12\x06ho.map\x1a\x19ho_protocols/common.proto\"\xaa\x01\n\nMapRequest\x12!\n\x06header\x18\x01 \x01(\x0b\x32\x11.ho.common.Header\x12\x33\n\x10weather_forecast\x18\x02 \x01(\x0b\x32\x17.ho.map.WeatherForecastH\x00\x12;\n\x14harvesting_resources\x18\x03 \x01(\x0b\x32\x1b.ho.map.HarvestingResourcesH\x00\x42\x07\n\x05query\"\x95\x01\n\x0bMapResponse\x12\x39\n\x10weather_forecast\x18\x02 \x01(\x0b\x32\x1d.ho.map.WeatherForecastResultH\x00\x12\x41\n\x14harvesting_resources\x18\x03 \x01(\x0b\x32!.ho.map.HarvestingResourcesResultH\x00\x42\x08\n\x06result\"<\n\x0fWeatherForecast\x12\x0b\n\x03lat\x18\x01 \x01(\x02\x12\x0b\n\x03lng\x18\x02 \x01(\x02\x12\x0f\n\x07periods\x18\x03 \x01(\x05\"\xaa\x01\n\x15WeatherForecastResult\x12\x30\n\x04item\x18\x01 \x03(\x0b\x32\".ho.map.WeatherForecastResult.Item\x1a_\n\x04Item\x12\n\n\x02ts\x18\x01 \x01(\x03\x12\x13\n\x0btemperature\x18\x02 \x01(\x02\x12\x10\n\x08humidity\x18\x03 \x01(\x02\x12\x12\n\nwind_speed\x18\x04 \x01(\x02\x12\x10\n\x08wind_deg\x18\x05 \x01(\x02\";\n\x13HarvestingResources\x12\x0b\n\x03lat\x18\x01 \x01(\x02\x12\x0b\n\x03lng\x18\x02 \x01(\x02\x12\n\n\x02ts\x18\x03 \x01(\x03\"\xf9\x01\n\x19HarvestingResourcesResult\x12\x15\n\roverall_index\x18\x01 \x01(\x02\x12\x14\n\x0cnectar_index\x18\x02 \x01(\x02\x12\x14\n\x0cpollen_index\x18\x03 \x01(\x02\x12\x13\n\x0bwater_index\x18\x04 \x01(\x02\x12\x12\n\nroad_index\x18\x05 \x01(\x02\x12\x36\n\x05\x66ield\x18\x06 \x03(\x0b\x32\'.ho.map.HarvestingResourcesResult.Field\x1a\x38\n\x05\x46ield\x12\x12\n\nplant_name\x18\x01 \x01(\t\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x02\x12\x0b\n\x03\x64ir\x18\x03 \x01(\x02\x42\x02H\x03\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aho_protocols/map/map.proto\x12\x06ho.map\x1a\x19ho_protocols/common.proto\"\xd5\x01\n\nMapRequest\x12!\n\x06header\x18\x01 \x01(\x0b\x32\x11.ho.common.Header\x12\x33\n\x10weather_forecast\x18\x02 \x01(\x0b\x32\x17.ho.map.WeatherForecastH\x00\x12;\n\x14harvesting_resources\x18\x03 \x01(\x0b\x32\x1b.ho.map.HarvestingResourcesH\x00\x12)\n\x0b\x63rowd_input\x18\x04 \x01(\x0b\x32\x12.ho.map.CrowdInputH\x00\x42\x07\n\x05query\"\xc6\x01\n\x0bMapResponse\x12\x39\n\x10weather_forecast\x18\x02 \x01(\x0b\x32\x1d.ho.map.WeatherForecastResultH\x00\x12\x41\n\x14harvesting_resources\x18\x03 \x01(\x0b\x32!.ho.map.HarvestingResourcesResultH\x00\x12/\n\x0b\x63rowd_input\x18\x04 \x01(\x0b\x32\x18.ho.map.CrowdInputResultH\x00\x42\x08\n\x06result\"<\n\x0fWeatherForecast\x12\x0b\n\x03lat\x18\x01 \x01(\x02\x12\x0b\n\x03lng\x18\x02 \x01(\x02\x12\x0f\n\x07periods\x18\x03 \x01(\x05\"\xaa\x01\n\x15WeatherForecastResult\x12\x30\n\x04item\x18\x01 \x03(\x0b\x32\".ho.map.WeatherForecastResult.Item\x1a_\n\x04Item\x12\n\n\x02ts\x18\x01 \x01(\x03\x12\x13\n\x0btemperature\x18\x02 \x01(\x02\x12\x10\n\x08humidity\x18\x03 \x01(\x02\x12\x12\n\nwind_speed\x18\x04 \x01(\x02\x12\x10\n\x08wind_deg\x18\x05 \x01(\x02\";\n\x13HarvestingResources\x12\x0b\n\x03lat\x18\x01 \x01(\x02\x12\x0b\n\x03lng\x18\x02 \x01(\x02\x12\n\n\x02ts\x18\x03 \x01(\x03\"\xf9\x01\n\x19HarvestingResourcesResult\x12\x15\n\roverall_index\x18\x01 \x01(\x02\x12\x14\n\x0cnectar_index\x18\x02 \x01(\x02\x12\x14\n\x0cpollen_index\x18\x03 \x01(\x02\x12\x13\n\x0bwater_index\x18\x04 \x01(\x02\x12\x12\n\nroad_index\x18\x05 \x01(\x02\x12\x36\n\x05\x66ield\x18\x06 \x03(\x0b\x32\'.ho.map.HarvestingResourcesResult.Field\x1a\x38\n\x05\x46ield\x12\x12\n\nplant_name\x18\x01 \x01(\t\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x02\x12\x0b\n\x03\x64ir\x18\x03 \x01(\x02\"@\n\nCrowdInput\x12\x0b\n\x03lat\x18\x01 \x01(\x02\x12\x0b\n\x03lng\x18\x02 \x01(\x02\x12\n\n\x02ts\x18\x03 \x01(\x03\x12\x0c\n\x04note\x18\x04 \x01(\t\"\x9f\x01\n\x10\x43rowdInputResult\x12\x31\n\x03\x61\x63k\x18\x01 \x01(\x0b\x32\".ho.map.CrowdInputResult.ACKResultH\x00\x12\x33\n\x04nack\x18\x02 \x01(\x0b\x32#.ho.map.CrowdInputResult.NACKResultH\x00\x1a\x0b\n\tACKResult\x1a\x0c\n\nNACKResultB\x08\n\x06statusB\x02H\x03\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ho_protocols.map.map_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'H\003'
   _globals['_MAPREQUEST']._serialized_start=66
-  _globals['_MAPREQUEST']._serialized_end=236
-  _globals['_MAPRESPONSE']._serialized_start=239
-  _globals['_MAPRESPONSE']._serialized_end=388
-  _globals['_WEATHERFORECAST']._serialized_start=390
-  _globals['_WEATHERFORECAST']._serialized_end=450
-  _globals['_WEATHERFORECASTRESULT']._serialized_start=453
-  _globals['_WEATHERFORECASTRESULT']._serialized_end=623
-  _globals['_WEATHERFORECASTRESULT_ITEM']._serialized_start=528
-  _globals['_WEATHERFORECASTRESULT_ITEM']._serialized_end=623
-  _globals['_HARVESTINGRESOURCES']._serialized_start=625
-  _globals['_HARVESTINGRESOURCES']._serialized_end=684
-  _globals['_HARVESTINGRESOURCESRESULT']._serialized_start=687
-  _globals['_HARVESTINGRESOURCESRESULT']._serialized_end=936
-  _globals['_HARVESTINGRESOURCESRESULT_FIELD']._serialized_start=880
-  _globals['_HARVESTINGRESOURCESRESULT_FIELD']._serialized_end=936
+  _globals['_MAPREQUEST']._serialized_end=279
+  _globals['_MAPRESPONSE']._serialized_start=282
+  _globals['_MAPRESPONSE']._serialized_end=480
+  _globals['_WEATHERFORECAST']._serialized_start=482
+  _globals['_WEATHERFORECAST']._serialized_end=542
+  _globals['_WEATHERFORECASTRESULT']._serialized_start=545
+  _globals['_WEATHERFORECASTRESULT']._serialized_end=715
+  _globals['_WEATHERFORECASTRESULT_ITEM']._serialized_start=620
+  _globals['_WEATHERFORECASTRESULT_ITEM']._serialized_end=715
+  _globals['_HARVESTINGRESOURCES']._serialized_start=717
+  _globals['_HARVESTINGRESOURCES']._serialized_end=776
+  _globals['_HARVESTINGRESOURCESRESULT']._serialized_start=779
+  _globals['_HARVESTINGRESOURCESRESULT']._serialized_end=1028
+  _globals['_HARVESTINGRESOURCESRESULT_FIELD']._serialized_start=972
+  _globals['_HARVESTINGRESOURCESRESULT_FIELD']._serialized_end=1028
+  _globals['_CROWDINPUT']._serialized_start=1030
+  _globals['_CROWDINPUT']._serialized_end=1094
+  _globals['_CROWDINPUTRESULT']._serialized_start=1097
+  _globals['_CROWDINPUTRESULT']._serialized_end=1256
+  _globals['_CROWDINPUTRESULT_ACKRESULT']._serialized_start=1221
+  _globals['_CROWDINPUTRESULT_ACKRESULT']._serialized_end=1232
+  _globals['_CROWDINPUTRESULT_NACKRESULT']._serialized_start=1234
+  _globals['_CROWDINPUTRESULT_NACKRESULT']._serialized_end=1246
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ho-protocols-0.2.0/src/ho_protocols/map/map_pb2.pyi` & `ho-protocols-0.2.1/src/ho_protocols/map/map_pb2.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -20,52 +20,60 @@
 @typing_extensions.final
 class MapRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HEADER_FIELD_NUMBER: builtins.int
     WEATHER_FORECAST_FIELD_NUMBER: builtins.int
     HARVESTING_RESOURCES_FIELD_NUMBER: builtins.int
+    CROWD_INPUT_FIELD_NUMBER: builtins.int
     @property
     def header(self) -> ho_protocols.common_pb2.Header: ...
     @property
     def weather_forecast(self) -> global___WeatherForecast: ...
     @property
     def harvesting_resources(self) -> global___HarvestingResources: ...
+    @property
+    def crowd_input(self) -> global___CrowdInput: ...
     def __init__(
         self,
         *,
         header: ho_protocols.common_pb2.Header | None = ...,
         weather_forecast: global___WeatherForecast | None = ...,
         harvesting_resources: global___HarvestingResources | None = ...,
+        crowd_input: global___CrowdInput | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["harvesting_resources", b"harvesting_resources", "header", b"header", "query", b"query", "weather_forecast", b"weather_forecast"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["harvesting_resources", b"harvesting_resources", "header", b"header", "query", b"query", "weather_forecast", b"weather_forecast"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["query", b"query"]) -> typing_extensions.Literal["weather_forecast", "harvesting_resources"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["crowd_input", b"crowd_input", "harvesting_resources", b"harvesting_resources", "header", b"header", "query", b"query", "weather_forecast", b"weather_forecast"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["crowd_input", b"crowd_input", "harvesting_resources", b"harvesting_resources", "header", b"header", "query", b"query", "weather_forecast", b"weather_forecast"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["query", b"query"]) -> typing_extensions.Literal["weather_forecast", "harvesting_resources", "crowd_input"] | None: ...
 
 global___MapRequest = MapRequest
 
 @typing_extensions.final
 class MapResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     WEATHER_FORECAST_FIELD_NUMBER: builtins.int
     HARVESTING_RESOURCES_FIELD_NUMBER: builtins.int
+    CROWD_INPUT_FIELD_NUMBER: builtins.int
     @property
     def weather_forecast(self) -> global___WeatherForecastResult: ...
     @property
     def harvesting_resources(self) -> global___HarvestingResourcesResult: ...
+    @property
+    def crowd_input(self) -> global___CrowdInputResult: ...
     def __init__(
         self,
         *,
         weather_forecast: global___WeatherForecastResult | None = ...,
         harvesting_resources: global___HarvestingResourcesResult | None = ...,
+        crowd_input: global___CrowdInputResult | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["harvesting_resources", b"harvesting_resources", "result", b"result", "weather_forecast", b"weather_forecast"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["harvesting_resources", b"harvesting_resources", "result", b"result", "weather_forecast", b"weather_forecast"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["result", b"result"]) -> typing_extensions.Literal["weather_forecast", "harvesting_resources"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["crowd_input", b"crowd_input", "harvesting_resources", b"harvesting_resources", "result", b"result", "weather_forecast", b"weather_forecast"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["crowd_input", b"crowd_input", "harvesting_resources", b"harvesting_resources", "result", b"result", "weather_forecast", b"weather_forecast"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["result", b"result"]) -> typing_extensions.Literal["weather_forecast", "harvesting_resources", "crowd_input"] | None: ...
 
 global___MapResponse = MapResponse
 
 @typing_extensions.final
 class WeatherForecast(google.protobuf.message.Message):
     """#####"""
 
@@ -197,7 +205,71 @@
         water_index: builtins.float = ...,
         road_index: builtins.float = ...,
         field: collections.abc.Iterable[global___HarvestingResourcesResult.Field] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["field", b"field", "nectar_index", b"nectar_index", "overall_index", b"overall_index", "pollen_index", b"pollen_index", "road_index", b"road_index", "water_index", b"water_index"]) -> None: ...
 
 global___HarvestingResourcesResult = HarvestingResourcesResult
+
+@typing_extensions.final
+class CrowdInput(google.protobuf.message.Message):
+    """######"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    LAT_FIELD_NUMBER: builtins.int
+    LNG_FIELD_NUMBER: builtins.int
+    TS_FIELD_NUMBER: builtins.int
+    NOTE_FIELD_NUMBER: builtins.int
+    lat: builtins.float
+    lng: builtins.float
+    ts: builtins.int
+    note: builtins.str
+    def __init__(
+        self,
+        *,
+        lat: builtins.float = ...,
+        lng: builtins.float = ...,
+        ts: builtins.int = ...,
+        note: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["lat", b"lat", "lng", b"lng", "note", b"note", "ts", b"ts"]) -> None: ...
+
+global___CrowdInput = CrowdInput
+
+@typing_extensions.final
+class CrowdInputResult(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
+    class ACKResult(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        def __init__(
+            self,
+        ) -> None: ...
+
+    @typing_extensions.final
+    class NACKResult(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        def __init__(
+            self,
+        ) -> None: ...
+
+    ACK_FIELD_NUMBER: builtins.int
+    NACK_FIELD_NUMBER: builtins.int
+    @property
+    def ack(self) -> global___CrowdInputResult.ACKResult: ...
+    @property
+    def nack(self) -> global___CrowdInputResult.NACKResult: ...
+    def __init__(
+        self,
+        *,
+        ack: global___CrowdInputResult.ACKResult | None = ...,
+        nack: global___CrowdInputResult.NACKResult | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["ack", b"ack", "nack", b"nack", "status", b"status"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["ack", b"ack", "nack", b"nack", "status", b"status"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["status", b"status"]) -> typing_extensions.Literal["ack", "nack"] | None: ...
+
+global___CrowdInputResult = CrowdInputResult
```

### Comparing `ho-protocols-0.2.0/src/ho_protocols/query/query_pb2.py` & `ho-protocols-0.2.1/src/ho_protocols/query/query_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols/query/query_pb2.pyi` & `ho-protocols-0.2.1/src/ho_protocols/query/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/src/ho_protocols.egg-info/PKG-INFO` & `ho-protocols-0.2.1/src/ho_protocols.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ho-protocols
-Version: 0.2.0
+Version: 0.2.1
 Summary: ProtoBuf definitions for HO components
 Home-page: https://github.com/hiveopolis/ho-protocols
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ho-protocols-0.2.0/src/ho_protocols.egg-info/SOURCES.txt` & `ho-protocols-0.2.1/src/ho_protocols.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.0/test/test.py` & `ho-protocols-0.2.1/test/test.py`

 * *Files identical despite different names*

