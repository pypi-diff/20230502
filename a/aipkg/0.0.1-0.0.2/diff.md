# Comparing `tmp/aipkg-0.0.1.tar.gz` & `tmp/aipkg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkg-0.0.1.tar", last modified: Mon May  1 14:38:26 2023, max compression
+gzip compressed data, was "aipkg-0.0.2.tar", last modified: Tue May  2 10:23:26 2023, max compression
```

## Comparing `aipkg-0.0.1.tar` & `aipkg-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 14:38:26.223308 aipkg-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-01 14:38:26.203310 aipkg-0.0.1/AI/
--rw-rw-rw-   0        0        0       20 2023-05-01 14:33:14.000000 aipkg-0.0.1/AI/__init__.py
--rw-rw-rw-   0        0        0       32 2023-05-01 14:32:57.000000 aipkg-0.0.1/AI/ai.py
--rw-rw-rw-   0        0        0      452 2023-05-01 14:38:26.223308 aipkg-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-01 14:38:26.221309 aipkg-0.0.1/aipkg.egg-info/
--rw-rw-rw-   0        0        0      452 2023-05-01 14:38:25.000000 aipkg-0.0.1/aipkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-05-01 14:38:26.000000 aipkg-0.0.1/aipkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 14:38:25.000000 aipkg-0.0.1/aipkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-05-01 14:38:25.000000 aipkg-0.0.1/aipkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 14:38:26.224309 aipkg-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      704 2023-05-01 14:38:22.000000 aipkg-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:23:26.258824 aipkg-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-02 10:23:26.243827 aipkg-0.0.2/AI/
+-rw-rw-rw-   0        0        0       26 2023-05-01 14:49:27.000000 aipkg-0.0.2/AI/__init__.py
+-rw-rw-rw-   0        0        0    11458 2023-05-02 10:15:09.000000 aipkg-0.0.2/AI/ai.py
+-rw-rw-rw-   0        0        0      452 2023-05-02 10:23:26.258824 aipkg-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 10:23:26.256825 aipkg-0.0.2/aipkg.egg-info/
+-rw-rw-rw-   0        0        0      452 2023-05-02 10:23:25.000000 aipkg-0.0.2/aipkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-05-02 10:23:26.000000 aipkg-0.0.2/aipkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 10:23:25.000000 aipkg-0.0.2/aipkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2023-05-02 10:23:25.000000 aipkg-0.0.2/aipkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 10:23:26.259830 aipkg-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      676 2023-05-02 10:22:46.000000 aipkg-0.0.2/setup.py
```

### Comparing `aipkg-0.0.1/setup.py` & `aipkg-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from setuptools import setup, find_packages
-import codecs
-import os
 
-
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Streaming video data via networks'
 
 
 # Setting up
 setup(
     name="aipkg",
     version=VERSION,
```

