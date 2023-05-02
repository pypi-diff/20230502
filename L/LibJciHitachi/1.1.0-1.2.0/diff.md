# Comparing `tmp/LibJciHitachi-1.1.0.tar.gz` & `tmp/LibJciHitachi-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LibJciHitachi-1.1.0.tar", last modified: Wed Jan  4 11:53:34 2023, max compression
+gzip compressed data, was "LibJciHitachi-1.2.0.tar", last modified: Tue May  2 14:49:10 2023, max compression
```

## Comparing `LibJciHitachi-1.1.0.tar` & `LibJciHitachi-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 11:53:34.243273 LibJciHitachi-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 11:53:34.243273 LibJciHitachi-1.1.0/JciHitachi/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-04 11:53:20.000000 LibJciHitachi-1.1.0/JciHitachi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40672 2023-01-04 11:53:20.000000 LibJciHitachi-1.1.0/JciHitachi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28568 2023-01-04 11:53:20.000000 LibJciHitachi-1.1.0/JciHitachi/aws_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 11:53:34.243273 LibJciHitachi-1.1.0/JciHitachi/cert/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-01-04 11:53:20.000000 LibJciHitachi-1.1.0/JciHitachi/cert/AmazonRootCA1.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-01-04 11:53:20.000000 LibJciHitachi-1.1.0/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-01-04 11:53:20.000000 LibJciHitachi-1.1.0/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-01-04 11:53:20.000000 LibJciHitachi-1.1.0/JciHitachi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    56094 2023-01-04 11:53:20.000000 LibJciHitachi-1.1.0/JciHitachi/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-01-04 11:53:20.000000 LibJciHitachi-1.1.0/JciHitachi/mqtt_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-01-04 11:53:20.000000 LibJciHitachi-1.1.0/JciHitachi/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-01-04 11:53:20.000000 LibJciHitachi-1.1.0/JciHitachi/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-01-04 11:53:20.000000 LibJciHitachi-1.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 11:53:34.243273 LibJciHitachi-1.1.0/LibJciHitachi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-01-04 11:53:34.000000 LibJciHitachi-1.1.0/LibJciHitachi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-01-04 11:53:34.000000 LibJciHitachi-1.1.0/LibJciHitachi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 11:53:34.000000 LibJciHitachi-1.1.0/LibJciHitachi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-04 11:53:34.000000 LibJciHitachi-1.1.0/LibJciHitachi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-04 11:53:34.000000 LibJciHitachi-1.1.0/LibJciHitachi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-01-04 11:53:34.243273 LibJciHitachi-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-01-04 11:53:20.000000 LibJciHitachi-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-04 11:53:34.243273 LibJciHitachi-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-01-04 11:53:20.000000 LibJciHitachi-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:49:10.580887 LibJciHitachi-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:49:10.576887 LibJciHitachi-1.2.0/JciHitachi/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40925 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35735 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/aws_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:49:10.576887 LibJciHitachi-1.2.0/JciHitachi/cert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/cert/AmazonRootCA1.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56244 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/mqtt_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:49:10.576887 LibJciHitachi-1.2.0/LibJciHitachi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-02 14:49:10.000000 LibJciHitachi-1.2.0/LibJciHitachi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-02 14:49:10.000000 LibJciHitachi-1.2.0/LibJciHitachi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:49:10.000000 LibJciHitachi-1.2.0/LibJciHitachi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 14:49:10.000000 LibJciHitachi-1.2.0/LibJciHitachi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 14:49:10.000000 LibJciHitachi-1.2.0/LibJciHitachi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-02 14:49:10.580887 LibJciHitachi-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:49:10.580887 LibJciHitachi-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:49:10.580887 LibJciHitachi-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18884 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/tests/test_aws_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/tests/test_sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/tests/test_status.py
```

### Comparing `LibJciHitachi-1.1.0/JciHitachi/api.py` & `LibJciHitachi-1.2.0/JciHitachi/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -851,15 +851,15 @@
     def type(self) -> str:
         """Device type.
 
         Returns
         -------
         str
             Device type. 
-            If not supported, 'unknown' will be returned. (currently supports: `AC`, `DH`)
+            If not supported, 'unknown' will be returned.
         """
 
         return self.supported_device_type.get(
             self._json['DeviceType'],
             'unknown'
         )
 
@@ -884,25 +884,25 @@
     """
 
     def __init__(self, 
         email : str,
         password : str,
         device_names : Optional[Union[list[str], str]] = None,
         max_retries : int = 5,
-        device_offline_timeout : float = 45.0,
+        device_offline_timeout : float = 10.0,
         print_response : bool = False
     ) -> None:
         self.email : str = email
         self.password : str = password
         self.device_names : Optional[Union[list[str], str]] = device_names
         self.max_retries : int = max_retries
-        self.device_offline_timeout : float = device_offline_timeout
         self.print_response : bool = print_response
 
         self._mqtt : Optional[aws_connection.JciHitachiAWSMqttConnection] = None
+        self._mqtt_timeout : float = device_offline_timeout
         self._shadow_names : Union[str, list] = ["info"]
         self._device_id : int = random.randint(1000, 6999)
         self._things : dict[str, AWSThing] = {}
         self._aws_tokens : Optional[aws_connection.AWSTokens] = None
         self._aws_identity : Optional[aws_connection.AWSIdentity] = None
         self._host_identity_id : Optional[str] = None
         self._task_id : int = 0
@@ -937,20 +937,20 @@
         current_time = time.time()
         if self._aws_tokens.expiration - current_time <= 300:
             self.reauth()
 
         if self._mqtt.mqtt_events.mqtt_error_event.is_set():
             self._mqtt.mqtt_events.mqtt_error_event.clear()
             self.reauth()
-        
-        # Clear events
-        self._mqtt.mqtt_events.device_control_event.clear()
-        self._mqtt.mqtt_events.device_shadow_event.clear()
-        self._mqtt.mqtt_events.device_status_event.clear()
-        self._mqtt.mqtt_events.device_support_event.clear()
+    
+    def _get_valid_things(self, device_name : Optional[str] = None) -> tuple[str, AWSThing]:
+        for name, thing in self._things.items():
+            if (device_name and name != device_name) or thing.type == "unknown":
+                continue
+            yield name, thing
 
     def _delay(self) -> None:
         time.sleep(0.2)
 
     def login(self) -> None:
         """Login API.
 
@@ -972,14 +972,15 @@
         conn_status, conn_json = conn.get_data()
 
         if conn_status == "OK":
             for user in conn_json["results"]["FamilyMemberList"]:
                 if user["isHost"]:
                     self._host_identity_id = user["userId"]
                     break
+            assert self._host_identity_id is not None, "Host is not found in the user list"
         else:
             raise RuntimeError(f"An error occurred when listing account users: {conn_status}")
 
         conn = aws_connection.GetAllDevice(self._aws_tokens, print_response=self.print_response)
         conn_status, conn_json = conn.get_data()
 
         if conn_status == "OK":
@@ -989,14 +990,15 @@
                 self.device_names
             )
             self.device_names = list(self._things.keys())
             thing_names = [value.thing_name for value in self._things.values()]
 
             # mqtt
             def get_credential_callable():
+                self._check_before_publish()
                 conn = aws_connection.GetCredentials(
                     email=self.email,
                     password=self.password,
                     aws_tokens=self._aws_tokens,
                     print_response=self.print_response,
                 )
                 conn_status, aws_credentials = conn.get_data(self._aws_identity)
