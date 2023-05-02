# Comparing `tmp/filum-utils-0.1.7.tar.gz` & `tmp/filum-utils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filum-utils-0.1.7.tar", last modified: Mon Apr 17 13:36:06 2023, max compression
+gzip compressed data, was "filum-utils-0.1.8.tar", last modified: Tue May  2 21:15:11 2023, max compression
```

## Comparing `filum-utils-0.1.7.tar` & `filum-utils-0.1.8.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-04-17 13:36:06.474290 filum-utils-0.1.7/
--rw-r--r--   0 hip        (502) staff       (20)      373 2023-04-17 13:36:06.474071 filum-utils-0.1.7/PKG-INFO
-drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-04-17 13:36:06.470595 filum-utils-0.1.7/filum_utils/
--rw-r--r--   0 hip        (502) staff       (20)      419 2023-04-17 13:34:58.000000 filum-utils-0.1.7/filum_utils/__init__.py
-drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-04-17 13:36:06.473842 filum-utils-0.1.7/filum_utils/clients/
--rw-r--r--   0 hip        (502) staff       (20)        0 2023-02-16 04:07:46.000000 filum-utils-0.1.7/filum_utils/clients/__init__.py
--rw-r--r--   0 hip        (502) staff       (20)     1327 2023-02-16 04:07:46.000000 filum-utils-0.1.7/filum_utils/clients/action.py
--rw-r--r--   0 hip        (502) staff       (20)       77 2023-02-16 04:07:46.000000 filum-utils-0.1.7/filum_utils/clients/analytics.py
--rw-r--r--   0 hip        (502) staff       (20)     1200 2023-02-16 04:07:46.000000 filum-utils-0.1.7/filum_utils/clients/common.py
--rw-r--r--   0 hip        (502) staff       (20)     8680 2023-04-17 13:35:10.000000 filum-utils-0.1.7/filum_utils/clients/connection.py
--rw-r--r--   0 hip        (502) staff       (20)     2189 2023-02-16 04:07:46.000000 filum-utils-0.1.7/filum_utils/clients/filum.py
--rw-r--r--   0 hip        (502) staff       (20)     1403 2023-02-16 04:07:46.000000 filum-utils-0.1.7/filum_utils/clients/log.py
--rw-r--r--   0 hip        (502) staff       (20)     2865 2023-04-17 13:35:10.000000 filum-utils-0.1.7/filum_utils/clients/mini_app.py
--rw-r--r--   0 hip        (502) staff       (20)     1806 2023-02-16 04:07:54.000000 filum-utils-0.1.7/filum_utils/clients/notification.py
--rw-r--r--   0 hip        (502) staff       (20)     1387 2023-04-17 13:34:58.000000 filum-utils-0.1.7/filum_utils/clients/subscription.py
--rw-r--r--   0 hip        (502) staff       (20)    16248 2023-04-17 13:35:10.000000 filum-utils-0.1.7/filum_utils/clients/subscription_object.py
--rw-r--r--   0 hip        (502) staff       (20)     1276 2023-04-17 13:34:58.000000 filum-utils-0.1.7/filum_utils/config.py
--rw-r--r--   0 hip        (502) staff       (20)      483 2023-04-17 13:34:58.000000 filum-utils-0.1.7/filum_utils/enums.py
--rw-r--r--   0 hip        (502) staff       (20)      182 2023-02-16 04:07:46.000000 filum-utils-0.1.7/filum_utils/errors.py
-drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-04-17 13:36:06.471489 filum-utils-0.1.7/filum_utils.egg-info/
--rw-r--r--   0 hip        (502) staff       (20)      373 2023-04-17 13:36:06.000000 filum-utils-0.1.7/filum_utils.egg-info/PKG-INFO
--rw-r--r--   0 hip        (502) staff       (20)      633 2023-04-17 13:36:06.000000 filum-utils-0.1.7/filum_utils.egg-info/SOURCES.txt
--rw-r--r--   0 hip        (502) staff       (20)        1 2023-04-17 13:36:06.000000 filum-utils-0.1.7/filum_utils.egg-info/dependency_links.txt
--rw-r--r--   0 hip        (502) staff       (20)       61 2023-04-17 13:36:06.000000 filum-utils-0.1.7/filum_utils.egg-info/requires.txt
--rw-r--r--   0 hip        (502) staff       (20)       12 2023-04-17 13:36:06.000000 filum-utils-0.1.7/filum_utils.egg-info/top_level.txt
--rw-r--r--   0 hip        (502) staff       (20)       38 2023-04-17 13:36:06.474352 filum-utils-0.1.7/setup.cfg
--rw-r--r--   0 hip        (502) staff       (20)      839 2023-04-17 13:35:47.000000 filum-utils-0.1.7/setup.py
+drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-05-02 21:15:11.821471 filum-utils-0.1.8/
+-rw-r--r--   0 hip        (502) staff       (20)      373 2023-05-02 21:15:11.821335 filum-utils-0.1.8/PKG-INFO
+drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-05-02 21:15:11.817937 filum-utils-0.1.8/filum_utils/
+-rw-r--r--   0 hip        (502) staff       (20)      469 2023-05-02 21:14:35.000000 filum-utils-0.1.8/filum_utils/__init__.py
+drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-05-02 21:15:11.821146 filum-utils-0.1.8/filum_utils/clients/
+-rw-r--r--   0 hip        (502) staff       (20)        0 2023-02-16 04:07:46.000000 filum-utils-0.1.8/filum_utils/clients/__init__.py
+-rw-r--r--   0 hip        (502) staff       (20)     1327 2023-02-16 04:07:46.000000 filum-utils-0.1.8/filum_utils/clients/action.py
+-rw-r--r--   0 hip        (502) staff       (20)       77 2023-02-16 04:07:46.000000 filum-utils-0.1.8/filum_utils/clients/analytics.py
+-rw-r--r--   0 hip        (502) staff       (20)     1200 2023-02-16 04:07:46.000000 filum-utils-0.1.8/filum_utils/clients/common.py
+-rw-r--r--   0 hip        (502) staff       (20)     8680 2023-04-17 13:35:10.000000 filum-utils-0.1.8/filum_utils/clients/connection.py
+-rw-r--r--   0 hip        (502) staff       (20)     2189 2023-02-16 04:07:46.000000 filum-utils-0.1.8/filum_utils/clients/filum.py
+-rw-r--r--   0 hip        (502) staff       (20)      534 2023-05-02 21:14:35.000000 filum-utils-0.1.8/filum_utils/clients/iam.py
+-rw-r--r--   0 hip        (502) staff       (20)     1403 2023-02-16 04:07:46.000000 filum-utils-0.1.8/filum_utils/clients/log.py
+-rw-r--r--   0 hip        (502) staff       (20)     2865 2023-04-17 13:35:10.000000 filum-utils-0.1.8/filum_utils/clients/mini_app.py
+-rw-r--r--   0 hip        (502) staff       (20)     1806 2023-02-16 04:07:54.000000 filum-utils-0.1.8/filum_utils/clients/notification.py
+-rw-r--r--   0 hip        (502) staff       (20)     1387 2023-04-17 13:34:58.000000 filum-utils-0.1.8/filum_utils/clients/subscription.py
+-rw-r--r--   0 hip        (502) staff       (20)    16721 2023-05-02 21:14:35.000000 filum-utils-0.1.8/filum_utils/clients/subscription_object.py
+-rw-r--r--   0 hip        (502) staff       (20)     1374 2023-05-02 21:14:35.000000 filum-utils-0.1.8/filum_utils/config.py
+-rw-r--r--   0 hip        (502) staff       (20)      483 2023-04-17 13:34:58.000000 filum-utils-0.1.8/filum_utils/enums.py
+-rw-r--r--   0 hip        (502) staff       (20)      182 2023-02-16 04:07:46.000000 filum-utils-0.1.8/filum_utils/errors.py
+drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-05-02 21:15:11.818664 filum-utils-0.1.8/filum_utils.egg-info/
+-rw-r--r--   0 hip        (502) staff       (20)      373 2023-05-02 21:15:11.000000 filum-utils-0.1.8/filum_utils.egg-info/PKG-INFO
+-rw-r--r--   0 hip        (502) staff       (20)      660 2023-05-02 21:15:11.000000 filum-utils-0.1.8/filum_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 hip        (502) staff       (20)        1 2023-05-02 21:15:11.000000 filum-utils-0.1.8/filum_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 hip        (502) staff       (20)       61 2023-05-02 21:15:11.000000 filum-utils-0.1.8/filum_utils.egg-info/requires.txt
+-rw-r--r--   0 hip        (502) staff       (20)       12 2023-05-02 21:15:11.000000 filum-utils-0.1.8/filum_utils.egg-info/top_level.txt
+-rw-r--r--   0 hip        (502) staff       (20)       38 2023-05-02 21:15:11.821519 filum-utils-0.1.8/setup.cfg
+-rw-r--r--   0 hip        (502) staff       (20)      839 2023-05-02 21:15:01.000000 filum-utils-0.1.8/setup.py
```

### Comparing `filum-utils-0.1.7/filum_utils/clients/action.py` & `filum-utils-0.1.8/filum_utils/clients/action.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.7/filum_utils/clients/common.py` & `filum-utils-0.1.8/filum_utils/clients/common.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.7/filum_utils/clients/connection.py` & `filum-utils-0.1.8/filum_utils/clients/connection.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.7/filum_utils/clients/filum.py` & `filum-utils-0.1.8/filum_utils/clients/filum.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.7/filum_utils/clients/log.py` & `filum-utils-0.1.8/filum_utils/clients/log.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.7/filum_utils/clients/mini_app.py` & `filum-utils-0.1.8/filum_utils/clients/mini_app.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.7/filum_utils/clients/notification.py` & `filum-utils-0.1.8/filum_utils/clients/notification.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.7/filum_utils/clients/subscription.py` & `filum-utils-0.1.8/filum_utils/clients/subscription.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.7/filum_utils/clients/subscription_object.py` & `filum-utils-0.1.8/filum_utils/clients/subscription_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 AutomatedActionType = Dict[str, Any]
 CampaignType = Dict[str, Any]
 EventType = Optional[Dict[str, Any]]
 ObjectType = Optional[Dict[str, Any]]
 UserType = Optional[Dict[str, Any]]
 SubscriptionDataType = Optional[Dict[str, Any]]
 ConnectionsType = Optional[List[Dict[str, Any]]]
