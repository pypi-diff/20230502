# Comparing `tmp/jaaql-monitor-1.2.16.tar.gz` & `tmp/jaaql-monitor-1.2.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.16.tar", last modified: Tue May  2 12:48:59 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.17.tar", last modified: Tue May  2 13:02:41 2023, max compression
```

## Comparing `jaaql-monitor-1.2.16.tar` & `jaaql-monitor-1.2.17.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 12:48:59.170497 jaaql-monitor-1.2.16/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.16/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-02 12:48:59.169497 jaaql-monitor-1.2.16/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.16/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 12:48:59.166494 jaaql-monitor-1.2.16/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-02 12:48:59.000000 jaaql-monitor-1.2.16/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-02 12:48:59.000000 jaaql-monitor-1.2.16/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 12:48:59.000000 jaaql-monitor-1.2.16/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 12:48:59.000000 jaaql-monitor-1.2.16/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 12:48:59.000000 jaaql-monitor-1.2.16/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 12:48:59.168496 jaaql-monitor-1.2.16/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.16/monitor/__init__.py
--rw-rw-rw-   0        0        0    22740 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.16/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-02 12:48:47.000000 jaaql-monitor-1.2.16/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-02 12:48:59.170497 jaaql-monitor-1.2.16/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:02:41.206868 jaaql-monitor-1.2.17/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.17/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-02 13:02:41.206868 jaaql-monitor-1.2.17/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.17/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 13:02:41.201854 jaaql-monitor-1.2.17/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-02 13:02:41.000000 jaaql-monitor-1.2.17/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-02 13:02:41.000000 jaaql-monitor-1.2.17/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 13:02:41.000000 jaaql-monitor-1.2.17/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 13:02:41.000000 jaaql-monitor-1.2.17/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 13:02:41.000000 jaaql-monitor-1.2.17/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 13:02:41.204851 jaaql-monitor-1.2.17/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.17/monitor/__init__.py
+-rw-rw-rw-   0        0        0    22771 2023-05-02 13:02:23.000000 jaaql-monitor-1.2.17/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-02 13:02:26.000000 jaaql-monitor-1.2.17/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-02 13:02:41.206868 jaaql-monitor-1.2.17/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.17/setup.py
```

### Comparing `jaaql-monitor-1.2.16/LICENSE.txt` & `jaaql-monitor-1.2.17/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.16/PKG-INFO` & `jaaql-monitor-1.2.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.16
+Version: 1.2.17
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.16/README.md` & `jaaql-monitor-1.2.17/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.16/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.17/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.16
+Version: 1.2.17
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.16/monitor/main.py` & `jaaql-monitor-1.2.17/monitor/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
             print_error(state, "Could not find named credentials file '" + connection_name + "' located at '" + file_name +
                         "', using working directory " + os.getcwd())
 
 
 def format_output_row(data, max_length, data_types, breaches):
     builder = ""
     for col, the_length, data_type, did_breach in zip(data, max_length, data_types, breaches):
-        col_str = str(col)
+        col_str = str(col) if col is not None else "null"
         builder += "|"
         spacing = "".join([" "] * max(the_length - len(col_str), 0))
         if did_breach and len(col_str) > the_length:
             col_str = col_str[0:min(the_length, len(col_str)) - 3]
             col_str += "..."
         else:
             col_str = col_str[0:min(the_length, len(col_str))]
```

### Comparing `jaaql-monitor-1.2.16/setup.py` & `jaaql-monitor-1.2.17/setup.py`

 * *Files identical despite different names*

