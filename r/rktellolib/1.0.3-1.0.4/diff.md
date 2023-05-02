# Comparing `tmp/rktellolib-1.0.3.tar.gz` & `tmp/rktellolib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rktellolib-1.0.3.tar", last modified: Sat Mar 13 01:16:41 2021, max compression
+gzip compressed data, was "rktellolib-1.0.4.tar", last modified: Tue May  2 06:51:59 2023, max compression
```

## Comparing `rktellolib-1.0.3.tar` & `rktellolib-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 ramsin     (501) staff       (20)        0 2021-03-13 01:16:41.207040 rktellolib-1.0.3/
--rw-r--r--   0 ramsin     (501) staff       (20)     3948 2021-03-13 01:16:41.207306 rktellolib-1.0.3/PKG-INFO
--rw-r--r--   0 ramsin     (501) staff       (20)     2086 2021-02-24 01:30:27.000000 rktellolib-1.0.3/README.md
-drwxr-xr-x   0 ramsin     (501) staff       (20)        0 2021-03-13 01:16:41.204890 rktellolib-1.0.3/rktellolib/
--rw-r--r--   0 ramsin     (501) staff       (20)     4985 2021-03-13 01:06:44.000000 rktellolib-1.0.3/rktellolib/Tello.py
--rw-r--r--   0 ramsin     (501) staff       (20)     2549 2021-02-23 01:56:56.000000 rktellolib-1.0.3/rktellolib/TelloCam.py
--rw-r--r--   0 ramsin     (501) staff       (20)     5008 2021-03-13 00:30:55.000000 rktellolib-1.0.3/rktellolib/TelloCommand.py
--rw-r--r--   0 ramsin     (501) staff       (20)     2930 2021-02-24 01:34:39.000000 rktellolib-1.0.3/rktellolib/TelloState.py
--rw-r--r--   0 ramsin     (501) staff       (20)      129 2021-02-23 06:53:17.000000 rktellolib-1.0.3/rktellolib/__init__.py
-drwxr-xr-x   0 ramsin     (501) staff       (20)        0 2021-03-13 01:16:41.206675 rktellolib-1.0.3/rktellolib.egg-info/
--rw-r--r--   0 ramsin     (501) staff       (20)     3948 2021-03-13 01:16:41.000000 rktellolib-1.0.3/rktellolib.egg-info/PKG-INFO
--rw-r--r--   0 ramsin     (501) staff       (20)      315 2021-03-13 01:16:41.000000 rktellolib-1.0.3/rktellolib.egg-info/SOURCES.txt
--rw-r--r--   0 ramsin     (501) staff       (20)        1 2021-03-13 01:16:41.000000 rktellolib-1.0.3/rktellolib.egg-info/dependency_links.txt
--rw-r--r--   0 ramsin     (501) staff       (20)       14 2021-03-13 01:16:41.000000 rktellolib-1.0.3/rktellolib.egg-info/requires.txt
--rw-r--r--   0 ramsin     (501) staff       (20)       11 2021-03-13 01:16:41.000000 rktellolib-1.0.3/rktellolib.egg-info/top_level.txt
--rw-r--r--   0 ramsin     (501) staff       (20)       79 2021-03-13 01:16:41.208154 rktellolib-1.0.3/setup.cfg
--rw-r--r--   0 ramsin     (501) staff       (20)     1218 2021-02-24 01:49:35.000000 rktellolib-1.0.3/setup.py
+drwxr-xr-x   0 ramsin     (501) staff       (20)        0 2023-05-02 06:51:59.505339 rktellolib-1.0.4/
+-rw-r--r--   0 ramsin     (501) staff       (20)     1062 2023-05-02 04:35:17.000000 rktellolib-1.0.4/License.txt
+-rw-r--r--   0 ramsin     (501) staff       (20)     3889 2023-05-02 06:51:59.505213 rktellolib-1.0.4/PKG-INFO
+-rw-r--r--   0 ramsin     (501) staff       (20)     2086 2023-05-02 04:35:17.000000 rktellolib-1.0.4/README.md
+-rw-r--r--   0 ramsin     (501) staff       (20)      842 2023-05-02 06:47:49.000000 rktellolib-1.0.4/pyproject.toml
+-rw-r--r--   0 ramsin     (501) staff       (20)       38 2023-05-02 06:51:59.505388 rktellolib-1.0.4/setup.cfg
+drwxr-xr-x   0 ramsin     (501) staff       (20)        0 2023-05-02 06:51:59.503418 rktellolib-1.0.4/src/
+drwxr-xr-x   0 ramsin     (501) staff       (20)        0 2023-05-02 06:51:59.504402 rktellolib-1.0.4/src/rktellolib/
+-rw-r--r--   0 ramsin     (501) staff       (20)     5168 2023-05-02 04:35:17.000000 rktellolib-1.0.4/src/rktellolib/Tello.py
+-rw-r--r--   0 ramsin     (501) staff       (20)     2549 2023-05-02 04:35:17.000000 rktellolib-1.0.4/src/rktellolib/TelloCam.py
+-rw-r--r--   0 ramsin     (501) staff       (20)     5008 2023-05-02 04:35:17.000000 rktellolib-1.0.4/src/rktellolib/TelloCommand.py
+-rw-r--r--   0 ramsin     (501) staff       (20)     3163 2023-05-02 04:35:17.000000 rktellolib-1.0.4/src/rktellolib/TelloState.py
+-rw-r--r--   0 ramsin     (501) staff       (20)      129 2023-05-02 04:35:17.000000 rktellolib-1.0.4/src/rktellolib/__init__.py
+drwxr-xr-x   0 ramsin     (501) staff       (20)        0 2023-05-02 06:51:59.505016 rktellolib-1.0.4/src/rktellolib.egg-info/
+-rw-r--r--   0 ramsin     (501) staff       (20)     3889 2023-05-02 06:51:59.000000 rktellolib-1.0.4/src/rktellolib.egg-info/PKG-INFO
+-rw-r--r--   0 ramsin     (501) staff       (20)      363 2023-05-02 06:51:59.000000 rktellolib-1.0.4/src/rktellolib.egg-info/SOURCES.txt
+-rw-r--r--   0 ramsin     (501) staff       (20)        1 2023-05-02 06:51:59.000000 rktellolib-1.0.4/src/rktellolib.egg-info/dependency_links.txt
+-rw-r--r--   0 ramsin     (501) staff       (20)       20 2023-05-02 06:51:59.000000 rktellolib-1.0.4/src/rktellolib.egg-info/requires.txt
+-rw-r--r--   0 ramsin     (501) staff       (20)       11 2023-05-02 06:51:59.000000 rktellolib-1.0.4/src/rktellolib.egg-info/top_level.txt
```

### Comparing `rktellolib-1.0.3/README.md` & `rktellolib-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rktellolib-1.0.3/rktellolib/Tello.py` & `rktellolib-1.0.4/src/rktellolib/Tello.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from rktellolib.TelloCommand import TelloCommand
 from rktellolib.TelloState import TelloState
 from rktellolib.TelloCam import TelloCam
