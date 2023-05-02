# Comparing `tmp/umnet_scripts-0.0.8.tar.gz` & `tmp/umnet_scripts-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/umnet_scripts-0.0.8.tar", last modified: Mon Dec  6 18:46:57 2021, max compression
+gzip compressed data, was "dist/umnet_scripts-0.0.9.tar", last modified: Tue Dec  7 23:15:55 2021, max compression
```

## Comparing `umnet_scripts-0.0.8.tar` & `umnet_scripts-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 amylieb  (156596) umnet      (200)        0 2021-12-06 18:46:57.000000 umnet_scripts-0.0.8/
-drwxr-xr-x   0 amylieb  (156596) umnet      (200)        0 2021-12-06 18:46:57.000000 umnet_scripts-0.0.8/bin/
--rwxr-xr-x   0 amylieb  (156596) umnet      (200)     3213 2021-06-01 19:56:17.000000 umnet_scripts-0.0.8/bin/equipdb_rancid_audit.py
-drwxr-xr-x   0 amylieb  (156596) umnet      (200)        0 2021-12-06 18:46:57.000000 umnet_scripts-0.0.8/umnet_scripts/
--rw-r--r--   0 amylieb  (156596) umnet      (200)      130 2021-12-06 18:45:51.000000 umnet_scripts-0.0.8/umnet_scripts/__init__.py
--rw-r--r--   0 amylieb  (156596) umnet      (200)     2548 2021-12-06 18:45:51.000000 umnet_scripts-0.0.8/umnet_scripts/constants.py
--rw-r--r--   0 amylieb  (156596) umnet      (200)     8029 2021-12-06 18:45:51.000000 umnet_scripts-0.0.8/umnet_scripts/rancid.py
--rw-r--r--   0 amylieb  (156596) umnet      (200)     2893 2021-12-06 18:45:51.000000 umnet_scripts-0.0.8/umnet_scripts/umnetdb.py
--rw-r--r--   0 amylieb  (156596) umnet      (200)     5095 2021-12-06 18:45:51.000000 umnet_scripts-0.0.8/umnet_scripts/umnetdisco.py
--rw-r--r--   0 amylieb  (156596) umnet      (200)     1516 2021-12-06 18:45:51.000000 umnet_scripts-0.0.8/umnet_scripts/umnetequip.py
--rw-r--r--   0 amylieb  (156596) umnet      (200)     3696 2021-12-06 18:45:51.000000 umnet_scripts-0.0.8/umnet_scripts/umnetinfo.py
--rw-r--r--   0 amylieb  (156596) umnet      (200)     6927 2021-02-11 14:14:08.000000 umnet_scripts-0.0.8/umnet_scripts/umnetnso_restconf.py
--rw-r--r--   0 amylieb  (156596) umnet      (200)     3023 2021-12-06 18:45:51.000000 umnet_scripts-0.0.8/umnet_scripts/utils.py
-drwxr-xr-x   0 amylieb  (156596) umnet      (200)        0 2021-12-06 18:46:57.000000 umnet_scripts-0.0.8/umnet_scripts.egg-info/
--rw-r--r--   0 amylieb  (156596) umnet      (200)      575 2021-12-06 18:46:56.000000 umnet_scripts-0.0.8/umnet_scripts.egg-info/PKG-INFO
--rw-r--r--   0 amylieb  (156596) umnet      (200)      473 2021-12-06 18:46:56.000000 umnet_scripts-0.0.8/umnet_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 amylieb  (156596) umnet      (200)        1 2021-12-06 18:46:56.000000 umnet_scripts-0.0.8/umnet_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 amylieb  (156596) umnet      (200)       71 2021-12-06 18:46:56.000000 umnet_scripts-0.0.8/umnet_scripts.egg-info/requires.txt
--rw-r--r--   0 amylieb  (156596) umnet      (200)       14 2021-12-06 18:46:56.000000 umnet_scripts-0.0.8/umnet_scripts.egg-info/top_level.txt
--rw-r--r--   0 amylieb  (156596) umnet      (200)      113 2021-02-11 14:14:08.000000 umnet_scripts-0.0.8/README.md
--rw-r--r--   0 amylieb  (156596) umnet      (200)      881 2021-12-06 18:46:29.000000 umnet_scripts-0.0.8/setup.py
--rw-r--r--   0 amylieb  (156596) umnet      (200)      575 2021-12-06 18:46:57.000000 umnet_scripts-0.0.8/PKG-INFO
--rw-r--r--   0 amylieb  (156596) umnet      (200)       38 2021-12-06 18:46:57.000000 umnet_scripts-0.0.8/setup.cfg
+drwxr-xr-x   0 amylieb  (156596) umnet      (200)        0 2021-12-07 23:15:55.000000 umnet_scripts-0.0.9/
+drwxr-xr-x   0 amylieb  (156596) umnet      (200)        0 2021-12-07 23:15:55.000000 umnet_scripts-0.0.9/bin/
+-rwxr-xr-x   0 amylieb  (156596) umnet      (200)     3213 2021-06-01 19:56:17.000000 umnet_scripts-0.0.9/bin/equipdb_rancid_audit.py
+drwxr-xr-x   0 amylieb  (156596) umnet      (200)        0 2021-12-07 23:15:55.000000 umnet_scripts-0.0.9/umnet_scripts/
+-rw-r--r--   0 amylieb  (156596) umnet      (200)      130 2021-12-06 18:45:51.000000 umnet_scripts-0.0.9/umnet_scripts/__init__.py
+-rw-r--r--   0 amylieb  (156596) umnet      (200)     2548 2021-12-06 18:45:51.000000 umnet_scripts-0.0.9/umnet_scripts/constants.py
+-rw-r--r--   0 amylieb  (156596) umnet      (200)     8358 2021-12-07 23:12:45.000000 umnet_scripts-0.0.9/umnet_scripts/rancid.py
+-rw-r--r--   0 amylieb  (156596) umnet      (200)     2893 2021-12-06 18:45:51.000000 umnet_scripts-0.0.9/umnet_scripts/umnetdb.py
+-rw-r--r--   0 amylieb  (156596) umnet      (200)     5095 2021-12-06 18:45:51.000000 umnet_scripts-0.0.9/umnet_scripts/umnetdisco.py
+-rw-r--r--   0 amylieb  (156596) umnet      (200)     1516 2021-12-06 18:45:51.000000 umnet_scripts-0.0.9/umnet_scripts/umnetequip.py
+-rw-r--r--   0 amylieb  (156596) umnet      (200)     3696 2021-12-06 18:45:51.000000 umnet_scripts-0.0.9/umnet_scripts/umnetinfo.py
+-rw-r--r--   0 amylieb  (156596) umnet      (200)     6927 2021-02-11 14:14:08.000000 umnet_scripts-0.0.9/umnet_scripts/umnetnso_restconf.py
+-rw-r--r--   0 amylieb  (156596) umnet      (200)     3023 2021-12-06 18:45:51.000000 umnet_scripts-0.0.9/umnet_scripts/utils.py
+drwxr-xr-x   0 amylieb  (156596) umnet      (200)        0 2021-12-07 23:15:55.000000 umnet_scripts-0.0.9/umnet_scripts.egg-info/
+-rw-r--r--   0 amylieb  (156596) umnet      (200)     3169 2021-12-07 23:15:54.000000 umnet_scripts-0.0.9/umnet_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 amylieb  (156596) umnet      (200)      473 2021-12-07 23:15:54.000000 umnet_scripts-0.0.9/umnet_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 amylieb  (156596) umnet      (200)        1 2021-12-07 23:15:54.000000 umnet_scripts-0.0.9/umnet_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 amylieb  (156596) umnet      (200)       71 2021-12-07 23:15:54.000000 umnet_scripts-0.0.9/umnet_scripts.egg-info/requires.txt
+-rw-r--r--   0 amylieb  (156596) umnet      (200)       14 2021-12-07 23:15:54.000000 umnet_scripts-0.0.9/umnet_scripts.egg-info/top_level.txt
+-rw-r--r--   0 amylieb  (156596) umnet      (200)     2435 2021-12-07 19:44:58.000000 umnet_scripts-0.0.9/README.md
+-rw-r--r--   0 amylieb  (156596) umnet      (200)      881 2021-12-07 23:15:41.000000 umnet_scripts-0.0.9/setup.py
+-rw-r--r--   0 amylieb  (156596) umnet      (200)     3169 2021-12-07 23:15:55.000000 umnet_scripts-0.0.9/PKG-INFO
+-rw-r--r--   0 amylieb  (156596) umnet      (200)       38 2021-12-07 23:15:55.000000 umnet_scripts-0.0.9/setup.cfg
```

### Comparing `umnet_scripts-0.0.8/bin/equipdb_rancid_audit.py` & `umnet_scripts-0.0.9/bin/equipdb_rancid_audit.py`

 * *Files identical despite different names*

### Comparing `umnet_scripts-0.0.8/umnet_scripts/constants.py` & `umnet_scripts-0.0.9/umnet_scripts/constants.py`

 * *Files identical despite different names*

### Comparing `umnet_scripts-0.0.8/umnet_scripts/rancid.py` & `umnet_scripts-0.0.9/umnet_scripts/rancid.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,28 @@
 
         if is_ip_address(self.rancid_name):
             return self.rancid_name
         
         return forward_resolve(self.rancid_name)
 
 