@@ -1123,45 +1125,51 @@
 
         Raises
         ------
         RuntimeError
             If an error occurs, RuntimeError will be raised.
         """
 
-        for name, thing in self._things.items():
-            if (device_name and name != device_name) or thing.type == "unknown":
-                continue
-
+        # queue tasks
+        for name, thing in self._get_valid_things(device_name):
             self._check_before_publish()
 
             if refresh_support_code:
-                self._mqtt.publish(f"{self._host_identity_id}/{thing.thing_name}/registration/request", {"Timestamp": time.time()})
-                if not self._mqtt.mqtt_events.device_support_event.wait(timeout=10.0):
-                    raise RuntimeError(f"An error occurred when refreshing {name} support code.")
-                if thing.thing_name not in self._mqtt.mqtt_events.device_support:
-                    raise RuntimeError(f"An event occurred but wasn't accompanied with data when refreshing {name} support code.")
-                
-                thing.support_code = self._mqtt.mqtt_events.device_support[thing.thing_name]
-
+                self._mqtt.publish(self._host_identity_id, thing.thing_name, "support", self._mqtt_timeout)
             if refresh_shadow:
                 self._mqtt.publish_shadow(thing.thing_name, "get", shadow_name="info")
-                if not self._mqtt.mqtt_events.device_shadow_event.wait(timeout=10.0):
-                    raise RuntimeError(f"An error occurred when refreshing {name} shadow.")
-                if thing.thing_name not in self._mqtt.mqtt_events.device_shadow:
-                    raise RuntimeError(f"An event occurred but wasn't accompanied with data when refreshing {name} shadow.")
-
-                thing.shadow = self._mqtt.mqtt_events.device_shadow[thing.thing_name]
-
-            self._mqtt.publish(f"{self._host_identity_id}/{thing.thing_name}/status/request", {"Timestamp": time.time()})
-            if not self._mqtt.mqtt_events.device_status_event.wait(timeout=10.0):
-                raise RuntimeError(f"An error occurred when refreshing {name} status code.")
-            if thing.thing_name not in self._mqtt.mqtt_events.device_status:
-                raise RuntimeError(f"An event occurred but wasn't accompanied with data when refreshing {name} status code.")
-            
-            thing.status_code = self._mqtt.mqtt_events.device_status[thing.thing_name]
+
+            self._mqtt.publish(self._host_identity_id, thing.thing_name, "status", self._mqtt_timeout)
+        
+        # execute
+        support_results, shadow_results, status_results, _ = self._mqtt.execute()
+
+        # gather results
+        for name, thing in self._get_valid_things(device_name):
+            if refresh_support_code:
+                if thing.thing_name in support_results:
+                    if thing.thing_name not in self._mqtt.mqtt_events.device_support:
+                        raise RuntimeError(f"An event occurred but wasn't accompanied with data when refreshing {name} support code.")
+                    thing.support_code = self._mqtt.mqtt_events.device_support[thing.thing_name]
+                else:
+                    raise RuntimeError(f"Timed out refreshing {name} support code. Please ensure the device is online and avoid opening the official app.")
+            if refresh_shadow:
+                if thing.thing_name in shadow_results:
+                    if thing.thing_name not in self._mqtt.mqtt_events.device_shadow:
+                        raise RuntimeError(f"An event occurred but wasn't accompanied with data when refreshing {name} shadow.")
+                    thing.shadow = self._mqtt.mqtt_events.device_shadow[thing.thing_name]
+                else:
+                    raise RuntimeError(f"Timed out refreshing {name} shadow. Please ensure the device is online and avoid opening the official app.")
+                
+            if thing.thing_name in status_results:
+                if thing.thing_name not in self._mqtt.mqtt_events.device_status:
+                    raise RuntimeError(f"An event occurred but wasn't accompanied with data when refreshing {name} status code.")
+                thing.status_code = self._mqtt.mqtt_events.device_status[thing.thing_name]
+            else:
+                raise RuntimeError(f"Timed out refreshing {name} status code. Please ensure the device is online and avoid opening the official app.")
 
     def get_status(self, device_name: Optional[str] = None, legacy: bool = False) -> dict[str, JciHitachiAWSStatus]:
         """Get device status after refreshing status.
 
         Parameters
         ----------
         device_name : str, optional
@@ -1174,17 +1182,15 @@
         Returns
         -------
         dict of JciHitachiAWSStatus.
             A dict of JciHitachiAWSStatus instances.
         """
         
         statuses = {}
-        for name, thing in self._things.items():
-            if (device_name and name != device_name) or thing.type == "unknown":
-                continue
+        for name, thing in self._get_valid_things(device_name):
             if legacy:
                 statuses[name] = thing.status_code.legacy_status
             else:
                 statuses[name] = thing.status_code
 
             # inject temp and humidity limitations from the support code
             if thing.type == "AC":
@@ -1260,38 +1266,39 @@
                         "reported": {
                             **shadow_publish_schema
                         }
                     }
                 },
                 shadow_name="info"
             )
-            if self._mqtt.mqtt_events.device_control_event.wait(timeout=10.0):
+            if self._mqtt.mqtt_events.device_control_event.wait(timeout=self._mqtt_timeout):
                 device_control = self._mqtt.mqtt_events.device_control.get(thing.thing_name)
                 if device_control["state"]["reported"][status_name] == bool(status_value):
                     self._mqtt.mqtt_events.device_control_event.clear()
                     self._delay()
                     return True
             return False
 
-        self._mqtt.publish(f"{self._host_identity_id}/{thing.thing_name}/control/request", {
+        self._mqtt.publish(
+            self._host_identity_id, thing.thing_name, "control", self._mqtt_timeout,
+            {
             "Condition": {
                 "ThingName": thing.thing_name,
                 "Index": 0,
                 "Geofencing": {
                     "Arrive": None,
                     "Leave": None,
                 },
             },
             status_name: status_value,
             "TaskID": self.task_id,
             "Timestamp": time.time(),
         })
 
-        for _ in range(self.max_retries):
-            if self._mqtt.mqtt_events.device_control_event.wait(timeout=10.0):
-                device_control = self._mqtt.mqtt_events.device_control.get(thing.thing_name)
-                if device_control.get(status_name) == status_value:
-                    thing.status_code.set_new_status(status_name, status_value)
-                    self._mqtt.mqtt_events.device_control_event.clear()
-                    return True
-            self._delay()
+        _, _, _, control_results = self._mqtt.execute()
+
+        if thing.thing_name in control_results:
+            device_control = self._mqtt.mqtt_events.device_control.get(thing.thing_name)
+            if device_control.get(status_name) == status_value:
+                thing.status_code.set_new_status(status_name, status_value)
+                return True
         return False
```

### Comparing `LibJciHitachi-1.1.0/JciHitachi/aws_connection.py` & `LibJciHitachi-1.2.0/JciHitachi/aws_connection.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
+import asyncio
 import datetime
 import json
 import logging
 import threading
 import time
 import uuid
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
+from random import random
 from typing import Callable, Optional, Union
 
 import awscrt
 import httpx
 from awsiot import iotshadow, mqtt_connection_builder
 
 from .model import JciHitachiAWSStatus, JciHitachiAWSStatusSupport
@@ -20,14 +22,15 @@
 AWS_COGNITO_ENDPOINT = f"cognito-identity.{AWS_REGION}.amazonaws.com"
 AWS_COGNITO_CLIENT_ID = "7kfnjsb66ei1qt5s5gjv6j1lp6"
 AWS_COGNITO_USERPOOL_ID = f"{AWS_REGION}_aTZeaievK"
 
 #AMAZON_ROOT_CERT = os.path.join(os.path.dirname(os.path.abspath(__file__)), './cert/AmazonRootCA1.pem')
 AWS_IOT_ENDPOINT = "iot-api.jci-hitachi-smarthome.com"
 AWS_MQTT_ENDPOINT = f"a8kcu267h96in-ats.iot.{AWS_REGION}.amazonaws.com"
+QOS = awscrt.mqtt.QoS.AT_LEAST_ONCE
 
 _LOGGER = logging.getLogger(__name__)
 
 @dataclass
 class AWSTokens:
     access_token: str
     id_token: str
@@ -43,48 +46,64 @@
 @dataclass
 class JciHitachiMqttEvents:
     device_status: dict[str, JciHitachiAWSStatus] = field(default_factory=dict)
     device_support: dict[str, JciHitachiAWSStatusSupport] = field(default_factory=dict)
     device_control: dict[str, dict] = field(default_factory=dict)
     device_shadow: dict[str, dict] = field(default_factory=dict)
     mqtt_error: str = field(default_factory=str)
-    device_status_event: threading.Event = field(default_factory=threading.Event)
-    device_support_event: threading.Event = field(default_factory=threading.Event)
-    device_control_event: threading.Event = field(default_factory=threading.Event)
-    device_shadow_event: threading.Event = field(default_factory=threading.Event)
+    device_status_event: dict[str, threading.Event] = field(default_factory=dict)
+    device_support_event: dict[str, threading.Event] = field(default_factory=dict)
+    device_control_event: dict[str, threading.Event] = field(default_factory=dict)
+    device_shadow_event: dict[str, threading.Event] = field(default_factory=dict)
     mqtt_error_event: threading.Event = field(default_factory=threading.Event)
 
+@dataclass
+class JciHitachiExecutionPools:
+    status_execution_pool: list = field(default_factory=list)
+    shadow_execution_pool: list = field(default_factory=list)
+    support_execution_pool: list = field(default_factory=list)
+    control_execution_pool: list = field(default_factory=list)
+
 
 class JciHitachiAWSHttpConnection(ABC):
     """Abstract class for AWS http connections."""
 
     @abstractmethod
     def __init__(self, print_response: bool):
         self._print_response = print_response
 
     @abstractmethod
+    def _generate_headers(self):
+        ...
+
+    @abstractmethod
     def _handle_response(self, response: httpx.Response):
         ...
 
     @abstractmethod
     def _send(self):
         ...
     
     def get_data(self):
         raise NotImplementedError
 
     def maybe_print_http_response(self, response: httpx.Response) -> None:
         if not self._print_response:
             return
         
+        try:
+            text = json.dumps(response.json(), indent=True)
+        except json.JSONDecodeError:
+            text = response.text
+        
         print('===================================================')
         print(self.__class__.__name__, 'Response:')
         print('headers:', response.headers)
         print('status_code:', response.status_code)
-        print('text:', json.dumps(response.json(), indent=True))
+        print('text:', text)
         print('===================================================')
 
 
 class JciHitachiAWSCognitoConnection(JciHitachiAWSHttpConnection):
     """Connecting to Jci-Hitachi AWS Cognito API.
 
     Parameters
