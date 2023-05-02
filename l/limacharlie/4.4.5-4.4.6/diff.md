# Comparing `tmp/limacharlie-4.4.5.tar.gz` & `tmp/limacharlie-4.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limacharlie-4.4.5.tar", last modified: Sun Apr 30 23:57:24 2023, max compression
+gzip compressed data, was "limacharlie-4.4.6.tar", last modified: Mon May  1 21:29:02 2023, max compression
```

## Comparing `limacharlie-4.4.5.tar` & `limacharlie-4.4.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-30 23:57:24.266409 limacharlie-4.4.5/
--rw-r--r--   0 maxime    (1000) maxime    (1000)    11357 2021-03-23 21:34:15.000000 limacharlie-4.4.5/LICENSE
--rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-30 23:57:24.266409 limacharlie-4.4.5/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10845 2023-04-28 15:20:27.000000 limacharlie-4.4.5/README.md
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-30 23:57:24.261409 limacharlie-4.4.5/limacharlie/
--rw-r--r--   0 maxime    (1000) maxime    (1000)    50463 2023-04-12 22:28:28.000000 limacharlie-4.4.5/limacharlie/Configs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     3361 2021-03-23 21:34:15.000000 limacharlie-4.4.5/limacharlie/DRCli.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     5057 2023-04-24 15:42:48.000000 limacharlie-4.4.5/limacharlie/Extensions.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    14867 2022-09-03 02:23:38.000000 limacharlie-4.4.5/limacharlie/Firehose.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10160 2023-04-24 16:27:39.000000 limacharlie-4.4.5/limacharlie/Hive.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2643 2021-03-23 21:34:15.000000 limacharlie-4.4.5/limacharlie/Jobs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    15935 2022-11-03 04:20:06.000000 limacharlie-4.4.5/limacharlie/Logs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    52973 2023-04-30 23:56:52.000000 limacharlie-4.4.5/limacharlie/Manager.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2803 2021-03-23 21:34:15.000000 limacharlie-4.4.5/limacharlie/Payloads.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    16039 2023-04-12 23:50:48.000000 limacharlie-4.4.5/limacharlie/Query.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    19246 2023-04-12 23:50:48.000000 limacharlie-4.4.5/limacharlie/Replay.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    12905 2022-11-26 21:02:39.000000 limacharlie-4.4.5/limacharlie/Replicants.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     8981 2023-04-06 18:48:27.000000 limacharlie-4.4.5/limacharlie/Search.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    17438 2023-04-06 18:48:27.000000 limacharlie-4.4.5/limacharlie/Sensor.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    24227 2022-09-23 18:58:57.000000 limacharlie-4.4.5/limacharlie/SpotCheck.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    10704 2022-07-08 00:49:08.000000 limacharlie-4.4.5/limacharlie/Spout.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    33649 2021-06-21 23:20:54.000000 limacharlie-4.4.5/limacharlie/Sync.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      970 2021-03-23 21:34:15.000000 limacharlie-4.4.5/limacharlie/Webhook.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2305 2023-04-30 23:56:52.000000 limacharlie-4.4.5/limacharlie/__init__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    16201 2023-04-30 23:56:52.000000 limacharlie-4.4.5/limacharlie/__main__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6821 2022-12-01 21:47:34.000000 limacharlie-4.4.5/limacharlie/utils.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-30 23:57:24.263409 limacharlie-4.4.5/limacharlie.egg-info/
--rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-04-30 23:57:24.000000 limacharlie-4.4.5/limacharlie.egg-info/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)      879 2023-04-30 23:57:24.000000 limacharlie-4.4.5/limacharlie.egg-info/SOURCES.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-04-30 23:57:24.000000 limacharlie-4.4.5/limacharlie.egg-info/dependency_links.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       58 2023-04-30 23:57:24.000000 limacharlie-4.4.5/limacharlie.egg-info/entry_points.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       43 2023-04-30 23:57:24.000000 limacharlie-4.4.5/limacharlie.egg-info/requires.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       12 2023-04-30 23:57:24.000000 limacharlie-4.4.5/limacharlie.egg-info/top_level.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2021-03-23 21:34:40.000000 limacharlie-4.4.5/limacharlie.egg-info/zip-safe
--rw-r--r--   0 maxime    (1000) maxime    (1000)       79 2023-04-30 23:57:24.267409 limacharlie-4.4.5/setup.cfg
--rw-r--r--   0 maxime    (1000) maxime    (1000)      892 2023-04-30 23:56:52.000000 limacharlie-4.4.5/setup.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-04-30 23:57:24.266409 limacharlie-4.4.5/tests/
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2394 2021-03-23 21:34:15.000000 limacharlie-4.4.5/tests/test_artifacts.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6000 2022-12-12 23:19:01.000000 limacharlie-4.4.5/tests/test_core.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1415 2021-03-23 21:34:15.000000 limacharlie-4.4.5/tests/test_insight.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      424 2021-03-23 21:34:15.000000 limacharlie-4.4.5/tests/test_replicants.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1327 2021-03-23 21:34:15.000000 limacharlie-4.4.5/tests/test_spout.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6055 2022-09-21 18:43:37.000000 limacharlie-4.4.5/tests/test_sync.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-01 21:29:02.863931 limacharlie-4.4.6/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    11357 2021-03-23 21:34:15.000000 limacharlie-4.4.6/LICENSE
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-05-01 21:29:02.864931 limacharlie-4.4.6/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10845 2023-04-28 15:20:27.000000 limacharlie-4.4.6/README.md
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-01 21:29:02.855931 limacharlie-4.4.6/limacharlie/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    50463 2023-04-12 22:28:28.000000 limacharlie-4.4.6/limacharlie/Configs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     3361 2021-03-23 21:34:15.000000 limacharlie-4.4.6/limacharlie/DRCli.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     5057 2023-04-24 15:42:48.000000 limacharlie-4.4.6/limacharlie/Extensions.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    14867 2022-09-03 02:23:38.000000 limacharlie-4.4.6/limacharlie/Firehose.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10160 2023-04-24 16:27:39.000000 limacharlie-4.4.6/limacharlie/Hive.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2643 2021-03-23 21:34:15.000000 limacharlie-4.4.6/limacharlie/Jobs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    15935 2022-11-03 04:20:06.000000 limacharlie-4.4.6/limacharlie/Logs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    52973 2023-04-30 23:56:52.000000 limacharlie-4.4.6/limacharlie/Manager.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2803 2021-03-23 21:34:15.000000 limacharlie-4.4.6/limacharlie/Payloads.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    16039 2023-04-12 23:50:48.000000 limacharlie-4.4.6/limacharlie/Query.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    19246 2023-04-12 23:50:48.000000 limacharlie-4.4.6/limacharlie/Replay.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    12905 2022-11-26 21:02:39.000000 limacharlie-4.4.6/limacharlie/Replicants.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     8981 2023-04-06 18:48:27.000000 limacharlie-4.4.6/limacharlie/Search.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    17438 2023-04-06 18:48:27.000000 limacharlie-4.4.6/limacharlie/Sensor.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    24227 2022-09-23 18:58:57.000000 limacharlie-4.4.6/limacharlie/SpotCheck.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    10781 2023-05-01 21:28:43.000000 limacharlie-4.4.6/limacharlie/Spout.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    33649 2021-06-21 23:20:54.000000 limacharlie-4.4.6/limacharlie/Sync.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      970 2021-03-23 21:34:15.000000 limacharlie-4.4.6/limacharlie/Webhook.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2305 2023-05-01 21:28:43.000000 limacharlie-4.4.6/limacharlie/__init__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    16201 2023-04-30 23:56:52.000000 limacharlie-4.4.6/limacharlie/__main__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6821 2022-12-01 21:47:34.000000 limacharlie-4.4.6/limacharlie/utils.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-01 21:29:02.859931 limacharlie-4.4.6/limacharlie.egg-info/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      344 2023-05-01 21:29:02.000000 limacharlie-4.4.6/limacharlie.egg-info/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      879 2023-05-01 21:29:02.000000 limacharlie-4.4.6/limacharlie.egg-info/SOURCES.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-05-01 21:29:02.000000 limacharlie-4.4.6/limacharlie.egg-info/dependency_links.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       58 2023-05-01 21:29:02.000000 limacharlie-4.4.6/limacharlie.egg-info/entry_points.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       43 2023-05-01 21:29:02.000000 limacharlie-4.4.6/limacharlie.egg-info/requires.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       12 2023-05-01 21:29:02.000000 limacharlie-4.4.6/limacharlie.egg-info/top_level.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2021-03-23 21:34:40.000000 limacharlie-4.4.6/limacharlie.egg-info/zip-safe
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       79 2023-05-01 21:29:02.865931 limacharlie-4.4.6/setup.cfg
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      892 2023-05-01 21:28:43.000000 limacharlie-4.4.6/setup.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-01 21:29:02.863931 limacharlie-4.4.6/tests/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2394 2021-03-23 21:34:15.000000 limacharlie-4.4.6/tests/test_artifacts.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6000 2022-12-12 23:19:01.000000 limacharlie-4.4.6/tests/test_core.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1415 2021-03-23 21:34:15.000000 limacharlie-4.4.6/tests/test_insight.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      424 2021-03-23 21:34:15.000000 limacharlie-4.4.6/tests/test_replicants.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1327 2021-03-23 21:34:15.000000 limacharlie-4.4.6/tests/test_spout.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6055 2022-09-21 18:43:37.000000 limacharlie-4.4.6/tests/test_sync.py
```

### Comparing `limacharlie-4.4.5/LICENSE` & `limacharlie-4.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/README.md` & `limacharlie-4.4.6/README.md`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Configs.py` & `limacharlie-4.4.6/limacharlie/Configs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/DRCli.py` & `limacharlie-4.4.6/limacharlie/DRCli.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Extensions.py` & `limacharlie-4.4.6/limacharlie/Extensions.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Firehose.py` & `limacharlie-4.4.6/limacharlie/Firehose.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Hive.py` & `limacharlie-4.4.6/limacharlie/Hive.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Jobs.py` & `limacharlie-4.4.6/limacharlie/Jobs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Logs.py` & `limacharlie-4.4.6/limacharlie/Logs.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Manager.py` & `limacharlie-4.4.6/limacharlie/Manager.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Payloads.py` & `limacharlie-4.4.6/limacharlie/Payloads.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Query.py` & `limacharlie-4.4.6/limacharlie/Query.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Replay.py` & `limacharlie-4.4.6/limacharlie/Replay.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Replicants.py` & `limacharlie-4.4.6/limacharlie/Replicants.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Search.py` & `limacharlie-4.4.6/limacharlie/Search.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Sensor.py` & `limacharlie-4.4.6/limacharlie/Sensor.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/SpotCheck.py` & `limacharlie-4.4.6/limacharlie/SpotCheck.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Spout.py` & `limacharlie-4.4.6/limacharlie/Spout.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         # Spouts work by doing a POST to the stream.limacharlie.io service with the
         # OID, Secret Key and any Output parameters we want. The HTTP response will
         # be a stream of data.
         self._hConn = self._getStream( spoutParams )
         if self._hConn.status_code != 200:
             raise LcApiException( 'failed to open Spout (%s): %s' % ( self._hConn.status_code, self._hConn.text ) )
         handleConnectionThread = threading.Thread( target = self._handleConnection, args = ( spoutParams, ) )
+        handleConnectionThread.daemon = True
         self._threads.append( handleConnectionThread )
         handleConnectionThread.start()
         self._futureCleanupInterval = 30
         cleanupFuturesThread = threading.Thread( target = self._cleanupFutures )
         cleanupFuturesThread.daemon = True
         cleanupFuturesThread.start()
 
@@ -243,15 +244,16 @@
                             tag = args.tag,
                             cat = args.cat,
                             sid = args.sid )
 
     def _signal_handler( signum, frame ):
         _printToStderr( 'You pressed Ctrl+C!' )
         sp._isStopStop = True
-        threading.Thread( target = sp.shutdown() ).start()
+        hTh = threading.Thread( target = sp.shutdown() ).start()
+        hTh.daemon = True
 
     signal.signal( signal.SIGINT, _signal_handler )
 
     _printToStderr( "Starting to listen..." )
     while not sp._isStop:
         try:
             data = sp.queue.get( timeout = 1 )
```

