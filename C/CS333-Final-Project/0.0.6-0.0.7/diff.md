# Comparing `tmp/CS333-Final-Project-0.0.6.tar.gz` & `tmp/CS333-Final-Project-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CS333-Final-Project-0.0.6.tar", last modified: Mon May  1 05:11:25 2023, max compression
+gzip compressed data, was "CS333-Final-Project-0.0.7.tar", last modified: Tue May  2 17:48:28 2023, max compression
```

## Comparing `CS333-Final-Project-0.0.6.tar` & `CS333-Final-Project-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:11:25.482141 CS333-Final-Project-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 05:11:25.482141 CS333-Final-Project-0.0.6/CS333_Final_Project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 05:11:25.000000 CS333-Final-Project-0.0.6/CS333_Final_Project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-01 05:11:25.000000 CS333-Final-Project-0.0.6/CS333_Final_Project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 05:11:25.000000 CS333-Final-Project-0.0.6/CS333_Final_Project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 05:11:25.000000 CS333-Final-Project-0.0.6/CS333_Final_Project.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 05:11:25.482141 CS333-Final-Project-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-05-01 05:11:10.000000 CS333-Final-Project-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 05:11:25.482141 CS333-Final-Project-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-01 05:11:10.000000 CS333-Final-Project-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:48:28.207527 CS333-Final-Project-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:48:28.207527 CS333-Final-Project-0.0.7/CS333_Final_Project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-02 17:48:28.000000 CS333-Final-Project-0.0.7/CS333_Final_Project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-02 17:48:28.000000 CS333-Final-Project-0.0.7/CS333_Final_Project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:48:28.000000 CS333-Final-Project-0.0.7/CS333_Final_Project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:48:28.000000 CS333-Final-Project-0.0.7/CS333_Final_Project.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-02 17:48:28.207527 CS333-Final-Project-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-05-02 17:48:17.000000 CS333-Final-Project-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:48:28.207527 CS333-Final-Project-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-02 17:48:17.000000 CS333-Final-Project-0.0.7/setup.py
```

### Comparing `CS333-Final-Project-0.0.6/README.md` & `CS333-Final-Project-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `CS333-Final-Project-0.0.6/setup.py` & `CS333-Final-Project-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'CS333 Final Project'
 LONG_DESCRIPTION = 'CS333 Testing and DevOps Final Project @ University of Nevada, Reno.'
 
 # Setting up
 setup(
     name="CS333-Final-Project",
     version=VERSION,
```

