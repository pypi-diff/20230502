# Comparing `tmp/pizurscan-0.1.2.tar.gz` & `tmp/pizurscan-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizurscan-0.1.2.tar", last modified: Mon May  1 12:03:50 2023, max compression
+gzip compressed data, was "pizurscan-0.1.3.tar", last modified: Mon May  1 13:02:13 2023, max compression
```

## Comparing `pizurscan-0.1.2.tar` & `pizurscan-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:50.171589 pizurscan-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 12:03:50.171589 pizurscan-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-01 12:03:35.000000 pizurscan-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:50.171589 pizurscan-0.1.2/pizurscan/
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-01 12:03:35.000000 pizurscan-0.1.2/pizurscan/InputProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-01 12:03:35.000000 pizurscan-0.1.2/pizurscan/OutputProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-01 12:03:35.000000 pizurscan-0.1.2/pizurscan/PI_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-01 12:03:35.000000 pizurscan-0.1.2/pizurscan/Scanners.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:35.000000 pizurscan-0.1.2/pizurscan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:50.171589 pizurscan-0.1.2/pizurscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 12:03:50.000000 pizurscan-0.1.2/pizurscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 12:03:50.000000 pizurscan-0.1.2/pizurscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 12:03:50.000000 pizurscan-0.1.2/pizurscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 12:03:50.000000 pizurscan-0.1.2/pizurscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 12:03:50.000000 pizurscan-0.1.2/pizurscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 12:03:50.171589 pizurscan-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-01 12:03:35.000000 pizurscan-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:50.171589 pizurscan-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    23152 2023-05-01 12:03:35.000000 pizurscan-0.1.2/tests/testclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:02:13.407973 pizurscan-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 13:02:13.407973 pizurscan-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-01 13:01:59.000000 pizurscan-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:02:13.407973 pizurscan-0.1.3/pizurscan/
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-01 13:01:59.000000 pizurscan-0.1.3/pizurscan/InputProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-01 13:01:59.000000 pizurscan-0.1.3/pizurscan/OutputProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-01 13:01:59.000000 pizurscan-0.1.3/pizurscan/PI_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-01 13:01:59.000000 pizurscan-0.1.3/pizurscan/Scanners.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 13:01:59.000000 pizurscan-0.1.3/pizurscan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:02:13.407973 pizurscan-0.1.3/pizurscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 13:02:13.000000 pizurscan-0.1.3/pizurscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 13:02:13.000000 pizurscan-0.1.3/pizurscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:02:13.000000 pizurscan-0.1.3/pizurscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 13:02:13.000000 pizurscan-0.1.3/pizurscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 13:02:13.000000 pizurscan-0.1.3/pizurscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 13:02:13.407973 pizurscan-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-01 13:01:59.000000 pizurscan-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:02:13.407973 pizurscan-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23204 2023-05-01 13:01:59.000000 pizurscan-0.1.3/tests/testclasses.py
```

### Comparing `pizurscan-0.1.2/PKG-INFO` & `pizurscan-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizurscan
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library to interface PI controllers and Zurich lock-in
 Home-page: https://pizur-scanner.readthedocs.io/
 Author: Giacomo Rizzi
 Author-email: rizzigiacomo@pm.me
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pizurscan-0.1.2/README.md` & `pizurscan-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.2/pizurscan/InputProcessor.py` & `pizurscan-0.1.3/pizurscan/InputProcessor.py`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.2/pizurscan/OutputProcessor.py` & `pizurscan-0.1.3/pizurscan/OutputProcessor.py`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.2/pizurscan/PI_commands.py` & `pizurscan-0.1.3/pizurscan/PI_commands.py`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.2/pizurscan/Scanners.py` & `pizurscan-0.1.3/pizurscan/Scanners.py`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.2/pizurscan.egg-info/PKG-INFO` & `pizurscan-0.1.3/pizurscan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizurscan
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library to interface PI controllers and Zurich lock-in
 Home-page: https://pizur-scanner.readthedocs.io/
 Author: Giacomo Rizzi
 Author-email: rizzigiacomo@pm.me
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pizurscan-0.1.2/setup.py` & `pizurscan-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="pizurscan",
-    version="0.1.2",
+    version="0.1.3",
     description="Library to interface PI controllers and Zurich lock-in",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pizur-scanner.readthedocs.io/",
     author="Giacomo Rizzi",
     author_email="rizzigiacomo@pm.me",
     license="MIT",
```

### Comparing `pizurscan-0.1.2/tests/testclasses.py` & `pizurscan-0.1.3/tests/testclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     
     def test_initialization_controller_axis(self):
         """Tests that when a Stepper object is initialized through
         the __init__ method, the attributes controller_id and axis_id are
         properly assigned."""
         controller = 'C-663'
         axis = 'L-406.40SD00'
+        # make id of controller and axis attributes
         assert self.stepper.controller_id == controller
         assert self.stepper.axis_id == axis
             
     def test_usb_return_list(self):
         """
         Tests that when a Stepper object is passed to 
         usb_plugged_devices the returned object is a list.
```

