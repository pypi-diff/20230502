# Comparing `tmp/local-logger-python-backend-0.0.1.tar.gz` & `tmp/local-logger-python-backend-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local-logger-python-backend-0.0.1.tar", last modified: Thu Apr 27 21:38:00 2023, max compression
+gzip compressed data, was "local-logger-python-backend-0.0.2.tar", last modified: Tue May  2 18:32:29 2023, max compression
```

## Comparing `local-logger-python-backend-0.0.1.tar` & `local-logger-python-backend-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:38:00.877240 local-logger-python-backend-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:38:00.877240 local-logger-python-backend-0.0.1/CirclesLocalLoggerPython/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-27 21:37:46.000000 local-logger-python-backend-0.0.1/CirclesLocalLoggerPython/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-27 21:37:46.000000 local-logger-python-backend-0.0.1/CirclesLocalLoggerPython/LoggerServiceSingleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-27 21:37:46.000000 local-logger-python-backend-0.0.1/CirclesLocalLoggerPython/MessageSeverity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-27 21:37:46.000000 local-logger-python-backend-0.0.1/CirclesLocalLoggerPython/Writer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:37:46.000000 local-logger-python-backend-0.0.1/CirclesLocalLoggerPython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-27 21:37:46.000000 local-logger-python-backend-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 21:38:00.877240 local-logger-python-backend-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 21:37:46.000000 local-logger-python-backend-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:38:00.877240 local-logger-python-backend-0.0.1/local_logger_python_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-27 21:38:00.000000 local-logger-python-backend-0.0.1/local_logger_python_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 21:38:00.000000 local-logger-python-backend-0.0.1/local_logger_python_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:38:00.000000 local-logger-python-backend-0.0.1/local_logger_python_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 21:38:00.000000 local-logger-python-backend-0.0.1/local_logger_python_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 21:38:00.000000 local-logger-python-backend-0.0.1/local_logger_python_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-27 21:37:46.000000 local-logger-python-backend-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 21:38:00.877240 local-logger-python-backend-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-27 21:37:46.000000 local-logger-python-backend-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:38:00.877240 local-logger-python-backend-0.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-27 21:37:46.000000 local-logger-python-backend-0.0.1/src/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-27 21:37:46.000000 local-logger-python-backend-0.0.1/src/LoggerServiceSingleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-27 21:37:46.000000 local-logger-python-backend-0.0.1/src/MessageSeverity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-27 21:37:46.000000 local-logger-python-backend-0.0.1/src/Writer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:37:46.000000 local-logger-python-backend-0.0.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:32:29.622350 local-logger-python-backend-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:32:29.622350 local-logger-python-backend-0.0.2/CirclesLocalLoggerPython/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/CirclesLocalLoggerPython/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/CirclesLocalLoggerPython/LoggerServiceSingleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/CirclesLocalLoggerPython/MessageSeverity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/CirclesLocalLoggerPython/Writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/CirclesLocalLoggerPython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/CirclesLocalLoggerPython/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-02 18:32:29.622350 local-logger-python-backend-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:32:29.622350 local-logger-python-backend-0.0.2/local_logger_python_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-02 18:32:29.000000 local-logger-python-backend-0.0.2/local_logger_python_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-02 18:32:29.000000 local-logger-python-backend-0.0.2/local_logger_python_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:32:29.000000 local-logger-python-backend-0.0.2/local_logger_python_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-02 18:32:29.000000 local-logger-python-backend-0.0.2/local_logger_python_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 18:32:29.622350 local-logger-python-backend-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:32:29.622350 local-logger-python-backend-0.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/src/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/src/LoggerServiceSingleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/src/MessageSeverity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/src/Writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 18:32:16.000000 local-logger-python-backend-0.0.2/src/__init__.py
```

### Comparing `local-logger-python-backend-0.0.1/CirclesLocalLoggerPython/LoggerService.py` & `local-logger-python-backend-0.0.2/src/LoggerService.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
-from CirclesLocalLoggerPython.MessageSeverity import MessageSeverity
-from CirclesLocalLoggerPython.Writer import Writer
+from src.MessageSeverity import MessageSeverity
+from src.Writer import Writer
 from mysql.connector.pooling import MySQLConnectionPool
 
 
 class LoggerService:
 
     def __init__(self):
         self._pool = MySQLConnectionPool(
@@ -51,9 +51,8 @@
 
     def verbose(self, *args, **kwargs):
         if args:
             self._writer.add_message(args[0], MessageSeverity.Verbose.value)
         else:
             if 'object' in kwargs:
                 kwargs['object']['severity_id'] = MessageSeverity.Verbose.value
-                self._writer.add(**kwargs)
-
+                self._writer.add(**kwargs)
```

### Comparing `local-logger-python-backend-0.0.1/CirclesLocalLoggerPython/Writer.py` & `local-logger-python-backend-0.0.2/src/Writer.py`

 * *Files identical despite different names*

### Comparing `local-logger-python-backend-0.0.1/LICENSE` & `local-logger-python-backend-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `local-logger-python-backend-0.0.1/local_logger_python_backend.egg-info/SOURCES.txt` & `local-logger-python-backend-0.0.2/local_logger_python_backend.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 pyproject.toml
 setup.py
 CirclesLocalLoggerPython/LoggerService.py
 CirclesLocalLoggerPython/LoggerServiceSingleton.py
 CirclesLocalLoggerPython/MessageSeverity.py
 CirclesLocalLoggerPython/Writer.py
 CirclesLocalLoggerPython/__init__.py
+CirclesLocalLoggerPython/test_writer.py
 local_logger_python_backend.egg-info/PKG-INFO
 local_logger_python_backend.egg-info/SOURCES.txt
 local_logger_python_backend.egg-info/dependency_links.txt
-local_logger_python_backend.egg-info/requires.txt
 local_logger_python_backend.egg-info/top_level.txt
 src/LoggerService.py
 src/LoggerServiceSingleton.py
 src/MessageSeverity.py
 src/Writer.py
 src/__init__.py
```

### Comparing `local-logger-python-backend-0.0.1/src/LoggerService.py` & `local-logger-python-backend-0.0.2/CirclesLocalLoggerPython/LoggerService.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
-from src.MessageSeverity import MessageSeverity
-from src.Writer import Writer
+from CirclesLocalLoggerPython.MessageSeverity import MessageSeverity
+from CirclesLocalLoggerPython.Writer import Writer
 from mysql.connector.pooling import MySQLConnectionPool
+from dotenv import load_dotenv
+load_dotenv()
 
 
 class LoggerService:
 
     def __init__(self):
         self._pool = MySQLConnectionPool(
             user=os.getenv('RDS_USERNAME'),
@@ -13,14 +15,17 @@
             host=os.getenv('RDS_HOSTNAME'),
             database=os.getenv('RDS_DB_NAME'),
             pool_name="loggerPool",
             pool_size=5
         )
         self._writer = Writer(self._pool)
 
+    def get_pool(self):
+        return self._pool
+
     def log(self, *args, **kwargs):
         if args:
             self._writer.add_message(args[0], MessageSeverity.Information.value)
         else:
             if 'object' in kwargs:
                 kwargs['object']['severity_id'] = MessageSeverity.Information.value
                 self._writer.add(**kwargs)
@@ -51,8 +56,9 @@
 
     def verbose(self, *args, **kwargs):
         if args:
             self._writer.add_message(args[0], MessageSeverity.Verbose.value)
         else:
             if 'object' in kwargs:
                 kwargs['object']['severity_id'] = MessageSeverity.Verbose.value
-                self._writer.add(**kwargs)
+                self._writer.add(**kwargs)
+
```

### Comparing `local-logger-python-backend-0.0.1/src/Writer.py` & `local-logger-python-backend-0.0.2/CirclesLocalLoggerPython/Writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
         try:
             params_to_insert = kwargs['object']
             # creating connection
             connection = self._pool.get_connection()
             cursor = connection.cursor()
             cursor.execute(
-                f"insert into location.location_table (coordinate) values (POINT({params_to_insert['latitude']},{params_to_insert['longitude']}));")
+                f"insert into location.location_table (coordinate) values (POINT({params_to_insert['latitude'] if params_to_insert['latitude'] != None else 0},{params_to_insert['longitude'] if params_to_insert['longitude'] != None else 0}));")
             coordinate_id = cursor.lastrowid
             params_to_insert.pop('latitude')
             params_to_insert.pop('longitude')
             params_to_insert['location_id'] = coordinate_id
             listed_values = list(params_to_insert.values())
             joined_keys = ','.join(list(params_to_insert.keys()))
             generate_values_pattern = ','.join(['%s' for i in range(len(listed_values))])
```