@@ -120,21 +139,21 @@
             self._aws_tokens = aws_tokens
         else:
             conn_status, self._aws_tokens = self.login()
             if conn_status != "OK":
                 raise RuntimeError(f"An error occurred when signing into AWS Cognito Service: {conn_status}")
     
     def _generate_headers(self, target: str) -> dict[str, str]:
-        normal_headers = {
+        headers = {
             "X-Amz-Target": target,
             "User-Agent": "Dalvik/2.1.0",
             "content-type": "application/x-amz-json-1.1",
             "Accept" : "application/json",
         }
-        return normal_headers
+        return headers
 
     def _handle_response(self, response: httpx.Response) -> tuple(str, dict):
         response_json = response.json()
         
         if response.status_code == httpx.codes.ok:    
             return "OK", response_json
         else:
@@ -192,15 +211,15 @@
                 },
                 "ClientId": AWS_COGNITO_CLIENT_ID,
             }
 
         login_headers = self._generate_headers("AWSCognitoIdentityProviderService.InitiateAuth")
 
         login_req = httpx.post(
-            f"https://{AWS_COGNITO_IDP_ENDPOINT}", 
+            f"https://{AWS_COGNITO_IDP_ENDPOINT}/",
             json=login_json_data,
             headers=login_headers,
             proxies=self._proxies,
         )
 
         self.maybe_print_http_response(login_req)
 
@@ -322,48 +341,49 @@
         AWS tokens.
     proxy : str, optional
         Proxy setting. Format:"IP:port", by default None. 
     print_response : bool, optional
         If set, all responses of httpx will be printed, by default False.
     """
 
-    def __init__(self, aws_tokens, proxy=None, print_response=False):
+    def __init__(self, aws_tokens: AWSTokens, proxy: Optional[str] = None, print_response: bool = False):
         super().__init__(print_response)
         self._aws_tokens = aws_tokens
         self._proxies = {'http': proxy, 'https': proxy} if proxy else None
     
-    def _generate_normal_headers(self) -> dict[str, str]:
-        normal_headers = {
+    def _generate_headers(self, need_access_token: bool) -> dict[str, str]:
+        headers = {
             "authorization": f"Bearer {self._aws_tokens.id_token}",
-            "accesstoken": f"Bearer {self._aws_tokens.access_token}",
             "User-Agent": "Dalvik/2.1.0",
             "content-type" : "application/json",
             "Accept" : "application/json",
         }
-        return normal_headers
+        if need_access_token:
+            headers["accesstoken"] = f"Bearer {self._aws_tokens.access_token}"
+        return headers
 
-    def _handle_response(self, response) -> tuple[int, str, dict]:
+    def _handle_response(self, response: httpx.Response) -> tuple[int, str, dict]:
         response_json = response.json()
         if response.status_code == httpx.codes.ok:
             code = response_json["status"]["code"]
             if code == 0:
                 return code, "OK", response_json
             elif code == 6:
                 return code, "Invalid email or password", response_json
             elif code == 12:
                 return code, "Invalid session token", response_json
             else:
                 return code, "Unknown error", response_json
         else:
             return response.status_code, f"HTTP exception {response.status_code}", response_json
 
-    def _send(self, api_name: str, json: Optional[dict] = None) -> tuple[str, dict]:
+    def _send(self, api_name: str, json: Optional[dict] = None, need_access_token: bool = True) -> tuple[str, dict]:
         req = httpx.post(
             f"https://{AWS_IOT_ENDPOINT}{api_name}",
-            headers=self._generate_normal_headers(),
+            headers=self._generate_headers(need_access_token),
             json=json,
             proxies=self._proxies,
         )
         
         self.maybe_print_http_response(req)
 
         code, message, response_json = self._handle_response(req)
@@ -380,15 +400,15 @@
         AWS tokens.
     """
 
     def __init__(self, aws_tokens: AWSTokens, **kwargs):
         super().__init__(aws_tokens, **kwargs)
 
     def get_data(self) -> tuple[str, dict]:
-        return self._send("/GetAllDevice")
+        return self._send("/GetAllDevice", need_access_token=False)
 
 
 class GetAllGroup(JciHitachiAWSIoTConnection):
     """API internal endpoint.
     
     Parameters
     ----------
@@ -412,15 +432,15 @@
         AWS tokens.
     """
 
     def __init__(self, aws_tokens: AWSTokens, **kwargs):
         super().__init__(aws_tokens, **kwargs)
 
     def get_data(self) -> tuple[str, dict]:
-        return self._send("/GetAllRegion")
+        return self._send("/GetAllRegion", need_access_token=False)
 
 
 class GetAvailableAggregationMonthlyData(JciHitachiAWSIoTConnection):
     """API internal endpoint.
     
     Parameters
     ----------
@@ -491,14 +511,16 @@
         self._get_credentials_callable = get_credentials_callable
         self._print_response = print_response
         
         self._mqttc = None
         self._shadow_mqttc = None
         self._client_tokens = {}
         self._mqtt_events = JciHitachiMqttEvents()
+        self._execution_lock = threading.Lock()
+        self._execution_pools = JciHitachiExecutionPools()
 
     def __del__(self):
         self.disconnect()
 
     @property
     def mqtt_events(self) -> JciHitachiMqttEvents:
         """MQTT events.
@@ -525,37 +547,37 @@
 
         split_topic = topic.split('/')
 
         if len(split_topic) >= 4 and split_topic[3] != "shadow":
             thing_name = split_topic[1]
             if split_topic[2] == "status" and split_topic[3] == "response":
                 self._mqtt_events.device_status[thing_name] = JciHitachiAWSStatus(payload)
-                self._mqtt_events.device_status_event.set()
+                self._mqtt_events.device_status_event[thing_name].set()
             elif split_topic[2] == "registration" and split_topic[3] == "response":
                 self._mqtt_events.device_support[thing_name] = JciHitachiAWSStatusSupport(payload)
-                self._mqtt_events.device_support_event.set()
+                self._mqtt_events.device_support_event[thing_name].set()
             elif split_topic[2] == "control" and split_topic[3] == "response":
                 self._mqtt_events.device_control[thing_name] = payload
-                self._mqtt_events.device_control_event.set()
+                self._mqtt_events.device_control_event[thing_name].set()
 
     def _on_update_named_shadow_accepted(self, response):
         try:
             thing_name = self._client_tokens.pop(response.client_token)
         except:
             _LOGGER.error(f"An unknown shadow response is received. Client token: {response.client_token}")
             return
         
         if self._print_response:
             print(f"An `update` shadow response is received: {response.state.reported}")
 
         if response.state:
             if response.state.reported:
                 self._mqtt_events.device_control[thing_name] = response.state.reported
-                self._mqtt_events.device_control_event.set()
-    
+                self._mqtt_events.device_control_event[thing_name].set()
+
     def _on_update_named_shadow_rejected(self, error):
         _LOGGER.error(f"A shadow request {error.client_token} was rejected by the API: {error.code} {error.message}")
 
     def _on_get_named_shadow_accepted(self, response):
         try:
             thing_name = self._client_tokens.pop(response.client_token)
         except:
@@ -564,22 +586,52 @@
         
         if self._print_response:
             print(f"A `get` shadow response is received: {response.state.reported}")
 
         if response.state:
             if response.state.reported:
                 self._mqtt_events.device_shadow[thing_name] = response.state.reported
-                self._mqtt_events.device_shadow_event.set()
-    
+                self._mqtt_events.device_shadow_event[thing_name].set()
+
     def _on_get_named_shadow_rejected(self, error):
         _LOGGER.error(f"A shadow request {error.client_token} was rejected by the API: {error.code} {error.message}")
 
     def _on_message(self, topic, payload, dup, qos, retain, **kwargs):
         return
 
