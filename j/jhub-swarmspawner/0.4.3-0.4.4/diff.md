# Comparing `tmp/jhub-swarmspawner-0.4.3.tar.gz` & `tmp/jhub-swarmspawner-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jhub-swarmspawner-0.4.3.tar", last modified: Tue May  2 11:25:05 2023, max compression
+gzip compressed data, was "jhub-swarmspawner-0.4.4.tar", last modified: Tue May  2 11:37:33 2023, max compression
```

## Comparing `jhub-swarmspawner-0.4.3.tar` & `jhub-swarmspawner-0.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:25:05.814332 jhub-swarmspawner-0.4.3/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1490 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.3/LICENSE
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    14462 2023-05-02 11:25:05.814332 jhub-swarmspawner-0.4.3/PKG-INFO
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    13652 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.3/README.rst
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:25:05.810332 jhub-swarmspawner-0.4.3/jhub/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       67 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.3/jhub/__init__.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2211 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.3/jhub/accelerators.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      148 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.3/jhub/defaults.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2475 2023-03-02 09:23:01.000000 jhub-swarmspawner-0.4.3/jhub/io.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4642 2023-05-02 11:23:14.000000 jhub-swarmspawner-0.4.3/jhub/mount.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      331 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.3/jhub/start.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    39502 2023-05-02 11:11:59.000000 jhub-swarmspawner-0.4.3/jhub/swarmspawner.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      778 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.3/jhub/util.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:25:05.810332 jhub-swarmspawner-0.4.3/jhub_swarmspawner.egg-info/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    14462 2023-05-02 11:25:05.000000 jhub-swarmspawner-0.4.3/jhub_swarmspawner.egg-info/PKG-INFO
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      465 2023-05-02 11:25:05.000000 jhub-swarmspawner-0.4.3/jhub_swarmspawner.egg-info/SOURCES.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        1 2023-05-02 11:25:05.000000 jhub-swarmspawner-0.4.3/jhub_swarmspawner.egg-info/dependency_links.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      204 2023-05-02 11:25:05.000000 jhub-swarmspawner-0.4.3/jhub_swarmspawner.egg-info/requires.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        5 2023-05-02 11:25:05.000000 jhub-swarmspawner-0.4.3/jhub_swarmspawner.egg-info/top_level.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       38 2023-05-02 11:25:05.814332 jhub-swarmspawner-0.4.3/setup.cfg
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1698 2023-03-02 09:23:01.000000 jhub-swarmspawner-0.4.3/setup.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:25:05.814332 jhub-swarmspawner-0.4.3/tests/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     9898 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.3/tests/test_auth_service.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     9373 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.3/tests/test_mount_service.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    10366 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.3/tests/test_service.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5319 2023-05-02 08:04:57.000000 jhub-swarmspawner-0.4.3/tests/test_ulimit_service.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:37:33.578182 jhub-swarmspawner-0.4.4/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1490 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.4/LICENSE
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    14462 2023-05-02 11:37:33.574182 jhub-swarmspawner-0.4.4/PKG-INFO
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    13652 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.4/README.rst
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:37:33.574182 jhub-swarmspawner-0.4.4/jhub/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       67 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.4/jhub/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2211 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.4/jhub/accelerators.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      148 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.4/jhub/defaults.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2475 2023-03-02 09:23:01.000000 jhub-swarmspawner-0.4.4/jhub/io.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4646 2023-05-02 11:36:34.000000 jhub-swarmspawner-0.4.4/jhub/mount.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      331 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.4/jhub/start.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    39502 2023-05-02 11:11:59.000000 jhub-swarmspawner-0.4.4/jhub/swarmspawner.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      778 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.4/jhub/util.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:37:33.574182 jhub-swarmspawner-0.4.4/jhub_swarmspawner.egg-info/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    14462 2023-05-02 11:37:33.000000 jhub-swarmspawner-0.4.4/jhub_swarmspawner.egg-info/PKG-INFO
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      465 2023-05-02 11:37:33.000000 jhub-swarmspawner-0.4.4/jhub_swarmspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        1 2023-05-02 11:37:33.000000 jhub-swarmspawner-0.4.4/jhub_swarmspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      204 2023-05-02 11:37:33.000000 jhub-swarmspawner-0.4.4/jhub_swarmspawner.egg-info/requires.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        5 2023-05-02 11:37:33.000000 jhub-swarmspawner-0.4.4/jhub_swarmspawner.egg-info/top_level.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       38 2023-05-02 11:37:33.578182 jhub-swarmspawner-0.4.4/setup.cfg
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1698 2023-03-02 09:23:01.000000 jhub-swarmspawner-0.4.4/setup.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:37:33.574182 jhub-swarmspawner-0.4.4/tests/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     9898 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.4/tests/test_auth_service.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     9373 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.4/tests/test_mount_service.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    10366 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.4/tests/test_service.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5319 2023-05-02 08:04:57.000000 jhub-swarmspawner-0.4.4/tests/test_ulimit_service.py
```

### Comparing `jhub-swarmspawner-0.4.3/LICENSE` & `jhub-swarmspawner-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.3/PKG-INFO` & `jhub-swarmspawner-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhub-swarmspawner
-Version: 0.4.3
+Version: 0.4.4
 Summary: SwarmSpawner enables JupyterHub to spawn jupyter
 Home-page: https://github.com/rasmunk/SwarmSpawner
 Author: Rasmus Munk
 Author-email: rasmus.munk@nbi.ku.dk
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jhub-swarmspawner-0.4.3/README.rst` & `jhub-swarmspawner-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.3/jhub/accelerators.py` & `jhub-swarmspawner-0.4.4/jhub/accelerators.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.3/jhub/io.py` & `jhub-swarmspawner-0.4.4/jhub/io.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.3/jhub/mount.py` & `jhub-swarmspawner-0.4.4/jhub/mount.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
     @gen.coroutine
     def format_config(self, config, **kwargs):
         # Dynamically overload the mount config
         self.log.debug("formatting mount config: {} with: {}".format(config, kwargs))
         for key, value in kwargs.items():
             recursive_format(config, value)
