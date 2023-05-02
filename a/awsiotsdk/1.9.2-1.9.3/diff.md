# Comparing `tmp/awsiotsdk-1.9.2.tar.gz` & `tmp/awsiotsdk-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/awsiotsdk-1.9.2.tar", last modified: Fri Feb 18 18:50:18 2022, max compression
+gzip compressed data, was "dist/awsiotsdk-1.9.3.tar", last modified: Tue Mar 15 20:44:32 2022, max compression
```

## Comparing `awsiotsdk-1.9.2.tar` & `awsiotsdk-1.9.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 18:50:18.000000 awsiotsdk-1.9.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 18:50:18.000000 awsiotsdk-1.9.2/awsiot/
--rw-r--r--   0 root         (0) root         (0)    32644 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/awsiot/eventstreamrpc.py
--rw-r--r--   0 root         (0) root         (0)    74150 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/awsiot/iotshadow.py
--rw-r--r--   0 root         (0) root         (0)     7651 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/awsiot/greengrass_discovery.py
--rw-r--r--   0 root         (0) root         (0)     6174 2022-02-18 18:50:18.000000 awsiotsdk-1.9.2/awsiot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25425 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/awsiot/iotidentity.py
--rw-r--r--   0 root         (0) root         (0)    66866 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/awsiot/iotjobs.py
--rw-r--r--   0 root         (0) root         (0)    17106 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/awsiot/mqtt_connection_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 18:50:18.000000 awsiotsdk-1.9.2/awsiot/greengrasscoreipc/
--rw-r--r--   0 root         (0) root         (0)    51508 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/awsiot/greengrasscoreipc/clientv2.py
--rw-r--r--   0 root         (0) root         (0)    51854 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/awsiot/greengrasscoreipc/client.py
--rw-r--r--   0 root         (0) root         (0)     2315 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/awsiot/greengrasscoreipc/__init__.py
--rw-r--r--   0 root         (0) root         (0)   160337 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/awsiot/greengrasscoreipc/model.py
--rw-r--r--   0 root         (0) root         (0)     1366 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/setup.py
--rw-r--r--   0 root         (0) root         (0)    11421 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       83 2022-02-18 18:50:18.000000 awsiotsdk-1.9.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      137 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/NOTICE
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 18:50:18.000000 awsiotsdk-1.9.2/awsiotsdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-18 18:50:18.000000 awsiotsdk-1.9.2/awsiotsdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      593 2022-02-18 18:50:18.000000 awsiotsdk-1.9.2/awsiotsdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-02-18 18:50:18.000000 awsiotsdk-1.9.2/awsiotsdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-02-18 18:50:18.000000 awsiotsdk-1.9.2/awsiotsdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     6706 2022-02-18 18:50:18.000000 awsiotsdk-1.9.2/awsiotsdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6706 2022-02-18 18:50:18.000000 awsiotsdk-1.9.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-18 18:50:18.000000 awsiotsdk-1.9.2/test/
--rw-r--r--   0 root         (0) root         (0)    18680 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/test/test_rpc.py
--rw-r--r--   0 root         (0) root         (0)     6460 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/test/test_mqtt.py
--rw-r--r--   0 root         (0) root         (0)     4274 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/test/test_samples.py
--rw-r--r--   0 root         (0) root         (0)     4093 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/test/test_ggv2.py
--rw-r--r--   0 root         (0) root         (0)     6156 2022-02-18 18:45:10.000000 awsiotsdk-1.9.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-15 20:44:32.000000 awsiotsdk-1.9.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-15 20:44:32.000000 awsiotsdk-1.9.3/awsiot/
+-rw-r--r--   0 root         (0) root         (0)    32644 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/awsiot/eventstreamrpc.py
+-rw-r--r--   0 root         (0) root         (0)    74150 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/awsiot/iotshadow.py
+-rw-r--r--   0 root         (0) root         (0)     7651 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/awsiot/greengrass_discovery.py
+-rw-r--r--   0 root         (0) root         (0)     6174 2022-03-15 20:44:31.000000 awsiotsdk-1.9.3/awsiot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25425 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/awsiot/iotidentity.py
+-rw-r--r--   0 root         (0) root         (0)    66866 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/awsiot/iotjobs.py
+-rw-r--r--   0 root         (0) root         (0)    17106 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/awsiot/mqtt_connection_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-15 20:44:32.000000 awsiotsdk-1.9.3/awsiot/greengrasscoreipc/
+-rw-r--r--   0 root         (0) root         (0)    52109 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/awsiot/greengrasscoreipc/clientv2.py
+-rw-r--r--   0 root         (0) root         (0)    51881 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/awsiot/greengrasscoreipc/client.py
+-rw-r--r--   0 root         (0) root         (0)     2315 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/awsiot/greengrasscoreipc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   160337 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/awsiot/greengrasscoreipc/model.py
+-rw-r--r--   0 root         (0) root         (0)     1366 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)    11421 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       83 2022-03-15 20:44:32.000000 awsiotsdk-1.9.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      137 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/NOTICE
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-15 20:44:32.000000 awsiotsdk-1.9.3/awsiotsdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-15 20:44:32.000000 awsiotsdk-1.9.3/awsiotsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      593 2022-03-15 20:44:32.000000 awsiotsdk-1.9.3/awsiotsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-03-15 20:44:32.000000 awsiotsdk-1.9.3/awsiotsdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2022-03-15 20:44:32.000000 awsiotsdk-1.9.3/awsiotsdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     6706 2022-03-15 20:44:32.000000 awsiotsdk-1.9.3/awsiotsdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6706 2022-03-15 20:44:32.000000 awsiotsdk-1.9.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-15 20:44:32.000000 awsiotsdk-1.9.3/test/
+-rw-r--r--   0 root         (0) root         (0)    18680 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/test/test_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     6460 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/test/test_mqtt.py
+-rw-r--r--   0 root         (0) root         (0)     4274 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/test/test_samples.py
+-rw-r--r--   0 root         (0) root         (0)     4715 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/test/test_ggv2.py
+-rw-r--r--   0 root         (0) root         (0)     6156 2022-03-15 20:38:12.000000 awsiotsdk-1.9.3/README.md
```

### Comparing `awsiotsdk-1.9.2/awsiot/eventstreamrpc.py` & `awsiotsdk-1.9.3/awsiot/eventstreamrpc.py`

 * *Files identical despite different names*

### Comparing `awsiotsdk-1.9.2/awsiot/iotshadow.py` & `awsiotsdk-1.9.3/awsiot/iotshadow.py`

 * *Files identical despite different names*

### Comparing `awsiotsdk-1.9.2/awsiot/greengrass_discovery.py` & `awsiotsdk-1.9.3/awsiot/greengrass_discovery.py`

 * *Files identical despite different names*

### Comparing `awsiotsdk-1.9.2/awsiot/__init__.py` & `awsiotsdk-1.9.3/awsiot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 
 from awscrt import mqtt
 from concurrent.futures import Future
 import json
 from typing import Any, Callable, Dict, Optional, Tuple, TypeVar
 