+    def _on_connection_interrupted(self, connection, error, **kwargs):
+        _LOGGER.error("MQTT connection was interrupted with exception {error}.")
+        self._mqtt_events.mqtt_error = error.__class__.__name__
+        self._mqtt_events.mqtt_error_event.set()
+
+    def _on_connection_resumed(self, connection, return_code, session_present, **kwargs):
+        if session_present:
+            _LOGGER.info("MQTT connection was resumed.")
+        else:
+            _LOGGER.info("MQTT connection was resumed, but the previous session was lost. Resubscribing...")
+            resubscribe_future, packet_id = connection.resubscribe_existing_topics()
+
+            def on_resubscribe_complete(resubscribe_future):
+                try:
+                    resubscribe_results = resubscribe_future.result()
+                    assert(resubscribe_results['packet_id'] == packet_id)
+                    for (topic, qos) in resubscribe_results['topics']:
+                        assert(qos is not None)
+                except Exception as e:
+                    _LOGGER.error("Resubscribe failure:", e)
+
+            resubscribe_future.add_done_callback(on_resubscribe_complete)
+            _LOGGER.info("Resubscribed successfully.")
+        return
+    
+    async def _wrap_async(self, identifier: str, fn: Callable, timeout: float) -> str:
+        await asyncio.sleep(random() / 2)  # randomly wait 0~0.5 seconds to prevent messages flooding to the broker.
+        await asyncio.wait_for(fn(), timeout)
+        return identifier
+
     def disconnect(self) -> None:
         """Disconnect from the MQTT broker.
         """
 
         if self._mqttc is not None:
             self._mqttc.disconnect()
 