+OrganizationType = Dict[str, Any]
 
 
 class BaseSubscriptionObjectClient(ABC):
     def __init__(self, subscription_id: int):
         self.subscription_client = SubscriptionClient(subscription_id)
         self.action_client = ActionClient(action_id=self.subscription_client.get_action_id())
         self.filum_client = FilumClient()
@@ -191,39 +192,42 @@
                 title=f"{self.automated_action.get('name')} failed to run",
                 subtitle=error.get("notification_message") or NOTIFICATION_ERROR_MESSAGE_MAPPINGS[error["type"]],
             )
 
     def handle_transactional_trigger(
         self,
         process_transactional_fn: Callable[
-            [ActionType, AutomatedActionType, EventType, SubscriptionDataType, ConnectionsType],
+            [ActionType, AutomatedActionType, EventType, SubscriptionDataType, ConnectionsType, OrganizationType],
             ProcessFunctionResponse
         ],
         events: List[Dict[str, Any]],
-        connections: List[Dict[str, Any]] = None
+        connections: List[Dict[str, Any]] = None,
+        organization: Dict[str, Any] = None
     ) -> TriggerFunctionResponse:
         for event in events:
             self._handle_trigger(
                 process_fn=process_transactional_fn,
                 data=event,
-                connections=connections
+                connections=connections,
+                organization=organization
             )
 
         return {"is_finished": True}
 
     def handle_segment_users_on_demand_trigger(
         self,
         process_segment_user_fn: Callable[
-            [ActionType, AutomatedActionType, UserType, SubscriptionDataType, ConnectionsType],
+            [ActionType, AutomatedActionType, UserType, SubscriptionDataType, ConnectionsType, OrganizationType],
             ProcessFunctionResponse
         ],
         properties: List[str] = None,
         required_properties: List[List[str]] = None,
         last_current_index: int = None,
-        connections: List[Dict[str, Any]] = None
+        connections: List[Dict[str, Any]] = None,
+        organization: Dict[str, Any] = None
     ) -> TriggerFunctionResponse:
         if not last_current_index:
             last_current_index = 0
 
         subscription_data = self.get_subscription_data()
         current_index = subscription_data.get("last_current_index") or 0
         if current_index != last_current_index:
