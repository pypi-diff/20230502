# Comparing `tmp/apf_base-2.1.5.tar.gz` & `tmp/apf_base-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/APF/APF/dist/.tmp-8suq76lh/apf_base-2.1.5.tar", last modified: Mon Mar  6 19:34:43 2023, max compression
+gzip compressed data, was "/home/runner/work/APF/APF/dist/.tmp-zkh9oaqp/apf_base-2.1.6.tar", last modified: Tue May  2 21:09:17 2023, max compression
```

## Comparing `apf_base-2.1.5.tar` & `apf_base-2.1.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-06 19:34:17.000000 apf_base-2.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-06 19:34:43.000000 apf_base-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-06 19:34:17.000000 apf_base-2.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/consumers/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/consumers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/consumers/avro_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/consumers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/consumers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/consumers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/consumers/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/core/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/management/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/core/templates/step/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/templates/step/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/core/templates/step/package/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/templates/step/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/templates/step/package/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/templates/step/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/core/templates/step/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/templates/step/scripts/run_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/templates/step/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/templates/step/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/topic_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/metrics/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/metrics/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/metrics/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/metrics/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/metrics/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/producers/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/producers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/producers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/producers/json_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/producers/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-06 19:34:17.000000 apf_base-2.1.5/scripts/apf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 19:34:43.000000 apf_base-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-06 19:34:17.000000 apf_base-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-02 21:08:24.000000 apf_base-2.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-02 21:09:17.000000 apf_base-2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-02 21:08:24.000000 apf_base-2.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/consumers/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/consumers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/consumers/avro_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/consumers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/consumers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/consumers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/consumers/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/management/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/core/templates/step/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/templates/step/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/core/templates/step/package/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/templates/step/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/templates/step/package/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/templates/step/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/core/templates/step/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/templates/step/scripts/run_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/templates/step/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/templates/step/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/core/topic_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/metrics/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/metrics/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/metrics/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/metrics/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/metrics/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf/producers/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/producers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/producers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/producers/json_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-02 21:08:24.000000 apf_base-2.1.6/apf/producers/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 21:09:17.000000 apf_base-2.1.6/apf_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:17.000000 apf_base-2.1.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-02 21:08:24.000000 apf_base-2.1.6/scripts/apf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:09:17.000000 apf_base-2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-02 21:08:24.000000 apf_base-2.1.6/setup.py
```

### Comparing `apf_base-2.1.5/LICENSE` & `apf_base-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/PKG-INFO` & `apf_base-2.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apf_base
-Version: 2.1.5
+Version: 2.1.6
 Summary: ALeRCE Alert Processing Framework.
 Author: ALeRCE Team
 Author-email: contact@alerce.online
 Project-URL: Github, https://github.com/alercebroker/APF
 Project-URL: Documentation, https://apf.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -36,18 +36,18 @@
 
 *apf* design
 ============
 
 *apf* is based on *steps* conected through [Apache
 Kafka](https://kafka.apache.org/) topics.
 
-Each *step* is composed by a **consumer** and is isolated from other
+Each *step* is composed by a `consumer` and is isolated from other
 steps inside a docker container.
 
-When running, the step calls the **execute()** method for each *message*
+When running, the step calls the **execute()** method for each *message* or *message batch*
 consumed. A step can have multiple producers and databases back-ends
 plugins that can be accessed inside the *execute* method to have a more
 complex logic.
 
 
 <p align="center">
   <img src="docs/source/_static/images/apf-flow.png">
```

### Comparing `apf_base-2.1.5/README.md` & `apf_base-2.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 
 *apf* design
 ============
 
 *apf* is based on *steps* conected through [Apache
 Kafka](https://kafka.apache.org/) topics.
 
-Each *step* is composed by a **consumer** and is isolated from other
+Each *step* is composed by a `consumer` and is isolated from other
 steps inside a docker container.
 
-When running, the step calls the **execute()** method for each *message*
+When running, the step calls the **execute()** method for each *message* or *message batch*
 consumed. A step can have multiple producers and databases back-ends
 plugins that can be accessed inside the *execute* method to have a more
 complex logic.
 
 
 <p align="center">
   <img src="docs/source/_static/images/apf-flow.png">
```

### Comparing `apf_base-2.1.5/apf/consumers/avro_file.py` & `apf_base-2.1.6/apf/consumers/avro_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,24 +35,26 @@
             num_messages = self.config["consume.messages"]
         elif "NUM_MESSAGES" in self.config:
             num_messages = self.config["NUM_MESSAGES"]
         else:
             num_messages = 1
 
         msgs = []
+        left = len(files)
         for file in files:
             self.logger.debug(f"Reading File: {file}")
+            left -= 1
             with open(file, "rb") as f:
                 avro_reader = fastavro.reader(f)
                 data = avro_reader.next()
             if num_messages == 1:
                 yield data
             else:
                 msgs.append(data)
-                if len(msgs) == num_messages:
+                if len(msgs) == num_messages or left + len(msgs) < num_messages:
                     return_msgs = msgs.copy()
                     msgs = []
                     yield return_msgs
 
 
 class AVROInfiniteConsumer(GenericConsumer):
     """Consume from a Infinite AVRO Files Directory.
```

### Comparing `apf_base-2.1.5/apf/consumers/csv.py` & `apf_base-2.1.6/apf/consumers/csv.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/consumers/generic.py` & `apf_base-2.1.6/apf/consumers/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/consumers/json.py` & `apf_base-2.1.6/apf/consumers/json.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/consumers/kafka.py` & `apf_base-2.1.6/apf/consumers/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/core/__init__.py` & `apf_base-2.1.6/apf/core/__init__.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/core/management/helpers.py` & `apf_base-2.1.6/apf/core/management/helpers.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/core/secret_manager.py` & `apf_base-2.1.6/apf/core/secret_manager.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/core/step.py` & `apf_base-2.1.6/apf/core/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,24 +172,24 @@
             datetime.timezone.utc
         )
         if isinstance(message, dict):
             message = [message]
         self.message = message
         if isinstance(self.message, dict):
             self.prometheus_metrics.consumed_messages.observe(1)
-            tid = self.message.get("tid")
-            if tid:
-                tid = str(tid).upper()
-                self.prometheus_metrics.telescope_id.state(tid)
+            # tid = self.message.get("tid")
+            # if tid:
+            #     tid = str(tid).upper()
+            #     self.prometheus_metrics.telescope_id.state(tid)
         if isinstance(self.message, list):
             self.prometheus_metrics.consumed_messages.observe(len(self.message))
-            tid = self.message[0].get("tid")
-            if tid:
-                tid = str(tid).upper()
-                self.prometheus_metrics.telescope_id.state(tid)
+            # tid = self.message[0].get("tid")
+            # if tid:
+            #     tid = str(tid).upper()
+            #     self.prometheus_metrics.telescope_id.state(tid)
         preprocessed = self.pre_execute(self.message)
         return preprocessed
 
     def pre_execute(self, messages: List[dict]):
         return messages
 
     @abstractmethod
@@ -347,15 +347,16 @@
         if isinstance(result, dict):
             to_produce = [result]
         else:
             to_produce = result
         for prod_message in to_produce:
             self.producer.produce(prod_message)
             n_messages += 1
-        self.logger.info(f"Produced {n_messages} messages")
+        if not isinstance(self.producer, DefaultProducer):
+            self.logger.info(f"Produced {n_messages} messages")
 
     def set_producer_key_field(self, key_field: str):
         """
         Set the producer key, used in producer.produce(message, key=message[key_field])
 
         Parameters
         ----------
```

### Comparing `apf_base-2.1.5/apf/core/templates/step/package/step.py` & `apf_base-2.1.6/apf/core/templates/step/package/step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/core/templates/step/scripts/run_step.py` & `apf_base-2.1.6/apf/core/templates/step/scripts/run_step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/core/topic_management.py` & `apf_base-2.1.6/apf/core/topic_management.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/metrics/generic.py` & `apf_base-2.1.6/apf/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/metrics/kafka.py` & `apf_base-2.1.6/apf/metrics/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/metrics/log.py` & `apf_base-2.1.6/apf/metrics/log.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/metrics/prometheus/prometheus.py` & `apf_base-2.1.6/apf/metrics/prometheus/prometheus.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,19 +12,19 @@
             "processed_messages",
             "Current number of messages processed",
         )
         self.execution_time = Summary(
             "execution_time",
             "Execution time of processed batch",
         )
-        self.telescope_id = Enum(
-            "telescope_id",
-            "Id of the telescope",
-            states=["ZTF", "ATLAS"],
-        )
+        # self.telescope_id = Enum(
+        #     "telescope_id",
+        #     "Id of the telescope",
+        #     states=["ZTF", "ATLAS"],
+        # )
 
 
 class DefaultPrometheusMetrics(PrometheusMetrics):
     def __init__(self):
         self.consumed_messages = MagicMock()
         self.processed_messages = MagicMock()
         self.execution_time = MagicMock()
```

### Comparing `apf_base-2.1.5/apf/producers/csv.py` & `apf_base-2.1.6/apf/producers/csv.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/producers/generic.py` & `apf_base-2.1.6/apf/producers/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/producers/json_prod.py` & `apf_base-2.1.6/apf/producers/json_prod.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf/producers/kafka.py` & `apf_base-2.1.6/apf/producers/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/apf_base.egg-info/PKG-INFO` & `apf_base-2.1.6/apf_base.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apf-base
-Version: 2.1.5
+Version: 2.1.6
 Summary: ALeRCE Alert Processing Framework.
 Author: ALeRCE Team
 Author-email: contact@alerce.online
 Project-URL: Github, https://github.com/alercebroker/APF
 Project-URL: Documentation, https://apf.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -36,18 +36,18 @@
 
 *apf* design
 ============
 
 *apf* is based on *steps* conected through [Apache
 Kafka](https://kafka.apache.org/) topics.
 
-Each *step* is composed by a **consumer** and is isolated from other
+Each *step* is composed by a `consumer` and is isolated from other
 steps inside a docker container.
 
-When running, the step calls the **execute()** method for each *message*
+When running, the step calls the **execute()** method for each *message* or *message batch*
 consumed. A step can have multiple producers and databases back-ends
 plugins that can be accessed inside the *execute* method to have a more
 complex logic.
 
 
 <p align="center">
   <img src="docs/source/_static/images/apf-flow.png">
```

### Comparing `apf_base-2.1.5/apf_base.egg-info/SOURCES.txt` & `apf_base-2.1.6/apf_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.5/setup.py` & `apf_base-2.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="apf_base",
-    version="2.1.5",
+    version="2.1.6",
     description="ALeRCE Alert Processing Framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ALeRCE Team",
     author_email="contact@alerce.online",
     packages=find_namespace_packages(include=["apf.*"]),
     scripts=["scripts/apf"],
```

