# Comparing `tmp/up_pps-1.0.2.tar.gz` & `tmp/up_pps-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_pps-1.0.2.tar", last modified: Fri Apr 28 15:13:48 2023, max compression
+gzip compressed data, was "up_pps-1.0.3.tar", last modified: Tue May  2 06:55:04 2023, max compression
```

## Comparing `up_pps-1.0.2.tar` & `up_pps-1.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:48.529796 up_pps-1.0.2/
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)    11323 2023-04-28 15:13:18.000000 up_pps-1.0.2/LICENSE
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      227 2023-04-28 15:13:48.529796 up_pps-1.0.2/PKG-INFO
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)       91 2023-04-28 15:13:18.000000 up_pps-1.0.2/README.md
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)       38 2023-04-28 15:13:48.529796 up_pps-1.0.2/setup.cfg
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      647 2023-04-28 15:13:18.000000 up_pps-1.0.2/setup.py
-drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:48.529796 up_pps-1.0.2/up_pps/
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      993 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/__init__.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)    15226 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/converter.py
-drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:48.529796 up_pps-1.0.2/up_pps/core/
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/core/__init__.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)    21868 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/core/cp_solver.py
-drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:48.529796 up_pps-1.0.2/up_pps/core/output/
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/core/output/__init__.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      222 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/core/output/cp_solution_output.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      224 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/core/output/solution_output.py
-drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:48.529796 up_pps-1.0.2/up_pps/dataenv/
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/__init__.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      752 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/activity.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      786 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/activity_activity_relation.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      554 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/element.py
-drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:48.529796 up_pps-1.0.2/up_pps/dataenv/internal/
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/internal/__init__.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      836 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/internal/activity_fact.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)     1882 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/internal/graph.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      390 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/parameter.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      235 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/res_setup.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      661 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/resource.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      549 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/resource_availability.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      307 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/resource_set.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      929 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/resource_set_activity_seize_release.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      535 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/resource_set_resource.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)     5261 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/dataenv/scheduling_problem.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)     3523 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/engine.py
-drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:48.529796 up_pps-1.0.2/up_pps/manager/
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/manager/__init__.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)     1524 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/manager/activity_fact_manager.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)     6277 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/manager/instance_manager.py
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)     2063 2023-04-28 15:13:18.000000 up_pps-1.0.2/up_pps/manager/task_manager.py
-drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:48.529796 up_pps-1.0.2/up_pps.egg-info/
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      227 2023-04-28 15:13:48.000000 up_pps-1.0.2/up_pps.egg-info/PKG-INFO
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)     1043 2023-04-28 15:13:48.000000 up_pps-1.0.2/up_pps.egg-info/SOURCES.txt
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        1 2023-04-28 15:13:48.000000 up_pps-1.0.2/up_pps.egg-info/dependency_links.txt
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)       44 2023-04-28 15:13:48.000000 up_pps-1.0.2/up_pps.egg-info/requires.txt
--rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        7 2023-04-28 15:13:48.000000 up_pps-1.0.2/up_pps.egg-info/top_level.txt
+drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-05-02 06:55:04.355576 up_pps-1.0.3/
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)    11323 2023-04-28 15:13:18.000000 up_pps-1.0.3/LICENSE
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      227 2023-05-02 06:55:04.355576 up_pps-1.0.3/PKG-INFO
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)       91 2023-04-28 15:13:18.000000 up_pps-1.0.3/README.md
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)       38 2023-05-02 06:55:04.355576 up_pps-1.0.3/setup.cfg
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      622 2023-05-02 06:54:55.000000 up_pps-1.0.3/setup.py
+drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-05-02 06:55:04.351576 up_pps-1.0.3/up_pps/
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      993 2023-05-02 06:54:55.000000 up_pps-1.0.3/up_pps/__init__.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)    15226 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/converter.py
+drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-05-02 06:55:04.351576 up_pps-1.0.3/up_pps/core/
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/core/__init__.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)    21868 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/core/cp_solver.py
+drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-05-02 06:55:04.351576 up_pps-1.0.3/up_pps/core/output/
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/core/output/__init__.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      222 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/core/output/cp_solution_output.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      224 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/core/output/solution_output.py
+drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-05-02 06:55:04.355576 up_pps-1.0.3/up_pps/dataenv/
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/__init__.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      752 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/activity.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      786 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/activity_activity_relation.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      554 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/element.py
+drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-05-02 06:55:04.355576 up_pps-1.0.3/up_pps/dataenv/internal/
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/internal/__init__.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      836 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/internal/activity_fact.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)     1882 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/internal/graph.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      390 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/parameter.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      235 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/res_setup.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      661 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/resource.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      549 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/resource_availability.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      307 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/resource_set.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      929 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/resource_set_activity_seize_release.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      535 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/resource_set_resource.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)     5261 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/dataenv/scheduling_problem.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)     3523 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/engine.py
+drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-05-02 06:55:04.355576 up_pps-1.0.3/up_pps/manager/
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/manager/__init__.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)     1524 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/manager/activity_fact_manager.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)     6277 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/manager/instance_manager.py
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)     2063 2023-04-28 15:13:18.000000 up_pps-1.0.3/up_pps/manager/task_manager.py
+drwxrwxr-x   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        0 2023-05-02 06:55:04.351576 up_pps-1.0.3/up_pps.egg-info/
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)      227 2023-05-02 06:55:04.000000 up_pps-1.0.3/up_pps.egg-info/PKG-INFO
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)     1043 2023-05-02 06:55:04.000000 up_pps-1.0.3/up_pps.egg-info/SOURCES.txt
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        1 2023-05-02 06:55:04.000000 up_pps-1.0.3/up_pps.egg-info/dependency_links.txt
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)       44 2023-05-02 06:55:04.000000 up_pps-1.0.3/up_pps.egg-info/requires.txt
+-rw-rw-r--   0 sabrinabassetto  (1001) sabrinabassetto  (1001)        7 2023-05-02 06:55:04.000000 up_pps-1.0.3/up_pps.egg-info/top_level.txt
```

### Comparing `up_pps-1.0.2/LICENSE` & `up_pps-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/setup.py` & `up_pps-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from setuptools import setup  # type: ignore
-import up_pps
 
 long_description = '''
 # UP_PPS
 
 UP_PPS is an engine that relies on CP-Sat of ORTOOLS
 to solve scheduling problems
 '''
 
 setup(name='up_pps',
-      version=up_pps.__version__,
+      version='1.0.3',
       description='up_pps',
       author='ACTOR',
       author_email='ahead@ahead-research.com',
       url='https://github.com/aiplan4eu/up-pps',
       packages=['up_pps', 'up_pps.dataenv', 'up_pps.dataenv.internal', 'up_pps.core','up_pps.core.output', 'up_pps.manager'],
       install_requires=['pip==22.3.1', 'numpy==1.24.1', 'ortools==9.5.2237'],
       python_requires='>=3.7',
```

### Comparing `up_pps-1.0.2/up_pps/__init__.py` & `up_pps-1.0.3/up_pps/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from up_pps.dataenv.resource_set import ResourceSet
 from up_pps.dataenv.resource_set_activity_seize_release import ResourceSetActivitySeizeRelease
 from up_pps.dataenv.resource_set_resource import ResourceSetResource
 from up_pps.dataenv.res_setup import SetupTime
 from up_pps.dataenv.scheduling_problem import Scheduling_problem
 
 
-VERSION = (1, 0, 2)
+VERSION = (1, 0, 3)
 __version__ = ".".join(str(x) for x in VERSION)
 
 __all__ = [
     "Resource",
     "Activity",
     "ActivityActivityRelation",
     "Element",
```

### Comparing `up_pps-1.0.2/up_pps/converter.py` & `up_pps-1.0.3/up_pps/converter.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/core/cp_solver.py` & `up_pps-1.0.3/up_pps/core/cp_solver.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/dataenv/activity.py` & `up_pps-1.0.3/up_pps/dataenv/activity.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/dataenv/activity_activity_relation.py` & `up_pps-1.0.3/up_pps/dataenv/activity_activity_relation.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/dataenv/element.py` & `up_pps-1.0.3/up_pps/dataenv/element.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/dataenv/internal/activity_fact.py` & `up_pps-1.0.3/up_pps/dataenv/internal/activity_fact.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/dataenv/internal/graph.py` & `up_pps-1.0.3/up_pps/dataenv/internal/graph.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/dataenv/resource.py` & `up_pps-1.0.3/up_pps/dataenv/resource.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/dataenv/resource_availability.py` & `up_pps-1.0.3/up_pps/dataenv/resource_availability.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/dataenv/resource_set_activity_seize_release.py` & `up_pps-1.0.3/up_pps/dataenv/resource_set_activity_seize_release.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/dataenv/resource_set_resource.py` & `up_pps-1.0.3/up_pps/dataenv/resource_set_resource.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/dataenv/scheduling_problem.py` & `up_pps-1.0.3/up_pps/dataenv/scheduling_problem.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/engine.py` & `up_pps-1.0.3/up_pps/engine.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/manager/activity_fact_manager.py` & `up_pps-1.0.3/up_pps/manager/activity_fact_manager.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/manager/instance_manager.py` & `up_pps-1.0.3/up_pps/manager/instance_manager.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps/manager/task_manager.py` & `up_pps-1.0.3/up_pps/manager/task_manager.py`

 * *Files identical despite different names*

### Comparing `up_pps-1.0.2/up_pps.egg-info/SOURCES.txt` & `up_pps-1.0.3/up_pps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

