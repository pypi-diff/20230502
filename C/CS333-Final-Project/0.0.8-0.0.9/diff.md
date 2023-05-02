# Comparing `tmp/CS333-Final-Project-0.0.8.tar.gz` & `tmp/CS333-Final-Project-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CS333-Final-Project-0.0.8.tar", last modified: Tue May  2 21:37:08 2023, max compression
+gzip compressed data, was "CS333-Final-Project-0.0.9.tar", last modified: Tue May  2 21:39:27 2023, max compression
```

## Comparing `CS333-Final-Project-0.0.8.tar` & `CS333-Final-Project-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:37:08.457431 CS333-Final-Project-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:37:08.457431 CS333-Final-Project-0.0.8/CS333_Final_Project.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-02 21:37:08.000000 CS333-Final-Project-0.0.8/CS333_Final_Project.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-02 21:37:08.000000 CS333-Final-Project-0.0.8/CS333_Final_Project.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:37:08.000000 CS333-Final-Project-0.0.8/CS333_Final_Project.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:37:08.000000 CS333-Final-Project-0.0.8/CS333_Final_Project.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-02 21:37:08.457431 CS333-Final-Project-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-05-02 21:36:57.000000 CS333-Final-Project-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:37:08.457431 CS333-Final-Project-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-02 21:36:57.000000 CS333-Final-Project-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:39:27.456165 CS333-Final-Project-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:39:27.456165 CS333-Final-Project-0.0.9/CS333_Final_Project.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-02 21:39:27.000000 CS333-Final-Project-0.0.9/CS333_Final_Project.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-02 21:39:27.000000 CS333-Final-Project-0.0.9/CS333_Final_Project.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:39:27.000000 CS333-Final-Project-0.0.9/CS333_Final_Project.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:39:27.000000 CS333-Final-Project-0.0.9/CS333_Final_Project.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-02 21:39:27.456165 CS333-Final-Project-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-05-02 21:39:16.000000 CS333-Final-Project-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:39:27.456165 CS333-Final-Project-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-02 21:39:16.000000 CS333-Final-Project-0.0.9/setup.py
```

### Comparing `CS333-Final-Project-0.0.8/README.md` & `CS333-Final-Project-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `CS333-Final-Project-0.0.8/setup.py` & `CS333-Final-Project-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'CS333 Final Project'
 LONG_DESCRIPTION = 'CS333 Testing and DevOps Final Project @ University of Nevada, Reno.'
 
 # Setting up
 setup(
     name="CS333-Final-Project",
     version=VERSION,
```