-__version__ = '1.9.2'
+__version__ = '1.9.3'
 
 T = TypeVar('T')
 
 PayloadObj = Dict[str, Any]
 PayloadToClassFn = Callable[[PayloadObj], T]
```

### Comparing `awsiotsdk-1.9.2/awsiot/iotidentity.py` & `awsiotsdk-1.9.3/awsiot/iotidentity.py`

 * *Files identical despite different names*

### Comparing `awsiotsdk-1.9.2/awsiot/iotjobs.py` & `awsiotsdk-1.9.3/awsiot/iotjobs.py`

 * *Files identical despite different names*

### Comparing `awsiotsdk-1.9.2/awsiot/mqtt_connection_builder.py` & `awsiotsdk-1.9.3/awsiot/mqtt_connection_builder.py`

 * *Files identical despite different names*

### Comparing `awsiotsdk-1.9.2/awsiot/greengrasscoreipc/clientv2.py` & `awsiotsdk-1.9.3/awsiot/greengrasscoreipc/clientv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def __init__(self, client: typing.Optional[GreengrassCoreIPCClient] = None,
                  executor: typing.Optional[concurrent.futures.Executor] = True):
         if client is None:
             import awsiot.greengrasscoreipc
             client = awsiot.greengrasscoreipc.connect()
         self.client = client
-        if executor == True:
+        if executor is True:
             executor = concurrent.futures.ThreadPoolExecutor()
         self.executor = executor
 
     def close(self, *, executor_wait=True) -> concurrent.futures.Future:
         """
         Close the underlying connection and shutdown the event executor (if any)
 
@@ -63,28 +63,46 @@
             try:
                 future1.result()
             except Exception as e:
                 future2.set_exception(e)
         future1.add_done_callback(callback)
         return future2
 
+    @staticmethod
+    def __handle_error():
+        import sys
+        import traceback
+        traceback.print_exc(file=sys.stderr)
+
+    def __wrap_error(self, func):
+        def wrapper(*args, **kwargs):
+            try:
+                return func(*args, **kwargs)
+            except Exception as e:
+                self.__handle_error()
+                raise e
+        return wrapper
+
     def __create_stream_handler(real_self, operation, on_stream_event, on_stream_error, on_stream_closed):
         stream_handler_type = type(operation + 'Handler', (getattr(client, operation + "StreamHandler"),), {})
         if on_stream_event is not None:
+            on_stream_event = real_self.__wrap_error(on_stream_event)
             def handler(self, event):
                 if real_self.executor is not None:
                     real_self.executor.submit(on_stream_event, event)
                 else:
                     on_stream_event(event)
             setattr(stream_handler_type, "on_stream_event", handler)
         if on_stream_error is not None:
+            on_stream_error = real_self.__wrap_error(on_stream_error)
             def handler(self, error):
                 return on_stream_error(error)
             setattr(stream_handler_type, "on_stream_error", handler)
         if on_stream_closed is not None:
+            on_stream_closed = real_self.__wrap_error(on_stream_closed)
             def handler(self):
                 if real_self.executor is not None:
                     real_self.executor.submit(on_stream_closed)
                 else:
                     on_stream_closed()
             setattr(stream_handler_type, "on_stream_closed", handler)
         return stream_handler_type()
```

### Comparing `awsiotsdk-1.9.2/awsiot/greengrasscoreipc/client.py` & `awsiotsdk-1.9.3/awsiot/greengrasscoreipc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1105,15 +1105,15 @@
         return super().close()
 
 
 class GreengrassCoreIPCClient(rpc.Client):
     """
     Client for the GreengrassCoreIPC service.
     There is a new V2 client available for testing in developer preview.
