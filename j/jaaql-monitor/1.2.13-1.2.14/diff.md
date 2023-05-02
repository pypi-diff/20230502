# Comparing `tmp/jaaql-monitor-1.2.13.tar.gz` & `tmp/jaaql-monitor-1.2.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.13.tar", last modified: Wed Apr 26 22:43:20 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.14.tar", last modified: Tue May  2 10:30:58 2023, max compression
```

## Comparing `jaaql-monitor-1.2.13.tar` & `jaaql-monitor-1.2.14.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 22:43:20.474217 jaaql-monitor-1.2.13/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.13/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-04-26 22:43:20.473219 jaaql-monitor-1.2.13/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.13/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 22:43:20.435119 jaaql-monitor-1.2.13/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-04-26 22:43:20.000000 jaaql-monitor-1.2.13/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-04-26 22:43:20.000000 jaaql-monitor-1.2.13/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 22:43:20.000000 jaaql-monitor-1.2.13/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-26 22:43:20.000000 jaaql-monitor-1.2.13/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 22:43:20.000000 jaaql-monitor-1.2.13/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 22:43:20.472219 jaaql-monitor-1.2.13/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.13/monitor/__init__.py
--rw-rw-rw-   0        0        0    20907 2023-04-26 22:43:04.000000 jaaql-monitor-1.2.13/monitor/main.py
--rw-rw-rw-   0        0        0       42 2023-04-26 22:43:20.474217 jaaql-monitor-1.2.13/setup.cfg
--rw-rw-rw-   0        0        0      828 2023-04-25 20:11:36.000000 jaaql-monitor-1.2.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:30:58.579572 jaaql-monitor-1.2.14/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.14/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-02 10:30:58.578572 jaaql-monitor-1.2.14/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.14/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 10:30:58.576571 jaaql-monitor-1.2.14/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-02 10:30:58.000000 jaaql-monitor-1.2.14/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-02 10:30:58.000000 jaaql-monitor-1.2.14/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 10:30:58.000000 jaaql-monitor-1.2.14/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 10:30:58.000000 jaaql-monitor-1.2.14/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 10:30:58.000000 jaaql-monitor-1.2.14/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 10:30:58.577571 jaaql-monitor-1.2.14/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.14/monitor/__init__.py
+-rw-rw-rw-   0        0        0    22399 2023-05-02 10:29:33.000000 jaaql-monitor-1.2.14/monitor/main.py
+-rw-rw-rw-   0        0        0       42 2023-05-02 10:30:58.579572 jaaql-monitor-1.2.14/setup.cfg
+-rw-rw-rw-   0        0        0      828 2023-04-25 20:11:36.000000 jaaql-monitor-1.2.14/setup.py
```

### Comparing `jaaql-monitor-1.2.13/LICENSE.txt` & `jaaql-monitor-1.2.14/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.13/PKG-INFO` & `jaaql-monitor-1.2.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.13
+Version: 1.2.14
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.13/README.md` & `jaaql-monitor-1.2.14/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.13/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.14/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.13
+Version: 1.2.14
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.13/monitor/main.py` & `jaaql-monitor-1.2.14/monitor/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 from version import print_version
 import sys
 import requests
 from sys import exit
 from getpass import getpass
 from inspect import getframeinfo, stack
 from datetime import datetime
+from base64 import urlsafe_b64encode as b64e, urlsafe_b64decode as b64d
 import os
 
+HEADER__security_bypass = "Authentication-Token-Bypass"
+HEADER__security_bypass_jaaql = "Authentication-Token-Bypass-Jaaql"
+HEADER__security = "Authentication-Token"
+MARKER__bypass = "bypass "
+MARKER__jaaql_bypass = "jaaql_bypass "
+
 ENDPOINT__oauth = "/oauth/token"
 ENDPOINT__submit = "/submit"
 ENDPOINT__attach = "/accounts"
 ENDPOINT__dispatchers = "/internal/dispatchers"
 ENDPOINT__wipe = "/internal/clean"
 
 COMMAND__initialiser = "\\"
@@ -35,14 +42,17 @@
 
 LINE_LENGTH_MAX = 115
 ROWS_MAX = 25
 
 METHOD__post = "POST"
 METHOD__get = "GET"
 
+ARGS__encoded_config = ['-e', '--encoded-config']
+ARGS__config = ['-c', '--config']
+
 
 class EOFMarker:
     pass
 
 
 class ConnectionInfo:
     def __init__(self, host, username, password, database):
@@ -114,25 +124,30 @@
                 "password": conn.password
             })
 
             if oauth_res.status_code != 200:
                 print_error(self, "Invalid credentials: response code " + str(oauth_res.status_code) + " content: " + oauth_res.text)
                 return None
 
