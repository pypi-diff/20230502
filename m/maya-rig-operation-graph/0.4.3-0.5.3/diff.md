# Comparing `tmp/maya-rig-operation-graph-0.4.3.tar.gz` & `tmp/maya-rig-operation-graph-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\maya-rig-operation-graph-0.4.3.tar", last modified: Tue May  2 03:39:07 2023, max compression
+gzip compressed data, was "dist\maya-rig-operation-graph-0.5.3.tar", last modified: Tue May  2 12:00:01 2023, max compression
```

## Comparing `maya-rig-operation-graph-0.4.3.tar` & `maya-rig-operation-graph-0.5.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 03:37:20.000000 maya-rig-operation-graph-0.4.3/
--rw-rw-rw-   0        0        0    11558 2022-10-23 14:57:04.000000 maya-rig-operation-graph-0.4.3/LICENSE
--rw-rw-rw-   0        0        0     3819 2023-05-02 03:39:08.000000 maya-rig-operation-graph-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     2622 2023-05-02 03:39:06.000000 maya-rig-operation-graph-0.4.3/README.rst
--rw-rw-rw-   0        0        0      112 2023-05-02 03:39:08.000000 maya-rig-operation-graph-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1912 2023-05-02 03:37:16.000000 maya-rig-operation-graph-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 03:37:20.000000 maya-rig-operation-graph-0.4.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 03:39:06.000000 maya-rig-operation-graph-0.4.3/src/maya_rig_operation_graph.egg-info/
--rw-rw-rw-   0        0        0     3819 2023-05-02 03:39:08.000000 maya-rig-operation-graph-0.4.3/src/maya_rig_operation_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      910 2023-05-02 03:39:08.000000 maya-rig-operation-graph-0.4.3/src/maya_rig_operation_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 03:39:08.000000 maya-rig-operation-graph-0.4.3/src/maya_rig_operation_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-02 03:39:08.000000 maya-rig-operation-graph-0.4.3/src/maya_rig_operation_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-02 03:39:08.000000 maya-rig-operation-graph-0.4.3/src/maya_rig_operation_graph.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 03:39:06.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/
--rw-rw-rw-   0        0        0      297 2022-05-11 13:52:18.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/__init__.py
--rw-rw-rw-   0        0        0     2987 2023-05-02 03:34:50.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/_utils.py
--rw-rw-rw-   0        0        0     1423 2022-10-06 03:06:38.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/additional.py
--rw-rw-rw-   0        0        0     1250 2023-05-02 01:39:06.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/all.py
--rw-rw-rw-   0        0        0     1271 2022-10-06 03:11:24.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/blend.py
--rw-rw-rw-   0        0        0     1243 2022-10-06 03:26:24.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/clamp.py
--rw-rw-rw-   0        0        0      858 2022-08-04 14:52:14.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/distance.py
--rw-rw-rw-   0        0        0      800 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/drive.py
--rw-rw-rw-   0        0        0     2267 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/logic.py
--rw-rw-rw-   0        0        0     4858 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/math.py
--rw-rw-rw-   0        0        0     1180 2022-08-04 17:29:44.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/math.pyi
--rw-rw-rw-   0        0        0     5541 2023-04-30 10:34:56.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/math3d.py
--rw-rw-rw-   0        0        0     1425 2022-10-23 15:51:16.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/math3d.pyi
--rw-rw-rw-   0        0        0     4714 2023-05-02 03:35:42.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/matrix.py
--rw-rw-rw-   0        0        0     3468 2023-05-02 01:39:06.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/quaternion.py
--rw-rw-rw-   0        0        0     2034 2022-08-23 07:56:04.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/random.py
--rw-rw-rw-   0        0        0      591 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/reverse.py
--rw-rw-rw-   0        0        0      566 2022-08-22 02:24:00.000000 maya-rig-operation-graph-0.4.3/src/rig_operation_graph/time.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:59:34.000000 maya-rig-operation-graph-0.5.3/
+-rw-rw-rw-   0        0        0    11558 2022-10-23 14:57:04.000000 maya-rig-operation-graph-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0     3819 2023-05-02 12:00:02.000000 maya-rig-operation-graph-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2622 2023-05-02 12:00:00.000000 maya-rig-operation-graph-0.5.3/README.rst
+-rw-rw-rw-   0        0        0      112 2023-05-02 12:00:02.000000 maya-rig-operation-graph-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1912 2023-05-02 11:59:06.000000 maya-rig-operation-graph-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:59:34.000000 maya-rig-operation-graph-0.5.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 12:00:01.000000 maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/
+-rw-rw-rw-   0        0        0     3819 2023-05-02 12:00:02.000000 maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2023-05-02 12:00:02.000000 maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 12:00:02.000000 maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-02 12:00:02.000000 maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-02 12:00:02.000000 maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 12:00:01.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/
+-rw-rw-rw-   0        0        0      297 2022-05-11 13:52:18.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/__init__.py
+-rw-rw-rw-   0        0        0     2987 2023-05-02 03:34:50.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/_utils.py
+-rw-rw-rw-   0        0        0     1423 2022-10-06 03:06:38.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/additional.py
+-rw-rw-rw-   0        0        0     1250 2023-05-02 01:39:06.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/all.py
+-rw-rw-rw-   0        0        0     1271 2022-10-06 03:11:24.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/blend.py
+-rw-rw-rw-   0        0        0     1243 2022-10-06 03:26:24.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/clamp.py
+-rw-rw-rw-   0        0        0      858 2022-08-04 14:52:14.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/distance.py
+-rw-rw-rw-   0        0        0      800 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/drive.py
+-rw-rw-rw-   0        0        0     2267 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/logic.py
+-rw-rw-rw-   0        0        0     4858 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math.py
+-rw-rw-rw-   0        0        0     1180 2022-08-04 17:29:44.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math.pyi
+-rw-rw-rw-   0        0        0     5541 2023-04-30 10:34:56.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math3d.py
+-rw-rw-rw-   0        0        0     1737 2023-05-02 11:47:16.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math3d.pyi
+-rw-rw-rw-   0        0        0     4714 2023-05-02 03:35:42.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/matrix.py
+-rw-rw-rw-   0        0        0     3468 2023-05-02 01:39:06.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/quaternion.py
+-rw-rw-rw-   0        0        0     2034 2022-08-23 07:56:04.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/random.py
+-rw-rw-rw-   0        0        0      591 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/reverse.py
+-rw-rw-rw-   0        0        0      566 2022-08-22 02:24:00.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/time.py
```

### Comparing `maya-rig-operation-graph-0.4.3/LICENSE` & `maya-rig-operation-graph-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/PKG-INFO` & `maya-rig-operation-graph-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya-rig-operation-graph
-Version: 0.4.3
+Version: 0.5.3
 Summary: maya计算图的实现
 Home-page: https://github.com/cpcgskill/maya-rig-operation-graph
 Author: ('cpcgskill',)
 Author-email: cpcgskill@outlook.com
 License: Apache Software License (Apache 2.0)
 Project-URL: Bug Tracker, https://github.com/cpcgskill/maya-rig-operation-graph/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `maya-rig-operation-graph-0.4.3/README.rst` & `maya-rig-operation-graph-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/setup.py` & `maya-rig-operation-graph-0.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 lib_name = 'maya-rig-operation-graph'
 
 author = 'cpcgskill',
 author_email = 'cpcgskill@outlook.com'
 
