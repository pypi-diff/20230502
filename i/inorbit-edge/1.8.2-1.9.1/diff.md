# Comparing `tmp/inorbit_edge-1.8.2.tar.gz` & `tmp/inorbit_edge-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inorbit_edge-1.8.2.tar", last modified: Fri Feb 24 18:37:18 2023, max compression
+gzip compressed data, was "inorbit_edge-1.9.1.tar", last modified: Tue May  2 16:39:28 2023, max compression
```

## Comparing `inorbit_edge-1.8.2.tar` & `inorbit_edge-1.9.1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 18:37:18.927822 inorbit_edge-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-02-24 18:37:14.000000 inorbit_edge-1.8.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-02-24 18:37:14.000000 inorbit_edge-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-24 18:37:14.000000 inorbit_edge-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-02-24 18:37:18.927822 inorbit_edge-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-02-24 18:37:14.000000 inorbit_edge-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 18:37:18.927822 inorbit_edge-1.8.2/inorbit_edge/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-24 18:37:14.000000 inorbit_edge-1.8.2/inorbit_edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   120194 2023-02-24 18:37:14.000000 inorbit_edge-1.8.2/inorbit_edge/inorbit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    39002 2023-02-24 18:37:14.000000 inorbit_edge-1.8.2/inorbit_edge/robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-02-24 18:37:14.000000 inorbit_edge-1.8.2/inorbit_edge/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-02-24 18:37:14.000000 inorbit_edge-1.8.2/inorbit_edge/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 18:37:18.927822 inorbit_edge-1.8.2/inorbit_edge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-02-24 18:37:18.000000 inorbit_edge-1.8.2/inorbit_edge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-02-24 18:37:18.000000 inorbit_edge-1.8.2/inorbit_edge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 18:37:18.000000 inorbit_edge-1.8.2/inorbit_edge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 18:37:18.000000 inorbit_edge-1.8.2/inorbit_edge.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-02-24 18:37:18.000000 inorbit_edge-1.8.2/inorbit_edge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-24 18:37:18.000000 inorbit_edge-1.8.2/inorbit_edge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-02-24 18:37:18.927822 inorbit_edge-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-02-24 18:37:14.000000 inorbit_edge-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:39:28.177492 inorbit_edge-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-02 16:39:28.177492 inorbit_edge-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:39:28.173492 inorbit_edge-1.9.1/inorbit_edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120194 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/inorbit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/missions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40986 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/inorbit_edge/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:39:28.177492 inorbit_edge-1.9.1/inorbit_edge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-02 16:39:28.000000 inorbit_edge-1.9.1/inorbit_edge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-02 16:39:28.000000 inorbit_edge-1.9.1/inorbit_edge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:39:28.000000 inorbit_edge-1.9.1/inorbit_edge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:39:28.000000 inorbit_edge-1.9.1/inorbit_edge.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-02 16:39:28.000000 inorbit_edge-1.9.1/inorbit_edge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 16:39:28.000000 inorbit_edge-1.9.1/inorbit_edge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-02 16:39:28.177492 inorbit_edge-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-02 16:39:21.000000 inorbit_edge-1.9.1/setup.py
```

### Comparing `inorbit_edge-1.8.2/CONTRIBUTING.md` & `inorbit_edge-1.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `inorbit_edge-1.8.2/LICENSE` & `inorbit_edge-1.9.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 If you are entering into this EULA agreement on behalf of a company or other legal entity, you represent that you have the authority to bind such entity and its affiliates to these terms and conditions. If you do not have such authority or if you do not agree with the terms and conditions of this EULA agreement, do not install or use the Software, and you must not accept this EULA agreement.
 
 This EULA agreement shall apply only to the Software supplied by InOrbit herewith regardless of whether other software is referred to or described herein. The terms also apply to any InOrbit updates, supplements, Internet-based services, and support services for the Software, unless other terms accompany those items on delivery. If so, those terms apply.
 
 ### License Grant
 
-InOrbit hereby grants you a personal, non-transferable, non-exclusive licence to use the InOrbit Edge SDK software on your devices in accordance with the terms of this EULA agreement.
+InOrbit hereby grants you a personal, non-transferable, non-exclusive license to use the InOrbit Edge SDK software on your devices in accordance with the terms of this EULA agreement.
 
 You are permitted to load the InOrbit Edge SDK software (for example a PC, laptop, mobile or tablet) under your control. You are responsible for ensuring your device meets the minimum requirements of the InOrbit Edge SDK software.
 
 You are not permitted to:
 
 *   Edit, alter, modify, adapt, translate or otherwise change the whole or any part of the Software nor permit the whole or any part of the Software to be combined with or become incorporated in any other software, nor decompile, disassemble or reverse engineer the Software or attempt to do any such things
 *   Reproduce, copy, distribute, resell or otherwise use the Software for any commercial purpose
@@ -27,15 +27,15 @@
 *   Use the Software in any way which breaches any applicable local, national or international law
 *   Use the Software for any purpose that InOrbit considers is a breach of this EULA agreement
 
 ### Intellectual Property and Ownership
 
 InOrbit shall at all times retain ownership of the Software as originally downloaded by you and all subsequent downloads of the Software by you. The Software (and the copyright, and other intellectual property rights of whatever nature in the Software, including any modifications made thereto) are and shall remain the property of InOrbit.
 
-InOrbit reserves the right to grant licences to use the Software to third parties.
+InOrbit reserves the right to grant licenses to use the Software to third parties.
 
 ### Termination
 
 This EULA agreement is effective from the date you first use the Software and shall continue until terminated. You may terminate it at any time upon written notice to InOrbit.
 
 It will also terminate immediately if you fail to comply with any term of this EULA agreement. Upon such termination, the licenses granted by this EULA agreement will immediately terminate and you agree to stop all access and use of the Software. The provisions that by their nature continue and survive will survive any termination of this EULA agreement.
```

