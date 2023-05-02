# Comparing `tmp/pharus-0.8.5.tar.gz` & `tmp/pharus-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pharus-0.8.5.tar", last modified: Wed Apr 26 15:33:05 2023, max compression
+gzip compressed data, was "pharus-0.8.6.tar", last modified: Tue May  2 19:51:02 2023, max compression
```

## Comparing `pharus-0.8.5.tar` & `pharus-0.8.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2023-04-26 15:33:05.525184 pharus-0.8.5/
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     1079 2023-04-26 15:31:50.000000 pharus-0.8.5/LICENSE
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     1799 2023-04-26 15:33:05.525184 pharus-0.8.5/PKG-INFO
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     1422 2023-04-26 15:31:50.000000 pharus-0.8.5/README.rst
-drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2023-04-26 15:33:05.525184 pharus-0.8.5/pharus/
--rw-r--r--   0 anaconda  (1001) anaconda   (101)      368 2023-04-26 15:31:50.000000 pharus-0.8.5/pharus/__init__.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)    22314 2023-04-26 15:31:50.000000 pharus-0.8.5/pharus/component_interface.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)    11118 2023-04-26 15:31:50.000000 pharus-0.8.5/pharus/dynamic_api_gen.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)      276 2023-04-26 15:31:50.000000 pharus-0.8.5/pharus/error.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)    19519 2023-04-26 15:31:50.000000 pharus-0.8.5/pharus/interface.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)    41895 2023-04-26 15:31:50.000000 pharus-0.8.5/pharus/server.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)       46 2023-04-26 15:31:50.000000 pharus-0.8.5/pharus/version.py
-drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2023-04-26 15:33:05.525184 pharus-0.8.5/pharus.egg-info/
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     1799 2023-04-26 15:33:05.000000 pharus-0.8.5/pharus.egg-info/PKG-INFO
--rw-r--r--   0 anaconda  (1001) anaconda   (101)      355 2023-04-26 15:33:05.000000 pharus-0.8.5/pharus.egg-info/SOURCES.txt
--rw-r--r--   0 anaconda  (1001) anaconda   (101)        1 2023-04-26 15:33:05.000000 pharus-0.8.5/pharus.egg-info/dependency_links.txt
--rw-r--r--   0 anaconda  (1001) anaconda   (101)       45 2023-04-26 15:33:05.000000 pharus-0.8.5/pharus.egg-info/entry_points.txt
--rw-r--r--   0 anaconda  (1001) anaconda   (101)      146 2023-04-26 15:33:05.000000 pharus-0.8.5/pharus.egg-info/requires.txt
--rw-r--r--   0 anaconda  (1001) anaconda   (101)        7 2023-04-26 15:33:05.000000 pharus-0.8.5/pharus.egg-info/top_level.txt
--rw-r--r--   0 anaconda  (1001) anaconda   (101)       38 2023-04-26 15:33:05.525184 pharus-0.8.5/setup.cfg
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     1277 2023-04-26 15:31:50.000000 pharus-0.8.5/setup.py
+drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2023-05-02 19:51:02.345365 pharus-0.8.6/
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)     1079 2023-05-02 19:50:07.000000 pharus-0.8.6/LICENSE
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)     1799 2023-05-02 19:51:02.345365 pharus-0.8.6/PKG-INFO
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)     1422 2023-05-02 19:50:07.000000 pharus-0.8.6/README.rst
+drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2023-05-02 19:51:02.341365 pharus-0.8.6/pharus/
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)      368 2023-05-02 19:50:07.000000 pharus-0.8.6/pharus/__init__.py
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)    22314 2023-05-02 19:50:07.000000 pharus-0.8.6/pharus/component_interface.py
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)    11118 2023-05-02 19:50:07.000000 pharus-0.8.6/pharus/dynamic_api_gen.py
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)      276 2023-05-02 19:50:07.000000 pharus-0.8.6/pharus/error.py
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)    19519 2023-05-02 19:50:07.000000 pharus-0.8.6/pharus/interface.py
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)    41895 2023-05-02 19:50:07.000000 pharus-0.8.6/pharus/server.py
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)       46 2023-05-02 19:50:07.000000 pharus-0.8.6/pharus/version.py
+drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2023-05-02 19:51:02.345365 pharus-0.8.6/pharus.egg-info/
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)     1799 2023-05-02 19:51:02.000000 pharus-0.8.6/pharus.egg-info/PKG-INFO
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)      355 2023-05-02 19:51:02.000000 pharus-0.8.6/pharus.egg-info/SOURCES.txt
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)        1 2023-05-02 19:51:02.000000 pharus-0.8.6/pharus.egg-info/dependency_links.txt
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)       45 2023-05-02 19:51:02.000000 pharus-0.8.6/pharus.egg-info/entry_points.txt
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)      146 2023-05-02 19:51:02.000000 pharus-0.8.6/pharus.egg-info/requires.txt
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)        7 2023-05-02 19:51:02.000000 pharus-0.8.6/pharus.egg-info/top_level.txt
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)       38 2023-05-02 19:51:02.345365 pharus-0.8.6/setup.cfg
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)     1277 2023-05-02 19:50:07.000000 pharus-0.8.6/setup.py
```

### Comparing `pharus-0.8.5/LICENSE` & `pharus-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pharus-0.8.5/PKG-INFO` & `pharus-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharus
-Version: 0.8.5
+Version: 0.8.6
 Summary: A generic REST API server backend for DataJoint pipelines.
 Home-page: https://github.com/datajoint/pharus
 Author: DataJoint Neuro
 Author-email: support@vathes.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
```

### Comparing `pharus-0.8.5/README.rst` & `pharus-0.8.6/README.rst`

 * *Files identical despite different names*

### Comparing `pharus-0.8.5/pharus/component_interface.py` & `pharus-0.8.6/pharus/component_interface.py`

 * *Files identical despite different names*

### Comparing `pharus-0.8.5/pharus/dynamic_api_gen.py` & `pharus-0.8.6/pharus/dynamic_api_gen.py`

 * *Files identical despite different names*

### Comparing `pharus-0.8.5/pharus/interface.py` & `pharus-0.8.6/pharus/interface.py`

 * *Files identical despite different names*

### Comparing `pharus-0.8.5/pharus/server.py` & `pharus-0.8.6/pharus/server.py`

 * *Files identical despite different names*

### Comparing `pharus-0.8.5/pharus.egg-info/PKG-INFO` & `pharus-0.8.6/pharus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharus
-Version: 0.8.5
+Version: 0.8.6
 Summary: A generic REST API server backend for DataJoint pipelines.
 Home-page: https://github.com/datajoint/pharus
 Author: DataJoint Neuro
 Author-email: support@vathes.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
```

### Comparing `pharus-0.8.5/setup.py` & `pharus-0.8.6/setup.py`

 * *Files identical despite different names*

