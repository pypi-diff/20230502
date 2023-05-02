# Comparing `tmp/vedirect-1.0.0.tar.gz` & `tmp/vedirect-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vedirect-1.0.0.tar", last modified: Tue Apr 18 17:43:54 2023, max compression
+gzip compressed data, was "dist/vedirect-1.1.0.tar", last modified: Tue May  2 19:23:24 2023, max compression
```

## Comparing `vedirect-1.0.0.tar` & `vedirect-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:43:54.000000 vedirect-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-18 17:43:54.000000 vedirect-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-18 17:43:49.000000 vedirect-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 17:43:54.000000 vedirect-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-18 17:43:49.000000 vedirect-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:43:54.000000 vedirect-1.0.0/vedirect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-18 17:43:54.000000 vedirect-1.0.0/vedirect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-18 17:43:54.000000 vedirect-1.0.0/vedirect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:43:54.000000 vedirect-1.0.0/vedirect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 17:43:54.000000 vedirect-1.0.0/vedirect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 17:43:54.000000 vedirect-1.0.0/vedirect.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2994 2023-04-18 17:43:49.000000 vedirect-1.0.0/vedirect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:23:24.000000 vedirect-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-02 19:23:24.000000 vedirect-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-02 19:23:16.000000 vedirect-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:23:24.000000 vedirect-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-02 19:23:16.000000 vedirect-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:23:24.000000 vedirect-1.1.0/vedirect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-02 19:23:24.000000 vedirect-1.1.0/vedirect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-02 19:23:24.000000 vedirect-1.1.0/vedirect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:23:24.000000 vedirect-1.1.0/vedirect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 19:23:24.000000 vedirect-1.1.0/vedirect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 19:23:24.000000 vedirect-1.1.0/vedirect.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2906 2023-05-02 19:23:16.000000 vedirect-1.1.0/vedirect.py
```

### Comparing `vedirect-1.0.0/PKG-INFO` & `vedirect-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedirect
-Version: 1.0.0
+Version: 1.1.0
 Summary: Interfaces with Victron VE.Direct devices
 Home-page: http://github.com/Frankkkkk/python-vedirect
 Author: Frank Villaro-Dixon
 Author-email: frank@villaro-dixon.eu
 License: MIT
 Keywords: victron vedirect ve.direct ve direct mppt
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `vedirect-1.0.0/README.md` & `vedirect-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vedirect-1.0.0/setup.py` & `vedirect-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="vedirect",
-    version="1.0.0",
+    version="1.1.0",
     author="Frank Villaro-Dixon",
     author_email="frank@villaro-dixon.eu",
     description=("Interfaces with Victron VE.Direct devices"),
     license="MIT",
     keywords="victron vedirect ve.direct ve direct mppt",
     url="http://github.com/Frankkkkk/python-vedirect",
     py_modules=['vedirect'],
```

### Comparing `vedirect-1.0.0/vedirect.egg-info/PKG-INFO` & `vedirect-1.1.0/vedirect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedirect
-Version: 1.0.0
+Version: 1.1.0
 Summary: Interfaces with Victron VE.Direct devices
 Home-page: http://github.com/Frankkkkk/python-vedirect
 Author: Frank Villaro-Dixon
 Author-email: frank@villaro-dixon.eu
 License: MIT
 Keywords: victron vedirect ve.direct ve direct mppt
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `vedirect-1.0.0/vedirect.py` & `vedirect-1.1.0/vedirect.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,16 +44,14 @@
             self._data[key] = value
 
 
     def _get_data(self) -> list[bytes]:
         ''' Returns a PDU array, one entry per line.'''
         data = []
         with serial.Serial(self.device, self.speed, timeout=4) as s:
-        #with open('example.pdu', 'rb') as f:
-            s = open('example.pdu', 'rb')
             # Wait for start of frame
             while True:
                 frame = s.readline()
                 if frame.startswith(b'PID'):
                     break
 
             # slurp all frames
```