### Comparing `inorbit_edge-1.8.2/PKG-INFO` & `inorbit_edge-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inorbit_edge
-Version: 1.8.2
+Version: 1.9.1
 Summary: InOrbit Python Edge SDK
 Home-page: https://github.com/inorbit-ai/edge-sdk-python
 Author: InOrbit
 Author-email: support@inorbit.ai
 License: UNKNOWN
 Keywords: inorbit_edge
 Platform: UNKNOWN
```

### Comparing `inorbit_edge-1.8.2/README.md` & `inorbit_edge-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `inorbit_edge-1.8.2/inorbit_edge/inorbit_pb2.py` & `inorbit_edge-1.9.1/inorbit_edge/inorbit_pb2.py`

 * *Files identical despite different names*

### Comparing `inorbit_edge-1.8.2/inorbit_edge/robot.py` & `inorbit_edge-1.9.1/inorbit_edge/robot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import json
 from inorbit_edge import __version__ as inorbit_edge_version
+from inorbit_edge.types import Pose, SpatialTolerance
 import os
 import logging
 import paho.mqtt.client as mqtt
 from urllib.parse import urlsplit
 import socks
 import ssl
 import threading
@@ -18,17 +19,25 @@
     LaserMessage,
     PathPoint,
     RobotPath,
     PathDataMessage,
     Echo,
     CustomScriptCommandMessage,
     CustomScriptStatusMessage,
+    CustomCommandRosMessage,
     CameraMessage,
 )
 from inorbit_edge.video import CameraStreamer, Camera
+from inorbit_edge.missions import MissionsModule
+from inorbit_edge.commands import (
+    COMMAND_INITIAL_POSE,
+    COMMAND_NAV_GOAL,
+    COMMAND_CUSTOM_COMMAND,
+    COMMAND_MESSAGE,
+)
 import time
 import requests
 import math
 from inorbit_edge.utils import encode_floating_point_list
 import certifi
 import subprocess
 import re