+from typing import Callable
 
 """
 Class Description:
   Tello is the primary interface to interact with the Tello drone.
   It utilizes the three classes TelloCommand, TelloState, and TelloCam to provide interfaces with the drone.
 Public Attributes: None
 Public Methods:
@@ -25,20 +26,21 @@
   __cam = None          # the TelloCam object to retrieve video streams
 
   __has_video = False   # boolean flag for using the video stream or not
   __is_flying = False   # boolean flag to determine is the drone is flying or not
 
   """
   Constructor that instantiates the needed objects
+  Argument: state_callback - A Callable that will receive the drone state on a separate thread 
   """
-  def __init__(self, debug: bool=False, has_video: bool=False):
+  def __init__(self, debug: bool=False, has_video: bool=False, state_callback: Callable[[str],None]=None):
     self.__has_video = has_video
 
     self.__command = TelloCommand(debug)
-    self.__state = TelloState(debug)
+    self.__state = TelloState(debug, state_callback)
 
     if has_video:
       self.__cam = TelloCam()
 
   """
   Operational commands
   """
```

### Comparing `rktellolib-1.0.3/rktellolib/TelloCam.py` & `rktellolib-1.0.4/src/rktellolib/TelloCam.py`

 * *Files identical despite different names*

### Comparing `rktellolib-1.0.3/rktellolib/TelloCommand.py` & `rktellolib-1.0.4/src/rktellolib/TelloCommand.py`

 * *Files identical despite different names*

### Comparing `rktellolib-1.0.3/rktellolib/TelloState.py` & `rktellolib-1.0.4/src/rktellolib/TelloState.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 import socket
 from threading import Thread
+from typing import Callable
 
 """
 Class Description:
   TelloCommand is a utility class to receive state information from the Tello drone.
 Public Attributes: None
 Public Methods:
   - start # start the drone communication
@@ -21,25 +22,28 @@
   __thread_started = False # Flag to determine if the thread is running
 
   __current_state = None   # String containing the most recent Tello state response (or None)
 
   """
   Constructor that creates the thread to receive responses
   """
-  def __init__(self, debug: bool=True):
+  def __init__(self, debug: bool=True, callback: Callable[[str],None]=None):
     self.__debug = debug
 
     # Open local UDP port for Tello communication
     self.__socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     self.__socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
     self.__socket.bind(('', self.__PORT))
 
     # Bind the thread to receive responses from the drone
     self.__thread = Thread(target=self.__thread_function, daemon=True)
 
+    # Set callback to send most recent state from the drone
+    self.__callback = callback
+
   """
   Destructor that only closes the socket when the object is deleted because sockets are not thread safe
   """
   def __del__(self):
     self.__socket.close()
 
   """
@@ -50,14 +54,16 @@
     while self.__thread_started:
       time.sleep(0.1)
       try:
         state, ip = self.__socket.recvfrom(1024)
         if self.__debug:
           print('[TelloState]: {}'.format(state))
         self.__current_state = state.decode("utf-8").rstrip("\r\n")
+        if self.__callback:
+          self.__callback(self.__current_state)
       except (UnicodeDecodeError, socket.error) as err:
         print('[TelloState] Error: {}'.format(err))
 
   """
   Internal method for retrieving a particular state field from the current state
   """
   def __get_state_field(self, name: str):
```