+    def __str__(self):
+        return str(dict(self))
+
+class DeviceSet(set):
+
+    def filter(self, **kwargs):
+        output = DeviceSet()
+
+        for k,v in kwargs.items():
+            if k in Device.valid_attrs:
+                output.update([d for d in self if d.__dict__[k] == v])
+        return output
+
+
 class Rancid:
     '''
     A class that provides easy access to rancid data
     stored on the local filesystem. This class is meant to
     be used on wallace/gromit. To use this succesfully
     on a different system you'll have to manually
     re-create '/home/rancid/' on your local system.
@@ -100,20 +114,21 @@
         
         # first we're going to populate an internal device
         # list with Device objects from every router.db
         # in every rancid directory
         self.rancid_dir = rancid_dir
         self.cfg_dirs = cfg_dirs
 
-        self._devices = []
+        self._devices = DeviceSet()
+
         for d in cfg_dirs:
             routerdb = f'{rancid_dir}/{d}/router.db'
             new_devices = self._parse_rdb(routerdb)
             if new_devices:
-                self._devices.extend(new_devices)
+                self._devices.update(new_devices)
             else:
                 logger.error(f'No devices found in {routerdb}')
 
         # Now we're going to parse topologywalker and build connections
         # between the devices
         for d in self._devices:
             neigh_dict = {}
@@ -216,54 +231,54 @@
         if len(device) == 0:
             return False
         if len(device) == 1:
             return device[0]
         raise LookupError(f'More than one device found for {name_or_ip}')
 
 
-    def get_devices(self, **kwargs) -> list:
+    def get_devices(self, **kwargs) -> DeviceSet:
         '''
         Look up a set of devices based on any set of device attributes.
         If no arguments are provided, the full device list is returned.
         '''
-        results = self._devices.copy()
+        results = DeviceSet()
 
         for k,v in kwargs.items():
-            results = [ r for r in results if getattr(r,k) == v ]
+            results.update({ r for r in results if getattr(r,k) == v })
 
         return results
  
     
-    def get_dlzone(self, zone:str) -> list:
+    def get_dlzone(self, zone:str) -> DeviceSet:
         '''
         Returns a list of devices in the same DL zone
         based on neighbors.
         '''
-        devices = []
+        devices = DeviceSet()
         dl1 = self.get_device(f'd-{zone.lower()}-1.umnet.umich.edu')
         if not(dl1):
-            return []
+            return devices
        
-        devices.append(dl1)
+        devices.add(dl1)
 
         dl2 = self.get_device(f'd-{zone.lower()}-2.umnet.umich.edu')
         if dl2:
-            devices.append(dl2)
+            devices.add(dl2)
 
         to_do = devices.copy()
 
         while(len(to_do)):
             d = to_do.pop()
             if not(d.neighbors):
                 continue
             for port, neigh in d.neighbors.items():
 
                 if neigh[0] in CORE_IPS:
                     continue
 
                 n_device = self.get_device(neigh[0])
                 if n_device and n_device not in devices:
-                    devices.append(n_device)
-                    to_do.append(n_device)
+                    devices.add(n_device)
+                    to_do.add(n_device)
                 
         return devices
```

### Comparing `umnet_scripts-0.0.8/umnet_scripts/umnetdb.py` & `umnet_scripts-0.0.9/umnet_scripts/umnetdb.py`

 * *Files identical despite different names*

### Comparing `umnet_scripts-0.0.8/umnet_scripts/umnetdisco.py` & `umnet_scripts-0.0.9/umnet_scripts/umnetdisco.py`

 * *Files identical despite different names*

### Comparing `umnet_scripts-0.0.8/umnet_scripts/umnetequip.py` & `umnet_scripts-0.0.9/umnet_scripts/umnetequip.py`

 * *Files identical despite different names*

### Comparing `umnet_scripts-0.0.8/umnet_scripts/umnetinfo.py` & `umnet_scripts-0.0.9/umnet_scripts/umnetinfo.py`

 * *Files identical despite different names*

### Comparing `umnet_scripts-0.0.8/umnet_scripts/umnetnso_restconf.py` & `umnet_scripts-0.0.9/umnet_scripts/umnetnso_restconf.py`

 * *Files identical despite different names*

### Comparing `umnet_scripts-0.0.8/umnet_scripts/utils.py` & `umnet_scripts-0.0.9/umnet_scripts/utils.py`

 * *Files identical despite different names*

### Comparing `umnet_scripts-0.0.8/setup.py` & `umnet_scripts-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="umnet_scripts",
-    version="0.0.8",
+    version="0.0.9",
     author="University of Michigan",
     author_email="amylieb@umich.edu",
     description="Python tools for interacting with UMnet's network tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.umich.edu/its-inf-net/umnet-scripts",
     packages=setuptools.find_packages(),
```

