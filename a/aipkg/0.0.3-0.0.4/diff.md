# Comparing `tmp/aipkg-0.0.3.tar.gz` & `tmp/aipkg-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkg-0.0.3.tar", last modified: Tue May  2 19:30:32 2023, max compression
+gzip compressed data, was "aipkg-0.0.4.tar", last modified: Tue May  2 19:36:46 2023, max compression
```

## Comparing `aipkg-0.0.3.tar` & `aipkg-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 19:30:32.285327 aipkg-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-02 19:30:32.246316 aipkg-0.0.3/AI/
--rw-rw-rw-   0        0        0       26 2023-05-01 14:49:27.000000 aipkg-0.0.3/AI/__init__.py
--rw-rw-rw-   0        0        0    27119 2023-05-02 19:29:16.000000 aipkg-0.0.3/AI/ai.py
--rw-rw-rw-   0        0        0      452 2023-05-02 19:30:32.282798 aipkg-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 19:30:32.277444 aipkg-0.0.3/aipkg.egg-info/
--rw-rw-rw-   0        0        0      452 2023-05-02 19:30:31.000000 aipkg-0.0.3/aipkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-05-02 19:30:31.000000 aipkg-0.0.3/aipkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 19:30:31.000000 aipkg-0.0.3/aipkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-05-02 19:30:31.000000 aipkg-0.0.3/aipkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 19:30:32.286313 aipkg-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      676 2023-05-02 19:30:09.000000 aipkg-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:36:46.974505 aipkg-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:36:46.955519 aipkg-0.0.4/AI/
+-rw-rw-rw-   0        0        0       26 2023-05-01 14:49:27.000000 aipkg-0.0.4/AI/__init__.py
+-rw-rw-rw-   0        0        0    27119 2023-05-02 19:29:16.000000 aipkg-0.0.4/AI/ai.py
+-rw-rw-rw-   0        0        0      452 2023-05-02 19:36:46.973506 aipkg-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 19:36:46.971508 aipkg-0.0.4/aipkg.egg-info/
+-rw-rw-rw-   0        0        0      452 2023-05-02 19:36:46.000000 aipkg-0.0.4/aipkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-05-02 19:36:46.000000 aipkg-0.0.4/aipkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 19:36:46.000000 aipkg-0.0.4/aipkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2023-05-02 19:36:46.000000 aipkg-0.0.4/aipkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 19:36:46.974505 aipkg-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      676 2023-05-02 19:36:45.000000 aipkg-0.0.4/setup.py
```

### Comparing `aipkg-0.0.3/AI/ai.py` & `aipkg-0.0.4/AI/ai.py`

 * *Files identical despite different names*

### Comparing `aipkg-0.0.3/setup.py` & `aipkg-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Streaming video data via networks'
 
 
 # Setting up
 setup(
     name="aipkg",
     version=VERSION,
-    author="YB03",
+    author="Deez",
     author_email="<hello@yahoo.com>",
     description=DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'ai', 'pkg'],
     classifiers=[
         "Development Status :: 1 - Planning",
```

