# Comparing `tmp/jaaql-monitor-1.2.20.tar.gz` & `tmp/jaaql-monitor-1.2.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.20.tar", last modified: Tue May  2 21:12:03 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.21.tar", last modified: Tue May  2 21:21:58 2023, max compression
```

## Comparing `jaaql-monitor-1.2.20.tar` & `jaaql-monitor-1.2.21.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:03.260475 jaaql-monitor-1.2.20/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.20/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-02 21:12:03.259477 jaaql-monitor-1.2.20/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.20/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:03.256474 jaaql-monitor-1.2.20/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-02 21:12:03.000000 jaaql-monitor-1.2.20/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-02 21:12:03.000000 jaaql-monitor-1.2.20/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 21:12:03.000000 jaaql-monitor-1.2.20/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 21:12:03.000000 jaaql-monitor-1.2.20/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 21:12:03.000000 jaaql-monitor-1.2.20/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 21:12:03.258476 jaaql-monitor-1.2.20/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.20/monitor/__init__.py
--rw-rw-rw-   0        0        0    23272 2023-05-02 21:11:50.000000 jaaql-monitor-1.2.20/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-02 21:11:51.000000 jaaql-monitor-1.2.20/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-02 21:12:03.260475 jaaql-monitor-1.2.20/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:21:58.549842 jaaql-monitor-1.2.21/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.21/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-02 21:21:58.549842 jaaql-monitor-1.2.21/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.21/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 21:21:58.545820 jaaql-monitor-1.2.21/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-02 21:21:58.000000 jaaql-monitor-1.2.21/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-02 21:21:58.000000 jaaql-monitor-1.2.21/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 21:21:58.000000 jaaql-monitor-1.2.21/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 21:21:58.000000 jaaql-monitor-1.2.21/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 21:21:58.000000 jaaql-monitor-1.2.21/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 21:21:58.548818 jaaql-monitor-1.2.21/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.21/monitor/__init__.py
+-rw-rw-rw-   0        0        0    23274 2023-05-02 21:19:12.000000 jaaql-monitor-1.2.21/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-02 21:21:45.000000 jaaql-monitor-1.2.21/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-02 21:21:58.550817 jaaql-monitor-1.2.21/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.21/setup.py
```

### Comparing `jaaql-monitor-1.2.20/LICENSE.txt` & `jaaql-monitor-1.2.21/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.20/PKG-INFO` & `jaaql-monitor-1.2.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.20
+Version: 1.2.21
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.20/README.md` & `jaaql-monitor-1.2.21/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.20/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.21/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.20
+Version: 1.2.21
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.20/monitor/main.py` & `jaaql-monitor-1.2.21/monitor/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 ARGS__encoded_config = ['-e', '--encoded-config']
 ARGS__config = ['-c', '--config']
 
 
 class JAAQLMonitorException(Exception):
     def __init__(self, *args, **kwargs):
-        super.__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
 
 class EOFMarker:
     pass
 
 
 class ConnectionInfo:
```

### Comparing `jaaql-monitor-1.2.20/setup.py` & `jaaql-monitor-1.2.21/setup.py`

 * *Files identical despite different names*