@@ -591,15 +643,17 @@
         host_resolver = awscrt.io.DefaultHostResolver(event_loop_group)
         client_bootstrap = awscrt.io.ClientBootstrap(event_loop_group, host_resolver)
         self._mqttc = mqtt_connection_builder.websockets_with_default_aws_signing(
             AWS_REGION,
             cred_provider,
             client_bootstrap=client_bootstrap,
             endpoint=AWS_MQTT_ENDPOINT,
-            client_id=str(uuid.uuid4())
+            client_id=str(uuid.uuid4()),
+            on_connection_interrupted=self._on_connection_interrupted,
+            on_connection_resumed=self._on_connection_resumed,
         )
         self._mqttc.on_message(self._on_message)
         self._shadow_mqttc = iotshadow.IotShadowClient(self._mqttc)
 
     def connect(
         self, 
         host_identity_id: str,
@@ -630,161 +684,241 @@
         except Exception as e:
             self._mqtt_events.mqtt_error = e.__class__.__name__
             self._mqtt_events.mqtt_error_event.set()
             _LOGGER.error('MQTT connection failed with exception {}'.format(e))
             return False
 
         try:
-            subscribe_future, _ = self._mqttc.subscribe(f"{host_identity_id}/#", awscrt.mqtt.QoS.AT_LEAST_ONCE, callback=self._on_publish)
+            subscribe_future, _ = self._mqttc.subscribe(f"{host_identity_id}/#", QOS, callback=self._on_publish)
             subscribe_future.result()
             
             if thing_names is not None and shadow_names is not None:
                 shadow_names = [shadow_names] if isinstance(shadow_names, str) else shadow_names
                 thing_names = [thing_names] if isinstance(thing_names, str) else thing_names
                 
                 for shadow_name in shadow_names:
                     for thing_name in thing_names:
                         update_accepted_subscribed_future, _ = self._shadow_mqttc.subscribe_to_update_named_shadow_accepted(
                             request=iotshadow.UpdateNamedShadowSubscriptionRequest(shadow_name=shadow_name, thing_name=thing_name),
-                            qos=awscrt.mqtt.QoS.AT_LEAST_ONCE,
+                            qos=QOS,
                             callback=self._on_update_named_shadow_accepted)
 
                         update_rejected_subscribed_future, _ = self._shadow_mqttc.subscribe_to_update_named_shadow_rejected(
                             request=iotshadow.UpdateNamedShadowSubscriptionRequest(shadow_name=shadow_name, thing_name=thing_name),
-                            qos=awscrt.mqtt.QoS.AT_LEAST_ONCE,
+                            qos=QOS,
                             callback=self._on_update_named_shadow_rejected)
 
                         # Wait for subscriptions to succeed
                         update_accepted_subscribed_future.result()
                         update_rejected_subscribed_future.result()
 
                         get_accepted_subscribed_future, _ = self._shadow_mqttc.subscribe_to_get_named_shadow_accepted(
                             request=iotshadow.GetNamedShadowSubscriptionRequest(shadow_name=shadow_name, thing_name=thing_name),
-                            qos=awscrt.mqtt.QoS.AT_LEAST_ONCE,
+                            qos=QOS,
                             callback=self._on_get_named_shadow_accepted)
 
                         get_rejected_subscribed_future, _ = self._shadow_mqttc.subscribe_to_get_named_shadow_rejected(
                             request=iotshadow.GetNamedShadowSubscriptionRequest(shadow_name=shadow_name, thing_name=thing_name),
-                            qos=awscrt.mqtt.QoS.AT_LEAST_ONCE,
+                            qos=QOS,
                             callback=self._on_get_named_shadow_rejected)
 
                         # Wait for subscriptions to succeed
                         get_accepted_subscribed_future.result()
                         get_rejected_subscribed_future.result()
         
         except Exception as e:
             self._mqtt_events.mqtt_error = e.__class__.__name__
             self._mqtt_events.mqtt_error_event.set()
             self.disconnect()
             _LOGGER.error('MQTT subscription failed with exception {}'.format(e))
             return False
         return True
 
-    def publish(self, topic: str, payload: dict) -> None:
-        """Publish message.
+    def publish(self, host_identity_id: str, thing_name: str, publish_type: str, timeout: float = 10.0, payload: Optional[dict] = None) -> None:
+        """Put messages to be published in the execution pool. execute() should be called to start async publish.
         
         Parameters
         ----------
-        topic : str
-            Topic to publish.
-        payload : dict
-            Payload to publish.
+        host_identity_id : str
+            Host identity id.
+        thing_name : str
+            Thing name.
+        publish_type: str
+            Publish type. There are three types available: `support`, `status`, and `control`.
+        timeout: float, optional
+            Timeout for messages published, by default 10.0.
+        payload : dict, optional
+            Payload to publish, by default None.
         """
+        
+        default_payload = {"Timestamp": time.time()}
+        
+        if publish_type == "support":
+            support_topic = f"{host_identity_id}/{thing_name}/registration/request"
+            if thing_name in self._mqtt_events.device_support_event:
+                self._mqtt_events.device_support_event[thing_name].clear()
+            else:
+                self._mqtt_events.device_support_event[thing_name] = threading.Event()
+                
+            async def wrapper():
+                publish_future, _ = self._mqttc.publish(support_topic, json.dumps(default_payload), QOS)
+                publish_future.result()
+                self._mqtt_events.device_support_event[thing_name].wait()
+            
+            self._execution_pools.support_execution_pool.append(self._wrap_async(thing_name, wrapper, timeout))
+        elif publish_type == "status":
+            status_topic = f"{host_identity_id}/{thing_name}/status/request"
+            if thing_name in self._mqtt_events.device_status_event:
+                self._mqtt_events.device_status_event[thing_name].clear()
+            else:
+                self._mqtt_events.device_status_event[thing_name] = threading.Event()
+            async def wrapper():
+                publish_future, _ = self._mqttc.publish(status_topic, json.dumps(default_payload), QOS)
+                publish_future.result()
+                self._mqtt_events.device_status_event[thing_name].wait()
+            self._execution_pools.status_execution_pool.append(self._wrap_async(thing_name, wrapper, timeout))
+        elif publish_type == "control":
+            control_topic = f"{host_identity_id}/{thing_name}/control/request"
+            if thing_name in self._mqtt_events.device_control_event:
+                self._mqtt_events.device_control_event[thing_name].clear()
+            else:
+                self._mqtt_events.device_control_event[thing_name] = threading.Event()
+            async def wrapper():
+                publish_future, _ = self._mqttc.publish(control_topic, json.dumps(payload), QOS)
+                publish_future.result()
+                self._mqtt_events.device_control_event[thing_name].wait()
+            self._execution_pools.control_execution_pool.append(self._wrap_async(thing_name, wrapper, timeout))
 
-        try:
-            publish_future, _ = self._mqttc.publish(topic, json.dumps(payload), awscrt.mqtt.QoS.AT_LEAST_ONCE)
-            publish_future.result()
-        except Exception as e:
-            self._mqtt_events.mqtt_error = e.__class__.__name__
-            self._mqtt_events.mqtt_error_event.set()
-            _LOGGER.error('Publish failed with exception: {}'.format(e))
+        else:
+            raise ValueError(f"Invalid publish_type: {publish_type}")
 
     def publish_shadow(
         self,
         thing_name: str,
         command_name: str,
         payload: dict = {},
-        shadow_name: Optional[str] = None
+        shadow_name: Optional[str] = None,
+        timeout: float = 10.0,
     ) -> None:
         """Publish message to IoT Shadow Service.
         
         Parameters
         ----------
         thing_name : str
             Thing name.
         command_name : str
             Command name, which can be `get` or `update`.
         payload : dict, optional
             Payload to publish, by default {}.
         shadow_name : str, optional
             Shadow name, by default None.
+        timeout: float, optional
+            Timeout for messages published, by default 10.0.
         """
 
         if command_name not in ["get", "update"]: # we don't subscribe delete
             raise ValueError("command_name must be one of `get` or `update`.")
 
         # The length of client token can't exceed 64 bytes, so we only use gateway mac address as the token.
         client_token = thing_name.split("_")[1] 
         self._client_tokens.update({client_token: thing_name})
+        if thing_name in self._mqtt_events.device_shadow_event:
+            self._mqtt_events.device_shadow_event[thing_name].clear()
+        else:
+            self._mqtt_events.device_shadow_event[thing_name] = threading.Event()
+        
 
-        if shadow_name is None:
-            if command_name == "get":
-                publish_future = self._shadow_mqttc.publish_get_shadow(
-                    iotshadow.GetShadowRequest(
-                        client_token=client_token,
-                        thing_name=thing_name
-                    ),
-                    qos=awscrt.mqtt.QoS.AT_LEAST_ONCE
-                )
-            elif command_name == "update":
-                publish_future = self._shadow_mqttc.publish_update_shadow(
-                    iotshadow.UpdateShadowRequest(
-                        client_token=client_token,
-                        state=iotshadow.ShadowState(reported=payload),
-                        thing_name=thing_name
-                    ),
-                    qos=awscrt.mqtt.QoS.AT_LEAST_ONCE
-                )
-            elif command_name == "delete":
-                publish_future = self._shadow_mqttc.publish_delete_shadow(
-                    iotshadow.DeleteShadowRequest(
-                        client_token=client_token,
-                        thing_name=thing_name
-                    ),
-                    qos=awscrt.mqtt.QoS.AT_LEAST_ONCE
-                )
+        async def wrapper():
+            if shadow_name is None:
+                if command_name == "get":
+                    publish_future = self._shadow_mqttc.publish_get_shadow(
+                        iotshadow.GetShadowRequest(
+                            client_token=client_token,
+                            thing_name=thing_name
+                        ),
+                        qos=QOS
+                    )
+                elif command_name == "update":
+                    publish_future = self._shadow_mqttc.publish_update_shadow(
+                        iotshadow.UpdateShadowRequest(
+                            client_token=client_token,
+                            state=iotshadow.ShadowState(reported=payload),
+                            thing_name=thing_name
+                        ),
+                        qos=QOS
+                    )
+                elif command_name == "delete":
+                    publish_future = self._shadow_mqttc.publish_delete_shadow(
+                        iotshadow.DeleteShadowRequest(
+                            client_token=client_token,
+                            thing_name=thing_name
+                        ),
+                        qos=QOS
+                    )
 
-        else:
-            if command_name == "get":
-                publish_future = self._shadow_mqttc.publish_get_named_shadow(
-                    iotshadow.GetNamedShadowRequest(
-                        client_token=client_token,
-                        shadow_name=shadow_name,
-                        thing_name=thing_name
-                    ),
-                    qos=awscrt.mqtt.QoS.AT_LEAST_ONCE
-                )
-            elif command_name == "update":
-                publish_future = self._shadow_mqttc.publish_update_named_shadow(
-                    iotshadow.UpdateNamedShadowRequest(
-                        client_token=client_token,
-                        shadow_name=shadow_name,
-                        state=iotshadow.ShadowState(reported=payload),
-                        thing_name=thing_name
-                    ),
-                    qos=awscrt.mqtt.QoS.AT_LEAST_ONCE
-                )
-            elif command_name == "delete":
-                publish_future = self._shadow_mqttc.publish_delete_named_shadow(
-                    iotshadow.DeleteNamedShadowRequest(
-                        client_token=client_token,
-                        shadow_name=shadow_name, 
-                        thing_name=thing_name
-                    ),
-                    qos=awscrt.mqtt.QoS.AT_LEAST_ONCE
-                )
-        try:
+            else:
+                if command_name == "get":
+                    publish_future = self._shadow_mqttc.publish_get_named_shadow(
+                        iotshadow.GetNamedShadowRequest(
+                            client_token=client_token,
+                            shadow_name=shadow_name,
+                            thing_name=thing_name
+                        ),
+                        qos=QOS
+                    )
+                elif command_name == "update":
+                    publish_future = self._shadow_mqttc.publish_update_named_shadow(
+                        iotshadow.UpdateNamedShadowRequest(
+                            client_token=client_token,
+                            shadow_name=shadow_name,
+                            state=iotshadow.ShadowState(reported=payload),
+                            thing_name=thing_name
+                        ),
+                        qos=QOS
+                    )
+                elif command_name == "delete":
+                    publish_future = self._shadow_mqttc.publish_delete_named_shadow(
+                        iotshadow.DeleteNamedShadowRequest(
+                            client_token=client_token,
+                            shadow_name=shadow_name, 
+                            thing_name=thing_name
+                        ),
+                        qos=QOS
+                    )
             publish_future.result()
-        except Exception as e:
-            self._mqtt_events.mqtt_error = e.__class__.__name__
-            self._mqtt_events.mqtt_error_event.set()
-            _LOGGER.error('Publish failed with exception: {}'.format(e))
+            self._mqtt_events.device_shadow_event[thing_name].wait()
+        self._execution_pools.shadow_execution_pool.append(self._wrap_async(thing_name, wrapper, timeout))
+    
+    def execute(self) -> list[list[Union[str, BaseException]], list[Union[str, BaseException]], list[Union[str, BaseException]], list[Union[str, BaseException]]]:
+        """Execute publish commands in the execution pools.
+        
+        Returns
+        -------
+        list
+            Execution results of support, shadow, status, control, respectively.
+            Each result is a list containing thing names if the execution was successful or BaseException(s) if an error occurred during execution.
+        """
+
+        async def runner():
+            a, b, c, d = None, None, None, None
+            try:
+                self._execution_lock.acquire()
+                if len(self._execution_pools.support_execution_pool) != 0:
+                    a = await asyncio.gather(*self._execution_pools.support_execution_pool, return_exceptions=True)
+                    self._execution_pools.support_execution_pool.clear()
+                if len(self._execution_pools.shadow_execution_pool) != 0:
+                    b = await asyncio.gather(*self._execution_pools.shadow_execution_pool, return_exceptions=True)
+                    self._execution_pools.shadow_execution_pool.clear()
+                if len(self._execution_pools.status_execution_pool) != 0:
+                    c = await asyncio.gather(*self._execution_pools.status_execution_pool, return_exceptions=True)
+                    self._execution_pools.status_execution_pool.clear()
+                if len(self._execution_pools.control_execution_pool) != 0:
+                    d = await asyncio.gather(*self._execution_pools.control_execution_pool, return_exceptions=True)
+                    self._execution_pools.control_execution_pool.clear()
+            finally:
+                self._execution_lock.release()
+            return a, b, c, d
+
+        results = asyncio.run(runner())
+        
+        return results
+
```

### Comparing `LibJciHitachi-1.1.0/JciHitachi/cert/AmazonRootCA1.pem` & `LibJciHitachi-1.2.0/JciHitachi/cert/AmazonRootCA1.pem`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.1.0/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem` & `LibJciHitachi-1.2.0/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.1.0/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem` & `LibJciHitachi-1.2.0/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.1.0/JciHitachi/connection.py` & `LibJciHitachi-1.2.0/JciHitachi/connection.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.1.0/JciHitachi/model.py` & `LibJciHitachi-1.2.0/JciHitachi/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from functools import lru_cache
+
 class JciHitachiStatus:  # pragma: no cover
     idx = {}
 
     def __init__(self, status, default) -> None:
         self._status = status
         self._default = default
 
@@ -49,15 +51,15 @@
     }
 
     def __init__(self, status, default=-1):
         super().__init__(status, default)
         
     @property
     def power(self):
-        """Power. Controlable.
+        """Power. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "off", "on", "unknown").
         """
 
@@ -69,15 +71,15 @@
         elif v == 1:
             return "on"
         else:
             return "unknown"
 
     @property
     def mode(self):
-        """Mode. Controlable.
+        """Mode. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "cool", "dry", "fan", "auto", "heat", "unknown").
         """
 
@@ -95,15 +97,15 @@
         elif v == 4:
             return "heat"
         else:
             return "unknown"
 
     @property
     def air_speed(self):
-        """Air speed. Controlable.
+        """Air speed. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "auto", "silent", "low", "moderate", "high", "unknown").
         """
 
