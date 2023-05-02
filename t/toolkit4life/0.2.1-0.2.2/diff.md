# Comparing `tmp/toolkit4life-0.2.1.tar.gz` & `tmp/toolkit4life-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolkit4life-0.2.1.tar", last modified: Wed Apr 26 15:24:42 2023, max compression
+gzip compressed data, was "toolkit4life-0.2.2.tar", last modified: Tue May  2 19:04:48 2023, max compression
```

## Comparing `toolkit4life-0.2.1.tar` & `toolkit4life-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:24:42.777644 toolkit4life-0.2.1/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      788 2023-04-26 15:24:42.773645 toolkit4life-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      371 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)      217 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 15:24:42.777644 toolkit4life-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1542 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:24:42.757650 toolkit4life-0.2.1/toolkit4life/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:24:42.761649 toolkit4life-0.2.1/toolkit4life/clients/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/clients/_sqlalchemy.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/clients/postgres.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/clients/redis.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/clients/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:24:42.761649 toolkit4life-0.2.1/toolkit4life/telegram/
--rw-r--r--   0 root         (0) root         (0)     2768 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/telegram/restrictors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:24:42.773645 toolkit4life-0.2.1/toolkit4life/utils/
--rw-r--r--   0 root         (0) root         (0)     4334 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     5397 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/utils/requests.py
--rw-r--r--   0 root         (0) root         (0)     2620 2023-04-26 15:18:14.000000 toolkit4life-0.2.1/toolkit4life/utils/threads.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:24:42.757650 toolkit4life-0.2.1/toolkit4life.egg-info/
--rw-r--r--   0 root         (0) root         (0)      788 2023-04-26 15:24:42.000000 toolkit4life-0.2.1/toolkit4life.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      548 2023-04-26 15:24:42.000000 toolkit4life-0.2.1/toolkit4life.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 15:24:42.000000 toolkit4life-0.2.1/toolkit4life.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      218 2023-04-26 15:24:42.000000 toolkit4life-0.2.1/toolkit4life.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 15:24:42.000000 toolkit4life-0.2.1/toolkit4life.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:04:48.588832 toolkit4life-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-04-26 15:18:14.000000 toolkit4life-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-26 15:18:14.000000 toolkit4life-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      788 2023-05-02 19:04:48.588832 toolkit4life-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      371 2023-04-26 15:18:14.000000 toolkit4life-0.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      217 2023-04-26 15:18:14.000000 toolkit4life-0.2.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 19:04:48.588832 toolkit4life-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-02 19:04:41.000000 toolkit4life-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:04:48.584832 toolkit4life-0.2.2/toolkit4life/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 15:18:14.000000 toolkit4life-0.2.2/toolkit4life/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:04:48.588832 toolkit4life-0.2.2/toolkit4life/clients/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 15:18:14.000000 toolkit4life-0.2.2/toolkit4life/clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-04-26 15:18:14.000000 toolkit4life-0.2.2/toolkit4life/clients/_sqlalchemy.py
+-rw-r--r--   0 root         (0) root         (0)     3228 2023-05-02 19:03:38.000000 toolkit4life-0.2.2/toolkit4life/clients/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-04-26 15:18:14.000000 toolkit4life-0.2.2/toolkit4life/clients/redis.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-04-26 15:18:14.000000 toolkit4life-0.2.2/toolkit4life/clients/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:04:48.588832 toolkit4life-0.2.2/toolkit4life/telegram/
+-rw-r--r--   0 root         (0) root         (0)     2768 2023-04-26 15:18:14.000000 toolkit4life-0.2.2/toolkit4life/telegram/restrictors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:04:48.588832 toolkit4life-0.2.2/toolkit4life/utils/
+-rw-r--r--   0 root         (0) root         (0)     4334 2023-04-26 15:18:14.000000 toolkit4life-0.2.2/toolkit4life/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     5397 2023-04-26 15:18:14.000000 toolkit4life-0.2.2/toolkit4life/utils/requests.py
+-rw-r--r--   0 root         (0) root         (0)     2620 2023-04-26 15:18:14.000000 toolkit4life-0.2.2/toolkit4life/utils/threads.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 19:04:48.584832 toolkit4life-0.2.2/toolkit4life.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      788 2023-05-02 19:04:48.000000 toolkit4life-0.2.2/toolkit4life.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      548 2023-05-02 19:04:48.000000 toolkit4life-0.2.2/toolkit4life.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 19:04:48.000000 toolkit4life-0.2.2/toolkit4life.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      218 2023-05-02 19:04:48.000000 toolkit4life-0.2.2/toolkit4life.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-02 19:04:48.000000 toolkit4life-0.2.2/toolkit4life.egg-info/top_level.txt
```

### Comparing `toolkit4life-0.2.1/LICENSE` & `toolkit4life-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toolkit4life-0.2.1/PKG-INFO` & `toolkit4life-0.2.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolkit4life
-Version: 0.2.1
+Version: 0.2.2
 Summary: Faster deployment is what we want!
 Home-page: https://github.com/keivanipchihagh/toolkit4life
 Author: Keivan Ipchi Hagh
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `toolkit4life-0.2.1/setup.py` & `toolkit4life-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name = "toolkit4life",                                      # This is the name of the package
-    version = "0.2.01",                                         # The initial release version
+    version = "0.2.2",                                          # The initial release version
     author = "Keivan Ipchi Hagh",                               # Full name of the author
     url = "https://github.com/keivanipchihagh/toolkit4life",    # URL to the github repository
     description = "Faster deployment is what we want!",
     long_description = long_description,                        # Long description read from the the readme file
     long_description_content_type = "text/markdown",
     packages = find_namespace_packages(
         include = ["toolkit4life", "toolkit4life.*"]            # List of all python modules to be installed
```