@@ -47,51 +56,55 @@
 MQTT_SUBTOPIC_OUT_CMD = "out_cmd"
 
 MQTT_TOPIC_ECHO = "echo"
 MQTT_NAV_GOAL_GOAL = "ros/loc/nav_goal"
 MQTT_NAV_GOAL_MULTI = "ros/loc/goal_path"
 MQTT_INITIAL_POSE = "ros/loc/set_pose"
 MQTT_CUSTOM_COMMAND = "custom_command/script/command"
+MQTT_CUSTOM_COMMAND_MESSAGE = "custom_command/ros"
 MQTT_SCRIPT_OUTPUT_TOPIC = "custom_command/script/status"
 MQTT_IN_CMD = "in_cmd"
 
-# InOrbit commands
-COMMAND_INITIAL_POSE = "initialPose"
-COMMAND_NAV_GOAL = "navGoal"
-COMMAND_CUSTOM_COMMAND = "customCommand"
 # InOrbit modules
 INORBIT_MODULE_CAMERAS = "RosImageAgentlet"
 # CustomCommand execution status
 CUSTOM_COMMAND_STATUS_FINISHED = "finished"
 CUSTOM_COMMAND_STATUS_ABORTED = "aborted"
 
 ROBOT_PATH_POINTS_LIMIT = 1000
 
 
 class RobotSession:
-    def __init__(self, robot_id, robot_name, api_key, **kwargs) -> None:
+    def __init__(
+        self, robot_id, robot_name, api_key=None, robot_key=None, **kwargs
+    ) -> None:
         """Initialize a robot session.
 
         Args:
             robot_id (str): ID of the robot.
             robot_name (str): Robot name.
             api_key (str): API key for authenticating against InOrbit Cloud services.
+            robot_key(str): Robot key for authenticating against InOrbit Cloud services
+            when using InOrbit Connect (https://connect.inorbit.ai/).
             endpoint (str): InOrbit URL. Defaults: INORBIT_CLOUD_SDK_ROBOT_CONFIG_URL.
             use_ssl (bool): Configures MQTT client to use SSL. Defaults: True.
         """
 
+        self.robot_key = robot_key
+        self.api_key = api_key
+
         self.logger = logging.getLogger(__class__.__name__)
 
         self.robot_id = robot_id
         self.robot_name = robot_name
-        self.api_key = api_key
         # The agent version is generated based on the InOrbit Edge SDK version
         self.agent_version = "{}.edgesdk_py".format(inorbit_edge_version)
         self.endpoint = kwargs.get("endpoint", INORBIT_CLOUD_SDK_ROBOT_CONFIG_URL)
-
+        # Track robot's current pose
+        self._last_pose = None
         # Use SSL by default
         self.use_ssl = kwargs.get("use_ssl", True)
 
         # Use TCP transport by default. The client will use websockets
         # transport if the environment variable HTTP_PROXY is set.
         self.use_websockets = kwargs.get("use_websockets", False)
 
@@ -140,20 +153,22 @@
 
         # Functions to handle incoming MQTT messages.
         # They are mapped by MQTT subtopic e.g.
         # 'ros/loc/set_pose': set_pose_message_handler
         self.message_handlers = {}
 
         self.command_callbacks = []
+        self.missions_module = MissionsModule(self)
         self.camera_streamers = {}
         self.camera_streaming_on = False
         self.camera_streaming_mutex = threading.Lock()
 
         self.message_handlers[MQTT_INITIAL_POSE] = self._handle_initial_pose
         self.message_handlers[MQTT_CUSTOM_COMMAND] = self._handle_custom_command
