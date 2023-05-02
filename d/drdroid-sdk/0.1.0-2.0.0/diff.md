# Comparing `tmp/drdroid-sdk-0.1.0.tar.gz` & `tmp/drdroid-sdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drdroid-sdk-0.1.0.tar", last modified: Fri Mar 17 09:24:12 2023, max compression
+gzip compressed data, was "drdroid-sdk-2.0.0.tar", last modified: Tue May  2 06:05:26 2023, max compression
```

## Comparing `drdroid-sdk-0.1.0.tar` & `drdroid-sdk-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mohit.goyal   (501) staff       (20)        0 2023-03-17 09:24:12.452309 drdroid-sdk-0.1.0/
--rw-r--r--   0 mohit.goyal   (501) staff       (20)     1073 2023-03-17 06:22:04.000000 drdroid-sdk-0.1.0/LICENSE.txt
--rw-r--r--   0 mohit.goyal   (501) staff       (20)      437 2023-03-17 09:24:12.452184 drdroid-sdk-0.1.0/PKG-INFO
--rw-r--r--   0 mohit.goyal   (501) staff       (20)     2554 2023-03-17 08:28:26.000000 drdroid-sdk-0.1.0/README.md
-drwxr-xr-x   0 mohit.goyal   (501) staff       (20)        0 2023-03-17 09:24:12.450649 drdroid-sdk-0.1.0/drdroid_sdk.egg-info/
--rw-r--r--   0 mohit.goyal   (501) staff       (20)      437 2023-03-17 09:24:12.000000 drdroid-sdk-0.1.0/drdroid_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mohit.goyal   (501) staff       (20)      373 2023-03-17 09:24:12.000000 drdroid-sdk-0.1.0/drdroid_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mohit.goyal   (501) staff       (20)        1 2023-03-17 09:24:12.000000 drdroid-sdk-0.1.0/drdroid_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mohit.goyal   (501) staff       (20)       17 2023-03-17 09:24:12.000000 drdroid-sdk-0.1.0/drdroid_sdk.egg-info/requires.txt
--rw-r--r--   0 mohit.goyal   (501) staff       (20)       14 2023-03-17 09:24:12.000000 drdroid-sdk-0.1.0/drdroid_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 mohit.goyal   (501) staff       (20)        0 2023-03-17 09:24:12.451860 drdroid-sdk-0.1.0/pydoctordroid/
--rw-r--r--   0 mohit.goyal   (501) staff       (20)      112 2023-03-17 06:22:04.000000 drdroid-sdk-0.1.0/pydoctordroid/__init__.py
--rw-r--r--   0 mohit.goyal   (501) staff       (20)     1243 2023-03-17 06:26:10.000000 drdroid-sdk-0.1.0/pydoctordroid/_event_exporter.py
--rw-r--r--   0 mohit.goyal   (501) staff       (20)      945 2023-03-17 06:26:28.000000 drdroid-sdk-0.1.0/pydoctordroid/_events.py
--rw-r--r--   0 mohit.goyal   (501) staff       (20)      476 2023-03-17 06:22:04.000000 drdroid-sdk-0.1.0/pydoctordroid/_logger.py
--rw-r--r--   0 mohit.goyal   (501) staff       (20)     3289 2023-03-17 06:22:04.000000 drdroid-sdk-0.1.0/pydoctordroid/_value.py
--rw-r--r--   0 mohit.goyal   (501) staff       (20)     2044 2023-03-17 06:39:32.000000 drdroid-sdk-0.1.0/pydoctordroid/lib.py
--rw-r--r--   0 mohit.goyal   (501) staff       (20)      105 2023-03-17 06:22:04.000000 drdroid-sdk-0.1.0/pyproject.toml
--rw-r--r--   0 mohit.goyal   (501) staff       (20)       38 2023-03-17 09:24:12.452355 drdroid-sdk-0.1.0/setup.cfg
--rw-r--r--   0 mohit.goyal   (501) staff       (20)      693 2023-03-17 08:51:35.000000 drdroid-sdk-0.1.0/setup.py
+drwxr-xr-x   0 mohit.goyal   (501) staff       (20)        0 2023-05-02 06:05:26.719469 drdroid-sdk-2.0.0/
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)     1073 2023-03-17 10:32:22.000000 drdroid-sdk-2.0.0/LICENSE.txt
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)      437 2023-05-02 06:05:26.719358 drdroid-sdk-2.0.0/PKG-INFO
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)     2687 2023-05-02 06:03:33.000000 drdroid-sdk-2.0.0/README.md
+drwxr-xr-x   0 mohit.goyal   (501) staff       (20)        0 2023-05-02 06:05:26.718294 drdroid-sdk-2.0.0/drdroid_sdk.egg-info/
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)      437 2023-05-02 06:05:26.000000 drdroid-sdk-2.0.0/drdroid_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)      373 2023-05-02 06:05:26.000000 drdroid-sdk-2.0.0/drdroid_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)        1 2023-05-02 06:05:26.000000 drdroid-sdk-2.0.0/drdroid_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)       17 2023-05-02 06:05:26.000000 drdroid-sdk-2.0.0/drdroid_sdk.egg-info/requires.txt
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)       14 2023-05-02 06:05:26.000000 drdroid-sdk-2.0.0/drdroid_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 mohit.goyal   (501) staff       (20)        0 2023-05-02 06:05:26.719196 drdroid-sdk-2.0.0/pydoctordroid/
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)      112 2023-03-17 10:32:22.000000 drdroid-sdk-2.0.0/pydoctordroid/__init__.py
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)     1243 2023-03-17 10:32:22.000000 drdroid-sdk-2.0.0/pydoctordroid/_event_exporter.py
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)     1004 2023-05-02 06:03:33.000000 drdroid-sdk-2.0.0/pydoctordroid/_events.py
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)      476 2023-03-17 10:32:22.000000 drdroid-sdk-2.0.0/pydoctordroid/_logger.py
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)     3289 2023-03-17 10:32:22.000000 drdroid-sdk-2.0.0/pydoctordroid/_value.py
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)     2032 2023-05-02 06:03:33.000000 drdroid-sdk-2.0.0/pydoctordroid/lib.py
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)      105 2023-03-17 10:32:22.000000 drdroid-sdk-2.0.0/pyproject.toml
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)       38 2023-05-02 06:05:26.719512 drdroid-sdk-2.0.0/setup.cfg
+-rw-r--r--   0 mohit.goyal   (501) staff       (20)      693 2023-05-02 06:04:59.000000 drdroid-sdk-2.0.0/setup.py
```

### Comparing `drdroid-sdk-0.1.0/LICENSE.txt` & `drdroid-sdk-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drdroid-sdk-0.1.0/README.md` & `drdroid-sdk-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,68 +6,81 @@
 ## Install the SDK
 
 Run this command to get the latest stable version of the SDK.
 
 ```
 pip install drdroid-sdk
 ```
