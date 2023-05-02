# Comparing `tmp/cloudmesh-gpu-4.3.8.tar.gz` & `tmp/cloudmesh-gpu-4.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudmesh-gpu-4.3.8.tar", last modified: Mon Mar  7 18:05:42 2022, max compression
+gzip compressed data, was "cloudmesh-gpu-4.3.9.tar", last modified: Sat Mar 12 14:38:57 2022, max compression
```

## Comparing `cloudmesh-gpu-4.3.8.tar` & `cloudmesh-gpu-4.3.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-07 18:05:42.308542 cloudmesh-gpu-4.3.8/
--rw-rw-r--   0 green     (1000) green     (1000)      778 2022-02-22 00:45:59.000000 cloudmesh-gpu-4.3.8/LICENSE
--rw-rw-r--   0 green     (1000) green     (1000)       99 2022-02-21 18:14:12.000000 cloudmesh-gpu-4.3.8/MANIFEST.in
--rw-rw-r--   0 green     (1000) green     (1000)     1248 2022-03-07 18:05:42.308542 cloudmesh-gpu-4.3.8/PKG-INFO
--rw-rw-r--   0 green     (1000) green     (1000)      426 2022-02-22 00:54:17.000000 cloudmesh-gpu-4.3.8/README.md
--rw-rw-r--   0 green     (1000) green     (1000)        5 2022-03-07 18:05:32.000000 cloudmesh-gpu-4.3.8/VERSION
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-07 18:05:42.308542 cloudmesh-gpu-4.3.8/cloudmesh/
--rw-rw-r--   0 green     (1000) green     (1000)       63 2022-02-21 18:14:12.000000 cloudmesh-gpu-4.3.8/cloudmesh/__init__.py
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-07 18:05:42.308542 cloudmesh-gpu-4.3.8/cloudmesh/gpu/
--rw-rw-r--   0 green     (1000) green     (1000)       22 2022-03-07 18:05:32.000000 cloudmesh-gpu-4.3.8/cloudmesh/gpu/__init__.py
--rw-rw-r--   0 green     (1000) green     (1000)       18 2022-03-07 18:05:32.000000 cloudmesh-gpu-4.3.8/cloudmesh/gpu/__version__.py
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-07 18:05:42.308542 cloudmesh-gpu-4.3.8/cloudmesh/gpu/command/
--rw-rw-r--   0 green     (1000) green     (1000)        0 2022-02-21 18:14:12.000000 cloudmesh-gpu-4.3.8/cloudmesh/gpu/command/__init__.py
--rw-rw-r--   0 green     (1000) green     (1000)     2478 2022-03-07 12:50:57.000000 cloudmesh-gpu-4.3.8/cloudmesh/gpu/command/gpu.py
--rw-rw-r--   0 green     (1000) green     (1000)     6847 2022-03-07 18:04:28.000000 cloudmesh-gpu-4.3.8/cloudmesh/gpu/gpu.py
-drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-07 18:05:42.308542 cloudmesh-gpu-4.3.8/cloudmesh_gpu.egg-info/
--rw-rw-r--   0 green     (1000) green     (1000)     1248 2022-03-07 18:05:42.000000 cloudmesh-gpu-4.3.8/cloudmesh_gpu.egg-info/PKG-INFO
--rw-rw-r--   0 green     (1000) green     (1000)      521 2022-03-07 18:05:42.000000 cloudmesh-gpu-4.3.8/cloudmesh_gpu.egg-info/SOURCES.txt
--rw-rw-r--   0 green     (1000) green     (1000)        1 2022-03-07 18:05:42.000000 cloudmesh-gpu-4.3.8/cloudmesh_gpu.egg-info/dependency_links.txt
--rw-rw-r--   0 green     (1000) green     (1000)       10 2022-03-07 18:05:42.000000 cloudmesh-gpu-4.3.8/cloudmesh_gpu.egg-info/namespace_packages.txt
--rw-rw-r--   0 green     (1000) green     (1000)        1 2022-03-07 18:05:42.000000 cloudmesh-gpu-4.3.8/cloudmesh_gpu.egg-info/not-zip-safe
--rw-rw-r--   0 green     (1000) green     (1000)       83 2022-03-07 18:05:42.000000 cloudmesh-gpu-4.3.8/cloudmesh_gpu.egg-info/requires.txt
--rw-rw-r--   0 green     (1000) green     (1000)       10 2022-03-07 18:05:42.000000 cloudmesh-gpu-4.3.8/cloudmesh_gpu.egg-info/top_level.txt
--rw-rw-r--   0 green     (1000) green     (1000)       23 2022-02-21 18:14:12.000000 cloudmesh-gpu-4.3.8/requirements-dev.txt
--rw-rw-r--   0 green     (1000) green     (1000)      663 2022-02-21 23:41:34.000000 cloudmesh-gpu-4.3.8/requirements.txt
--rw-rw-r--   0 green     (1000) green     (1000)       67 2022-03-07 18:05:42.308542 cloudmesh-gpu-4.3.8/setup.cfg
--rw-rw-r--   0 green     (1000) green     (1000)     2859 2022-02-21 23:41:34.000000 cloudmesh-gpu-4.3.8/setup.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-12 14:38:57.847973 cloudmesh-gpu-4.3.9/
+-rw-rw-r--   0 green     (1000) green     (1000)      778 2022-02-22 00:45:59.000000 cloudmesh-gpu-4.3.9/LICENSE
+-rw-rw-r--   0 green     (1000) green     (1000)       99 2022-02-21 18:14:12.000000 cloudmesh-gpu-4.3.9/MANIFEST.in
+-rw-rw-r--   0 green     (1000) green     (1000)     1248 2022-03-12 14:38:57.847973 cloudmesh-gpu-4.3.9/PKG-INFO
+-rw-rw-r--   0 green     (1000) green     (1000)      426 2022-02-22 00:54:17.000000 cloudmesh-gpu-4.3.9/README.md
+-rw-rw-r--   0 green     (1000) green     (1000)        5 2022-03-12 14:38:47.000000 cloudmesh-gpu-4.3.9/VERSION
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-12 14:38:57.847973 cloudmesh-gpu-4.3.9/cloudmesh/
+-rw-rw-r--   0 green     (1000) green     (1000)       63 2022-02-21 18:14:12.000000 cloudmesh-gpu-4.3.9/cloudmesh/__init__.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-12 14:38:57.847973 cloudmesh-gpu-4.3.9/cloudmesh/gpu/
+-rw-rw-r--   0 green     (1000) green     (1000)       22 2022-03-12 14:38:47.000000 cloudmesh-gpu-4.3.9/cloudmesh/gpu/__init__.py
+-rw-rw-r--   0 green     (1000) green     (1000)       18 2022-03-12 14:38:47.000000 cloudmesh-gpu-4.3.9/cloudmesh/gpu/__version__.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-12 14:38:57.847973 cloudmesh-gpu-4.3.9/cloudmesh/gpu/command/
+-rw-rw-r--   0 green     (1000) green     (1000)        0 2022-02-21 18:14:12.000000 cloudmesh-gpu-4.3.9/cloudmesh/gpu/command/__init__.py
+-rw-rw-r--   0 green     (1000) green     (1000)     2882 2022-03-12 14:38:04.000000 cloudmesh-gpu-4.3.9/cloudmesh/gpu/command/gpu.py
+-rw-rw-r--   0 green     (1000) green     (1000)     9135 2022-03-12 14:31:51.000000 cloudmesh-gpu-4.3.9/cloudmesh/gpu/gpu.py
+drwxrwxr-x   0 green     (1000) green     (1000)        0 2022-03-12 14:38:57.847973 cloudmesh-gpu-4.3.9/cloudmesh_gpu.egg-info/
+-rw-rw-r--   0 green     (1000) green     (1000)     1248 2022-03-12 14:38:57.000000 cloudmesh-gpu-4.3.9/cloudmesh_gpu.egg-info/PKG-INFO
+-rw-rw-r--   0 green     (1000) green     (1000)      521 2022-03-12 14:38:57.000000 cloudmesh-gpu-4.3.9/cloudmesh_gpu.egg-info/SOURCES.txt
+-rw-rw-r--   0 green     (1000) green     (1000)        1 2022-03-12 14:38:57.000000 cloudmesh-gpu-4.3.9/cloudmesh_gpu.egg-info/dependency_links.txt
+-rw-rw-r--   0 green     (1000) green     (1000)       10 2022-03-12 14:38:57.000000 cloudmesh-gpu-4.3.9/cloudmesh_gpu.egg-info/namespace_packages.txt
+-rw-rw-r--   0 green     (1000) green     (1000)        1 2022-03-12 14:38:57.000000 cloudmesh-gpu-4.3.9/cloudmesh_gpu.egg-info/not-zip-safe
+-rw-rw-r--   0 green     (1000) green     (1000)       83 2022-03-12 14:38:57.000000 cloudmesh-gpu-4.3.9/cloudmesh_gpu.egg-info/requires.txt
+-rw-rw-r--   0 green     (1000) green     (1000)       10 2022-03-12 14:38:57.000000 cloudmesh-gpu-4.3.9/cloudmesh_gpu.egg-info/top_level.txt
+-rw-rw-r--   0 green     (1000) green     (1000)       23 2022-02-21 18:14:12.000000 cloudmesh-gpu-4.3.9/requirements-dev.txt
+-rw-rw-r--   0 green     (1000) green     (1000)      663 2022-02-21 23:41:34.000000 cloudmesh-gpu-4.3.9/requirements.txt
+-rw-rw-r--   0 green     (1000) green     (1000)       67 2022-03-12 14:38:57.847973 cloudmesh-gpu-4.3.9/setup.cfg
+-rw-rw-r--   0 green     (1000) green     (1000)     2859 2022-02-21 23:41:34.000000 cloudmesh-gpu-4.3.9/setup.py
```

### Comparing `cloudmesh-gpu-4.3.8/LICENSE` & `cloudmesh-gpu-4.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudmesh-gpu-4.3.8/PKG-INFO` & `cloudmesh-gpu-4.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmesh-gpu
-Version: 4.3.8
+Version: 4.3.9
 Summary: A command called gpu and foo for the cloudmesh shell
 Home-page: https://github.com/cloudmesh/cloudmesh-gpu
 Author: Gregor von Laszewski
 Author-email: laszewski@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cloudmesh-gpu-4.3.8/cloudmesh/gpu/command/gpu.py` & `cloudmesh-gpu-4.3.9/cloudmesh/gpu/command/gpu.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,44 +16,56 @@
     # noinspection PyUnusedLocal
     @command
     def do_gpu(self, args, arguments):
         """
         ::
 
           Usage:
+                gpu watch [--delay=SECONDS] [--logfile=LOGFILE]
                 gpu --json [--pretty]
                 gpu --xml
                 gpu --yaml
                 gpu processes
                 gpu system
                 gpu status
                 gpu count
                 gpu
 
           This command returns some information about NVIDIA GPUs if your 
           system has them.
 
           Options:
-              --json   returns the information in json
-              --xml    returns the information in xml
-              --yaml   returns the information in xml
-
+              --json              returns the information in json
+              --xml               returns the information in xml
+              --yaml              returns the information in xml
+              --logfile=LOGFILE   the logfile
 
         """
 
