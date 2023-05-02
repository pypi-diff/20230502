# Comparing `tmp/aiosow-0.1.tar.gz` & `tmp/aiosow-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosow-0.1.tar", last modified: Fri Apr 28 06:00:08 2023, max compression
+gzip compressed data, was "aiosow-0.1.2.tar", last modified: Tue May  2 11:13:50 2023, max compression
```

## Comparing `aiosow-0.1.tar` & `aiosow-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-28 06:00:08.390691 aiosow-0.1/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      125 2023-04-28 06:00:08.390691 aiosow-0.1/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8115 2023-04-27 12:46:26.000000 aiosow-0.1/README.md
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-28 06:00:08.390691 aiosow-0.1/aiosow/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       34 2023-03-22 07:46:41.000000 aiosow-0.1/aiosow/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4471 2023-04-27 12:46:26.000000 aiosow-0.1/aiosow/autofill.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    13356 2023-04-27 12:46:26.000000 aiosow-0.1/aiosow/bindings.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2898 2023-04-27 12:46:26.000000 aiosow-0.1/aiosow/command.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1974 2023-03-24 08:23:50.000000 aiosow-0.1/aiosow/http.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      827 2023-04-27 12:46:26.000000 aiosow-0.1/aiosow/options.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4001 2023-04-27 12:46:26.000000 aiosow-0.1/aiosow/perpetuate.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3629 2023-04-27 12:46:26.000000 aiosow-0.1/aiosow/routines.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1427 2023-04-27 12:46:26.000000 aiosow-0.1/aiosow/setup.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      305 2023-03-25 09:33:57.000000 aiosow-0.1/aiosow/shell.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      373 2023-04-26 12:14:34.000000 aiosow-0.1/aiosow/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-28 06:00:08.390691 aiosow-0.1/aiosow.egg-info/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      125 2023-04-28 06:00:08.000000 aiosow-0.1/aiosow.egg-info/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      571 2023-04-28 06:00:08.000000 aiosow-0.1/aiosow.egg-info/SOURCES.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-04-28 06:00:08.000000 aiosow-0.1/aiosow.egg-info/dependency_links.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       46 2023-04-28 06:00:08.000000 aiosow-0.1/aiosow.egg-info/entry_points.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       88 2023-04-28 06:00:08.000000 aiosow-0.1/aiosow.egg-info/requires.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        7 2023-04-28 06:00:08.000000 aiosow-0.1/aiosow.egg-info/top_level.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-04-28 06:00:08.390691 aiosow-0.1/setup.cfg
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      539 2023-04-28 05:59:53.000000 aiosow-0.1/setup.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-28 06:00:08.390691 aiosow-0.1/tests/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3253 2023-03-25 11:26:27.000000 aiosow-0.1/tests/test_autofill.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7291 2023-04-27 12:46:26.000000 aiosow-0.1/tests/test_bindings.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-03-22 07:46:41.000000 aiosow-0.1/tests/test_command.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      185 2023-03-22 07:46:41.000000 aiosow-0.1/tests/test_http.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      864 2023-03-25 11:37:11.000000 aiosow-0.1/tests/test_perpetuate.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1938 2023-04-27 12:46:26.000000 aiosow-0.1/tests/test_routines.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      653 2023-03-25 11:26:15.000000 aiosow-0.1/tests/test_setup.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      725 2023-03-22 07:46:41.000000 aiosow-0.1/tests/test_utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 11:13:50.315181 aiosow-0.1.2/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8293 2023-05-02 11:13:50.315181 aiosow-0.1.2/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8115 2023-04-27 12:46:26.000000 aiosow-0.1.2/README.md
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 11:13:50.315181 aiosow-0.1.2/aiosow/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       34 2023-03-22 07:46:41.000000 aiosow-0.1.2/aiosow/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4471 2023-04-27 12:46:26.000000 aiosow-0.1.2/aiosow/autofill.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    13356 2023-04-27 12:46:26.000000 aiosow-0.1.2/aiosow/bindings.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2898 2023-04-27 12:46:26.000000 aiosow-0.1.2/aiosow/command.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1974 2023-03-24 08:23:50.000000 aiosow-0.1.2/aiosow/http.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      827 2023-04-27 12:46:26.000000 aiosow-0.1.2/aiosow/options.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4014 2023-05-02 11:11:02.000000 aiosow-0.1.2/aiosow/perpetuate.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3629 2023-04-27 12:46:26.000000 aiosow-0.1.2/aiosow/routines.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1427 2023-04-27 12:46:26.000000 aiosow-0.1.2/aiosow/setup.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      373 2023-04-26 12:14:34.000000 aiosow-0.1.2/aiosow/utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 11:13:50.315181 aiosow-0.1.2/aiosow.egg-info/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8293 2023-05-02 11:13:50.000000 aiosow-0.1.2/aiosow.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      555 2023-05-02 11:13:50.000000 aiosow-0.1.2/aiosow.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-05-02 11:13:50.000000 aiosow-0.1.2/aiosow.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       46 2023-05-02 11:13:50.000000 aiosow-0.1.2/aiosow.egg-info/entry_points.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       69 2023-05-02 11:13:50.000000 aiosow-0.1.2/aiosow.egg-info/requires.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        7 2023-05-02 11:13:50.000000 aiosow-0.1.2/aiosow.egg-info/top_level.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-05-02 11:13:50.315181 aiosow-0.1.2/setup.cfg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      688 2023-05-02 11:12:19.000000 aiosow-0.1.2/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 11:13:50.315181 aiosow-0.1.2/tests/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3253 2023-03-25 11:26:27.000000 aiosow-0.1.2/tests/test_autofill.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7291 2023-04-27 12:46:26.000000 aiosow-0.1.2/tests/test_bindings.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-03-22 07:46:41.000000 aiosow-0.1.2/tests/test_command.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      185 2023-03-22 07:46:41.000000 aiosow-0.1.2/tests/test_http.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      864 2023-03-25 11:37:11.000000 aiosow-0.1.2/tests/test_perpetuate.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1938 2023-04-27 12:46:26.000000 aiosow-0.1.2/tests/test_routines.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      653 2023-03-25 11:26:15.000000 aiosow-0.1.2/tests/test_setup.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      725 2023-03-22 07:46:41.000000 aiosow-0.1.2/tests/test_utils.py
```

### Comparing `aiosow-0.1/README.md` & `aiosow-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `aiosow-0.1/aiosow/autofill.py` & `aiosow-0.1.2/aiosow/autofill.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1/aiosow/bindings.py` & `aiosow-0.1.2/aiosow/bindings.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1/aiosow/command.py` & `aiosow-0.1.2/aiosow/command.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1/aiosow/http.py` & `aiosow-0.1.2/aiosow/http.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1/aiosow/options.py` & `aiosow-0.1.2/aiosow/options.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1/aiosow/perpetuate.py` & `aiosow-0.1.2/aiosow/perpetuate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging, json
 import asyncio
-from typing import Callable, Any
+from typing import Callable, Any, Union
 from collections.abc import Iterable
 
 from aiosow.autofill import autofill
 
 ONS = {}
 
 
-def on(variable_name: str, condition: Callable | None = None, singularize=False):
+def on(variable_name: str, condition: Union[Callable, None] = None, singularize=False):
     """
     Decorator function that registers a function to be executed when a variable
     of specified name is perpetuated in memory.
 
     **Args**:
     - variable_name (str): Name of the event to listen to.
     - condition (Callable|None, optional): Callable object that takes the value
```