+        self.message_handlers[MQTT_CUSTOM_COMMAND_MESSAGE] = self._handle_custom_message
         self.message_handlers[MQTT_NAV_GOAL_GOAL] = self._handle_nav_goal
         self.message_handlers[MQTT_IN_CMD] = self._handle_in_cmd
 
         # Internal variables for configuring throttling
         # The throttling is done by method instead of by topic because the same topic
         # might be used for sending different type of messages e.g. pose and laser.
         # Each throttling has a ``last_ts`` that is the last time a method was called
@@ -240,20 +255,24 @@
     def _fetch_robot_config(self):
         """Gets robot config by posting appkey and robot/agent info.
         All params are provided on the RobotSession constructor
         """
         self.logger.info("Fetching config for robot {}".format(self.robot_id))
         # get params from self
         params = {
-            "appKey": self.api_key,
             "robotId": self.robot_id,
             "hostname": self.robot_name,
             "agentVersion": self.agent_version,
         }
 
+        if self.robot_key:
+            params["robotKey"] = self.robot_key
+        elif self.api_key:
+            params["appKey"] = self.api_key
+
         # post request to fetch robot config
         response = requests.post(self.endpoint, data=params)
         response.raise_for_status()
 
         # TODO: validate fetched config
         return response.json()
 
@@ -287,14 +306,17 @@
         self.client.subscribe(
             topic=self._get_robot_subtopic(subtopic=MQTT_INITIAL_POSE)
         )
         self.client.subscribe(
             topic=self._get_robot_subtopic(subtopic=MQTT_CUSTOM_COMMAND)
         )
         self.client.subscribe(
+            topic=self._get_robot_subtopic(subtopic=MQTT_CUSTOM_COMMAND_MESSAGE)
+        )
+        self.client.subscribe(
             topic=self._get_robot_subtopic(subtopic=MQTT_NAV_GOAL_GOAL)
         )
         self.client.subscribe(topic=self._get_robot_subtopic(subtopic=MQTT_IN_CMD))
         # ask server to resend modules, so our state is consistent with the server side
         self._resend_modules()
 
     def _on_message(self, client, userdata, msg):
@@ -357,43 +379,54 @@
         seq = args[0]
         ts = args[1]  # noqa: F841
         x = args[2]
         y = args[3]
         theta = args[4]
 
         # Hand over to callback for processing, using the proper format
