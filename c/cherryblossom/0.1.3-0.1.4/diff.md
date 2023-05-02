# Comparing `tmp/cherryblossom-0.1.3.tar.gz` & `tmp/cherryblossom-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cherryblossom-0.1.3.tar", last modified: Tue May  2 06:25:27 2023, max compression
+gzip compressed data, was "cherryblossom-0.1.4.tar", last modified: Tue May  2 06:27:53 2023, max compression
```

## Comparing `cherryblossom-0.1.3.tar` & `cherryblossom-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-02 06:25:27.535958 cherryblossom-0.1.3/
--rw-r--r--   0 arjun      (501) staff       (20)       32 2023-04-17 05:21:05.000000 cherryblossom-0.1.3/MANIFEST.in
--rw-r--r--   0 arjun      (501) staff       (20)      396 2023-05-02 06:25:27.535780 cherryblossom-0.1.3/PKG-INFO
--rw-r--r--   0 arjun      (501) staff       (20)       13 2023-04-16 05:11:44.000000 cherryblossom-0.1.3/README.md
--rw-r--r--   0 arjun      (501) staff       (20)     1568 2023-05-02 06:25:08.000000 cherryblossom-0.1.3/pyproject.toml
--rw-r--r--   0 arjun      (501) staff       (20)       38 2023-05-02 06:25:27.536002 cherryblossom-0.1.3/setup.cfg
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-02 06:25:27.527515 cherryblossom-0.1.3/src/
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-02 06:25:27.533105 cherryblossom-0.1.3/src/cherryblossom/
--rw-r--r--   0 arjun      (501) staff       (20)     4601 2023-04-16 02:36:30.000000 cherryblossom-0.1.3/src/cherryblossom/.key
--rw-r--r--   0 arjun      (501) staff       (20)       82 2023-04-17 01:04:25.000000 cherryblossom-0.1.3/src/cherryblossom/Analyzer.py
--rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:04:20.000000 cherryblossom-0.1.3/src/cherryblossom/Blossom.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:17.000000 cherryblossom-0.1.3/src/cherryblossom/Channels.py
--rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:04:00.000000 cherryblossom-0.1.3/src/cherryblossom/Chat.py
--rw-r--r--   0 arjun      (501) staff       (20)       64 2023-04-17 01:03:39.000000 cherryblossom-0.1.3/src/cherryblossom/DB.py
--rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:03:43.000000 cherryblossom-0.1.3/src/cherryblossom/Data.py
--rw-r--r--   0 arjun      (501) staff       (20)       81 2023-04-17 01:03:33.000000 cherryblossom-0.1.3/src/cherryblossom/Functions.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:03:25.000000 cherryblossom-0.1.3/src/cherryblossom/GPTModel.py
--rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:03:20.000000 cherryblossom-0.1.3/src/cherryblossom/Index.py
--rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:04:04.000000 cherryblossom-0.1.3/src/cherryblossom/Plots.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:04.000000 cherryblossom-0.1.3/src/cherryblossom/Timezone.py
--rw-r--r--   0 arjun      (501) staff       (20)       19 2023-04-17 01:04:31.000000 cherryblossom-0.1.3/src/cherryblossom/__init__.py
--rw-r--r--   0 arjun      (501) staff       (20)     1213 2023-04-16 04:16:55.000000 cherryblossom-0.1.3/src/cherryblossom/get_file.py
--rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:03:19.000000 cherryblossom-0.1.3/src/cherryblossom/imports.py
--rw-r--r--   0 arjun      (501) staff       (20)     4685 2023-05-02 06:21:57.000000 cherryblossom-0.1.3/src/cherryblossom/key.py
--rw-r--r--   0 arjun      (501) staff       (20)      569 2023-05-02 06:24:40.000000 cherryblossom-0.1.3/src/cherryblossom/main.py
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-02 06:25:27.534297 cherryblossom-0.1.3/src/cherryblossom.egg-info/
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-02 06:25:27.535450 cherryblossom-0.1.3/src/cherryblossom.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 arjun      (501) staff       (20)      713 2023-04-17 20:05:12.000000 cherryblossom-0.1.3/src/cherryblossom.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 arjun      (501) staff       (20)        1 2023-04-17 20:05:12.000000 cherryblossom-0.1.3/src/cherryblossom.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-r--r--   0 arjun      (501) staff       (20)      101 2023-04-17 20:05:12.000000 cherryblossom-0.1.3/src/cherryblossom.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 arjun      (501) staff       (20)       14 2023-04-17 20:05:12.000000 cherryblossom-0.1.3/src/cherryblossom.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 arjun      (501) staff       (20)      396 2023-05-02 06:25:27.000000 cherryblossom-0.1.3/src/cherryblossom.egg-info/PKG-INFO
--rw-r--r--   0 arjun      (501) staff       (20)     1026 2023-05-02 06:25:27.000000 cherryblossom-0.1.3/src/cherryblossom.egg-info/SOURCES.txt
--rw-r--r--   0 arjun      (501) staff       (20)        1 2023-05-02 06:25:27.000000 cherryblossom-0.1.3/src/cherryblossom.egg-info/dependency_links.txt
--rw-r--r--   0 arjun      (501) staff       (20)      101 2023-05-02 06:25:27.000000 cherryblossom-0.1.3/src/cherryblossom.egg-info/requires.txt
--rw-r--r--   0 arjun      (501) staff       (20)       14 2023-05-02 06:25:27.000000 cherryblossom-0.1.3/src/cherryblossom.egg-info/top_level.txt
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-02 06:27:53.520020 cherryblossom-0.1.4/
+-rw-r--r--   0 arjun      (501) staff       (20)       32 2023-04-17 05:21:05.000000 cherryblossom-0.1.4/MANIFEST.in
+-rw-r--r--   0 arjun      (501) staff       (20)      396 2023-05-02 06:27:53.519880 cherryblossom-0.1.4/PKG-INFO
+-rw-r--r--   0 arjun      (501) staff       (20)       13 2023-04-16 05:11:44.000000 cherryblossom-0.1.4/README.md
+-rw-r--r--   0 arjun      (501) staff       (20)     1568 2023-05-02 06:27:33.000000 cherryblossom-0.1.4/pyproject.toml
+-rw-r--r--   0 arjun      (501) staff       (20)       38 2023-05-02 06:27:53.520058 cherryblossom-0.1.4/setup.cfg
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-02 06:27:53.512844 cherryblossom-0.1.4/src/
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-02 06:27:53.517726 cherryblossom-0.1.4/src/cherryblossom/
+-rw-r--r--   0 arjun      (501) staff       (20)     4601 2023-04-16 02:36:30.000000 cherryblossom-0.1.4/src/cherryblossom/.key
+-rw-r--r--   0 arjun      (501) staff       (20)       82 2023-04-17 01:04:25.000000 cherryblossom-0.1.4/src/cherryblossom/Analyzer.py
+-rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:04:20.000000 cherryblossom-0.1.4/src/cherryblossom/Blossom.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:17.000000 cherryblossom-0.1.4/src/cherryblossom/Channels.py
+-rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:04:00.000000 cherryblossom-0.1.4/src/cherryblossom/Chat.py
+-rw-r--r--   0 arjun      (501) staff       (20)       64 2023-04-17 01:03:39.000000 cherryblossom-0.1.4/src/cherryblossom/DB.py
+-rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:03:43.000000 cherryblossom-0.1.4/src/cherryblossom/Data.py
+-rw-r--r--   0 arjun      (501) staff       (20)       81 2023-04-17 01:03:33.000000 cherryblossom-0.1.4/src/cherryblossom/Functions.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:03:25.000000 cherryblossom-0.1.4/src/cherryblossom/GPTModel.py
+-rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:03:20.000000 cherryblossom-0.1.4/src/cherryblossom/Index.py
+-rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:04:04.000000 cherryblossom-0.1.4/src/cherryblossom/Plots.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:04.000000 cherryblossom-0.1.4/src/cherryblossom/Timezone.py
+-rw-r--r--   0 arjun      (501) staff       (20)       19 2023-04-17 01:04:31.000000 cherryblossom-0.1.4/src/cherryblossom/__init__.py
+-rw-r--r--   0 arjun      (501) staff       (20)     1213 2023-04-16 04:16:55.000000 cherryblossom-0.1.4/src/cherryblossom/get_file.py
+-rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:03:19.000000 cherryblossom-0.1.4/src/cherryblossom/imports.py
+-rw-r--r--   0 arjun      (501) staff       (20)     4685 2023-05-02 06:21:57.000000 cherryblossom-0.1.4/src/cherryblossom/key.py
+-rw-r--r--   0 arjun      (501) staff       (20)      586 2023-05-02 06:27:14.000000 cherryblossom-0.1.4/src/cherryblossom/main.py
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-02 06:27:53.518532 cherryblossom-0.1.4/src/cherryblossom.egg-info/
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-05-02 06:27:53.519583 cherryblossom-0.1.4/src/cherryblossom.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 arjun      (501) staff       (20)      713 2023-04-17 20:05:12.000000 cherryblossom-0.1.4/src/cherryblossom.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 arjun      (501) staff       (20)        1 2023-04-17 20:05:12.000000 cherryblossom-0.1.4/src/cherryblossom.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 arjun      (501) staff       (20)      101 2023-04-17 20:05:12.000000 cherryblossom-0.1.4/src/cherryblossom.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 arjun      (501) staff       (20)       14 2023-04-17 20:05:12.000000 cherryblossom-0.1.4/src/cherryblossom.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 arjun      (501) staff       (20)      396 2023-05-02 06:27:53.000000 cherryblossom-0.1.4/src/cherryblossom.egg-info/PKG-INFO
+-rw-r--r--   0 arjun      (501) staff       (20)     1026 2023-05-02 06:27:53.000000 cherryblossom-0.1.4/src/cherryblossom.egg-info/SOURCES.txt
+-rw-r--r--   0 arjun      (501) staff       (20)        1 2023-05-02 06:27:53.000000 cherryblossom-0.1.4/src/cherryblossom.egg-info/dependency_links.txt
+-rw-r--r--   0 arjun      (501) staff       (20)      101 2023-05-02 06:27:53.000000 cherryblossom-0.1.4/src/cherryblossom.egg-info/requires.txt
+-rw-r--r--   0 arjun      (501) staff       (20)       14 2023-05-02 06:27:53.000000 cherryblossom-0.1.4/src/cherryblossom.egg-info/top_level.txt
```

### Comparing `cherryblossom-0.1.3/pyproject.toml` & `cherryblossom-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 cherryblossom = [".key", "src/cherryblossom/*.py", "src/cherryblossom/.key", "cherryblossom/.key"]
 
 [project]
 name = "cherryblossom"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Arjun Naik", email="arjunsatishnaik@gmail.com" },
 ]
 description = "CherryBlossom: an API for Nosedive AI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cherryblossom-0.1.3/src/cherryblossom/.key` & `cherryblossom-0.1.4/src/cherryblossom/.key`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.1.3/src/cherryblossom/get_file.py` & `cherryblossom-0.1.4/src/cherryblossom/get_file.py`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.1.3/src/cherryblossom/key.py` & `cherryblossom-0.1.4/src/cherryblossom/key.py`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.1.3/src/cherryblossom/main.py` & `cherryblossom-0.1.4/src/cherryblossom/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 try:
     from .key import *
+except:
+    pass
 from .get_file import TOS
 
 print(TOS)
 print()
 if input("Do you agree with the Terms of Service? y/n: ") == 'y':
     print('Loading...', end = '\r')
     print()
```

### Comparing `cherryblossom-0.1.3/src/cherryblossom.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt` & `cherryblossom-0.1.4/src/cherryblossom.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.1.3/src/cherryblossom.egg-info/SOURCES.txt` & `cherryblossom-0.1.4/src/cherryblossom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