@@ -121,15 +123,15 @@
         elif v == 4:
             return "high"
         else:
             return "unknown"
 
     @property
     def target_temp(self):
-        """Target temperature. Controlable.
+        """Target temperature. Controllable.
 
         Returns
         -------
         int
             Celsius temperature.
         """
 
@@ -171,28 +173,28 @@
             Celsius temperature.
         """
 
         return 16
 
     @property
     def sleep_timer(self):
-        """Sleep timer. Controlable.
+        """Sleep timer. Controllable.
         
         Returns
         -------
         int
             Sleep timer (hours).
         """
 
         v = self._status.get(self.idx['sleep_timer'], self._default)
         return v
     
     @property
     def vertical_wind_swingable(self):
-        """Vertical wind swingable. Controlable.
+        """Vertical wind swingable. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "disabled", "enabled", "unknown").
         """
         
@@ -204,28 +206,28 @@
         elif v == 1:
             return "enabled"
         else:
             return "unknown"
 
     @property
     def vertical_wind_direction(self):
-        """Vertical wind direction. Controlable.
+        """Vertical wind direction. Controllable.
 
         Returns
         -------
         int
             Value between 0 to 15.
         """
 
         v = self._status.get(self.idx['vertical_wind_direction'], self._default)
         return v
 
     @property
     def horizontal_wind_direction(self):
-        """Horizontal wind direction. Controlable.
+        """Horizontal wind direction. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "auto", "leftmost", "middleleft", "central", "middleright", "rightmost", "unknown").
         """
 
@@ -248,15 +250,15 @@
         elif v == 5:
             return "rightmost"
         else:
             return "unknown"
 
     @property
     def mold_prev(self):
-        """Mold prevention. Controlable.
+        """Mold prevention. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "disabled", "enabled", "unknown").
         """
 
@@ -268,15 +270,15 @@
         elif v == 1:
             return "enabled"
         else:
             return "unknown"
     
     @property
     def fast_op(self):
-        """Fast operation. Controlable.
+        """Fast operation. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "disabled", "enabled", "unknown").
         """
 
@@ -288,15 +290,15 @@
         elif v == 1:
             return "enabled"
         else:
             return "unknown"
     
     @property
     def energy_save(self):
-        """Energy saving. Controlable.
+        """Energy saving. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "disabled", "enabled", "unknown").
         """
 
@@ -308,15 +310,15 @@
         elif v == 1:
             return "enabled"
         else:
             return "unknown"
 
     @property
     def sound_prompt(self):
-        """Sound prompt. Controlable.
+        """Sound prompt. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "enabled", "disabled", "unknown").
         """
 
@@ -356,15 +358,15 @@
         v = self._status.get(self.idx['power_kwh'], self._default)
         if v == -1:
             return v
         return v / 10.0
 
     @property
     def freeze_clean(self):
-        """Freeze clean. Controlable.
+        """Freeze clean. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "off", "on", "unknown").
         """
 
@@ -414,15 +416,15 @@
     }
 
     def __init__(self, status, default=-1):
         super().__init__(status, default)
     
     @property
     def power(self):
-        """Power. Controlable.
+        """Power. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "off", "on", "unknown").
         """
 
@@ -434,15 +436,15 @@
         elif v == 1:
             return "on"
         else:
             return "unknown"
     
     @property
     def mode(self):
-        """Mode. Controlable.
+        """Mode. Controllable.
 
         Returns
         -------
         str
             One of (
             "unsupported", "auto", "custom", "continuous", "clothes_dry",
             "air_purify", "mold_prev", "low_humidity", "eco_comfort", "unknown"
@@ -469,15 +471,15 @@
         elif v == 9:
             return "eco_comfort"
         else:
             return "unknown"
 
     @property
     def target_humidity(self):
-        """Target humidity. Controlable.
+        """Target humidity. Controllable.
 
         Returns
         -------
         int
             Relative humidity.
         """
 
@@ -519,15 +521,15 @@
             Relative humidity.
         """
 
         return 40
 
     @property
     def wind_swingable(self):
-        """Wind swingable. Controlable.
+        """Wind swingable. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "off", "on", "unknown").
         """
 
@@ -559,15 +561,15 @@
         elif v == 1:
             return "on"  # activated
         else:
             return "unknown"
     
     @property
     def clean_filter_notify(self):
-        """Clean filter notify control. Controlable.
+        """Clean filter notify control. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "disabled", "enabled", "unknown").
         """
 
@@ -590,15 +592,15 @@
         str
             Not implemented.
         """
         return "unsupported"
 
     @property
     def air_speed(self):
-        """Air speed. Controlable.
+        """Air speed. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "auto", "silent", "low", "moderate", "high", "unknown").
         """
 
@@ -636,15 +638,15 @@
         elif v == 1:
             return "on"
         else:
             return "unknown"
 
     @property
     def sound_control(self):
-        """Sound control. Controlable.
+        """Sound control. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "silent", "button", "button+waterfull", "unknown").
         """
 
@@ -671,15 +673,15 @@
         """
 
         v = self._status.get(self.idx['error_code'], self._default)
         return v
 
     @property
     def mold_prev(self):
-        """Mold prevention. Controlable.
+        """Mold prevention. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "off", "on", "unknown").
         """
 
@@ -741,15 +743,15 @@
         """
 
         v = self._status.get(self.idx['pm25_value'], self._default)
         return v
     
     @property
     def display_brightness(self):
-        """Display brightness. Controlable.
+        """Display brightness. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "bright", "dark", "off", "all_off" "unknown").
         """
         v = self._status.get(self.idx['display_brightness'], self._default)
@@ -952,60 +954,60 @@
     }
 
     def __init__(self, status, default=0):
         super().__init__(status, default)
 
     @property
     def power(self):
-        """Power. Controlable.
+        """Power. Controllable.
 
         Returns
         -------
         (bool, int, int)
             (is_support, off, on).
         """
 
         v = self._status.get(self.idx['power'], self._default)
         supports = self._functional_v(v)
 
         return (v != 0, *supports)
 
     @property
     def mode(self):
-        """Mode. Controlable.
+        """Mode. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, (cool, dry, fan, auto, heat, 0...).
         """
 
         v = self._status.get(self.idx['mode'], self._default)
         supports = self._functional_v(v)
 
         return (v != 0, *supports)
 
     @property
     def air_speed(self):
-        """Air speed. Controlable.
+        """Air speed. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, ("auto", "silent", "low", "moderate", "high", 0...).
         """
 
         v = self._status.get(self.idx['air_speed'], self._default)
         supports = self._functional_v(v)
 
         return (v != 0, *supports)
 
     @property
     def target_temp(self):
-        """Target temperature. Controlable.
+        """Target temperature. Controllable.
 
         Returns
         -------
         (bool, int, int)
             (is_support, minimum, maximum)
         """
 
@@ -1027,60 +1029,60 @@
         v = self._status.get(self.idx['indoor_temp'], self._default)
         supports = self._dual_v(v)
 
         return (v != 0, *supports)
 
     @property
     def sleep_timer(self):
-        """Sleep timer. Controlable.
+        """Sleep timer. Controllable.
         
         Returns
         -------
         (bool, int)
             (is_support, maximum).
         """
 
         v = self._status.get(self.idx['sleep_timer'], self._default)
         support = self._uni_v(v)
 
         return (v != 0, support)
     
     @property
     def vertical_wind_swingable(self):