-    See the GreengrassCoreIPCClientV2 class.
+    See the GreengrassCoreIPCClientV2 class in the clientv2 subpackage.
 
     Args:
         connection: Connection that this client will use.
     """
 
     def __init__(self, connection: rpc.Connection):
         super().__init__(connection, model.SHAPE_INDEX)
```

### Comparing `awsiotsdk-1.9.2/awsiot/greengrasscoreipc/__init__.py` & `awsiotsdk-1.9.3/awsiot/greengrasscoreipc/__init__.py`

 * *Files identical despite different names*

### Comparing `awsiotsdk-1.9.2/awsiot/greengrasscoreipc/model.py` & `awsiotsdk-1.9.3/awsiot/greengrasscoreipc/model.py`

 * *Files identical despite different names*

### Comparing `awsiotsdk-1.9.2/setup.py` & `awsiotsdk-1.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,11 +36,11 @@
     packages=find_packages(include=['awsiot*']),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'awscrt==0.13.3',
+        'awscrt==0.13.5',
     ],
     python_requires='>=3.6',
 )
```

### Comparing `awsiotsdk-1.9.2/LICENSE` & `awsiotsdk-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `awsiotsdk-1.9.2/awsiotsdk.egg-info/SOURCES.txt` & `awsiotsdk-1.9.3/awsiotsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `awsiotsdk-1.9.2/awsiotsdk.egg-info/PKG-INFO` & `awsiotsdk-1.9.3/awsiotsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsiotsdk
-Version: 1.9.2
+Version: 1.9.3
 Summary: AWS IoT SDK based on the AWS Common Runtime
 Home-page: https://github.com/aws/aws-iot-device-sdk-python-v2
 Author: AWS SDK Common Runtime Team
 License: License :: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `awsiotsdk-1.9.2/PKG-INFO` & `awsiotsdk-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsiotsdk
-Version: 1.9.2
+Version: 1.9.3
 Summary: AWS IoT SDK based on the AWS Common Runtime
 Home-page: https://github.com/aws/aws-iot-device-sdk-python-v2
 Author: AWS SDK Common Runtime Team
 License: License :: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `awsiotsdk-1.9.2/test/test_rpc.py` & `awsiotsdk-1.9.3/test/test_rpc.py`

 * *Files identical despite different names*

### Comparing `awsiotsdk-1.9.2/test/test_mqtt.py` & `awsiotsdk-1.9.3/test/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `awsiotsdk-1.9.2/test/test_samples.py` & `awsiotsdk-1.9.3/test/test_samples.py`

 * *Files identical despite different names*

### Comparing `awsiotsdk-1.9.2/test/test_ggv2.py` & `awsiotsdk-1.9.3/test/test_ggv2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import concurrent.futures
 import threading
 from unittest import TestCase
 from unittest.mock import patch
+import io
+import contextlib
 
 from awsiot.greengrasscoreipc.client import SubscribeToTopicStreamHandler
 from awsiot.greengrasscoreipc.model import CreateLocalDeploymentResponse, SubscribeToTopicResponse, \
     SubscriptionResponseMessage, BinaryMessage
 
 TIMEOUT = 10.0 # seconds
 
@@ -79,7 +81,19 @@
         self.assertEqual("abc", resp.topic_name)
 
         sub_handler = mock_client.new_subscribe_to_topic.call_args[0][0]
         sub_handler.on_stream_event(SubscriptionResponseMessage(binary_message=BinaryMessage(message="xyz")))
 
         self.assertEqual("xyz".encode("utf-8"), subscription_fut.result(TIMEOUT).binary_message.message)
         self.assertEqual(threading.get_ident(), thread_id_fut.result(TIMEOUT))
+
+        # Verify we nicely print errors in user-provided handler methods
+        def on_stream_event(r):
+            raise ValueError("Broken!")
+
+        c.subscribe_to_topic(topic="abc", on_stream_event=on_stream_event)
+        sub_handler = mock_client.new_subscribe_to_topic.call_args[0][0]
+        f = io.StringIO()
+        with contextlib.redirect_stderr(f):
+            self.assertRaises(ValueError, lambda: sub_handler.on_stream_event(
+                SubscriptionResponseMessage(binary_message=BinaryMessage(message="xyz"))))
+        self.assertIn("ValueError: Broken!", f.getvalue())
```

### Comparing `awsiotsdk-1.9.2/README.md` & `awsiotsdk-1.9.3/README.md`

 * *Files identical despite different names*

