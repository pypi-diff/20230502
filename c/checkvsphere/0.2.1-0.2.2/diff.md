# Comparing `tmp/checkvsphere-0.2.1.tar.gz` & `tmp/checkvsphere-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkvsphere-0.2.1.tar", last modified: Fri Apr 21 14:20:19 2023, max compression
+gzip compressed data, was "checkvsphere-0.2.2.tar", last modified: Tue May  2 14:13:36 2023, max compression
```

## Comparing `checkvsphere-0.2.1.tar` & `checkvsphere-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      275 2023-04-21 14:16:49.947749 checkvsphere-0.2.1/README.md
--rw-r--r--   0        0        0      174 2023-04-21 14:16:49.947749 checkvsphere-0.2.1/checkvsphere/__init__.py
--rw-r--r--   0        0        0     3882 2023-04-21 14:16:49.959749 checkvsphere-0.2.1/checkvsphere/cli.py
--rw-r--r--   0        0        0      760 2023-04-21 14:16:49.971748 checkvsphere-0.2.1/checkvsphere/tools/__init__.py
--rw-r--r--   0        0        0    16614 2023-04-21 14:16:49.971748 checkvsphere-0.2.1/checkvsphere/tools/cli.py
--rw-r--r--   0        0        0     6363 2023-04-21 14:16:49.971748 checkvsphere-0.2.1/checkvsphere/tools/helper.py
--rw-r--r--   0        0        0     5200 2023-04-21 14:16:49.971748 checkvsphere-0.2.1/checkvsphere/tools/pchelper.py
--rw-r--r--   0        0        0     2183 2023-04-21 14:16:49.971748 checkvsphere-0.2.1/checkvsphere/tools/service_instance.py
--rw-r--r--   0        0        0     4153 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/tools/serviceutil.py
--rw-r--r--   0        0        0      760 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/vcmd/__init__.py
--rw-r--r--   0        0        0     1819 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/vcmd/about.py
--rw-r--r--   0        0        0     6509 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/vcmd/datastores.py
--rw-r--r--   0        0        0     4497 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/vcmd/hostnic.py
--rw-r--r--   0        0        0    10722 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/vcmd/hostruntime.py
--rw-r--r--   0        0        0     4038 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/vcmd/hostservice.py
--rw-r--r--   0        0        0     7633 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/vcmd/hoststorage.py
--rw-r--r--   0        0        0     2039 2023-04-21 14:16:49.983748 checkvsphere-0.2.1/checkvsphere/vcmd/listmetrics.py
--rw-r--r--   0        0        0     3341 2023-04-21 14:16:49.983748 checkvsphere-0.2.1/checkvsphere/vcmd/media.py
--rw-r--r--   0        0        0     8301 2023-04-21 14:16:49.983748 checkvsphere-0.2.1/checkvsphere/vcmd/perf.py
--rw-r--r--   0        0        0     4929 2023-04-21 14:16:49.983748 checkvsphere-0.2.1/checkvsphere/vcmd/snapshots.py
--rw-r--r--   0        0        0     8945 2023-04-21 14:16:49.983748 checkvsphere-0.2.1/checkvsphere/vcmd/vsan.py
--rw-r--r--   0        0        0      941 2023-04-21 14:16:49.987748 checkvsphere-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 checkvsphere-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      275 2023-04-21 14:16:49.947749 checkvsphere-0.2.2/README.md
+-rw-r--r--   0        0        0      174 2023-04-21 14:16:49.947749 checkvsphere-0.2.2/checkvsphere/__init__.py
+-rw-r--r--   0        0        0     3882 2023-04-21 14:16:49.959749 checkvsphere-0.2.2/checkvsphere/cli.py
+-rw-r--r--   0        0        0      760 2023-04-21 14:16:49.971748 checkvsphere-0.2.2/checkvsphere/tools/__init__.py
+-rw-r--r--   0        0        0    16614 2023-04-21 14:16:49.971748 checkvsphere-0.2.2/checkvsphere/tools/cli.py
+-rw-r--r--   0        0        0     6363 2023-04-21 14:16:49.971748 checkvsphere-0.2.2/checkvsphere/tools/helper.py
+-rw-r--r--   0        0        0     5200 2023-04-21 14:16:49.971748 checkvsphere-0.2.2/checkvsphere/tools/pchelper.py
+-rw-r--r--   0        0        0     2183 2023-04-21 14:16:49.971748 checkvsphere-0.2.2/checkvsphere/tools/service_instance.py
+-rw-r--r--   0        0        0     4153 2023-04-21 14:16:49.975748 checkvsphere-0.2.2/checkvsphere/tools/serviceutil.py
+-rw-r--r--   0        0        0      760 2023-04-21 14:16:49.975748 checkvsphere-0.2.2/checkvsphere/vcmd/__init__.py
+-rw-r--r--   0        0        0     1819 2023-04-21 14:16:49.975748 checkvsphere-0.2.2/checkvsphere/vcmd/about.py
+-rw-r--r--   0        0        0     6692 2023-05-02 11:25:14.016969 checkvsphere-0.2.2/checkvsphere/vcmd/datastores.py
+-rw-r--r--   0        0        0     4497 2023-04-21 14:16:49.975748 checkvsphere-0.2.2/checkvsphere/vcmd/hostnic.py
+-rw-r--r--   0        0        0    11156 2023-04-28 12:52:00.785872 checkvsphere-0.2.2/checkvsphere/vcmd/hostruntime.py
+-rw-r--r--   0        0        0     4038 2023-04-21 14:16:49.975748 checkvsphere-0.2.2/checkvsphere/vcmd/hostservice.py
+-rw-r--r--   0        0        0     7633 2023-04-21 14:16:49.975748 checkvsphere-0.2.2/checkvsphere/vcmd/hoststorage.py
+-rw-r--r--   0        0        0     2039 2023-04-21 14:16:49.983748 checkvsphere-0.2.2/checkvsphere/vcmd/listmetrics.py
+-rw-r--r--   0        0        0     3341 2023-04-21 14:16:49.983748 checkvsphere-0.2.2/checkvsphere/vcmd/media.py
+-rw-r--r--   0        0        0     8301 2023-04-21 14:16:49.983748 checkvsphere-0.2.2/checkvsphere/vcmd/perf.py
+-rw-r--r--   0        0        0     4929 2023-04-21 14:16:49.983748 checkvsphere-0.2.2/checkvsphere/vcmd/snapshots.py
+-rw-r--r--   0        0        0     8945 2023-04-21 14:16:49.983748 checkvsphere-0.2.2/checkvsphere/vcmd/vsan.py
+-rw-r--r--   0        0        0      941 2023-05-02 14:12:48.139031 checkvsphere-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 checkvsphere-0.2.2/PKG-INFO
```

### Comparing `checkvsphere-0.2.1/checkvsphere/cli.py` & `checkvsphere-0.2.2/checkvsphere/cli.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/tools/__init__.py` & `checkvsphere-0.2.2/checkvsphere/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/tools/cli.py` & `checkvsphere-0.2.2/checkvsphere/tools/cli.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/tools/helper.py` & `checkvsphere-0.2.2/checkvsphere/tools/helper.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/tools/pchelper.py` & `checkvsphere-0.2.2/checkvsphere/tools/pchelper.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/tools/service_instance.py` & `checkvsphere-0.2.2/checkvsphere/tools/service_instance.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/tools/serviceutil.py` & `checkvsphere-0.2.2/checkvsphere/tools/serviceutil.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/vcmd/__init__.py` & `checkvsphere-0.2.2/checkvsphere/vcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/vcmd/about.py` & `checkvsphere-0.2.2/checkvsphere/vcmd/about.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/vcmd/datastores.py` & `checkvsphere-0.2.2/checkvsphere/vcmd/datastores.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,30 +144,34 @@
         objectSet = objs,
         propSet = [propspec],
     )
 
     result = retrieve( [filter_spec] )
     stores = process_retrieve_content(result)
 