+
 ## Env vars
 
 | Env Var Name       | Description                                 | Default                   |
 |--------------------|---------------------------------------------|---------------------------|
 | DRDROID_HOSTNAME   | Ingestion endpoint for the events collected | https://ingest.drdroid.io |
 | DRDROID_AUTH_TOKEN | Authentication token for platform           | ---                       |
 | DRDROID_DEBUG      | Enable debug logs for sdk                   | False                     |
 
-
 ## Configuration
+
 Identify the auth token needed for the events to be published to the platform by visiting [site](https://app.drdroid.io)
 Once auth token is available, you can set the env var as:
+
 ```shell
 export DRDROID_AUTH_TOKEN=<TOKEN>
 ```
 
-
 ## Start sending events
+
 A global instance of `DrDroid` is created by default based on the config provided through the env vars.
 The global instance can then be used to publish events by directly calling the `publish` api.
 
 ```python
 import pydoctordroid
 
 pydoctordroid.publish("Order_Created", {"ID": "13432", "City": "BLR", "IS_COD": False})
 ```
 
 Alternatively, you can import the module in your python file and create a DrDroid object.
+
 ```python
 from pydoctordroid import DrDroid
+
 dr = DrDroid()
 ```
 
 You can then send events in the following format:
 
 ```
 dr.publish('Event_Name', Attribute_KeyValue_Dict)
 ```
 
 For example, creating events for an order placement workflow could look like:
 
 ```python
+from pydoctordroid import DrDroid
+
+dr = DrDroid()
+
 dr.publish("Order_Created", {"ID": "13432", "City": "BLR", "IS_COD": False})
 ```
 
 If you want to publish with a certain timestamp and not default to the current system time, you can pass _event_time_ in
-epoch time format (seconds).
+epoch time format (milliseconds).
 
 ```python
-dr.publish("Order_Created", {"ID": "13432", "City": "BLR", "IS_COD": False}, event_time=datetime.now())
-```
+import time
+from pydoctordroid import DrDroid
+
+dr = DrDroid()
 
+dr.publish("Order_Created", {"ID": "13432", "City": "BLR", "IS_COD": False}, event_time=round(time.time() * 1000))
+```
 
 ## View your workflows
 
-Once your events have been published, you can view the workflow these events in your DrDroid account @ [https://app.drdroid.io](https://app.drdroid.io).
+Once your events have been published, you can view the workflow these events in your DrDroid account
+@ [https://app.drdroid.io](https://app.drdroid.io).
 
 Visit [Doctor Droid website](https://drdroid.io?utm_param=github-py) for getting early access.
 Go through our [documentation](https://docs.drdroid.io?utm_param=github-py) to learn more.
 
 For any queries, reach out at [dipesh@drdroid.io](mailto:dipesh@drdroid.io).
```

### Comparing `drdroid-sdk-0.1.0/pydoctordroid/_event_exporter.py` & `drdroid-sdk-2.0.0/pydoctordroid/_event_exporter.py`

 * *Files identical despite different names*

### Comparing `drdroid-sdk-0.1.0/pydoctordroid/_events.py` & `drdroid-sdk-2.0.0/pydoctordroid/_events.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import json
+import time
 from datetime import datetime, timezone
 from typing import Any, Dict, List
 
 from pydoctordroid._value import process_payload, Value
 
 EventType = Dict
 
 
-def create_event(name: str, payload: dict, event_time: datetime = None) -> EventType:
+def current_milli_time():
+    return round(time.time() * 1000)
+
+
+def create_event(name: str, payload: dict, event_time=None) -> EventType:
     return {
         'name': name,
-        'timestamp': (event_time or datetime.now(timezone.utc)),
+        'timestamp': (event_time or current_milli_time()),
         'kvs': process_payload(payload or {})
     }
 
 
 class EventEncoder(json.JSONEncoder):
     fmt = '%Y-%m-%dT%H:%M:%S.%fZ'
```

### Comparing `drdroid-sdk-0.1.0/pydoctordroid/_value.py` & `drdroid-sdk-2.0.0/pydoctordroid/_value.py`

 * *Files identical despite different names*

### Comparing `drdroid-sdk-0.1.0/pydoctordroid/lib.py` & `drdroid-sdk-2.0.0/pydoctordroid/lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             self._logger = setup_logger('drdroid.sdk.instance', False)
 
         self._event_exporter = HttpEventExporter(self._token, self._hostname, self._logger)
         if self._event_exporter:
             self._setup = True
         return
 
-    def publish(self, name: str, payload: dict = None, event_time: datetime = None):
+    def publish(self, name: str, payload: dict = None, event_time=None):
         if not self._setup:
             return
         try:
             event = create_event(name, payload, event_time)
             self._event_exporter.export(event)
         except Exception as e:
             self._logger.debug(msg=f'Error exporting event: {e}')
```

### Comparing `drdroid-sdk-0.1.0/setup.py` & `drdroid-sdk-2.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #     long_description = fh.read()
 
 setup(
     name='drdroid-sdk',
     setup_requires=['wheel'],
     packages=['pydoctordroid'],
     include_package_data=True,
-    version='0.1.0',
+    version='2.0.0',
     description='Code Marker Library from Doctor Droid to generate custom events',
     author='Dipesh Mittal',
     author_email="dipesh@drdroid.io",
     license='MIT',
     python_requires=">=3.6",
     classifiers=[
         "Programming Language :: Python :: 3",
```