-        """Vertical wind swingable. Controlable.
+        """Vertical wind swingable. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, ("enabled", "disabled", 0...).
         """
         
         v = self._status.get(self.idx['vertical_wind_swingable'], self._default)
         supports = self._functional_v(v)
 
         return (v != 0, *supports)
 
     @property
     def vertical_wind_direction(self):
-        """Vertical wind direction. Controlable.
+        """Vertical wind direction. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, ("auto", "level1", "level2", "level3", "level4", "level5", "level6", "level7", 0...).
         """
 
         v = self._status.get(self.idx['vertical_wind_direction'], self._default)
         supports = self._functional_v(v)
 
         return (v != 0, *supports)
 
     @property
     def horizontal_wind_direction(self):
-        """Horizontal wind direction. Controlable.
+        """Horizontal wind direction. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, ("auto", "leftmost", "middleleft", "central", "middleright", "rightmost", 0...).
         """
 
@@ -1088,60 +1090,60 @@
         if v > 0: v = 6-v
 
         supports = self._functional_v(v)
         return (v != 0, *supports)
 
     @property
     def mold_prev(self):
-        """Mold prevention. Controlable.
+        """Mold prevention. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, ("enabled", "disabled", 0...).
         """
 
         v = self._status.get(self.idx['mold_prev'], self._default)
         supports = self._functional_v(v)
 
         return (v != 0, *supports)
     
     @property
     def fast_op(self):
-        """Fast operation. Controlable.
+        """Fast operation. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, ("disabled", "enabled", 0...).
         """
 
         v = self._status.get(self.idx['fast_op'], self._default)
         supports = self._functional_v(v)
 
         return (v != 0, *supports)
     
     @property
     def energy_save(self):
-        """Energy saving. Controlable.
+        """Energy saving. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, ("enabled", "disabled", 0...).
         """
 
         v = self._status.get(self.idx['energy_save'], self._default)
         supports = self._functional_v(v)
 
         return (v != 0, *supports)
 
     @property
     def sound_prompt(self):
-        """Sound prompt. Controlable.
+        """Sound prompt. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, ("enabled", "disabled", 0...).
         """
 
@@ -1243,45 +1245,45 @@
     }
 
     def __init__(self, status, default=0):
         super().__init__(status, default)
     
     @property
     def power(self):
-        """Power. Controlable.
+        """Power. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             (is_support, off, on).
         """
 
         v = self._status.get(self.idx['power'], self._default)
         supports = self._functional_v(v)
 
         return (v != 0, *supports)
     
     @property
     def mode(self):
-        """Mode. Controlable.
+        """Mode. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, (auto, custom, continuous, clothes_dry, air_purify, mold_prev, air_supply, human_comfort, low_humidity, eco_comfort, 0...). 
         """
 
         v = self._status.get(self.idx['mode'], self._default)
         supports = self._functional_v(v)
 
         return (v != 0, *supports)
 
     @property
     def target_humidity(self):
-        """Target humidity. Controlable.
+        """Target humidity. Controllable.
 
         Returns
         -------
         (bool, int, int)
             (is_support, minimum, maximum)
         """
 
@@ -1303,15 +1305,15 @@
         v = self._status.get(self.idx['indoor_humidity'], self._default)
         supports = self._dual_v(v)
 
         return (v != 0, *supports)
 
     @property
     def wind_swingable(self):
-        """Wind swingable. Controlable.
+        """Wind swingable. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, ("off", "on", 0...).
         """
         
@@ -1334,15 +1336,15 @@
         v = self._status.get(self.idx['water_full_warning'], self._default)
         supports = self._functional_v(v)
 
         return (v != 0, *supports)
     
     @property
     def clean_filter_notify(self):
-        """Clean filter notify control. Controlable.
+        """Clean filter notify control. Controllable.
 
         Returns
         -------
         str
             One of ("unsupported", "disabled", "enabled", "unknown").
         """
 
@@ -1361,15 +1363,15 @@
             Not implemented.
         """
         
         return "unsupported"
 
     @property
     def air_speed(self):
-        """Air speed. Controlable.
+        """Air speed. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, ("auto", "silent", "low", "moderate", "high", 0...).
         """
 
@@ -1391,15 +1393,15 @@
         v = self._status.get(self.idx['side_vent'], self._default)
         supports = self._functional_v(v)
 
         return (v != 0, *supports)
 
     @property
     def sound_control(self):
-        """Sound control. Controlable.
+        """Sound control. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, ("silent", "button", "button+waterfull", 0...).    
         """
 
@@ -1420,15 +1422,15 @@
 
         v = self._status.get(self.idx['error_code'], self._default)
 
         return (v != 0,)
 
     @property
     def mold_prev(self):
-        """Mold prevention. Controlable.
+        """Mold prevention. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, ("silent", "off", "on",, 0...).  
         """
 
@@ -1487,15 +1489,15 @@
         v = self._status.get(self.idx['pm25_value'], self._default)
         supports = self._uni_v(v)
 
         return (v != 0, supports)
     
     @property
     def display_brightness(self):