-
     for store in stores:
-
-        name = store['summary'].name
+        name = f"{ store['moref']._moId }_{store['summary'].name}"
         datastore_type = store['summary'].type
 
         if isbanned(args, f"{name}"):
             continue
         if not isallowed(args, f"{name}"):
             continue
 
         if not store['summary'].accessible:
             check.add_message(Status.CRITICAL, f"{name} is not accessible")
             continue
 
-        space = Space(store['summary'].capacity, store['summary'].freeSpace)
+        try:
+            space = Space(store['summary'].capacity, store['summary'].freeSpace)
+        except ZeroDivisionError:
+            check.add_message(Status.CRITICAL, f"{name} has a capacity of zero")
+            continue
+
+
         for metric in ['usage', 'free', 'used', 'capacity']:
             opts = {}
 
             # Check threshold against this metric
             if args.metric.startswith(metric) and (args.warning or args.critical):
                 value = space[args.metric]
                 _, uom, *_ = (args.metric.split('_') + ['%' if 'usage' in args.metric else 'B'])
```

### Comparing `checkvsphere-0.2.1/checkvsphere/vcmd/hostnic.py` & `checkvsphere-0.2.2/checkvsphere/vcmd/hostnic.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/vcmd/hostruntime.py` & `checkvsphere-0.2.2/checkvsphere/vcmd/hostruntime.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,14 +202,27 @@
         check.add_message(state, f"{name} is {info.healthState.key}")
 
     return "All temperature sensors green"
 
 def check_health(check, vm, args, result):
     runtime = vm['props']['runtime']
     healthsystem = runtime.healthSystemRuntime
