# Comparing `tmp/jhub-swarmspawner-0.4.4.tar.gz` & `tmp/jhub-swarmspawner-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jhub-swarmspawner-0.4.4.tar", last modified: Tue May  2 11:37:33 2023, max compression
+gzip compressed data, was "jhub-swarmspawner-0.4.5.tar", last modified: Tue May  2 11:50:36 2023, max compression
```

## Comparing `jhub-swarmspawner-0.4.4.tar` & `jhub-swarmspawner-0.4.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:37:33.578182 jhub-swarmspawner-0.4.4/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1490 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.4/LICENSE
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    14462 2023-05-02 11:37:33.574182 jhub-swarmspawner-0.4.4/PKG-INFO
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    13652 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.4/README.rst
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:37:33.574182 jhub-swarmspawner-0.4.4/jhub/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       67 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.4/jhub/__init__.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2211 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.4/jhub/accelerators.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      148 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.4/jhub/defaults.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2475 2023-03-02 09:23:01.000000 jhub-swarmspawner-0.4.4/jhub/io.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4646 2023-05-02 11:36:34.000000 jhub-swarmspawner-0.4.4/jhub/mount.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      331 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.4/jhub/start.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    39502 2023-05-02 11:11:59.000000 jhub-swarmspawner-0.4.4/jhub/swarmspawner.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      778 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.4/jhub/util.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:37:33.574182 jhub-swarmspawner-0.4.4/jhub_swarmspawner.egg-info/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    14462 2023-05-02 11:37:33.000000 jhub-swarmspawner-0.4.4/jhub_swarmspawner.egg-info/PKG-INFO
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      465 2023-05-02 11:37:33.000000 jhub-swarmspawner-0.4.4/jhub_swarmspawner.egg-info/SOURCES.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        1 2023-05-02 11:37:33.000000 jhub-swarmspawner-0.4.4/jhub_swarmspawner.egg-info/dependency_links.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      204 2023-05-02 11:37:33.000000 jhub-swarmspawner-0.4.4/jhub_swarmspawner.egg-info/requires.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        5 2023-05-02 11:37:33.000000 jhub-swarmspawner-0.4.4/jhub_swarmspawner.egg-info/top_level.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       38 2023-05-02 11:37:33.578182 jhub-swarmspawner-0.4.4/setup.cfg
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1698 2023-03-02 09:23:01.000000 jhub-swarmspawner-0.4.4/setup.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:37:33.574182 jhub-swarmspawner-0.4.4/tests/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     9898 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.4/tests/test_auth_service.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     9373 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.4/tests/test_mount_service.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    10366 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.4/tests/test_service.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5319 2023-05-02 08:04:57.000000 jhub-swarmspawner-0.4.4/tests/test_ulimit_service.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:50:36.774813 jhub-swarmspawner-0.4.5/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1490 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.5/LICENSE
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    14462 2023-05-02 11:50:36.774813 jhub-swarmspawner-0.4.5/PKG-INFO
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    13652 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.5/README.rst
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:50:36.774813 jhub-swarmspawner-0.4.5/jhub/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       67 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.5/jhub/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2211 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.5/jhub/accelerators.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      148 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.5/jhub/defaults.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2475 2023-03-02 09:23:01.000000 jhub-swarmspawner-0.4.5/jhub/io.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4646 2023-05-02 11:45:55.000000 jhub-swarmspawner-0.4.5/jhub/mount.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      331 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.5/jhub/start.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    39502 2023-05-02 11:48:24.000000 jhub-swarmspawner-0.4.5/jhub/swarmspawner.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      778 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.5/jhub/util.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:50:36.774813 jhub-swarmspawner-0.4.5/jhub_swarmspawner.egg-info/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    14462 2023-05-02 11:50:36.000000 jhub-swarmspawner-0.4.5/jhub_swarmspawner.egg-info/PKG-INFO
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      465 2023-05-02 11:50:36.000000 jhub-swarmspawner-0.4.5/jhub_swarmspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        1 2023-05-02 11:50:36.000000 jhub-swarmspawner-0.4.5/jhub_swarmspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      204 2023-05-02 11:50:36.000000 jhub-swarmspawner-0.4.5/jhub_swarmspawner.egg-info/requires.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        5 2023-05-02 11:50:36.000000 jhub-swarmspawner-0.4.5/jhub_swarmspawner.egg-info/top_level.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       38 2023-05-02 11:50:36.774813 jhub-swarmspawner-0.4.5/setup.cfg
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1698 2023-03-02 09:23:01.000000 jhub-swarmspawner-0.4.5/setup.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 11:50:36.774813 jhub-swarmspawner-0.4.5/tests/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     9898 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.5/tests/test_auth_service.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     9373 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.5/tests/test_mount_service.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    10366 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.5/tests/test_service.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5319 2023-05-02 08:04:57.000000 jhub-swarmspawner-0.4.5/tests/test_ulimit_service.py
```

### Comparing `jhub-swarmspawner-0.4.4/LICENSE` & `jhub-swarmspawner-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.4/PKG-INFO` & `jhub-swarmspawner-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhub-swarmspawner
-Version: 0.4.4
+Version: 0.4.5
 Summary: SwarmSpawner enables JupyterHub to spawn jupyter
 Home-page: https://github.com/rasmunk/SwarmSpawner
 Author: Rasmus Munk
 Author-email: rasmus.munk@nbi.ku.dk
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jhub-swarmspawner-0.4.4/README.rst` & `jhub-swarmspawner-0.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.4/jhub/accelerators.py` & `jhub-swarmspawner-0.4.5/jhub/accelerators.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.4/jhub/io.py` & `jhub-swarmspawner-0.4.5/jhub/io.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.4/jhub/mount.py` & `jhub-swarmspawner-0.4.5/jhub/mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         if not isinstance(config, dict):
             raise Exception("A dictionary typed config is expected")
         if not config:
             raise Exception("A non-zero sized dictionary is expected")
         # Ensure that we don't change the passed in config,
         # But only use it. Deep copy is allowed if it is of type Config
         self.log.debug("instantiating Mounter with config: {}".format(config))
-        self.config = copy.deepcopy(Config(config))
+        self.config = Config(copy.deepcopy(config))
 
     @gen.coroutine
     def gen_config_copy(self):
         return copy.deepcopy(self.config)
 
     @gen.coroutine
     def format_config(self, config, **kwargs):
```

### Comparing `jhub-swarmspawner-0.4.4/jhub/swarmspawner.py` & `jhub-swarmspawner-0.4.5/jhub/swarmspawner.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.4/jhub/util.py` & `jhub-swarmspawner-0.4.5/jhub/util.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.4/jhub_swarmspawner.egg-info/PKG-INFO` & `jhub-swarmspawner-0.4.5/jhub_swarmspawner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhub-swarmspawner
-Version: 0.4.4
+Version: 0.4.5
 Summary: SwarmSpawner enables JupyterHub to spawn jupyter
 Home-page: https://github.com/rasmunk/SwarmSpawner
 Author: Rasmus Munk
 Author-email: rasmus.munk@nbi.ku.dk
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jhub-swarmspawner-0.4.4/setup.py` & `jhub-swarmspawner-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.4/tests/test_auth_service.py` & `jhub-swarmspawner-0.4.5/tests/test_auth_service.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.4/tests/test_mount_service.py` & `jhub-swarmspawner-0.4.5/tests/test_mount_service.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.4/tests/test_service.py` & `jhub-swarmspawner-0.4.5/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.4/tests/test_ulimit_service.py` & `jhub-swarmspawner-0.4.5/tests/test_ulimit_service.py`

 * *Files identical despite different names*

