# Comparing `tmp/jhub-swarmspawner-0.4.2.tar.gz` & `tmp/jhub-swarmspawner-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jhub-swarmspawner-0.4.2.tar", last modified: Tue May  2 08:52:19 2023, max compression
+gzip compressed data, was "jhub-swarmspawner-0.4.3.tar", last modified: Tue May  2 11:25:05 2023, max compression
```

## Comparing `jhub-swarmspawner-0.4.2.tar` & `jhub-swarmspawner-0.4.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 08:52:19.174488 jhub-swarmspawner-0.4.2/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1490 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.2/LICENSE
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    14462 2023-05-02 08:52:19.174488 jhub-swarmspawner-0.4.2/PKG-INFO
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    13652 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.2/README.rst
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 08:52:19.174488 jhub-swarmspawner-0.4.2/jhub/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       67 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.2/jhub/__init__.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2211 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.2/jhub/accelerators.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      148 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.2/jhub/defaults.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2475 2023-03-02 09:23:01.000000 jhub-swarmspawner-0.4.2/jhub/io.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4241 2023-05-02 07:57:31.000000 jhub-swarmspawner-0.4.2/jhub/mount.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      331 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.2/jhub/start.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    39670 2023-05-02 08:03:46.000000 jhub-swarmspawner-0.4.2/jhub/swarmspawner.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      778 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.2/jhub/util.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 08:52:19.174488 jhub-swarmspawner-0.4.2/jhub_swarmspawner.egg-info/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    14462 2023-05-02 08:52:19.000000 jhub-swarmspawner-0.4.2/jhub_swarmspawner.egg-info/PKG-INFO
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      465 2023-05-02 08:52:19.000000 jhub-swarmspawner-0.4.2/jhub_swarmspawner.egg-info/SOURCES.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        1 2023-05-02 08:52:19.000000 jhub-swarmspawner-0.4.2/jhub_swarmspawner.egg-info/dependency_links.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      204 2023-05-02 08:52:19.000000 jhub-swarmspawner-0.4.2/jhub_swarmspawner.egg-info/requires.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        5 2023-05-02 08:52:19.000000 jhub-swarmspawner-0.4.2/jhub_swarmspawner.egg-info/top_level.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       38 2023-05-02 08:52:19.174488 jhub-swarmspawner-0.4.2/setup.cfg
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1698 2023-03-02 09:23:01.000000 jhub-swarmspawner-0.4.2/setup.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 08:52:19.174488 jhub-swarmspawner-0.4.2/tests/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     9898 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.2/tests/test_auth_service.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     9373 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.2/tests/test_mount_service.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    10366 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.2/tests/test_service.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5319 2023-05-02 08:04:57.000000 jhub-swarmspawner-0.4.2/tests/test_ulimit_service.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:25:05.814332 jhub-swarmspawner-0.4.3/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1490 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.3/LICENSE
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    14462 2023-05-02 11:25:05.814332 jhub-swarmspawner-0.4.3/PKG-INFO
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    13652 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.3/README.rst
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:25:05.810332 jhub-swarmspawner-0.4.3/jhub/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       67 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.3/jhub/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2211 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.3/jhub/accelerators.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      148 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.3/jhub/defaults.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2475 2023-03-02 09:23:01.000000 jhub-swarmspawner-0.4.3/jhub/io.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4642 2023-05-02 11:23:14.000000 jhub-swarmspawner-0.4.3/jhub/mount.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      331 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.3/jhub/start.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    39502 2023-05-02 11:11:59.000000 jhub-swarmspawner-0.4.3/jhub/swarmspawner.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      778 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.3/jhub/util.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:25:05.810332 jhub-swarmspawner-0.4.3/jhub_swarmspawner.egg-info/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    14462 2023-05-02 11:25:05.000000 jhub-swarmspawner-0.4.3/jhub_swarmspawner.egg-info/PKG-INFO
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      465 2023-05-02 11:25:05.000000 jhub-swarmspawner-0.4.3/jhub_swarmspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        1 2023-05-02 11:25:05.000000 jhub-swarmspawner-0.4.3/jhub_swarmspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      204 2023-05-02 11:25:05.000000 jhub-swarmspawner-0.4.3/jhub_swarmspawner.egg-info/requires.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        5 2023-05-02 11:25:05.000000 jhub-swarmspawner-0.4.3/jhub_swarmspawner.egg-info/top_level.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       38 2023-05-02 11:25:05.814332 jhub-swarmspawner-0.4.3/setup.cfg
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1698 2023-03-02 09:23:01.000000 jhub-swarmspawner-0.4.3/setup.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:25:05.814332 jhub-swarmspawner-0.4.3/tests/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     9898 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.3/tests/test_auth_service.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     9373 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.3/tests/test_mount_service.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    10366 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.3/tests/test_service.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5319 2023-05-02 08:04:57.000000 jhub-swarmspawner-0.4.3/tests/test_ulimit_service.py
```

### Comparing `jhub-swarmspawner-0.4.2/LICENSE` & `jhub-swarmspawner-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.2/PKG-INFO` & `jhub-swarmspawner-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhub-swarmspawner
-Version: 0.4.2
+Version: 0.4.3
 Summary: SwarmSpawner enables JupyterHub to spawn jupyter
 Home-page: https://github.com/rasmunk/SwarmSpawner
 Author: Rasmus Munk
 Author-email: rasmus.munk@nbi.ku.dk
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jhub-swarmspawner-0.4.2/README.rst` & `jhub-swarmspawner-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.2/jhub/accelerators.py` & `jhub-swarmspawner-0.4.3/jhub/accelerators.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.2/jhub/io.py` & `jhub-swarmspawner-0.4.3/jhub/io.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.2/jhub/mount.py` & `jhub-swarmspawner-0.4.3/jhub/mount.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,108 +10,115 @@
         LoggingConfigurable.__init__(self)
         if not isinstance(config, dict):
             raise Exception("A dictionary typed config is expected")
         if not config:
             raise Exception("A non-zero sized dictionary is expected")
         # Ensure that we don't change the passed in config,
         # But only use it. Deep copy is allowed if it is of type Config
