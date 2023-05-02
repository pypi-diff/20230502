# Comparing `tmp/netcontrol-1.93.tar.gz` & `tmp/netcontrol-1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netcontrol-1.93.tar", last modified: Tue May  2 16:32:59 2023, max compression
+gzip compressed data, was "netcontrol-1.94.tar", last modified: Tue May  2 16:35:00 2023, max compression
```

## Comparing `netcontrol-1.93.tar` & `netcontrol-1.94.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:59.517627 netcontrol-1.93/
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)     1074 2023-05-02 16:32:59.000000 netcontrol-1.93/LICENSE
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)      243 2023-05-02 16:32:57.000000 netcontrol-1.93/MANIFEST.in
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)      672 2023-05-02 16:32:59.517627 netcontrol-1.93/PKG-INFO
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)      130 2023-05-02 16:32:57.000000 netcontrol-1.93/README.md
-drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:59.505627 netcontrol-1.93/netcontrol/
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/__init__.py
-drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:59.509627 netcontrol-1.93/netcontrol/fortigate/
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/fortigate/__init__.py
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)    25066 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/fortigate/fortigate.py
-drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:59.509627 netcontrol-1.93/netcontrol/fortiswitch/
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/fortiswitch/__init__.py
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)     4766 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/fortiswitch/fortiswitch.py
-drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:59.509627 netcontrol-1.93/netcontrol/fpoc/
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/fpoc/__init__.py
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)     6871 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/fpoc/fpoc.py
-drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:59.513627 netcontrol-1.93/netcontrol/ssh/
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/ssh/__init__.py
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)    23900 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/ssh/ssh.py
--rwxrwxr-x   0 cgustave  (1000) cgustave  (1000)      411 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/ssh/test2_paramiko.py
--rwxrwxr-x   0 cgustave  (1000) cgustave  (1000)      356 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/ssh/test3_paramiko.py
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)      240 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/ssh/test4.py
--rwxrwxr-x   0 cgustave  (1000) cgustave  (1000)      382 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/ssh/test4_paramiko.py
--rwxrwxr-x   0 cgustave  (1000) cgustave  (1000)      345 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/ssh/test_paramiko.py
-drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:59.513627 netcontrol-1.93/netcontrol/vm/
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/vm/__init__.py
--rwxrwxr-x   0 cgustave  (1000) cgustave  (1000)      199 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/vm/test5.py
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)    43035 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/vm/vm.py
-drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:59.517627 netcontrol-1.93/netcontrol/vyos/
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/vyos/__init__.py
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)    13216 2023-05-02 16:32:57.000000 netcontrol-1.93/netcontrol/vyos/vyos.py
-drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:32:59.509627 netcontrol-1.93/netcontrol.egg-info/
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)      672 2023-05-02 16:32:59.000000 netcontrol-1.93/netcontrol.egg-info/PKG-INFO
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)      714 2023-05-02 16:32:59.000000 netcontrol-1.93/netcontrol.egg-info/SOURCES.txt
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        1 2023-05-02 16:32:59.000000 netcontrol-1.93/netcontrol.egg-info/dependency_links.txt
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)       11 2023-05-02 16:32:59.000000 netcontrol-1.93/netcontrol.egg-info/top_level.txt
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)       38 2023-05-02 16:32:59.517627 netcontrol-1.93/setup.cfg
--rw-rw-r--   0 cgustave  (1000) cgustave  (1000)      732 2023-05-02 16:32:59.000000 netcontrol-1.93/setup.py
+drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:35:00.162760 netcontrol-1.94/
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)     1074 2023-05-02 16:34:59.000000 netcontrol-1.94/LICENSE
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)      243 2023-05-02 16:34:57.000000 netcontrol-1.94/MANIFEST.in
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)      672 2023-05-02 16:35:00.162760 netcontrol-1.94/PKG-INFO
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)      130 2023-05-02 16:34:57.000000 netcontrol-1.94/README.md
+drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:35:00.154760 netcontrol-1.94/netcontrol/
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/__init__.py
+drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:35:00.154760 netcontrol-1.94/netcontrol/fortigate/
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/fortigate/__init__.py
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)    25066 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/fortigate/fortigate.py
+drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:35:00.158760 netcontrol-1.94/netcontrol/fortiswitch/
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/fortiswitch/__init__.py
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)     4766 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/fortiswitch/fortiswitch.py
+drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:35:00.158760 netcontrol-1.94/netcontrol/fpoc/
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/fpoc/__init__.py
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)     6871 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/fpoc/fpoc.py
+drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:35:00.158760 netcontrol-1.94/netcontrol/ssh/
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/ssh/__init__.py
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)    23900 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/ssh/ssh.py
+-rwxrwxr-x   0 cgustave  (1000) cgustave  (1000)      411 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/ssh/test2_paramiko.py
+-rwxrwxr-x   0 cgustave  (1000) cgustave  (1000)      356 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/ssh/test3_paramiko.py
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)      240 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/ssh/test4.py
+-rwxrwxr-x   0 cgustave  (1000) cgustave  (1000)      382 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/ssh/test4_paramiko.py
+-rwxrwxr-x   0 cgustave  (1000) cgustave  (1000)      345 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/ssh/test_paramiko.py
+drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:35:00.162760 netcontrol-1.94/netcontrol/vm/
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/vm/__init__.py
+-rwxrwxr-x   0 cgustave  (1000) cgustave  (1000)      199 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/vm/test5.py
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)    43147 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/vm/vm.py
+drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:35:00.162760 netcontrol-1.94/netcontrol/vyos/
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/vyos/__init__.py
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)    13216 2023-05-02 16:34:57.000000 netcontrol-1.94/netcontrol/vyos/vyos.py
+drwxrwxr-x   0 cgustave  (1000) cgustave  (1000)        0 2023-05-02 16:35:00.154760 netcontrol-1.94/netcontrol.egg-info/
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)      672 2023-05-02 16:35:00.000000 netcontrol-1.94/netcontrol.egg-info/PKG-INFO
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)      714 2023-05-02 16:35:00.000000 netcontrol-1.94/netcontrol.egg-info/SOURCES.txt
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)        1 2023-05-02 16:35:00.000000 netcontrol-1.94/netcontrol.egg-info/dependency_links.txt
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)       11 2023-05-02 16:35:00.000000 netcontrol-1.94/netcontrol.egg-info/top_level.txt
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)       38 2023-05-02 16:35:00.162760 netcontrol-1.94/setup.cfg
+-rw-rw-r--   0 cgustave  (1000) cgustave  (1000)      732 2023-05-02 16:34:59.000000 netcontrol-1.94/setup.py
```

### Comparing `netcontrol-1.93/LICENSE` & `netcontrol-1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `netcontrol-1.93/PKG-INFO` & `netcontrol-1.94/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netcontrol
-Version: 1.93
+Version: 1.94
 Summary: Package netcontrol
 Home-page: https://github.com/cgustave/netcontrol
 Author: Cedric GUSTAVE
 Author-email: cgustave@free.fr
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netcontrol-1.93/netcontrol/fortigate/fortigate.py` & `netcontrol-1.94/netcontrol/fortigate/fortigate.py`

 * *Files identical despite different names*