@@ -250,15 +254,16 @@
         for user in users:
             current_index += 1
             total_processed_users += 1
 
             self._handle_trigger(
                 process_fn=process_segment_user_fn,
                 data=user,
-                connections=connections
+                connections=connections,
+                organization=organization
             )
 
         if total_processed_users >= config.SEGMENT_RECORD_LIMIT:
             self.update_subscription_data({"last_current_index": current_index})
             self.action_client.sync({
                 "subscription_id": self.subscription_client.subscription["id"],
                 "last_current_index": last_current_index
@@ -267,18 +272,19 @@
             return {"is_finished": False}
 
         return {"is_finished": True}
 
     def handle_object_on_demand_trigger(
         self,
         process_segment_fn: Callable[
-            [ActionType, AutomatedActionType, ObjectType, SubscriptionDataType, ConnectionsType],
+            [ActionType, AutomatedActionType, ObjectType, SubscriptionDataType, ConnectionsType, OrganizationType],
             ProcessFunctionResponse
         ],
-        connections: List[Dict[str, Any]] = None
+        connections: List[Dict[str, Any]] = None,
+        organization: Dict[str, Any] = None
     ) -> TriggerFunctionResponse:
 
         context_type = self.get_context_type()
 
         data = {}
         if context_type == Object.SEGMENT:
             data = self.filum_client.get_segment(
@@ -287,29 +293,37 @@
             )
         elif context_type == Object.CAMPAIGN:
             data = self.filum_client.get_campaign(campaign_id=self.get_context_id())
 
         self._handle_trigger(
             process_fn=process_segment_fn,
             data=data,
-            connections=connections
+            connections=connections,
+            organization=organization
         )
 
         return {"is_finished": True}
 
-    def _handle_trigger(self, process_fn: Callable, data: Dict[str, Any], connections: List[Dict[str, Any]] = None):
+    def _handle_trigger(
+        self,
+        process_fn: Callable,
+        data: Dict[str, Any],
+        connections: List[Dict[str, Any]] = None,
+        organization: Dict[str, Any] = None
+    ):
         if not connections:
             connections = []
 
         params = {
             "action": self.action_client.action,
             "automated_action": self.automated_action,
             "data": data,
             "subscription_data": self.get_subscription_data(),
-            "connections": connections
+            "connections": connections,
+            "organization": organization
         }
 
         process_fn(**params)
 
     def _get_object_route(self):
         return {
             "path": RoutePath.AUTOMATED_ACTIONS_DETAIL,
```

### Comparing `filum-utils-0.1.7/filum_utils/config.py` & `filum-utils-0.1.8/filum_utils/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     SUBSCRIPTION_USERNAME = "subscription@filum"
     SUBSCRIPTION_PASSWORD = ""
 
     FILUM_BASE_URL = "https://api.filum.asia"
     FILUM_USERNAME = "filum_dev"
     FILUM_PASSWORD = ""
 
+    IAM_BASE_URL = "https://iam.filum.asia"
+    IAM_USERNAME = "filum_dev"
+    IAM_PASSWORD = ""
+
     EVENT_API_BASE_URL = "https://event.filum.asia"
 
     SEGMENT_RECORD_LIMIT = 3000
 
     def __init__(self):
         for attr in dir(self):
             if not attr.isupper():
```

### Comparing `filum-utils-0.1.7/filum_utils.egg-info/SOURCES.txt` & `filum-utils-0.1.8/filum_utils.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -10,12 +10,13 @@
 filum_utils.egg-info/top_level.txt
 filum_utils/clients/__init__.py
 filum_utils/clients/action.py
 filum_utils/clients/analytics.py
 filum_utils/clients/common.py
 filum_utils/clients/connection.py
 filum_utils/clients/filum.py
+filum_utils/clients/iam.py
 filum_utils/clients/log.py
 filum_utils/clients/mini_app.py
 filum_utils/clients/notification.py
 filum_utils/clients/subscription.py
 filum_utils/clients/subscription_object.py
```

### Comparing `filum-utils-0.1.7/setup.py` & `filum-utils-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 
 from setuptools import setup, find_packages
 
 sys.path.insert(0, os.path.join(os.path.dirname(__file__), 'filum_analytics'))
 
-VERSION = "0.1.7"
+VERSION = "0.1.8"
 DESCRIPTION = "Filum Utils"
 LONG_DESCRIPTION = "Filum Utils"
 
 install_requires = [
     "requests==2.25.1",
     "filum-analytics-python==1.1.1",
     "glom==20.11.0",
```

