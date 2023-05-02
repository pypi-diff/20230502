# Comparing `tmp/jaaql-monitor-1.2.17.tar.gz` & `tmp/jaaql-monitor-1.2.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.17.tar", last modified: Tue May  2 13:02:41 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.18.tar", last modified: Tue May  2 20:46:05 2023, max compression
```

## Comparing `jaaql-monitor-1.2.17.tar` & `jaaql-monitor-1.2.18.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 13:02:41.206868 jaaql-monitor-1.2.17/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.17/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-02 13:02:41.206868 jaaql-monitor-1.2.17/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.17/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 13:02:41.201854 jaaql-monitor-1.2.17/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-02 13:02:41.000000 jaaql-monitor-1.2.17/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-02 13:02:41.000000 jaaql-monitor-1.2.17/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 13:02:41.000000 jaaql-monitor-1.2.17/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 13:02:41.000000 jaaql-monitor-1.2.17/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 13:02:41.000000 jaaql-monitor-1.2.17/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 13:02:41.204851 jaaql-monitor-1.2.17/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.17/monitor/__init__.py
--rw-rw-rw-   0        0        0    22771 2023-05-02 13:02:23.000000 jaaql-monitor-1.2.17/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-02 13:02:26.000000 jaaql-monitor-1.2.17/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-02 13:02:41.206868 jaaql-monitor-1.2.17/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:46:05.886672 jaaql-monitor-1.2.18/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.18/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-02 20:46:05.885671 jaaql-monitor-1.2.18/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.18/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 20:46:05.880673 jaaql-monitor-1.2.18/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-02 20:46:05.000000 jaaql-monitor-1.2.18/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-02 20:46:05.000000 jaaql-monitor-1.2.18/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 20:46:05.000000 jaaql-monitor-1.2.18/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 20:46:05.000000 jaaql-monitor-1.2.18/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 20:46:05.000000 jaaql-monitor-1.2.18/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 20:46:05.884674 jaaql-monitor-1.2.18/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.18/monitor/__init__.py
+-rw-rw-rw-   0        0        0    22934 2023-05-02 20:45:49.000000 jaaql-monitor-1.2.18/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-02 20:45:53.000000 jaaql-monitor-1.2.18/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-02 20:46:05.886672 jaaql-monitor-1.2.18/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.18/setup.py
```

### Comparing `jaaql-monitor-1.2.17/LICENSE.txt` & `jaaql-monitor-1.2.18/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.17/PKG-INFO` & `jaaql-monitor-1.2.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.17
+Version: 1.2.18
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.17/README.md` & `jaaql-monitor-1.2.18/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.17/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.18/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.17
+Version: 1.2.18
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.17/monitor/main.py` & `jaaql-monitor-1.2.18/monitor/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,17 +521,18 @@
         state.connections[configuration_name] = candidate_content_or_file_name
 
         if arg in ARGS__encoded_config:
             content_split = candidate_content_or_file_name.split(":")
 
             db = None
             if len(content_split) == 4:
-                db = b64d(content_split[3])
+                db = b64d(content_split[3]).decode()
 
-            state.connection_info[configuration_name] = ConnectionInfo(b64d(content_split[0]), b64d(content_split[1]), b64d(content_split[2]), db)
+            state.connection_info[configuration_name] = ConnectionInfo(b64d(content_split[0]).decode(), b64d(content_split[1]).decode(),
+                                                                       b64d(content_split[2]).decode(), db)
 
     deal_with_input(state, file_content)
 
 
 def initialise(file_name: str, file_content: str, configs: list[[str, str]], encoded_configs: list[[str, str, str, str, str | None]]):
     args = ["-s"]
 
@@ -541,15 +542,16 @@
         args.append(config[1])
 
     for encoded_config in encoded_configs:
         args.append("-e")
         args.append(encoded_config[0])
         db_part = ""
         if encoded_config[4]:
-            db_part = ":" + b64e(encoded_config[4]).decode()
-        args.append(b64e(encoded_config[1]).decode() + ":" + b64e(encoded_config[2]).decode() + ":" + b64e(encoded_config[3]).decode() + db_part)
+            db_part = ":" + b64e(encoded_config[4].encode()).decode()
+        args.append(b64e(encoded_config[1].encode()).decode() + ":" + b64e(encoded_config[2].encode()).decode() + ":" +
+                    b64e(encoded_config[3].encode()).decode() + db_part)
 
     initialise_from_args(args, file_name, file_content)
 
 
 if __name__ == "__main__":
     initialise_from_args(sys.argv[1:])
```

### Comparing `jaaql-monitor-1.2.17/setup.py` & `jaaql-monitor-1.2.18/setup.py`

 * *Files identical despite different names*