### Comparing `limacharlie-4.4.5/limacharlie/Sync.py` & `limacharlie-4.4.6/limacharlie/Sync.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/Webhook.py` & `limacharlie-4.4.6/limacharlie/Webhook.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/__init__.py` & `limacharlie-4.4.6/limacharlie/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """limacharlie API for limacharlie.io"""
 
-__version__ = "4.4.5"
+__version__ = "4.4.6"
 __author__ = "Maxime Lamothe-Brassard ( Refraction Point, Inc )"
 __author_email__ = "maxime@refractionpoint.com"
 __license__ = "Apache v2"
 __copyright__ = "Copyright (c) 2020 Refraction Point, Inc"
 
 # Global API Credentials
 import os
```

### Comparing `limacharlie-4.4.5/limacharlie/__main__.py` & `limacharlie-4.4.6/limacharlie/__main__.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie/utils.py` & `limacharlie-4.4.6/limacharlie/utils.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/limacharlie.egg-info/SOURCES.txt` & `limacharlie-4.4.6/limacharlie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/setup.py` & `limacharlie-4.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "4.4.5"
+__version__ = "4.4.6"
 __author__ = "Maxime Lamothe-Brassard ( Refraction Point, Inc )"
 __author_email__ = "maxime@refractionpoint.com"
 __license__ = "Apache v2"
 __copyright__ = "Copyright (c) 2020 Refraction Point, Inc"
 
 setup( name = 'limacharlie',
        version = __version__,
```

### Comparing `limacharlie-4.4.5/tests/test_artifacts.py` & `limacharlie-4.4.6/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/tests/test_core.py` & `limacharlie-4.4.6/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/tests/test_insight.py` & `limacharlie-4.4.6/tests/test_insight.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/tests/test_spout.py` & `limacharlie-4.4.6/tests/test_spout.py`

 * *Files identical despite different names*

### Comparing `limacharlie-4.4.5/tests/test_sync.py` & `limacharlie-4.4.6/tests/test_sync.py`

 * *Files identical despite different names*

