# Comparing `tmp/mnm-0.1.0.tar.gz` & `tmp/mnm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnm-0.1.0.tar", last modified: Mon May  1 13:02:41 2023, max compression
+gzip compressed data, was "mnm-0.1.2.tar", last modified: Tue May  2 00:29:31 2023, max compression
```

## Comparing `mnm-0.1.0.tar` & `mnm-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-01 13:02:41.552071 mnm-0.1.0/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1067 2023-05-01 04:28:16.000000 mnm-0.1.0/LICENSE
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      926 2023-05-01 13:02:41.552071 mnm-0.1.0/PKG-INFO
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      403 2023-05-01 12:59:53.000000 mnm-0.1.0/README.md
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      636 2023-05-01 13:02:31.000000 mnm-0.1.0/pyproject.toml
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       38 2023-05-01 13:02:41.552071 mnm-0.1.0/setup.cfg
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-01 13:02:41.542071 mnm-0.1.0/src/
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-01 13:02:41.552071 mnm-0.1.0/src/mnm/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     4061 2023-05-01 12:57:05.000000 mnm-0.1.0/src/mnm/__init__.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      183 2023-05-01 12:58:39.000000 mnm-0.1.0/src/mnm/example.py
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-01 13:02:41.552071 mnm-0.1.0/src/mnm.egg-info/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      926 2023-05-01 13:02:41.000000 mnm-0.1.0/src/mnm.egg-info/PKG-INFO
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      225 2023-05-01 13:02:41.000000 mnm-0.1.0/src/mnm.egg-info/SOURCES.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        1 2023-05-01 13:02:41.000000 mnm-0.1.0/src/mnm.egg-info/dependency_links.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       29 2023-05-01 13:02:41.000000 mnm-0.1.0/src/mnm.egg-info/requires.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        4 2023-05-01 13:02:41.000000 mnm-0.1.0/src/mnm.egg-info/top_level.txt
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-02 00:29:31.962648 mnm-0.1.2/
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1067 2023-05-01 04:28:16.000000 mnm-0.1.2/LICENSE
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      926 2023-05-02 00:29:31.962648 mnm-0.1.2/PKG-INFO
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      403 2023-05-01 12:59:53.000000 mnm-0.1.2/README.md
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      636 2023-05-02 00:29:28.000000 mnm-0.1.2/pyproject.toml
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       38 2023-05-02 00:29:31.962648 mnm-0.1.2/setup.cfg
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-02 00:29:31.962648 mnm-0.1.2/src/
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-02 00:29:31.962648 mnm-0.1.2/src/mnm/
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     4267 2023-05-02 00:26:30.000000 mnm-0.1.2/src/mnm/__init__.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      183 2023-05-01 13:05:36.000000 mnm-0.1.2/src/mnm/example.py
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-02 00:29:31.962648 mnm-0.1.2/src/mnm.egg-info/
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      926 2023-05-02 00:29:31.000000 mnm-0.1.2/src/mnm.egg-info/PKG-INFO
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      225 2023-05-02 00:29:31.000000 mnm-0.1.2/src/mnm.egg-info/SOURCES.txt
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        1 2023-05-02 00:29:31.000000 mnm-0.1.2/src/mnm.egg-info/dependency_links.txt
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       29 2023-05-02 00:29:31.000000 mnm-0.1.2/src/mnm.egg-info/requires.txt
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        4 2023-05-02 00:29:31.000000 mnm-0.1.2/src/mnm.egg-info/top_level.txt
```

### Comparing `mnm-0.1.0/LICENSE` & `mnm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mnm-0.1.0/PKG-INFO` & `mnm-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnm
-Version: 0.1.0
+Version: 0.1.2
 Summary: A simple python library for pentesting firewall protected webapp
 Author-email: ohk990102 <ohk990102@gmail.com>
 Project-URL: Homepage, https://github.com/ohk990102/mnm
 Project-URL: Bug Tracker, https://github.com/ohk990102/mnm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `mnm-0.1.0/pyproject.toml` & `mnm-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mnm"
-version = "0.1.0"
+version = "0.1.2"
 authors = [
   { name="ohk990102", email="ohk990102@gmail.com" },
 ]
 description = "A simple python library for pentesting firewall protected webapp"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `mnm-0.1.0/src/mnm/__init__.py` & `mnm-0.1.2/src/mnm/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,35 +13,39 @@
     global saved_socket
     if saved_socket:
         return
     import socket
 
 
     def flush_socket(sock: socket.socket) -> bool:
-        from ctypes import c_ulong
+        from sys import platform
         from time import sleep
-        from termios import TIOCOUTQ
-        from fcntl import ioctl
-        import time
-        
-        cu = time.time()
-
-        while time.time() - cu < timeout and sock.fileno() != -1: # if fd is -1, then it has been probably close()'d
-            remaining = c_ulong.from_buffer_copy(
-                ioctl(sock.fileno(), TIOCOUTQ, bytearray(8), False)).value
-
-            if remaining == 0:
-                # all data has been sent and ACKed
-                return True
-
-            # wait a bit before retrying,
-            # sleep(0) was meant like yield current thread,
-            # but will probably be close to busy-waiting,
-            # feel free to change it to fit your needs
-            sleep(interval)
+        if platform == 'linux' or platform == 'linux2':
+            from ctypes import c_ulong
+            from termios import TIOCOUTQ
+            from fcntl import ioctl
+            import time
+            
+            cu = time.time()
+
+            while time.time() - cu < timeout and sock.fileno() != -1: # if fd is -1, then it has been probably close()'d
+                remaining = c_ulong.from_buffer_copy(
+                    ioctl(sock.fileno(), TIOCOUTQ, bytearray(8), False)).value
+
+                if remaining == 0:
+                    # all data has been sent and ACKed
+                    return True
+
+                # wait a bit before retrying,
+                # sleep(0) was meant like yield current thread,
+                # but will probably be close to busy-waiting,
+                # feel free to change it to fit your needs
+                sleep(interval)
+            else:
+                sleep(timeout)
 
         # not all data has been sent
         return False
 
     def send(self, data, flags=0):
         nbytes = 0
         for i in range(0, len(data), 1):
```

### Comparing `mnm-0.1.0/src/mnm.egg-info/PKG-INFO` & `mnm-0.1.2/src/mnm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnm
-Version: 0.1.0
+Version: 0.1.2
 Summary: A simple python library for pentesting firewall protected webapp
 Author-email: ohk990102 <ohk990102@gmail.com>
 Project-URL: Homepage, https://github.com/ohk990102/mnm
 Project-URL: Bug Tracker, https://github.com/ohk990102/mnm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