### Comparing `toolkit4life-0.2.1/toolkit4life/clients/_sqlalchemy.py` & `toolkit4life-0.2.2/toolkit4life/clients/_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `toolkit4life-0.2.1/toolkit4life/clients/redis.py` & `toolkit4life-0.2.2/toolkit4life/clients/redis.py`

 * *Files identical despite different names*

### Comparing `toolkit4life-0.2.1/toolkit4life/clients/trino.py` & `toolkit4life-0.2.2/toolkit4life/clients/trino.py`

 * *Files identical despite different names*

### Comparing `toolkit4life-0.2.1/toolkit4life/telegram/restrictors.py` & `toolkit4life-0.2.2/toolkit4life/telegram/restrictors.py`

 * *Files identical despite different names*

### Comparing `toolkit4life-0.2.1/toolkit4life/utils/logger.py` & `toolkit4life-0.2.2/toolkit4life/utils/logger.py`

 * *Files identical despite different names*

### Comparing `toolkit4life-0.2.1/toolkit4life/utils/requests.py` & `toolkit4life-0.2.2/toolkit4life/utils/requests.py`

 * *Files identical despite different names*

### Comparing `toolkit4life-0.2.1/toolkit4life/utils/threads.py` & `toolkit4life-0.2.2/toolkit4life/utils/threads.py`

 * *Files identical despite different names*

### Comparing `toolkit4life-0.2.1/toolkit4life.egg-info/PKG-INFO` & `toolkit4life-0.2.2/toolkit4life.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolkit4life
-Version: 0.2.1
+Version: 0.2.2
 Summary: Faster deployment is what we want!
 Home-page: https://github.com/keivanipchihagh/toolkit4life
 Author: Keivan Ipchi Hagh
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `toolkit4life-0.2.1/toolkit4life.egg-info/SOURCES.txt` & `toolkit4life-0.2.2/toolkit4life.egg-info/SOURCES.txt`

 * *Files identical despite different names*

