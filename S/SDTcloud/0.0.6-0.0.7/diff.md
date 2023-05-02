# Comparing `tmp/SDTcloud-0.0.6.tar.gz` & `tmp/SDTcloud-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SDTcloud-0.0.6.tar", last modified: Fri Apr 28 07:44:53 2023, max compression
+gzip compressed data, was "SDTcloud-0.0.7.tar", last modified: Tue May  2 05:17:52 2023, max compression
```

## Comparing `SDTcloud-0.0.6.tar` & `SDTcloud-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:44:53.886171 SDTcloud-0.0.6/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-04-28 07:44:53.886049 SDTcloud-0.0.6/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)       12 2023-04-27 00:33:43.000000 SDTcloud-0.0.6/README.md
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:44:53.885443 SDTcloud-0.0.6/SDTcloud/
--rw-r--r--   0 june       (501) staff       (20)       75 2023-04-27 00:34:53.000000 SDTcloud-0.0.6/SDTcloud/__init__.py
--rw-r--r--   0 june       (501) staff       (20)     5090 2023-04-28 07:44:21.000000 SDTcloud-0.0.6/SDTcloud/sdtcloud.py
-drwxr-xr-x   0 june       (501) staff       (20)        0 2023-04-28 07:44:53.885895 SDTcloud-0.0.6/SDTcloud.egg-info/
--rw-r--r--   0 june       (501) staff       (20)      398 2023-04-28 07:44:53.000000 SDTcloud-0.0.6/SDTcloud.egg-info/PKG-INFO
--rw-r--r--   0 june       (501) staff       (20)      188 2023-04-28 07:44:53.000000 SDTcloud-0.0.6/SDTcloud.egg-info/SOURCES.txt
--rw-r--r--   0 june       (501) staff       (20)        1 2023-04-28 07:44:53.000000 SDTcloud-0.0.6/SDTcloud.egg-info/dependency_links.txt
--rw-r--r--   0 june       (501) staff       (20)        9 2023-04-28 07:44:53.000000 SDTcloud-0.0.6/SDTcloud.egg-info/top_level.txt
--rw-r--r--   0 june       (501) staff       (20)       38 2023-04-28 07:44:53.886208 SDTcloud-0.0.6/setup.cfg
--rw-r--r--   0 june       (501) staff       (20)      656 2023-04-28 07:44:31.000000 SDTcloud-0.0.6/setup.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-02 05:17:52.127193 SDTcloud-0.0.7/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-02 05:17:52.127062 SDTcloud-0.0.7/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)       12 2023-04-27 00:33:43.000000 SDTcloud-0.0.7/README.md
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-02 05:17:52.126029 SDTcloud-0.0.7/SDTcloud/
+-rw-r--r--   0 june       (501) staff       (20)       75 2023-04-27 00:34:53.000000 SDTcloud-0.0.7/SDTcloud/__init__.py
+-rw-r--r--   0 june       (501) staff       (20)     5090 2023-04-28 07:44:21.000000 SDTcloud-0.0.7/SDTcloud/sdtcloud.py
+drwxr-xr-x   0 june       (501) staff       (20)        0 2023-05-02 05:17:52.126816 SDTcloud-0.0.7/SDTcloud.egg-info/
+-rw-r--r--   0 june       (501) staff       (20)      398 2023-05-02 05:17:52.000000 SDTcloud-0.0.7/SDTcloud.egg-info/PKG-INFO
+-rw-r--r--   0 june       (501) staff       (20)      188 2023-05-02 05:17:52.000000 SDTcloud-0.0.7/SDTcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 june       (501) staff       (20)        1 2023-05-02 05:17:52.000000 SDTcloud-0.0.7/SDTcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 june       (501) staff       (20)        9 2023-05-02 05:17:52.000000 SDTcloud-0.0.7/SDTcloud.egg-info/top_level.txt
+-rw-r--r--   0 june       (501) staff       (20)       38 2023-05-02 05:17:52.127226 SDTcloud-0.0.7/setup.cfg
+-rw-r--r--   0 june       (501) staff       (20)      656 2023-05-02 04:07:52.000000 SDTcloud-0.0.7/setup.py
```

### Comparing `SDTcloud-0.0.6/SDTcloud/sdtcloud.py` & `SDTcloud-0.0.7/SDTcloud/sdtcloud.py`

 * *Files identical despite different names*

### Comparing `SDTcloud-0.0.6/setup.py` & `SDTcloud-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SDTcloud", # Replace with your own username
-    version="0.0.6",
+    version="0.0.7",
     author="sujune",
     author_email="hoakw@sdt.inc",
     description="SDT cloud API Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

