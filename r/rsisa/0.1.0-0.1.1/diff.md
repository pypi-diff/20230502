# Comparing `tmp/rsisa-0.1.0.tar.gz` & `tmp/rsisa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsisa-0.1.0.tar", last modified: Mon May  1 22:57:00 2023, max compression
+gzip compressed data, was "rsisa-0.1.1.tar", last modified: Mon May  1 23:18:44 2023, max compression
```

## Comparing `rsisa-0.1.0.tar` & `rsisa-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:57:00.456731 rsisa-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      709 2023-05-01 22:57:00.456731 rsisa-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-18 20:53:45.000000 rsisa-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:57:00.456731 rsisa-0.1.0/rsisa/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-18 18:49:34.000000 rsisa-0.1.0/rsisa/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    23196 2023-04-28 01:01:33.000000 rsisa-0.1.0/rsisa/annotation_map_split.py
--rw-rw-r--   0 root         (0) root         (0)     5160 2023-04-28 20:05:12.000000 rsisa-0.1.0/rsisa/ellipse_instance_generation.py
--rw-rw-r--   0 root         (0) root         (0)     2567 2023-04-28 17:31:14.000000 rsisa-0.1.0/rsisa/evaluation.py
--rw-rw-r--   0 root         (0) root         (0)    29670 2023-05-01 19:35:36.000000 rsisa-0.1.0/rsisa/instance_registration.py
--rw-rw-r--   0 root         (0) root         (0)     6291 2023-05-01 19:34:49.000000 rsisa-0.1.0/rsisa/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:57:00.456731 rsisa-0.1.0/rsisa.egg-info/
--rw-r--r--   0 root         (0) root         (0)      709 2023-05-01 22:57:00.000000 rsisa-0.1.0/rsisa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-05-01 22:57:00.000000 rsisa-0.1.0/rsisa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 22:57:00.000000 rsisa-0.1.0/rsisa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-01 22:57:00.000000 rsisa-0.1.0/rsisa.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-01 22:57:00.000000 rsisa-0.1.0/rsisa.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 22:57:00.456731 rsisa-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1124 2023-05-01 22:56:49.000000 rsisa-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:57:00.456731 rsisa-0.1.0/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-18 23:46:40.000000 rsisa-0.1.0/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2469 2023-05-01 22:46:56.000000 rsisa-0.1.0/tests/test_annotation_map_split.py
--rw-rw-r--   0 root         (0) root         (0)      228 2023-05-01 22:47:02.000000 rsisa-0.1.0/tests/test_ellipse_instance_generation.py
--rw-rw-r--   0 root         (0) root         (0)      430 2023-04-29 00:21:00.000000 rsisa-0.1.0/tests/test_evaluation.py
--rw-rw-r--   0 root         (0) root         (0)      966 2023-05-01 22:47:13.000000 rsisa-0.1.0/tests/test_instance_registration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 23:18:44.641098 rsisa-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)      932 2023-05-01 23:18:44.641098 rsisa-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      174 2023-05-01 23:14:29.000000 rsisa-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 23:18:44.641098 rsisa-0.1.1/rsisa/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-18 18:49:34.000000 rsisa-0.1.1/rsisa/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    23196 2023-04-28 01:01:33.000000 rsisa-0.1.1/rsisa/annotation_map_split.py
+-rw-rw-r--   0 root         (0) root         (0)     5160 2023-04-28 20:05:12.000000 rsisa-0.1.1/rsisa/ellipse_instance_generation.py
+-rw-rw-r--   0 root         (0) root         (0)     2567 2023-04-28 17:31:14.000000 rsisa-0.1.1/rsisa/evaluation.py
+-rw-rw-r--   0 root         (0) root         (0)    29670 2023-05-01 19:35:36.000000 rsisa-0.1.1/rsisa/instance_registration.py
+-rw-rw-r--   0 root         (0) root         (0)     6291 2023-05-01 19:34:49.000000 rsisa-0.1.1/rsisa/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 23:18:44.641098 rsisa-0.1.1/rsisa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      932 2023-05-01 23:18:44.000000 rsisa-0.1.1/rsisa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-01 23:18:44.000000 rsisa-0.1.1/rsisa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 23:18:44.000000 rsisa-0.1.1/rsisa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-01 23:18:44.000000 rsisa-0.1.1/rsisa.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-01 23:18:44.000000 rsisa-0.1.1/rsisa.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 23:18:44.641098 rsisa-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1283 2023-05-01 23:17:49.000000 rsisa-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 23:18:44.641098 rsisa-0.1.1/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-18 23:46:40.000000 rsisa-0.1.1/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2469 2023-05-01 22:46:56.000000 rsisa-0.1.1/tests/test_annotation_map_split.py
+-rw-rw-r--   0 root         (0) root         (0)      228 2023-05-01 22:47:02.000000 rsisa-0.1.1/tests/test_ellipse_instance_generation.py
+-rw-rw-r--   0 root         (0) root         (0)      430 2023-04-29 00:21:00.000000 rsisa-0.1.1/tests/test_evaluation.py
+-rw-rw-r--   0 root         (0) root         (0)      966 2023-05-01 22:47:13.000000 rsisa-0.1.1/tests/test_instance_registration.py
```

### Comparing `rsisa-0.1.0/rsisa/annotation_map_split.py` & `rsisa-0.1.1/rsisa/annotation_map_split.py`

 * *Files identical despite different names*

### Comparing `rsisa-0.1.0/rsisa/ellipse_instance_generation.py` & `rsisa-0.1.1/rsisa/ellipse_instance_generation.py`

 * *Files identical despite different names*

### Comparing `rsisa-0.1.0/rsisa/evaluation.py` & `rsisa-0.1.1/rsisa/evaluation.py`

 * *Files identical despite different names*

### Comparing `rsisa-0.1.0/rsisa/instance_registration.py` & `rsisa-0.1.1/rsisa/instance_registration.py`

 * *Files identical despite different names*

### Comparing `rsisa-0.1.0/rsisa/workflow.py` & `rsisa-0.1.1/rsisa/workflow.py`

 * *Files identical despite different names*

### Comparing `rsisa-0.1.0/setup.py` & `rsisa-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
 setup(
     name='rsisa',
-    version='0.1.0',
+    version='0.1.1',
     description='Remote Sensing Instance Segmentation Algorithms',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     url='https://github.com/ZhiangChen/instance_segmentation_remote_sensing',
     author='Zhiang Chen',
     author_email='zxc251@case.edu',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
```

### Comparing `rsisa-0.1.0/tests/test_annotation_map_split.py` & `rsisa-0.1.1/tests/test_annotation_map_split.py`

 * *Files identical despite different names*

### Comparing `rsisa-0.1.0/tests/test_instance_registration.py` & `rsisa-0.1.1/tests/test_instance_registration.py`

 * *Files identical despite different names*