### Comparing `aiosow-0.1/aiosow/routines.py` & `aiosow-0.1.2/aiosow/routines.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1/aiosow/setup.py` & `aiosow-0.1.2/aiosow/setup.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1/aiosow.egg-info/SOURCES.txt` & `aiosow-0.1.2/aiosow.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 aiosow/bindings.py
 aiosow/command.py
 aiosow/http.py
 aiosow/options.py
 aiosow/perpetuate.py
 aiosow/routines.py
 aiosow/setup.py
-aiosow/shell.py
 aiosow/utils.py
 aiosow.egg-info/PKG-INFO
 aiosow.egg-info/SOURCES.txt
 aiosow.egg-info/dependency_links.txt
 aiosow.egg-info/entry_points.txt
 aiosow.egg-info/requires.txt
 aiosow.egg-info/top_level.txt
```

### Comparing `aiosow-0.1/tests/test_autofill.py` & `aiosow-0.1.2/tests/test_autofill.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1/tests/test_bindings.py` & `aiosow-0.1.2/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1/tests/test_perpetuate.py` & `aiosow-0.1.2/tests/test_perpetuate.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1/tests/test_routines.py` & `aiosow-0.1.2/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1/tests/test_setup.py` & `aiosow-0.1.2/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1/tests/test_utils.py` & `aiosow-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

