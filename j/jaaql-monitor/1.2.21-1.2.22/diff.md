# Comparing `tmp/jaaql-monitor-1.2.21.tar.gz` & `tmp/jaaql-monitor-1.2.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.21.tar", last modified: Tue May  2 21:21:58 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.22.tar", last modified: Tue May  2 21:39:27 2023, max compression
```

## Comparing `jaaql-monitor-1.2.21.tar` & `jaaql-monitor-1.2.22.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 21:21:58.549842 jaaql-monitor-1.2.21/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.21/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-02 21:21:58.549842 jaaql-monitor-1.2.21/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.21/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 21:21:58.545820 jaaql-monitor-1.2.21/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-02 21:21:58.000000 jaaql-monitor-1.2.21/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-02 21:21:58.000000 jaaql-monitor-1.2.21/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 21:21:58.000000 jaaql-monitor-1.2.21/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 21:21:58.000000 jaaql-monitor-1.2.21/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 21:21:58.000000 jaaql-monitor-1.2.21/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 21:21:58.548818 jaaql-monitor-1.2.21/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.21/monitor/__init__.py
--rw-rw-rw-   0        0        0    23274 2023-05-02 21:19:12.000000 jaaql-monitor-1.2.21/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-02 21:21:45.000000 jaaql-monitor-1.2.21/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-02 21:21:58.550817 jaaql-monitor-1.2.21/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:39:27.874698 jaaql-monitor-1.2.22/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.22/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-02 21:39:27.874698 jaaql-monitor-1.2.22/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.22/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 21:39:27.867696 jaaql-monitor-1.2.22/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-02 21:39:27.000000 jaaql-monitor-1.2.22/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-02 21:39:27.000000 jaaql-monitor-1.2.22/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 21:39:27.000000 jaaql-monitor-1.2.22/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 21:39:27.000000 jaaql-monitor-1.2.22/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 21:39:27.000000 jaaql-monitor-1.2.22/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 21:39:27.872700 jaaql-monitor-1.2.22/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.22/monitor/__init__.py
+-rw-rw-rw-   0        0        0    23300 2023-05-02 21:38:55.000000 jaaql-monitor-1.2.22/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-02 21:39:10.000000 jaaql-monitor-1.2.22/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-02 21:39:27.875697 jaaql-monitor-1.2.22/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.22/setup.py
```

### Comparing `jaaql-monitor-1.2.21/LICENSE.txt` & `jaaql-monitor-1.2.22/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.21/PKG-INFO` & `jaaql-monitor-1.2.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.21
+Version: 1.2.22
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.21/README.md` & `jaaql-monitor-1.2.22/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.21/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.22/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.21
+Version: 1.2.22
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.21/monitor/main.py` & `jaaql-monitor-1.2.22/monitor/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
     elif not state.is_script():
         print(state, "Type jaaql url or \"file [config_file_location]\"")
         state.set_current_connection(handle_login(state, input("LOGIN>").strip()))
 
     if state.is_script():
         try:
             if file_content:
-                state.file_lines = file_content.replace("\r\n", "\n").split("\n")
+                state.file_lines = [line + "\n" for line in file_content.replace("\r\n", "\n").split("\n")]
             else:
                 state.file_lines = open(state.file_name, "r").readlines()
             state.file_lines.append(EOFMarker())  # Ignore warning. We can have multiple types. This is python
         except FileNotFoundError as ex:
             print_error(state, "Could not load file for processing '" + state.file_name + "'")
         except Exception as ex:
             print_error(state, "Unhandled exception whilst processing file '" + state.file_name + "' " + str(ex))
```

### Comparing `jaaql-monitor-1.2.21/setup.py` & `jaaql-monitor-1.2.22/setup.py`

 * *Files identical despite different names*