### Comparing `netcontrol-1.93/netcontrol/fortiswitch/fortiswitch.py` & `netcontrol-1.94/netcontrol/fortiswitch/fortiswitch.py`

 * *Files identical despite different names*

### Comparing `netcontrol-1.93/netcontrol/fpoc/fpoc.py` & `netcontrol-1.94/netcontrol/fpoc/fpoc.py`

 * *Files identical despite different names*

### Comparing `netcontrol-1.93/netcontrol/ssh/ssh.py` & `netcontrol-1.94/netcontrol/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `netcontrol-1.93/netcontrol/vm/vm.py` & `netcontrol-1.94/netcontrol/vm/vm.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,14 +443,16 @@
                 match_name = re.search("(?P<vm_name>\S+)\s\[(?P<create_user>\S+)\]\s(?P<system>\S+)", line)
                 if match_name:
                     vm_name = match_name.group('vm_name')
                     create_user = match_name.group('create_user')
                     system = match_name.group('system')
                     self._vms_total['number'] += 1
                     log.debug("Found new vm_name={} create_user={} system={} total_number={}".format(vm_name, create_user, system, self._vms_total['number']))
+                else:
+                    log.warning("VM does not look like an LMS vms")
             if esx_start:
                 match_esxid = re.search("VMX\sCartel\sID:\s(?P<vm_esxid>\d+)", line)
                 if match_esxid:
                     vm_esxid = match_esxid.group('vm_esxid')
                     log.debug("Found {} vm_esxid={}".format(vm_name, vm_esxid))
                     self._vms_esx_id_map[vm_esxid] = vm_name
                     if vm_esxid in self._vms_esx_memory:
@@ -498,20 +500,21 @@
                         ret = False
                     self._vms.append(vm)
                 else:
                     log.warning("got unexpected instance format instance={}".format(instance))
                     ret = False
         return ret
 
-    def _get_vm_instance_from_name(self,name=""):
+    def _get_vm_instance_from_name(self, name=""):
         """
         VM instance is like 001, 011, 122 and so on.
         It should be extracted from server name (ex: uranium-tam-esx42)
         """
         log.debug("Enter with name={}".format(name))
+        result = "" 
         match_inst = re.search("(?P<inst>\d+)$", name)
         if match_inst:
             inst = match_inst.group('inst')
             result = str(inst).zfill(3)
             log.debug("formatted instance result={}".format(result))
         else:
             log.warning("Could not extract formatted instance from name={}".format(name))
```

### Comparing `netcontrol-1.93/netcontrol/vyos/vyos.py` & `netcontrol-1.94/netcontrol/vyos/vyos.py`

 * *Files identical despite different names*

### Comparing `netcontrol-1.93/netcontrol.egg-info/PKG-INFO` & `netcontrol-1.94/netcontrol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netcontrol
-Version: 1.93
+Version: 1.94
 Summary: Package netcontrol
 Home-page: https://github.com/cgustave/netcontrol
 Author: Cedric GUSTAVE
 Author-email: cgustave@free.fr
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `netcontrol-1.93/netcontrol.egg-info/SOURCES.txt` & `netcontrol-1.94/netcontrol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netcontrol-1.93/setup.py` & `netcontrol-1.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="netcontrol",
-    version="1.93",
+    version="1.94",
     author="Cedric GUSTAVE",
     author_email="cgustave@free.fr",
     description="Package netcontrol",
 	long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/cgustave/netcontrol",
     packages=find_packages(),
```

