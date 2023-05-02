# Comparing `tmp/maya-rig-operation-graph-0.2.3.tar.gz` & `tmp/maya-rig-operation-graph-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\maya-rig-operation-graph-0.2.3.tar", last modified: Sun Apr 30 10:36:39 2023, max compression
+gzip compressed data, was "dist\maya-rig-operation-graph-0.3.3.tar", last modified: Tue May  2 02:24:19 2023, max compression
```

## Comparing `maya-rig-operation-graph-0.2.3.tar` & `maya-rig-operation-graph-0.3.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 10:36:39.000000 maya-rig-operation-graph-0.2.3/
--rw-rw-rw-   0        0        0    11558 2022-10-23 14:57:04.000000 maya-rig-operation-graph-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     3819 2023-04-30 10:36:40.000000 maya-rig-operation-graph-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2622 2023-04-30 10:36:36.000000 maya-rig-operation-graph-0.2.3/README.rst
--rw-rw-rw-   0        0        0      112 2023-04-30 10:36:40.000000 maya-rig-operation-graph-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1912 2023-04-30 10:36:08.000000 maya-rig-operation-graph-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 10:36:39.000000 maya-rig-operation-graph-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 10:36:39.000000 maya-rig-operation-graph-0.2.3/src/maya_rig_operation_graph.egg-info/
--rw-rw-rw-   0        0        0     3819 2023-04-30 10:36:40.000000 maya-rig-operation-graph-0.2.3/src/maya_rig_operation_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      872 2023-04-30 10:36:40.000000 maya-rig-operation-graph-0.2.3/src/maya_rig_operation_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 10:36:40.000000 maya-rig-operation-graph-0.2.3/src/maya_rig_operation_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-30 10:36:40.000000 maya-rig-operation-graph-0.2.3/src/maya_rig_operation_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-30 10:36:40.000000 maya-rig-operation-graph-0.2.3/src/maya_rig_operation_graph.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 10:36:39.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/
--rw-rw-rw-   0        0        0      297 2022-05-11 13:52:18.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/__init__.py
--rw-rw-rw-   0        0        0     1582 2023-04-30 10:03:08.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/_utils.py
--rw-rw-rw-   0        0        0     1423 2022-10-06 03:06:38.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/additional.py
--rw-rw-rw-   0        0        0     1204 2022-10-06 03:07:24.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/all.py
--rw-rw-rw-   0        0        0     1271 2022-10-06 03:11:24.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/blend.py
--rw-rw-rw-   0        0        0     1243 2022-10-06 03:26:24.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/clamp.py
--rw-rw-rw-   0        0        0      858 2022-08-04 14:52:14.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/distance.py
--rw-rw-rw-   0        0        0      800 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/drive.py
--rw-rw-rw-   0        0        0     2267 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/logic.py
--rw-rw-rw-   0        0        0     4858 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/math.py
--rw-rw-rw-   0        0        0     1180 2022-08-04 17:29:44.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/math.pyi
--rw-rw-rw-   0        0        0     5541 2023-04-30 10:34:56.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/math3d.py
--rw-rw-rw-   0        0        0     1425 2022-10-23 15:51:16.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/math3d.pyi
--rw-rw-rw-   0        0        0     4446 2022-08-04 16:50:04.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/matrix.py
--rw-rw-rw-   0        0        0     2034 2022-08-23 07:56:04.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/random.py
--rw-rw-rw-   0        0        0      591 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/reverse.py
--rw-rw-rw-   0        0        0      566 2022-08-22 02:24:00.000000 maya-rig-operation-graph-0.2.3/src/rig_operation_graph/time.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:24:19.000000 maya-rig-operation-graph-0.3.3/
+-rw-rw-rw-   0        0        0    11558 2022-10-23 14:57:04.000000 maya-rig-operation-graph-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     3819 2023-05-02 02:24:20.000000 maya-rig-operation-graph-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2622 2023-05-02 02:24:16.000000 maya-rig-operation-graph-0.3.3/README.rst
+-rw-rw-rw-   0        0        0      112 2023-05-02 02:24:20.000000 maya-rig-operation-graph-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1912 2023-05-02 02:24:02.000000 maya-rig-operation-graph-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 02:24:19.000000 maya-rig-operation-graph-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 02:24:19.000000 maya-rig-operation-graph-0.3.3/src/maya_rig_operation_graph.egg-info/
+-rw-rw-rw-   0        0        0     3819 2023-05-02 02:24:20.000000 maya-rig-operation-graph-0.3.3/src/maya_rig_operation_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2023-05-02 02:24:20.000000 maya-rig-operation-graph-0.3.3/src/maya_rig_operation_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 02:24:20.000000 maya-rig-operation-graph-0.3.3/src/maya_rig_operation_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-02 02:24:20.000000 maya-rig-operation-graph-0.3.3/src/maya_rig_operation_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-02 02:24:20.000000 maya-rig-operation-graph-0.3.3/src/maya_rig_operation_graph.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 02:24:19.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/
+-rw-rw-rw-   0        0        0      297 2022-05-11 13:52:18.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/__init__.py
+-rw-rw-rw-   0        0        0     2132 2023-05-01 23:57:12.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/_utils.py
+-rw-rw-rw-   0        0        0     1423 2022-10-06 03:06:38.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/additional.py
+-rw-rw-rw-   0        0        0     1250 2023-05-02 01:39:06.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/all.py
+-rw-rw-rw-   0        0        0     1271 2022-10-06 03:11:24.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/blend.py
+-rw-rw-rw-   0        0        0     1243 2022-10-06 03:26:24.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/clamp.py
+-rw-rw-rw-   0        0        0      858 2022-08-04 14:52:14.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/distance.py
+-rw-rw-rw-   0        0        0      800 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/drive.py
+-rw-rw-rw-   0        0        0     2267 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/logic.py
+-rw-rw-rw-   0        0        0     4858 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/math.py
+-rw-rw-rw-   0        0        0     1180 2022-08-04 17:29:44.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/math.pyi
+-rw-rw-rw-   0        0        0     5541 2023-04-30 10:34:56.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/math3d.py
+-rw-rw-rw-   0        0        0     1425 2022-10-23 15:51:16.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/math3d.pyi
+-rw-rw-rw-   0        0        0     4446 2022-08-04 16:50:04.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/matrix.py
+-rw-rw-rw-   0        0        0     3468 2023-05-02 01:39:06.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/quaternion.py
+-rw-rw-rw-   0        0        0     2034 2022-08-23 07:56:04.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/random.py
+-rw-rw-rw-   0        0        0      591 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/reverse.py
+-rw-rw-rw-   0        0        0      566 2022-08-22 02:24:00.000000 maya-rig-operation-graph-0.3.3/src/rig_operation_graph/time.py
```

### Comparing `maya-rig-operation-graph-0.2.3/LICENSE` & `maya-rig-operation-graph-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/PKG-INFO` & `maya-rig-operation-graph-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya-rig-operation-graph
-Version: 0.2.3
+Version: 0.3.3
 Summary: maya计算图的实现
 Home-page: https://github.com/cpcgskill/maya-rig-operation-graph
 Author: ('cpcgskill',)
 Author-email: cpcgskill@outlook.com
 License: Apache Software License (Apache 2.0)
 Project-URL: Bug Tracker, https://github.com/cpcgskill/maya-rig-operation-graph/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `maya-rig-operation-graph-0.2.3/README.rst` & `maya-rig-operation-graph-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/setup.py` & `maya-rig-operation-graph-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 lib_name = 'maya-rig-operation-graph'
 
 author = 'cpcgskill',
 author_email = 'cpcgskill@outlook.com'
 
