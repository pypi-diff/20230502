# Comparing `tmp/ewms-pilot-0.9.0.tar.gz` & `tmp/ewms-pilot-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ewms-pilot-0.9.0.tar", last modified: Fri Apr 28 21:12:54 2023, max compression
+gzip compressed data, was "ewms-pilot-0.9.1.tar", last modified: Fri Apr 28 21:48:37 2023, max compression
```

## Comparing `ewms-pilot-0.9.0.tar` & `ewms-pilot-0.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:12:54.487920 ewms-pilot-0.9.0/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-04-28 21:12:50.000000 ewms-pilot-0.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2459 2023-04-28 21:12:54.487920 ewms-pilot-0.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1352 2023-04-28 21:12:50.000000 ewms-pilot-0.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:12:54.487920 ewms-pilot-0.9.0/ewms_pilot/
--rw-r--r--   0 root         (0) root         (0)      683 2023-04-28 21:12:51.000000 ewms-pilot-0.9.0/ewms_pilot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1455 2023-04-28 21:12:50.000000 ewms-pilot-0.9.0/ewms_pilot/config.py
--rw-r--r--   0 root         (0) root         (0)    19678 2023-04-28 21:12:50.000000 ewms-pilot-0.9.0/ewms_pilot/pilot.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:12:50.000000 ewms-pilot-0.9.0/ewms_pilot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:12:54.487920 ewms-pilot-0.9.0/ewms_pilot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2459 2023-04-28 21:12:54.000000 ewms-pilot-0.9.0/ewms_pilot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      289 2023-04-28 21:12:54.000000 ewms-pilot-0.9.0/ewms_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 21:12:54.000000 ewms-pilot-0.9.0/ewms_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      186 2023-04-28 21:12:54.000000 ewms-pilot-0.9.0/ewms_pilot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-28 21:12:54.000000 ewms-pilot-0.9.0/ewms_pilot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1938 2023-04-28 21:12:54.487920 ewms-pilot-0.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-28 21:12:50.000000 ewms-pilot-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:48:37.995358 ewms-pilot-0.9.1/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-04-28 21:48:35.000000 ewms-pilot-0.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-04-28 21:48:37.995358 ewms-pilot-0.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-04-28 21:48:35.000000 ewms-pilot-0.9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:48:37.991358 ewms-pilot-0.9.1/ewms_pilot/
+-rw-r--r--   0 root         (0) root         (0)      683 2023-04-28 21:48:36.000000 ewms-pilot-0.9.1/ewms_pilot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-04-28 21:48:35.000000 ewms-pilot-0.9.1/ewms_pilot/config.py
+-rw-r--r--   0 root         (0) root         (0)    19678 2023-04-28 21:48:35.000000 ewms-pilot-0.9.1/ewms_pilot/pilot.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 21:48:35.000000 ewms-pilot-0.9.1/ewms_pilot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:48:37.995358 ewms-pilot-0.9.1/ewms_pilot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2459 2023-04-28 21:48:37.000000 ewms-pilot-0.9.1/ewms_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      289 2023-04-28 21:48:37.000000 ewms-pilot-0.9.1/ewms_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 21:48:37.000000 ewms-pilot-0.9.1/ewms_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      186 2023-04-28 21:48:37.000000 ewms-pilot-0.9.1/ewms_pilot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-28 21:48:37.000000 ewms-pilot-0.9.1/ewms_pilot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-04-28 21:48:37.995358 ewms-pilot-0.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-28 21:48:35.000000 ewms-pilot-0.9.1/setup.py
```

### Comparing `ewms-pilot-0.9.0/LICENSE` & `ewms-pilot-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ewms-pilot-0.9.0/PKG-INFO` & `ewms-pilot-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewms-pilot
-Version: 0.9.0
+Version: 0.9.1
 Summary: EWMS Pilot: MQ-Task Interface API
 Home-page: https://github.com/Observation-Management-Service/ewms-pilot
 Download-URL: https://pypi.org/project/ewms-pilot/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/ewms-pilot/issues
```

### Comparing `ewms-pilot-0.9.0/README.md` & `ewms-pilot-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ewms-pilot-0.9.0/ewms_pilot/__init__.py` & `ewms-pilot-0.9.1/ewms_pilot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 __all__ = [
     "consume_and_reply",
     "FileType",
 ]
 
 # version is a human-readable version number.
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
 version_info = (
```

### Comparing `ewms-pilot-0.9.0/ewms_pilot/config.py` & `ewms-pilot-0.9.1/ewms_pilot/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,11 +42,11 @@
             )
             if self.EWMS_PILOT_TASK_TIMEOUT is not None:
                 LOGGER.warning(
                     "Ignoring 'EWMS_PILOT_SUBPROC_TIMEOUT' since 'EWMS_PILOT_TASK_TIMEOUT' was provided."
                 )
             else:
                 # b/c frozen
-                object.__setattr__(self, "EWMS_PILOT_TASK_TIMEOUT", timeout)
+                object.__setattr__(self, "EWMS_PILOT_TASK_TIMEOUT", int(timeout))
 
 
 ENV = from_environment_as_dataclass(EnvConfig)
```

### Comparing `ewms-pilot-0.9.0/ewms_pilot/pilot.py` & `ewms-pilot-0.9.1/ewms_pilot/pilot.py`

 * *Files identical despite different names*

### Comparing `ewms-pilot-0.9.0/ewms_pilot.egg-info/PKG-INFO` & `ewms-pilot-0.9.1/ewms_pilot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewms-pilot
-Version: 0.9.0
+Version: 0.9.1
 Summary: EWMS Pilot: MQ-Task Interface API
 Home-page: https://github.com/Observation-Management-Service/ewms-pilot
 Download-URL: https://pypi.org/project/ewms-pilot/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/ewms-pilot/issues
```

### Comparing `ewms-pilot-0.9.0/setup.cfg` & `ewms-pilot-0.9.1/setup.cfg`

 * *Files identical despite different names*