-            conn.oauth_token = {"Authentication-Token": oauth_res.json()}
+            conn.oauth_token = {HEADER__security: oauth_res.json()}
         except requests.exceptions.RequestException:
             print_error(self, "Could not connect to JAAQL running on " + conn.host + "\nPlease make sure that JAAQL is running and accessible")
 
     def time_delta_ms(self, start_time: datetime, end_time: datetime) -> int:
         return int(round((end_time - start_time).total_seconds() * 1000))
 
     def request_handler(self, method, endpoint, send_json=None, handle_error: bool = True):
         conn = self.get_current_connection()
         if conn.oauth_token is None:
-            self._fetch_oauth_token_for_current_connection()
+            if conn.password.startswith(MARKER__bypass):
+                conn.oauth_token = {HEADER__security_bypass: conn.password.split(MARKER__bypass)[1]}
+            elif conn.password.startswith(MARKER__jaaql_bypass):
+                conn.oauth_token = {HEADER__security_bypass_jaaql: conn.password.split(MARKER__jaaql_bypass)[1]}
+            else:
+                self._fetch_oauth_token_for_current_connection()
 
         start_time = datetime.now()
         res = requests.request(method, conn.get_http_url() + endpoint, json=send_json, headers=conn.oauth_token)
 
         if res.status_code == 401:
             self.log("Refreshing oauth token")
             self._fetch_oauth_token_for_current_connection()
@@ -473,45 +488,62 @@
     state.is_verbose = len([arg for arg in args if arg in ['-v', '--verbose']]) != 0
     state.is_debugging = len([arg for arg in args if arg in ['-d', '--debugging']]) != 0
     state.single_query = len([arg for arg in args if arg in ['-s', '--single-query']]) != 0
 
     if state.is_verbose:
         print_version()
 
-    has_config = len([arg for arg in args if arg in ['-c', '--config']]) != 0
-    if has_config:
-        for arg, arg_idx in zip(args, range(len(args))):
-            if arg not in ['-c', '--config']:
-                continue
-            if arg_idx == len(args) - 1:
-                print_error(state, "The config flag is the last argument. You need to supply a file")
-            configuration_name = args[arg_idx + 1]
-            candidate_file_name = None
-            if arg_idx < len(args) - 2:
-                candidate_file_name = args[arg_idx + 2]
-
-            # The following branch of logic will use the supplied configuration name as the file name and set the configuration name to default
-            if candidate_file_name is None or candidate_file_name.startswith("<") or candidate_file_name.startswith("-"):
-                candidate_file_name = configuration_name
-                configuration_name = DEFAULT_CONNECTION
+    for arg, arg_idx in zip(args, range(len(args))):
+        if arg not in ARGS__encoded_config and arg not in ARGS__config:
+            continue
+
+        if arg_idx == len(args) - 1:
+            print_error(state, "The config flag is the last argument. You need to supply a file")
+
+        configuration_name = args[arg_idx + 1]
+        candidate_content_or_file_name = None
+        if arg_idx < len(args) - 2:
+            candidate_content_or_file_name = args[arg_idx + 2]
 
-            if configuration_name in state.connections:
-                print_error(state, "The configuration with name '" + configuration_name + "' already exists")
+        # The following branch of logic will use the supplied configuration name as the file name and set the configuration name to default
+        if candidate_content_or_file_name is None or candidate_content_or_file_name.startswith("<") or candidate_content_or_file_name.startswith("-"):
+            candidate_content_or_file_name = configuration_name
+            configuration_name = DEFAULT_CONNECTION
 
-            state.connections[configuration_name] = candidate_file_name
+        if candidate_content_or_file_name in state.connections:
+            print_error(state, "The configuration with name '" + configuration_name + "' already exists")
+
+        state.connections[configuration_name] = candidate_content_or_file_name
+
+        if arg in ARGS__encoded_config:
+            content_split = candidate_content_or_file_name.split(":")
+
+            db = None
+            if len(content_split) == 4:
+                db = b64d(content_split[3])
+
+            state.connection_info[configuration_name] = ConnectionInfo(b64d(content_split[0]), b64d(content_split[1]), b64d(content_split[2]), db)
 
     deal_with_input(state)
 
 
-def initialise(file_name: str, configs: list[[str, str]]):
+def initialise(file_name: str, configs: list[[str, str]], encoded_configs: list[[str, str, str, str, str | None]]):
     args = ["-f", file_name, "-s"]
 
     for config in configs:
         args.append("-c")
         args.append(config[0])
         args.append(config[1])
 
+    for encoded_config in encoded_configs:
+        args.append("-e")
+        args.append(encoded_config[0])
+        db_part = ""
+        if encoded_config[4]:
+            db_part = ":" + b64e(encoded_config[4]).decode()
+        args.append(b64e(encoded_config[1]).decode() + ":" + b64e(encoded_config[2]).decode() + ":" + b64e(encoded_config[3]).decode() + db_part)
+
     initialise_from_args(args)
 
 
 if __name__ == "__main__":
     initialise_from_args(sys.argv[1:])
```

### Comparing `jaaql-monitor-1.2.13/setup.py` & `jaaql-monitor-1.2.14/setup.py`

 * *Files identical despite different names*

