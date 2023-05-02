# Comparing `tmp/jaaql-monitor-1.2.14.tar.gz` & `tmp/jaaql-monitor-1.2.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.14.tar", last modified: Tue May  2 10:30:58 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.15.tar", last modified: Tue May  2 12:44:49 2023, max compression
```

## Comparing `jaaql-monitor-1.2.14.tar` & `jaaql-monitor-1.2.15.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 10:30:58.579572 jaaql-monitor-1.2.14/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.14/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-02 10:30:58.578572 jaaql-monitor-1.2.14/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.14/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 10:30:58.576571 jaaql-monitor-1.2.14/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-02 10:30:58.000000 jaaql-monitor-1.2.14/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-05-02 10:30:58.000000 jaaql-monitor-1.2.14/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 10:30:58.000000 jaaql-monitor-1.2.14/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 10:30:58.000000 jaaql-monitor-1.2.14/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 10:30:58.000000 jaaql-monitor-1.2.14/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 10:30:58.577571 jaaql-monitor-1.2.14/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.14/monitor/__init__.py
--rw-rw-rw-   0        0        0    22399 2023-05-02 10:29:33.000000 jaaql-monitor-1.2.14/monitor/main.py
--rw-rw-rw-   0        0        0       42 2023-05-02 10:30:58.579572 jaaql-monitor-1.2.14/setup.cfg
--rw-rw-rw-   0        0        0      828 2023-04-25 20:11:36.000000 jaaql-monitor-1.2.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:44:49.030802 jaaql-monitor-1.2.15/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.15/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-02 12:44:49.029802 jaaql-monitor-1.2.15/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.15/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 12:44:49.026803 jaaql-monitor-1.2.15/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-02 12:44:48.000000 jaaql-monitor-1.2.15/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-02 12:44:48.000000 jaaql-monitor-1.2.15/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 12:44:48.000000 jaaql-monitor-1.2.15/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 12:44:48.000000 jaaql-monitor-1.2.15/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 12:44:48.000000 jaaql-monitor-1.2.15/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 12:44:49.028802 jaaql-monitor-1.2.15/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.15/monitor/__init__.py
+-rw-rw-rw-   0        0        0    22732 2023-05-02 12:33:40.000000 jaaql-monitor-1.2.15/monitor/main.py
+-rw-rw-rw-   0        0        0       42 2023-05-02 12:44:49.030802 jaaql-monitor-1.2.15/setup.cfg
+-rw-rw-rw-   0        0        0      828 2023-04-25 20:11:36.000000 jaaql-monitor-1.2.15/setup.py
```

### Comparing `jaaql-monitor-1.2.14/LICENSE.txt` & `jaaql-monitor-1.2.15/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.14/PKG-INFO` & `jaaql-monitor-1.2.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.14
+Version: 1.2.15
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.14/README.md` & `jaaql-monitor-1.2.15/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.14/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.15/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.14
+Version: 1.2.15
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.14/monitor/main.py` & `jaaql-monitor-1.2.15/monitor/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,26 +385,29 @@
         print_error(state, "Expected user without spaces, instead found spaces in user: '" + potential_user + "'")
     if not potential_user.startswith("@"):
         print_error(state, "Malformatted user, expected user to start with @")
 
     return potential_user.split("@")[1].split(" ")[0]
 
 
-def deal_with_input(state: State):
+def deal_with_input(state: State, file_content: str = None):
     if len(state.connections) == 0 and state.is_script():
         print_error(state, "Must supply credentials file as argument in script mode")
     if len(state.connections) != 0 and state.connections.get(DEFAULT_CONNECTION):
         state.set_current_connection(get_connection_info(state, DEFAULT_CONNECTION))  # Preloads the default connection
     elif not state.is_script():
         print(state, "Type jaaql url or \"file [config_file_location]\"")
         state.set_current_connection(handle_login(state, input("LOGIN>").strip()))
 
     if state.is_script():
         try:
-            state.file_lines = open(state.file_name, "r").readlines()
+            if file_content:
+                state.file_lines = file_content.replace("\r\n", "\n").split("\n")
+            else:
+                state.file_lines = open(state.file_name, "r").readlines()
             state.file_lines.append(EOFMarker())  # Ignore warning. We can have multiple types. This is python
         except FileNotFoundError as ex:
             print_error(state, "Could not load file for processing '" + state.file_name + "'")
         except Exception as ex:
             print_error(state, "Unhandled exception whilst processing file '" + state.file_name + "' " + str(ex))
 
     while True:
@@ -474,20 +477,23 @@
     if len(state.fetched_query) != 0:
         if state.single_query:
             on_go(state)
         else:
             print_error(state, "Attempting to quit with non-empty buffer. Please submit with \\g or clear with \\r")
 
 
-def initialise_from_args(args):
+def initialise_from_args(args, file_name: str = None, file_content: str = None):
     state = State()
 
-    file_name = [idx for arg, idx in zip(args, range(len(args))) if arg in ['-f', '--file']]
-    if len(file_name) != 0:
-        state.file_name = args[file_name[0] + 1]
+    if file_name is None:
+        file_name = [idx for arg, idx in zip(args, range(len(args))) if arg in ['-f', '--file']]
+        if len(file_name) != 0:
+            state.file_name = args[file_name[0] + 1]
+    else:
+        state.file_name = file_name
 
     state.is_verbose = len([arg for arg in args if arg in ['-v', '--verbose']]) != 0
     state.is_debugging = len([arg for arg in args if arg in ['-d', '--debugging']]) != 0
     state.single_query = len([arg for arg in args if arg in ['-s', '--single-query']]) != 0
 
     if state.is_verbose:
         print_version()
@@ -519,31 +525,31 @@
 
             db = None
             if len(content_split) == 4:
                 db = b64d(content_split[3])
 
             state.connection_info[configuration_name] = ConnectionInfo(b64d(content_split[0]), b64d(content_split[1]), b64d(content_split[2]), db)
 
-    deal_with_input(state)
+    deal_with_input(state, file_content)
 
 
-def initialise(file_name: str, configs: list[[str, str]], encoded_configs: list[[str, str, str, str, str | None]]):
-    args = ["-f", file_name, "-s"]
+def initialise(file_name: str, file_content: str, configs: list[[str, str]], encoded_configs: list[[str, str, str, str, str | None]]):
+    args = ["-s"]
 
     for config in configs:
         args.append("-c")
         args.append(config[0])
         args.append(config[1])
 
     for encoded_config in encoded_configs:
         args.append("-e")
         args.append(encoded_config[0])
         db_part = ""
         if encoded_config[4]:
             db_part = ":" + b64e(encoded_config[4]).decode()
         args.append(b64e(encoded_config[1]).decode() + ":" + b64e(encoded_config[2]).decode() + ":" + b64e(encoded_config[3]).decode() + db_part)
 
-    initialise_from_args(args)
+    initialise_from_args(args, file_name, file_content)
 
 
 if __name__ == "__main__":
     initialise_from_args(sys.argv[1:])
```

### Comparing `jaaql-monitor-1.2.14/setup.py` & `jaaql-monitor-1.2.15/setup.py`

 * *Files identical despite different names*