-        self._dispatch_command(
+        self.dispatch_command(
             command_name=COMMAND_INITIAL_POSE,
             args=[{"x": x, "y": y, "theta": theta}],
             execution_id=seq,  # NOTE: Using seq as the execution ID
         )
 
     def _handle_custom_command(self, msg):
         """Handle incoming MQTT_CUSTOM_COMMAND message."""
 
         custom_script_msg = CustomScriptCommandMessage()
         custom_script_msg.ParseFromString(msg)
         # Hand over to callback for processing, using the proper format
-        self._dispatch_command(
+        self.dispatch_command(
             command_name=COMMAND_CUSTOM_COMMAND,
             args=[custom_script_msg.file_name, custom_script_msg.arg_options],
             execution_id=custom_script_msg.execution_id,
         )
 
+    def _handle_custom_message(self, msg):
+        """Handle incoming MQTT_CUSTOM_COMMAND_MESSAGE message."""
+
+        custom_command_message = CustomCommandRosMessage()
+        custom_command_message.ParseFromString(msg)
+        # Hand over to callback for processing, using the proper format
+        self.dispatch_command(
+            command_name=COMMAND_MESSAGE,
+            args=[custom_command_message.cmd],
+        )
+
     def _handle_nav_goal(self, msg):
         """Handle incoming MQTT_NAV_GOAL_GOAL message."""
 
         args = msg.decode("utf-8").split("|")
         seq = args[0]
         ts = args[1]  # noqa: F841
         x = args[2]
         y = args[3]
         theta = args[4]
         # Hand over to callback for processing, using the proper format
-        self._dispatch_command(
+        self.dispatch_command(
             command_name=COMMAND_NAV_GOAL,
             args=[{"x": x, "y": y, "theta": theta}],
             execution_id=seq,  # NOTE: Using seq as the execution ID
         )
 
     def _handle_in_cmd(self, msg):
         """Handles an in_cmd message"""
@@ -435,20 +468,21 @@
         msg.camera_id = camera_id
         msg.width = width
         msg.height = height
         msg.ts = ts
         msg.image = image
         self.publish_protobuf(MQTT_SUBTOPIC_CAMERA_V2, msg)
 
-    def _dispatch_command(self, command_name, args, execution_id):
+    def dispatch_command(self, command_name, args, execution_id=None):
         """Executes registered command callbacks for a specific incoming command."""
         for callback in self.command_callbacks:
 
             def result_function(result_code):
-                return self.report_command_result(args, execution_id, result_code)
+                if execution_id is not None:
+                    return self.report_command_result(args, execution_id, result_code)
 
             # TODO: Implement progress reporting function
             def progress_function(output, error):
                 return 1
 
             options = {
                 "result_function": result_function,
@@ -742,25 +776,42 @@
 
         msg = LocationAndPoseMessage()
         msg.ts = ts if ts else int(time.time() * 1000)
         msg.pos_x = x
         msg.pos_y = y
         msg.yaw = yaw
         msg.frame_id = frame_id
+        self._last_pose = Pose(frame_id=frame_id, x=x, y=y, theta=yaw)
         self.publish_protobuf(MQTT_SUBTOPIC_POSE, msg)
 
-    def publish_key_values(self, key_values, custom_field="0"):
+    def reached_waypoint(self, waypoint: Pose, tolerance: SpatialTolerance):
+        if self._last_pose is None:
+            return False
+        return (
+            math.sqrt(
+                (self._last_pose.x - waypoint.x) ** 2
+                + (self._last_pose.y - waypoint.y) ** 2,
+            )
+            <= tolerance.positionMeters
+            and (self._last_pose.theta - waypoint.theta) % (2 * math.pi)
+            <= tolerance.angularRadians
+        )
+
+    def publish_key_values(self, key_values, custom_field="0", is_event=False):
         """Publish key value pairs
 
         Args:
             key_values (dict): Key value mappings to publish
             custom_field (str, optional): ID of the CustomData element. Defaults to "0".
+            is_event (bool): Events are not throttled
         """
 
-        if not self._should_publish_message(method="publish_key_values"):
+        if not is_event and not self._should_publish_message(
+            method="publish_key_values"
+        ):
             return None
 
         def convert_value(value):
             if isinstance(value, object):
                 return json.dumps(value)
             else:
                 return str(value)
```

### Comparing `inorbit_edge-1.8.2/inorbit_edge/utils.py` & `inorbit_edge-1.9.1/inorbit_edge/utils.py`

 * *Files identical despite different names*

### Comparing `inorbit_edge-1.8.2/inorbit_edge/video.py` & `inorbit_edge-1.9.1/inorbit_edge/video.py`

 * *Files identical despite different names*

### Comparing `inorbit_edge-1.8.2/inorbit_edge.egg-info/PKG-INFO` & `inorbit_edge-1.9.1/inorbit_edge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inorbit-edge
-Version: 1.8.2
+Version: 1.9.1
 Summary: InOrbit Python Edge SDK
 Home-page: https://github.com/inorbit-ai/edge-sdk-python
 Author: InOrbit
 Author-email: support@inorbit.ai
 License: UNKNOWN
 Keywords: inorbit_edge
 Platform: UNKNOWN
```

### Comparing `inorbit_edge-1.8.2/inorbit_edge.egg-info/requires.txt` & `inorbit_edge-1.9.1/inorbit_edge.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `inorbit_edge-1.8.2/setup.py` & `inorbit_edge-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,10 +89,10 @@
     setup_requires=setup_requirements,
     test_suite="inorbit_edge/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/inorbit-ai/edge-sdk-python",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="1.8.2",
+    version="1.9.1",
     zip_safe=False,
 )
```