+        # VERBOSE(arguments)
+
         map_parameters(arguments,
                        "json",
                        "xml",
                        "yaml",
-                       "pretty")
+                       "pretty",
+                       "delay",
+                       "logfile")
 
         try:
             gpu = Gpu()
 
-            if arguments.xml:
+            if arguments.watch:
+
+                gpu.watch(logfile=arguments.logfile,
+                          delay=arguments.delay)
+
+                return ""
+
+            elif arguments.xml:
                 try:
                     result = gpu.smi(output="xml")
                 except:
                     Console.error("nvidia-smi must be installed on the system")
                     return ""
 
             elif arguments.json and arguments.pertty:
@@ -77,14 +89,15 @@
                 arguments.pretty = True
                 result = gpu.status()
 
             elif arguments.count:
                 arguments.pretty = True
                 result = gpu.count
 
+
             else:
                 result = gpu.smi()
 
             try:
                 if arguments.pretty:
                     result = json.dumps(result, indent=2)
             except:
```

### Comparing `cloudmesh-gpu-4.3.8/cloudmesh_gpu.egg-info/PKG-INFO` & `cloudmesh-gpu-4.3.9/cloudmesh_gpu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmesh-gpu
-Version: 4.3.8
+Version: 4.3.9
 Summary: A command called gpu and foo for the cloudmesh shell
 Home-page: https://github.com/cloudmesh/cloudmesh-gpu
 Author: Gregor von Laszewski
 Author-email: laszewski@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cloudmesh-gpu-4.3.8/cloudmesh_gpu.egg-info/SOURCES.txt` & `cloudmesh-gpu-4.3.9/cloudmesh_gpu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudmesh-gpu-4.3.8/requirements.txt` & `cloudmesh-gpu-4.3.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `cloudmesh-gpu-4.3.8/setup.py` & `cloudmesh-gpu-4.3.9/setup.py`

 * *Files identical despite different names*

