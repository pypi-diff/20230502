# Comparing `tmp/aipkg-0.0.2.tar.gz` & `tmp/aipkg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkg-0.0.2.tar", last modified: Tue May  2 10:23:26 2023, max compression
+gzip compressed data, was "aipkg-0.0.3.tar", last modified: Tue May  2 19:30:32 2023, max compression
```

## Comparing `aipkg-0.0.2.tar` & `aipkg-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 10:23:26.258824 aipkg-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-02 10:23:26.243827 aipkg-0.0.2/AI/
--rw-rw-rw-   0        0        0       26 2023-05-01 14:49:27.000000 aipkg-0.0.2/AI/__init__.py
--rw-rw-rw-   0        0        0    11458 2023-05-02 10:15:09.000000 aipkg-0.0.2/AI/ai.py
--rw-rw-rw-   0        0        0      452 2023-05-02 10:23:26.258824 aipkg-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 10:23:26.256825 aipkg-0.0.2/aipkg.egg-info/
--rw-rw-rw-   0        0        0      452 2023-05-02 10:23:25.000000 aipkg-0.0.2/aipkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-05-02 10:23:26.000000 aipkg-0.0.2/aipkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 10:23:25.000000 aipkg-0.0.2/aipkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-05-02 10:23:25.000000 aipkg-0.0.2/aipkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 10:23:26.259830 aipkg-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      676 2023-05-02 10:22:46.000000 aipkg-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:30:32.285327 aipkg-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:30:32.246316 aipkg-0.0.3/AI/
+-rw-rw-rw-   0        0        0       26 2023-05-01 14:49:27.000000 aipkg-0.0.3/AI/__init__.py
+-rw-rw-rw-   0        0        0    27119 2023-05-02 19:29:16.000000 aipkg-0.0.3/AI/ai.py
+-rw-rw-rw-   0        0        0      452 2023-05-02 19:30:32.282798 aipkg-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 19:30:32.277444 aipkg-0.0.3/aipkg.egg-info/
+-rw-rw-rw-   0        0        0      452 2023-05-02 19:30:31.000000 aipkg-0.0.3/aipkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-05-02 19:30:31.000000 aipkg-0.0.3/aipkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 19:30:31.000000 aipkg-0.0.3/aipkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2023-05-02 19:30:31.000000 aipkg-0.0.3/aipkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 19:30:32.286313 aipkg-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      676 2023-05-02 19:30:09.000000 aipkg-0.0.3/setup.py
```

### Comparing `aipkg-0.0.2/setup.py` & `aipkg-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Streaming video data via networks'
 
 
 # Setting up
 setup(
     name="aipkg",
     version=VERSION,
```