+        self.log.debug("new formatted config: {}".format(config))
 
 
 class VolumeMounter(Mounter):
     def __init__(self, config):
         Mounter.__init__(self, config)
 
     @gen.coroutine
@@ -41,17 +42,17 @@
 
     @gen.coroutine
     def create(self, **format_config_kwargs):
         self.log.debug(
             "Creating VolumeMount with options {}".format(format_config_kwargs)
         )
         new_config = yield self.gen_config_copy()
-        formatted_config = yield self.format_config(new_config, **format_config_kwargs)
-        yield self.validate_config(formatted_config)
-        mount = yield self.create_mount(formatted_config)
+        yield self.format_config(new_config, **format_config_kwargs)
+        yield self.validate_config(new_config)
+        mount = yield self.create_mount(new_config)
         return mount
 
     @gen.coroutine
     def validate_config(self, config):
         self.log.debug("validate_config")
         required_config_keys = ["source", "target"]
         missing_keys = [key for key in required_config_keys if key not in config]
@@ -114,11 +115,11 @@
             raise ValueError(
                 "A mount configuration error was encountered, due to missing values"
             )
 
     @gen.coroutine
     def create(self, **format_config_kwargs):
         new_config = yield self.gen_config_copy()
-        formatted_config = yield self.format_config(new_config, **format_config_kwargs)
-        yield self.validate_config(formatted_config)
-        mount = yield self.create_mount(formatted_config)
+        yield self.format_config(new_config, **format_config_kwargs)
+        yield self.validate_config(new_config)
+        mount = yield self.create_mount(new_config)
         return mount
```

### Comparing `jhub-swarmspawner-0.4.3/jhub/swarmspawner.py` & `jhub-swarmspawner-0.4.4/jhub/swarmspawner.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.3/jhub/util.py` & `jhub-swarmspawner-0.4.4/jhub/util.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.3/jhub_swarmspawner.egg-info/PKG-INFO` & `jhub-swarmspawner-0.4.4/jhub_swarmspawner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhub-swarmspawner
-Version: 0.4.3
+Version: 0.4.4
 Summary: SwarmSpawner enables JupyterHub to spawn jupyter
 Home-page: https://github.com/rasmunk/SwarmSpawner
 Author: Rasmus Munk
 Author-email: rasmus.munk@nbi.ku.dk
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jhub-swarmspawner-0.4.3/setup.py` & `jhub-swarmspawner-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.3/tests/test_auth_service.py` & `jhub-swarmspawner-0.4.4/tests/test_auth_service.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.3/tests/test_mount_service.py` & `jhub-swarmspawner-0.4.4/tests/test_mount_service.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.3/tests/test_service.py` & `jhub-swarmspawner-0.4.4/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.3/tests/test_ulimit_service.py` & `jhub-swarmspawner-0.4.4/tests/test_ulimit_service.py`

 * *Files identical despite different names*