+        self.log.debug("instantiating Mounter with config: {}".format(config))
         self.config = copy.deepcopy(Config(config))
 
     @gen.coroutine
-    def format_config(self, **kwargs):
+    def gen_config_copy(self):
+        return copy.deepcopy(self.config)
+
+    @gen.coroutine
+    def format_config(self, config, **kwargs):
         # Dynamically overload the mount config
-        self.log.debug("formatting mount config with {}".format(kwargs))
+        self.log.debug("formatting mount config: {} with: {}".format(config, kwargs))
         for key, value in kwargs.items():
-            recursive_format(self.config, value)
+            recursive_format(config, value)
 
 
 class VolumeMounter(Mounter):
     def __init__(self, config):
         Mounter.__init__(self, config)
 
     @gen.coroutine
-    def create_mount(self):
+    def create_mount(self, config):
         mount = {}
-        mount.update(self.config)
+        mount.update(config)
         return Mount(**mount)
 
     @gen.coroutine
     def create(self, **format_config_kwargs):
         self.log.debug(
             "Creating VolumeMount with options {}".format(format_config_kwargs)
         )
-        yield self.format_config(**format_config_kwargs)
-        yield self.validate_config()
-        mount = yield self.create_mount()
+        new_config = yield self.gen_config_copy()
+        formatted_config = yield self.format_config(new_config, **format_config_kwargs)
+        yield self.validate_config(formatted_config)
+        mount = yield self.create_mount(formatted_config)
         return mount
 
     @gen.coroutine
-    def validate_config(self):
+    def validate_config(self, config):
         self.log.debug("validate_config")
         required_config_keys = ["source", "target"]
-        missing_keys = [key for key in required_config_keys if key not in self.config]
+        missing_keys = [key for key in required_config_keys if key not in config]
 
         if missing_keys:
             self.log.error("Missing configure keys {}".format(",".join(missing_keys)))
             raise KeyError(
                 "A mount configuration error was encountered due to missing keys."
             )
 
         required_config_values = ["target"]
-        empty_values = [key for key in required_config_values if not self.config[key]]
+        empty_values = [key for key in required_config_values if not config[key]]
         if empty_values:
             self.log.error(
                 "Missing configuring values {}".format(",".join(empty_values))
             )
             raise ValueError(
                 "A mount configuration error was encountered due to missing values."
             )
 
 
 class SSHFSMounter(Mounter):
     def __init__(self, config):
         Mounter.__init__(self, config)
 
     @gen.coroutine