-        """Display brightness. Controlable.
+        """Display brightness. Controllable.
 
         Returns
         -------
         (bool, Tuple[int])
             is_support, ("bright", "dark", "off", 0...).  
         """
 
@@ -1551,483 +1553,483 @@
     def __init__(self, status, default=0):
         super().__init__(status, default)
 
 
 STATUS_DICT = {
     "AC": {
         'DeviceType': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": False,
             "legacy_name": "DeviceType",
             "id2str": {
                 1: "AC",
                 2: "DH",
                 3: "HE",
                 4: "PM25_PANEL",
             }
         },
         'Switch': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": "power",
             "id2str": {
                 0: "off",
                 1: "on",
             }
         },
         'Mode': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": "mode",
             "id2str": {
                 0: "cool",
                 1: "dry",
                 2: "fan",
                 3: "auto",
                 4: "heat",
             }
         },
         'FanSpeed': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": "air_speed",
             "id2str": {
                 0: "auto",
                 1: "silent",
                 2: "low",
                 3: "moderate",
                 4: "high",
                 5: "rapid",
                 6: "express",
             }
         },
         'TemperatureSetting': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": True,
             "legacy_name": "target_temp",
         },
         'IndoorTemperature': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": "indoor_temp",
         },
         'SleepModeRemainingTime': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": True,
             "legacy_name": "sleep_timer",
         },
         'VerticalWindDirectionSwitch': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": "vertical_wind_swingable",
             "id2str": {
                 0: "disabled",
                 1: "enabled",
             }
         },
         'VerticalWindDirectionSetting': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": True,
             "legacy_name": "vertical_wind_direction",
         },
         'HorizontalWindDirectionSetting': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": 'horizontal_wind_direction',
             "id2str": {
                 0: "auto",
                 1: "leftmost",
                 2: "middleleft",
                 3: "central",
                 4: "middleright",
                 5: "rightmost"
             }
         },
         'MildewProof': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": 'mold_prev',
             "id2str": {
                 0: "disabled",
                 1: "enabled",
             }
         },
         'QuickMode': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": 'fast_op',
             "id2str": {
                 0: "disabled",
                 1: "enabled",
             }
         },
         'PowerSaving': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name":'energy_save',
             "id2str": {
                 0: "disabled",
                 1: "enabled",
             }
         },
         'ControlTone': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name":'sound_prompt',
             "id2str": {
                 0: "enabled",
                 1: "disabled",
             }
         },
         'PowerConsumption': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name":'power_kwh',
         },
         'TaiseiaError': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": None,
         },
         'FilterElapsedHour': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": None,
         },
         'CleanSwitch': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name":'freeze_clean',
             "id2str": {
                 0: "off",
                 1: "on",
             }
         },
         'CleanNotification': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": None,
         },
         'CleanStatus': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": None,
         },
         'Error': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": None,
         },
         'max_temp': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": 'max_temp',
         },
         'min_temp': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": 'min_temp',
         },
     },
     "DH": {
         'DeviceType': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": False,
             "legacy_name": "DeviceType",
             "id2str": {
                 1: "AC",
                 2: "DH",
                 3: "HE",
                 4: "PM25_PANEL",
             }
         },
         'Switch': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": "power",
             "id2str": {
                 0: "off",
                 1: "on",
             }
         },
         'Mode': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": "mode",
             "id2str": {
                 0: "auto",
                 1: "custom",
                 2: "continuous",
                 3: "clothes_dry",
                 4: "air_purify",
                 5: "mold_prev",
                 8: "low_humidity",
                 9: "eco_comfort",
             }
         },
         'FanSpeed': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": "air_speed",
             "id2str": {
                 0: "auto",
                 1: "silent",
                 2: "low",
                 3: "moderate",
                 4: "high",
             }
         },
         'MildewProof': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": "mold_prev",
             "id2str": {
                 0: "disabled",
                 1: "enabled",
             }
         },
         'ControlTone': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": 'sound_control',
             "id2str": {
                 0: "silent",
                 1: "button",
                 2: "button+waterfull",
             }
         },
         'SaaControlTone': {  # currently not supported
-            "controlable": False,
+            "controllable": False,
             "is_numeric": False,
             "legacy_name": None,
             "id2str": {
             }
         },
         'PowerConsumption': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": 'power_kwh',
         },
         'Ion': {  # currently not supported
-            "controlable": False,
+            "controllable": False,
             "is_numeric": False,
             "legacy_name": None,
             "id2str": {
             }
         },
         'HumiditySetting': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": True,
             "legacy_name": 'target_humidity',
         },
         'AutoWindDirection': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": 'wind_swingable',
             "id2str": {
                 0: "disabled",
                 1: "enabled",
             }
         },
         'KeypadLock': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": None,
             "id2str": {
             }
         },
         'DisplayBrightness': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": 'display_brightness',
             "id2str": {
                 0: "bright",
                 1: "dark",
                 2: "off",
                 3: "all_off",
             }
         },
         'FilterControl': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": 'air_cleaning_filter',
             "id2str": {
                 0: "disabled",
                 1: "enabled",
             }
         },
         'PM25': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": 'pm25_value',
         },
         'IndoorHumidity': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": 'indoor_humidity',
         },
         'SideAirOutlet': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": False,
             "legacy_name": 'side_vent',
             "id2str": {
                 0: "off",
                 1: "on",
             }
         },
         'Defrost': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": None,
             "id2str": {
             }
         },
         'SmellIndex': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": False,
             "legacy_name": 'odor_level',
             "id2str": {
                 0: "low",
                 1: "middle",
                 2: "high",
             }
         },
         'CleanFilterNotification': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": 'clean_filter_notify',
             "id2str": {
                 0: "disabled",
                 1: "enabled",
             }
         },
         'TankFullNotification': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": False,
             "legacy_name": 'water_full_warning',
             "id2str": {
                 0: "off",  # not activated
                 1: "on",  # activated
             }
         },
         'TaiseiaError': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": None,
         },
         'Error': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": 'error_code',
         },
         'max_humidity': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": 'max_humidity',
         },
         'min_humidity': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": 'min_humidity',
         },
     },
     "HE": {
         'DeviceType': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": False,
             "legacy_name": "DeviceType",
             "id2str": {
                 1: "AC",
                 2: "DH",
                 3: "HE",
                 4: "PM25_PANEL",
             }
         },
         'Switch': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": None,
             "id2str": {
                 0: "off",
                 1: "on",
             }
         },
         'Mode': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": None,
             "id2str": {
                 0: "air_condition",
                 1: "dehumidification",
                 2: "air_supply",
                 3: "auto",
                 4: "heater",
             }
         },
         'FanSpeed': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": None,
             "id2str": {
                 0: "auto",
                 1: "silent",
                 2: "low",
                 3: "moderate",
                 4: "high",
             }
         },
         'IndoorTemperature': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": None,
         },
         'TaiseiaError': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": None,
         },
         'CleanFilterNotification': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": False,
             "legacy_name": None,
             "id2str": {
                 0: "disabled",
                 1: "enabled",
             }
         },
         'BreathMode': {
-            "controlable": True,
+            "controllable": True,
             "is_numeric": False,
             "legacy_name": None,
             "id2str": {
                 0: "auto",
                 1: "energy_recovery",
                 2: "normal"
             }
         },
         'FrontFilterNotification': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": False,
             "legacy_name": None,
             "id2str": {
                 0: "disabled",
                 1: "enabled",
             }
         },
         'Pm25FilterNotification': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": False,
             "legacy_name": None,
             "id2str": {
                 0: "disabled",
                 1: "enabled",
             }
         },
         'Error': {
-            "controlable": False,
+            "controllable": False,
             "is_numeric": True,
             "legacy_name": None,
         },
     },
     "PM25_PANEL": {
 
     }
@@ -2112,14 +2114,15 @@
                     # no legacy name
                     status.update({status_name: status_value})
                 else:
                     status.update({STATUS_DICT[device_type][status_name]["legacy_name"]: status_value})
         return JciHitachiAWSStatus(status, legacy=True)
 
     @staticmethod
+    @lru_cache
     def str2id(device_type: str, status_name: str, status_value: int = None, status_str_value: str = None, support_code: int = None):
         is_valid = (status_value is not None) ^ (status_str_value is not None)
 
         # Name check
         if is_valid:
             if status_name not in STATUS_DICT[device_type]:
                 legacy2new = {specs["legacy_name"]: new_status_name for new_status_name, specs in STATUS_DICT[device_type].items()}
```

### Comparing `LibJciHitachi-1.1.0/JciHitachi/mqtt_connection.py` & `LibJciHitachi-1.2.0/JciHitachi/mqtt_connection.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.1.0/JciHitachi/status.py` & `LibJciHitachi-1.2.0/JciHitachi/status.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.1.0/JciHitachi/utility.py` & `LibJciHitachi-1.2.0/JciHitachi/utility.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.1.0/LICENSE` & `LibJciHitachi-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.1.0/LibJciHitachi.egg-info/PKG-INFO` & `LibJciHitachi-1.2.0/LibJciHitachi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: LibJciHitachi
-Version: 1.1.0
+Version: 1.2.0
 Summary: A library for controlling Jci Hitachi devices.
 Home-page: https://github.com/qqaatw/LibJciHitachi
 Author: Allan Lin
 Author-email: qqaatw@gmail.com
 Project-URL: Issue Tracker, https://github.com/qqaatw/LibJciHitachi/issues
 Project-URL: Documentation, https://libjcihitachi.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Jci-Hitachi Library
 
 [![System Status](https://github.com/qqaatw/LibJciHitachi/actions/workflows/Status.yml/badge.svg)](https://github.com/qqaatw/LibJciHitachi/actions/workflows/Status.yml)
 [![CI](https://github.com/qqaatw/LibJciHitachi/actions/workflows/CI.yml/badge.svg)](https://github.com/qqaatw/LibJciHitachi/actions/workflows/CI.yml)
```

### Comparing `LibJciHitachi-1.1.0/LibJciHitachi.egg-info/SOURCES.txt` & `LibJciHitachi-1.2.0/LibJciHitachi.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,8 +12,14 @@
 JciHitachi/cert/AmazonRootCA1.pem
 JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem
 JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem
 LibJciHitachi.egg-info/PKG-INFO
 LibJciHitachi.egg-info/SOURCES.txt
 LibJciHitachi.egg-info/dependency_links.txt
 LibJciHitachi.egg-info/requires.txt
-LibJciHitachi.egg-info/top_level.txt
+LibJciHitachi.egg-info/top_level.txt
+tests/test_api.py
+tests/test_aws_connection.py
+tests/test_integration.py
+tests/test_model.py
+tests/test_sanity.py
+tests/test_status.py
```

### Comparing `LibJciHitachi-1.1.0/PKG-INFO` & `LibJciHitachi-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: LibJciHitachi
-Version: 1.1.0
+Version: 1.2.0
 Summary: A library for controlling Jci Hitachi devices.
 Home-page: https://github.com/qqaatw/LibJciHitachi
 Author: Allan Lin
 Author-email: qqaatw@gmail.com
 Project-URL: Issue Tracker, https://github.com/qqaatw/LibJciHitachi/issues
 Project-URL: Documentation, https://libjcihitachi.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Jci-Hitachi Library
 
 [![System Status](https://github.com/qqaatw/LibJciHitachi/actions/workflows/Status.yml/badge.svg)](https://github.com/qqaatw/LibJciHitachi/actions/workflows/Status.yml)
 [![CI](https://github.com/qqaatw/LibJciHitachi/actions/workflows/CI.yml/badge.svg)](https://github.com/qqaatw/LibJciHitachi/actions/workflows/CI.yml)
```

### Comparing `LibJciHitachi-1.1.0/README.md` & `LibJciHitachi-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.1.0/setup.py` & `LibJciHitachi-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,21 +27,20 @@
         long_description_content_type="text/markdown",
         url="https://github.com/qqaatw/LibJciHitachi",
         project_urls={
             "Issue Tracker": "https://github.com/qqaatw/LibJciHitachi/issues",
             "Documentation": "https://libjcihitachi.readthedocs.io/en/latest/",
         },
         classifiers=[
-            "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
         ],
         packages=setuptools.find_packages(include=['JciHitachi']),
         package_data={'JciHitachi': ['cert/*.pem']},
-        python_requires=">=3.7",
+        python_requires=">=3.8",
         install_requires=install_requires,
         tests_require=tests_require,
     )
```