-version = '0.4.3'
+version = '0.5.3'
 
 description = 'maya计算图的实现'
 with open("README.rst", "rb") as f:
     long_description = f.read().decode(encoding='utf-8')
 
 project_homepage = 'https://github.com/cpcgskill/maya-rig-operation-graph'
 project_urls = {
```

### Comparing `maya-rig-operation-graph-0.4.3/src/maya_rig_operation_graph.egg-info/PKG-INFO` & `maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya-rig-operation-graph
-Version: 0.4.3
+Version: 0.5.3
 Summary: maya计算图的实现
 Home-page: https://github.com/cpcgskill/maya-rig-operation-graph
 Author: ('cpcgskill',)
 Author-email: cpcgskill@outlook.com
 License: Apache Software License (Apache 2.0)
 Project-URL: Bug Tracker, https://github.com/cpcgskill/maya-rig-operation-graph/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `maya-rig-operation-graph-0.4.3/src/maya_rig_operation_graph.egg-info/SOURCES.txt` & `maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/_utils.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/_utils.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/additional.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/additional.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/all.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/all.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/blend.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/blend.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/clamp.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/clamp.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/distance.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/distance.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/drive.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/drive.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/logic.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/logic.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/math.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/math.pyi` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math.pyi`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/math3d.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math3d.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/math3d.pyi` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math3d.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -5,19 +5,14 @@
 from typing import Tuple, Union, Any
 
 Number = Union[float, int]
 Vector3d = Tuple[Union[float, int], Union[float, int], Union[float, int]]
 InValue = Union[Vector3d, Attr, Any]
 OutAttr = Attr
 
-__all__ = [
-    'add3d', 'sub3d', 'mul3d', 'div3d', 'pow3d', 'mean3d', 'sum3d',
-    'vector_add', 'vector_sub', 'vector_mul', 'vector_div', 'vector_pow', 'vector_mean', 'vector_sum'
-]
-
 
 def add3d(ctx: Ctx, a: InValue, b: InValue) -> OutAttr: pass
 
 
 def sub3d(ctx: Ctx, a: InValue, b: InValue) -> OutAttr: pass
 
 
@@ -51,7 +46,23 @@
 def vector_pow(ctx: Ctx, a: InValue, b: InValue) -> OutAttr: pass
 
 
 def vector_mean(ctx: Ctx, *values: InValue) -> OutAttr: pass
 
 
 def vector_sum(ctx: Ctx, *values: InValue) -> OutAttr: pass
+
+
+def vector_dot_product(ctx, left: InValue, right: InValue) -> OutAttr: pass
+
+
+def vector_cross_product(ctx, left: InValue, right: InValue) -> OutAttr: pass
+
+
+def vector_normalization(ctx, in_attr: InValue) -> OutAttr: pass
+
+
+__all__ = [
+    'add3d', 'sub3d', 'mul3d', 'div3d', 'pow3d', 'mean3d', 'sum3d',
+    'vector_add', 'vector_sub', 'vector_mul', 'vector_div', 'vector_pow', 'vector_mean', 'vector_sum',
+    'vector_dot_product', 'vector_cross_product', 'vector_normalization',
+]
```

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/matrix.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/matrix.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/quaternion.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/quaternion.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/random.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/random.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/reverse.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/reverse.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.4.3/src/rig_operation_graph/time.py` & `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/time.py`

 * *Files identical despite different names*