-    def create_mount(self):
-        self.log.debug("create_mount from config: {}".format(self.config))
+    def create_mount(self, config):
+        self.log.debug("create_mount from config: {}".format(config))
         # Adapt mount options into appropriate types
         driver_config = DriverConfig(
-            self.config["driver_config"]["name"],
-            self.config["driver_config"]["options"],
+            config["driver_config"]["name"],
+            config["driver_config"]["options"],
         )
 
         mount_config = {}
-        mount_config.update(self.config)
+        mount_config.update(config)
         # Override the DriverConfig to be the correct type
         # as expected by the Docker module.
         mount_config["driver_config"] = driver_config
         return Mount(**mount_config)
 
     @gen.coroutine
-    def validate_config(self):
+    def validate_config(self, config):
         self.log.debug("validate_config")
         required_config_keys = ["source", "target", "type", "driver_config"]
-        missing_keys = [key for key in required_config_keys if key not in self.config]
+        missing_keys = [key for key in required_config_keys if key not in config]
 
         if missing_keys:
             self.log.error("Missing configure keys {}".format(",".join(missing_keys)))
             raise KeyError(
                 "A mount configuration error was encountered, " "due to missing keys"
             )
 
         required_config_values = ["type", "driver_config", "target"]
-        empty_values = [key for key in required_config_values if not self.config[key]]
+        empty_values = [key for key in required_config_values if not config[key]]
         if empty_values:
             self.log.error(
                 "Missing configuring values {}".format(",".join(empty_values))
             )
             raise ValueError(
                 "A mount configuration error was encountered, due to missing values"
             )
 
     @gen.coroutine
     def create(self, **format_config_kwargs):
-        yield self.format_config(**format_config_kwargs)
-        yield self.validate_config()
-        mount = yield self.create_mount()
+        new_config = yield self.gen_config_copy()
+        formatted_config = yield self.format_config(new_config, **format_config_kwargs)
+        yield self.validate_config(formatted_config)
+        mount = yield self.create_mount(formatted_config)
         return mount
```

### Comparing `jhub-swarmspawner-0.4.2/jhub/swarmspawner.py` & `jhub-swarmspawner-0.4.3/jhub/swarmspawner.py`

 * *Files 1% similar despite different names*

```diff
@@ -723,26 +723,21 @@
                         value = getattr(self.user, attr)
                         if not isinstance(value, dict):
                             value = {attr: value}
                         format_mount_kwargs[attr] = value
 
             # Mounts can be declared as regular dictionaries
             # or as special Mountable objects (see mount.py)
-
-            # Ensure that the formatted mount config does not persist
-            # across user sessions
-            mount_templates = copy.deepcopy(mounts)
-            for mount in mount_templates:
+            for mount in mounts:
                 if isinstance(mount, dict):
                     m = VolumeMounter(mount)
                     m = yield m.create(**format_mount_kwargs)
                 else:
                     # Custom type mount defined
                     # Is instantiated in the config
-
                     m = yield mount.create(**format_mount_kwargs)
                 container_spec["mounts"].append(m)
 
             # Some envs are required by the single-user-image
             if "env" in container_spec:
                 container_spec["env"].update(self.get_env())
             else:
```

### Comparing `jhub-swarmspawner-0.4.2/jhub/util.py` & `jhub-swarmspawner-0.4.3/jhub/util.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.2/jhub_swarmspawner.egg-info/PKG-INFO` & `jhub-swarmspawner-0.4.3/jhub_swarmspawner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhub-swarmspawner
-Version: 0.4.2
+Version: 0.4.3
 Summary: SwarmSpawner enables JupyterHub to spawn jupyter
 Home-page: https://github.com/rasmunk/SwarmSpawner
 Author: Rasmus Munk
 Author-email: rasmus.munk@nbi.ku.dk
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jhub-swarmspawner-0.4.2/setup.py` & `jhub-swarmspawner-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.2/tests/test_auth_service.py` & `jhub-swarmspawner-0.4.3/tests/test_auth_service.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.2/tests/test_mount_service.py` & `jhub-swarmspawner-0.4.3/tests/test_mount_service.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.2/tests/test_service.py` & `jhub-swarmspawner-0.4.3/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.2/tests/test_ulimit_service.py` & `jhub-swarmspawner-0.4.3/tests/test_ulimit_service.py`

 * *Files identical despite different names*

