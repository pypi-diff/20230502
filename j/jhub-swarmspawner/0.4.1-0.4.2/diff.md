# Comparing `tmp/jhub-swarmspawner-0.4.1.tar.gz` & `tmp/jhub-swarmspawner-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jhub-swarmspawner-0.4.1.tar", last modified: Thu Feb  9 11:06:01 2023, max compression
+gzip compressed data, was "jhub-swarmspawner-0.4.2.tar", last modified: Tue May  2 08:52:19 2023, max compression
```

## Comparing `jhub-swarmspawner-0.4.1.tar` & `jhub-swarmspawner-0.4.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 go         (988) go         (982)        0 2023-02-09 11:06:01.657412 jhub-swarmspawner-0.4.1/
--rw-r--r--   0 go         (988) go         (982)     1490 2023-02-09 10:55:55.000000 jhub-swarmspawner-0.4.1/LICENSE
--rw-r--r--   0 go         (988) go         (982)    14462 2023-02-09 11:06:01.656412 jhub-swarmspawner-0.4.1/PKG-INFO
--rw-r--r--   0 go         (988) go         (982)    13652 2023-02-09 10:55:55.000000 jhub-swarmspawner-0.4.1/README.rst
-drwxr-xr-x   0 go         (988) go         (982)        0 2023-02-09 11:06:01.652412 jhub-swarmspawner-0.4.1/jhub/
--rw-r--r--   0 go         (988) go         (982)       67 2023-02-09 10:55:55.000000 jhub-swarmspawner-0.4.1/jhub/__init__.py
--rw-r--r--   0 go         (988) go         (982)     2211 2023-02-09 10:55:55.000000 jhub-swarmspawner-0.4.1/jhub/accelerators.py
--rw-r--r--   0 go         (988) go         (982)      148 2023-02-09 10:55:55.000000 jhub-swarmspawner-0.4.1/jhub/defaults.py
--rw-r--r--   0 go         (988) go         (982)     2475 2023-02-09 10:55:55.000000 jhub-swarmspawner-0.4.1/jhub/io.py
--rw-r--r--   0 go         (988) go         (982)     4241 2023-02-09 10:55:55.000000 jhub-swarmspawner-0.4.1/jhub/mount.py
--rw-r--r--   0 go         (988) go         (982)      331 2023-02-09 10:55:55.000000 jhub-swarmspawner-0.4.1/jhub/start.py
--rw-r--r--   0 go         (988) go         (982)    39502 2023-02-09 10:55:55.000000 jhub-swarmspawner-0.4.1/jhub/swarmspawner.py
--rw-r--r--   0 go         (988) go         (982)      778 2023-02-09 10:55:55.000000 jhub-swarmspawner-0.4.1/jhub/util.py
-drwxr-xr-x   0 go         (988) go         (982)        0 2023-02-09 11:06:01.654412 jhub-swarmspawner-0.4.1/jhub_swarmspawner.egg-info/
--rw-r--r--   0 go         (988) go         (982)    14462 2023-02-09 11:06:01.000000 jhub-swarmspawner-0.4.1/jhub_swarmspawner.egg-info/PKG-INFO
--rw-r--r--   0 go         (988) go         (982)      436 2023-02-09 11:06:01.000000 jhub-swarmspawner-0.4.1/jhub_swarmspawner.egg-info/SOURCES.txt
--rw-r--r--   0 go         (988) go         (982)        1 2023-02-09 11:06:01.000000 jhub-swarmspawner-0.4.1/jhub_swarmspawner.egg-info/dependency_links.txt
--rw-r--r--   0 go         (988) go         (982)      187 2023-02-09 11:06:01.000000 jhub-swarmspawner-0.4.1/jhub_swarmspawner.egg-info/requires.txt
--rw-r--r--   0 go         (988) go         (982)        5 2023-02-09 11:06:01.000000 jhub-swarmspawner-0.4.1/jhub_swarmspawner.egg-info/top_level.txt
--rw-r--r--   0 go         (988) go         (982)       38 2023-02-09 11:06:01.657412 jhub-swarmspawner-0.4.1/setup.cfg
--rw-r--r--   0 go         (988) go         (982)     1698 2023-02-09 10:55:55.000000 jhub-swarmspawner-0.4.1/setup.py
-drwxr-xr-x   0 go         (988) go         (982)        0 2023-02-09 11:06:01.656412 jhub-swarmspawner-0.4.1/tests/
--rw-r--r--   0 go         (988) go         (982)     9898 2023-02-09 10:55:55.000000 jhub-swarmspawner-0.4.1/tests/test_auth_service.py
--rw-r--r--   0 go         (988) go         (982)     9373 2023-02-09 10:55:55.000000 jhub-swarmspawner-0.4.1/tests/test_mount_service.py
--rw-r--r--   0 go         (988) go         (982)    10366 2023-02-09 10:55:55.000000 jhub-swarmspawner-0.4.1/tests/test_service.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 08:52:19.174488 jhub-swarmspawner-0.4.2/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1490 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.2/LICENSE
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    14462 2023-05-02 08:52:19.174488 jhub-swarmspawner-0.4.2/PKG-INFO
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    13652 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.2/README.rst
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 08:52:19.174488 jhub-swarmspawner-0.4.2/jhub/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       67 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.2/jhub/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2211 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.2/jhub/accelerators.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      148 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.2/jhub/defaults.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2475 2023-03-02 09:23:01.000000 jhub-swarmspawner-0.4.2/jhub/io.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4241 2023-05-02 07:57:31.000000 jhub-swarmspawner-0.4.2/jhub/mount.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      331 2023-03-02 08:06:52.000000 jhub-swarmspawner-0.4.2/jhub/start.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    39670 2023-05-02 08:03:46.000000 jhub-swarmspawner-0.4.2/jhub/swarmspawner.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      778 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.2/jhub/util.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 08:52:19.174488 jhub-swarmspawner-0.4.2/jhub_swarmspawner.egg-info/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    14462 2023-05-02 08:52:19.000000 jhub-swarmspawner-0.4.2/jhub_swarmspawner.egg-info/PKG-INFO
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      465 2023-05-02 08:52:19.000000 jhub-swarmspawner-0.4.2/jhub_swarmspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        1 2023-05-02 08:52:19.000000 jhub-swarmspawner-0.4.2/jhub_swarmspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      204 2023-05-02 08:52:19.000000 jhub-swarmspawner-0.4.2/jhub_swarmspawner.egg-info/requires.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        5 2023-05-02 08:52:19.000000 jhub-swarmspawner-0.4.2/jhub_swarmspawner.egg-info/top_level.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       38 2023-05-02 08:52:19.174488 jhub-swarmspawner-0.4.2/setup.cfg
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1698 2023-03-02 09:23:01.000000 jhub-swarmspawner-0.4.2/setup.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2023-05-02 08:52:19.174488 jhub-swarmspawner-0.4.2/tests/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     9898 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.2/tests/test_auth_service.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     9373 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.2/tests/test_mount_service.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    10366 2023-05-02 07:51:24.000000 jhub-swarmspawner-0.4.2/tests/test_service.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     5319 2023-05-02 08:04:57.000000 jhub-swarmspawner-0.4.2/tests/test_ulimit_service.py
```

### Comparing `jhub-swarmspawner-0.4.1/LICENSE` & `jhub-swarmspawner-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.1/PKG-INFO` & `jhub-swarmspawner-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhub-swarmspawner
-Version: 0.4.1
+Version: 0.4.2
 Summary: SwarmSpawner enables JupyterHub to spawn jupyter
 Home-page: https://github.com/rasmunk/SwarmSpawner
 Author: Rasmus Munk
 Author-email: rasmus.munk@nbi.ku.dk
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jhub-swarmspawner-0.4.1/README.rst` & `jhub-swarmspawner-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.1/jhub/accelerators.py` & `jhub-swarmspawner-0.4.2/jhub/accelerators.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.1/jhub/io.py` & `jhub-swarmspawner-0.4.2/jhub/io.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.1/jhub/mount.py` & `jhub-swarmspawner-0.4.2/jhub/mount.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.1/jhub/swarmspawner.py` & `jhub-swarmspawner-0.4.2/jhub/swarmspawner.py`

 * *Files 1% similar despite different names*

```diff
@@ -723,21 +723,26 @@
                         value = getattr(self.user, attr)
                         if not isinstance(value, dict):
                             value = {attr: value}
                         format_mount_kwargs[attr] = value
 
             # Mounts can be declared as regular dictionaries
             # or as special Mountable objects (see mount.py)