+    if not healthsystem:
+        check.exit(
+            Status.UNKNOWN,
+            "system health status not available, "
+            "no vim.Host.runtime.healthSystemRuntime found"
+        )
+    if not healthsystem.hardwareStatusInfo:
+        check.exit(
+            Status.UNKNOWN,
+            "hardware health information not available, "
+            "no vim.Host.runtime.healthSystemRuntime.hardwareStatusInfo found"
+        )
+
     filterunknown = lambda x: x.status.key != "unknown"
     cpustatus = healthsystem.hardwareStatusInfo.cpuStatusInfo
     storagestatus = list(filter(filterunknown, healthsystem.hardwareStatusInfo.storageStatusInfo))
     memorystatus = list(filter(filterunknown, healthsystem.hardwareStatusInfo.memoryStatusInfo))
     numericsensor = healthsystem.systemHealthInfo.numericSensorInfo
 
     count = {}
```

### Comparing `checkvsphere-0.2.1/checkvsphere/vcmd/hostservice.py` & `checkvsphere-0.2.2/checkvsphere/vcmd/hostservice.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/vcmd/hoststorage.py` & `checkvsphere-0.2.2/checkvsphere/vcmd/hoststorage.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/vcmd/listmetrics.py` & `checkvsphere-0.2.2/checkvsphere/vcmd/listmetrics.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/vcmd/media.py` & `checkvsphere-0.2.2/checkvsphere/vcmd/media.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/vcmd/perf.py` & `checkvsphere-0.2.2/checkvsphere/vcmd/perf.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/vcmd/snapshots.py` & `checkvsphere-0.2.2/checkvsphere/vcmd/snapshots.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/checkvsphere/vcmd/vsan.py` & `checkvsphere-0.2.2/checkvsphere/vcmd/vsan.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.1/pyproject.toml` & `checkvsphere-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "checkvsphere"
 readme = "README.md"
 description = "check_vsphere monitoring plugin"
-version = "0.2.1"
+version = "0.2.2"
 requires-python = ">= 3.6"
 authors = [
     { name = "Danijel Tasov", email = "danijel.tasov@consol.de" }
 ]
 dependencies = [
     "pyvmomi >= 8.0.0.1, < 9",
-    "monplugin >= 0.6.0",
+    "monplugin >= 0.6.1",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: System :: Monitoring",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
 ]
```

### Comparing `checkvsphere-0.2.1/PKG-INFO` & `checkvsphere-0.2.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: checkvsphere
-Version: 0.2.1
+Version: 0.2.2
 Summary: check_vsphere monitoring plugin
 Author-email: Danijel Tasov <danijel.tasov@consol.de>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Dist: pyvmomi >= 8.0.0.1, < 9
-Requires-Dist: monplugin >= 0.6.0
+Requires-Dist: monplugin >= 0.6.1
 Project-URL: documentation, https://consol.github.io/check_vsphere
 Project-URL: homepage, https://github.com/consol/check_vsphere
 Project-URL: issues, https://github.com/consol/check_vsphere/issues
 Project-URL: repository, https://github.com/consol/check_vsphere.git
 
 [Documentation](https://consol-monitoring.github.io/check_vsphere/#/)
```

