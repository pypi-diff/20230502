# Comparing `tmp/robotControl-1.0.4.tar.gz` & `tmp/robotControl-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotControl-1.0.4.tar", last modified: Tue May  2 10:59:45 2023, max compression
+gzip compressed data, was "robotControl-1.0.6.tar", last modified: Tue May  2 11:04:16 2023, max compression
```

## Comparing `robotControl-1.0.4.tar` & `robotControl-1.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 10:59:45.385340 robotControl-1.0.4/
--rw-rw-rw-   0        0        0      110 2023-05-02 10:59:45.385340 robotControl-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 10:59:45.377067 robotControl-1.0.4/robotControl.egg-info/
--rw-rw-rw-   0        0        0      110 2023-05-02 10:59:45.000000 robotControl-1.0.4/robotControl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-05-02 10:59:45.000000 robotControl-1.0.4/robotControl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 10:59:45.000000 robotControl-1.0.4/robotControl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 10:59:45.000000 robotControl-1.0.4/robotControl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 10:59:45.385340 robotControl-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-05-02 10:59:40.000000 robotControl-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:04:16.328292 robotControl-1.0.6/
+-rw-rw-rw-   0        0        0      110 2023-05-02 11:04:16.328292 robotControl-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 11:04:16.328292 robotControl-1.0.6/robotControl.egg-info/
+-rw-rw-rw-   0        0        0      110 2023-05-02 11:04:16.000000 robotControl-1.0.6/robotControl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-05-02 11:04:16.000000 robotControl-1.0.6/robotControl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 11:04:16.000000 robotControl-1.0.6/robotControl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 11:04:16.000000 robotControl-1.0.6/robotControl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 11:04:16.328292 robotControl-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      569 2023-05-02 11:03:45.000000 robotControl-1.0.6/setup.py
```

### Comparing `robotControl-1.0.4/setup.py` & `robotControl-1.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, Extension
 import os
 
 # get the path of the directory containing the setup.py script
 base_dir = os.path.abspath(os.path.dirname(__file__))
 
-robotControl = Extension('robotControl', sources=[], build_temp=os.path.join(base_dir, 'build'),)
+robotControl = Extension('robotControl', sources=[], build_temp=base_dir,)
 
 setup(
     name='robotControl',
-    version='1.0.4',
+    version='1.0.6',
     description='My Python extension module',
     author='Carl',
     ext_modules=[robotControl],
     package_data={'': ['CommandLayerEthernet.dll','CommandLayerWindows.dll','CommunicationLayerEthernet.dll','CommunicationLayerWindows.dll' 'jaco2.pyd']},
 )
```