-version = '0.2.3'
+version = '0.3.3'
 
 description = 'maya计算图的实现'
 with open("README.rst", "rb") as f:
     long_description = f.read().decode(encoding='utf-8')
 
 project_homepage = 'https://github.com/cpcgskill/maya-rig-operation-graph'
 project_urls = {
```

### Comparing `maya-rig-operation-graph-0.2.3/src/maya_rig_operation_graph.egg-info/PKG-INFO` & `maya-rig-operation-graph-0.3.3/src/maya_rig_operation_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya-rig-operation-graph
-Version: 0.2.3
+Version: 0.3.3
 Summary: maya计算图的实现
 Home-page: https://github.com/cpcgskill/maya-rig-operation-graph
 Author: ('cpcgskill',)
 Author-email: cpcgskill@outlook.com
 License: Apache Software License (Apache 2.0)
 Project-URL: Bug Tracker, https://github.com/cpcgskill/maya-rig-operation-graph/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `maya-rig-operation-graph-0.2.3/src/maya_rig_operation_graph.egg-info/SOURCES.txt` & `maya-rig-operation-graph-0.3.3/src/maya_rig_operation_graph.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,10 +17,11 @@
 src/rig_operation_graph/drive.py
 src/rig_operation_graph/logic.py
 src/rig_operation_graph/math.py
 src/rig_operation_graph/math.pyi
 src/rig_operation_graph/math3d.py
 src/rig_operation_graph/math3d.pyi
 src/rig_operation_graph/matrix.py
+src/rig_operation_graph/quaternion.py
 src/rig_operation_graph/random.py
 src/rig_operation_graph/reverse.py
 src/rig_operation_graph/time.py
```

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/_utils.py` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,8 +54,22 @@
     if is_attr(in_value):
         in_attr = cc.new_object(in_value)
         in_attr >> out_attr
         return
     out_attr.set_value(in_value)
 
 
-__all__ = ['is_attr', 'set_or_connect', 'set_or_connect_3d', 'set_or_connect_matrix']
+def set_or_connect_quaternion(in_value, out_attr):
+    if is_attr(in_value):
+        in_attr = cc.new_object(in_value)
+        in_attr >> out_attr
+        return
+    attr_plug = out_attr.api1_m_plug()
+    out_attr_list = [cc.new_object(attr_plug.child(i).name()) for i in range(attr_plug.numChildren())]
+
+    set_or_connect(in_value[0], out_attr_list[0])
+    set_or_connect(in_value[1], out_attr_list[1])
+    set_or_connect(in_value[2], out_attr_list[2])
+    set_or_connect(in_value[3], out_attr_list[3])
+
+
+__all__ = ['is_attr', 'set_or_connect', 'set_or_connect_3d', 'set_or_connect_matrix', 'set_or_connect_quaternion']
```

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/additional.py` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/additional.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/all.py` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/all.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,7 +33,9 @@
 from rig_operation_graph.logic import *
 from rig_operation_graph.math import *
 from rig_operation_graph.math3d import *
 from rig_operation_graph.time import *
 from rig_operation_graph.random import *
 
 from rig_operation_graph.additional import *
+
+from rig_operation_graph.quaternion import *
```

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/blend.py` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/blend.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/clamp.py` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/clamp.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/distance.py` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/distance.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/drive.py` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/drive.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/logic.py` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/logic.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/math.py` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/math.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/math.pyi` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/math.pyi`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/math3d.py` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/math3d.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/math3d.pyi` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/math3d.pyi`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/matrix.py` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/matrix.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/random.py` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/random.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/reverse.py` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/reverse.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.2.3/src/rig_operation_graph/time.py` & `maya-rig-operation-graph-0.3.3/src/rig_operation_graph/time.py`

 * *Files identical despite different names*

