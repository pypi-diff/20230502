# Comparing `tmp/whitson_tool_helper-0.1.2.tar.gz` & `tmp/whitson_tool_helper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitson_tool_helper-0.1.2.tar", last modified: Fri Apr 28 08:44:24 2023, max compression
+gzip compressed data, was "whitson_tool_helper-0.1.3.tar", last modified: Tue May  2 11:39:10 2023, max compression
```

## Comparing `whitson_tool_helper-0.1.2.tar` & `whitson_tool_helper-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-28 08:44:24.399978 whitson_tool_helper-0.1.2/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-04-28 08:44:24.389978 whitson_tool_helper-0.1.2/PKG-INFO
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      705 2023-04-28 08:44:18.000000 whitson_tool_helper-0.1.2/pyproject.toml
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       38 2023-04-28 08:44:24.399978 whitson_tool_helper-0.1.2/setup.cfg
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-28 08:44:24.389978 whitson_tool_helper-0.1.2/src/
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-28 08:44:24.389978 whitson_tool_helper-0.1.2/src/whitson_tool_helper/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      107 2023-04-26 09:24:26.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/__init__.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       66 2023-04-26 13:22:55.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/logger.py
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-28 08:44:24.389978 whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      370 2023-04-26 13:32:24.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/aux.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     2738 2023-04-28 08:39:14.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/main.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     4403 2023-04-26 14:33:47.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/pubsub.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     3494 2023-04-28 08:40:03.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/rabbitmq.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      574 2023-04-26 07:15:11.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/timeout.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      704 2023-04-26 12:52:42.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/whitson_exceptions.py
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-28 08:44:24.389978 whitson_tool_helper-0.1.2/src/whitson_tool_helper.egg-info/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-04-28 08:44:24.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper.egg-info/PKG-INFO
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      572 2023-04-28 08:44:24.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper.egg-info/SOURCES.txt
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)        1 2023-04-28 08:44:24.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper.egg-info/dependency_links.txt
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      116 2023-04-28 08:44:24.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper.egg-info/requires.txt
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       20 2023-04-28 08:44:24.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper.egg-info/top_level.txt
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-02 11:39:10.140303 whitson_tool_helper-0.1.3/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-05-02 11:39:10.140303 whitson_tool_helper-0.1.3/PKG-INFO
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      705 2023-05-02 11:39:04.000000 whitson_tool_helper-0.1.3/pyproject.toml
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       38 2023-05-02 11:39:10.140303 whitson_tool_helper-0.1.3/setup.cfg
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-02 11:39:10.140303 whitson_tool_helper-0.1.3/src/
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-02 11:39:10.140303 whitson_tool_helper-0.1.3/src/whitson_tool_helper/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      107 2023-04-26 09:24:26.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/__init__.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       66 2023-04-26 13:22:55.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/logger.py
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-02 11:39:10.140303 whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      370 2023-04-26 13:32:24.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/aux.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     2738 2023-05-02 09:42:15.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/main.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     4382 2023-05-02 09:41:25.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/pubsub.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     3725 2023-05-02 11:17:35.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/rabbitmq.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      574 2023-04-26 07:15:11.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/timeout.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      704 2023-04-26 12:52:42.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper/whitson_exceptions.py
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-05-02 11:39:10.140303 whitson_tool_helper-0.1.3/src/whitson_tool_helper.egg-info/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-05-02 11:39:10.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper.egg-info/PKG-INFO
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      572 2023-05-02 11:39:10.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)        1 2023-05-02 11:39:10.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      116 2023-05-02 11:39:10.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper.egg-info/requires.txt
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       20 2023-05-02 11:39:10.000000 whitson_tool_helper-0.1.3/src/whitson_tool_helper.egg-info/top_level.txt
```

### Comparing `whitson_tool_helper-0.1.2/pyproject.toml` & `whitson_tool_helper-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whitson_tool_helper"
-version =  "0.1.2"
+version =  "0.1.3"
 authors = [
   { name="Markus Blytt", email="blytt@whitson.com" },
   { name="Jason Hu", email="jason@whitson.com" },
   { name="Arnaud Hoffmann", email="arnaud@whitson.com" },
 ]
 description = "A Toolbox for whitson cloud software solutions"
 dependencies = ["pika==1.3.1", "google-auth==2.16.0","google-cloud-pubsub==2.14.0", "google-cloud-storage==2.7.0","google-cloud-logging==3.5.0"]
```

### Comparing `whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/main.py` & `whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/main.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/pubsub.py` & `whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/pubsub.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,21 @@
 from whitson_tool_helper.logger import LOGGER
 
 
 class PubsubConsumer:
     def __init__(self, process_func, to_dict=False):
         check_environment_variables(
             [
-                "PVT_UTILS_SUBSCRIPTION",
                 "GOOGLE_PROJECT",
                 "GOOGLE_APPLICATION_CREDENTIALS",
             ]
         )
         self.decode_json = to_dict
         self.process_func = process_func
-        self.subscription = os.environ["PVT_UTILS_GOOGLE_PUBSUB_SUBSCRIPTION"]
+        self.subscription = os.environ["MESSAGING_SUBSCRIPTION"]
 
         self.google_project_name = os.environ["GOOGLE_PROJECT"]
         self.subscriber = pubsub_v1.SubscriberClient()
 
     @property
     def subscription_path(self):
         if self.subscriber:
@@ -52,17 +51,18 @@
                 raise
             for received_message in response.received_messages:
                 msg = received_message.message
                 LOGGER.info(
                     f"Received PubSub message {msg.message_id}",
                     {"pubsub_msg_id": msg.message_id},
                 )
-                data = json.loads(msg.data.decode("utf8")) if self.decode_json else msg
+                data = json.loads(msg.data.decode("utf8"))
+                meta_data = msg.attributes
                 try:
-                    self.process_func(data)
+                    self.process_func(data, meta_data=meta_data)
                 except Exception as e:
                     LOGGER.error(e)
                     LOGGER.error(traceback.format_exc())
                     LOGGER.warning(f"ACKING UNPROCESSED MESSAGE: {msg.message_id}")
                 else:
                     LOGGER.info(f"ACKING MESSAGE: {msg.message_id}")
                 self.subscriber.acknowledge(
```

### Comparing `whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/rabbitmq.py` & `whitson_tool_helper-0.1.3/src/whitson_tool_helper/messaging/rabbitmq.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,21 @@
         self.channel = self.connection.channel()
         subscription = os.getenv("MESSAGING_SUBSCRIPTION")
         self.channel.queue_declare(
             queue=subscription,
             durable=True,
             arguments={"x-max-priority": 100, "x-queue-type": "classic"},
         )
+        exchange = "engines"
+        if subscription.endswith("-calculated"):
+            exchange = "clients"
+
+        self.channel.queue_bind(
+            queue=subscription, exchange=exchange, routing_key=subscription
+        )
 
         self.channel.basic_qos(prefetch_count=1)
 
         def callback(ch, method, properties, body):
             if not body or body.decode("utf-8") == "":
                 ch.basic_ack(delivery_tag=method.delivery_tag)
                 LOGGER.info("Recieved faulty message")
```

### Comparing `whitson_tool_helper-0.1.2/src/whitson_tool_helper/timeout.py` & `whitson_tool_helper-0.1.3/src/whitson_tool_helper/timeout.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.2/src/whitson_tool_helper/whitson_exceptions.py` & `whitson_tool_helper-0.1.3/src/whitson_tool_helper/whitson_exceptions.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.2/src/whitson_tool_helper.egg-info/SOURCES.txt` & `whitson_tool_helper-0.1.3/src/whitson_tool_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