-            for mount in mounts:
+
+            # Ensure that the formatted mount config does not persist
+            # across user sessions
+            mount_templates = copy.deepcopy(mounts)
+            for mount in mount_templates:
                 if isinstance(mount, dict):
                     m = VolumeMounter(mount)
                     m = yield m.create(**format_mount_kwargs)
                 else:
                     # Custom type mount defined
                     # Is instantiated in the config
+
                     m = yield mount.create(**format_mount_kwargs)
                 container_spec["mounts"].append(m)
 
             # Some envs are required by the single-user-image
             if "env" in container_spec:
                 container_spec["env"].update(self.get_env())
             else:
```

### Comparing `jhub-swarmspawner-0.4.1/jhub/util.py` & `jhub-swarmspawner-0.4.2/jhub/util.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.1/jhub_swarmspawner.egg-info/PKG-INFO` & `jhub-swarmspawner-0.4.2/jhub_swarmspawner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhub-swarmspawner
-Version: 0.4.1
+Version: 0.4.2
 Summary: SwarmSpawner enables JupyterHub to spawn jupyter
 Home-page: https://github.com/rasmunk/SwarmSpawner
 Author: Rasmus Munk
 Author-email: rasmus.munk@nbi.ku.dk
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jhub-swarmspawner-0.4.1/setup.py` & `jhub-swarmspawner-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.1/tests/test_auth_service.py` & `jhub-swarmspawner-0.4.2/tests/test_auth_service.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.1/tests/test_mount_service.py` & `jhub-swarmspawner-0.4.2/tests/test_mount_service.py`

 * *Files identical despite different names*

### Comparing `jhub-swarmspawner-0.4.1/tests/test_service.py` & `jhub-swarmspawner-0.4.2/tests/test_service.py`

 * *Files identical despite different names*

