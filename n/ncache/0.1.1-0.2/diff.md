# Comparing `tmp/ncache-0.1.1.tar.gz` & `tmp/ncache-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncache-0.1.1.tar", last modified: Thu Feb 16 19:42:46 2023, max compression
+gzip compressed data, was "ncache-0.2.tar", last modified: Tue May  2 09:33:09 2023, max compression
```

## Comparing `ncache-0.1.1.tar` & `ncache-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-02-16 19:42:46.443384 ncache-0.1.1/
--rw-r--r--   0 ok        (1000) ok        (1000)     1800 2023-02-16 19:42:46.443384 ncache-0.1.1/PKG-INFO
--rw-r--r--   0 ok        (1000) ok        (1000)      988 2023-02-13 21:10:03.000000 ncache-0.1.1/README.md
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-02-16 19:42:46.442384 ncache-0.1.1/ncache/
--rw-r--r--   0 ok        (1000) ok        (1000)       21 2023-02-16 19:17:55.000000 ncache-0.1.1/ncache/__init__.py
--rw-r--r--   0 ok        (1000) ok        (1000)     2169 2023-02-16 19:17:16.000000 ncache-0.1.1/ncache/ncache.py
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-02-16 19:42:46.442384 ncache-0.1.1/ncache.egg-info/
--rw-r--r--   0 ok        (1000) ok        (1000)     1800 2023-02-16 19:42:46.000000 ncache-0.1.1/ncache.egg-info/PKG-INFO
--rw-r--r--   0 ok        (1000) ok        (1000)      178 2023-02-16 19:42:46.000000 ncache-0.1.1/ncache.egg-info/SOURCES.txt
--rw-r--r--   0 ok        (1000) ok        (1000)        1 2023-02-16 19:42:46.000000 ncache-0.1.1/ncache.egg-info/dependency_links.txt
--rw-r--r--   0 ok        (1000) ok        (1000)        7 2023-02-16 19:42:46.000000 ncache-0.1.1/ncache.egg-info/top_level.txt
--rw-r--r--   0 ok        (1000) ok        (1000)       38 2023-02-16 19:42:46.443384 ncache-0.1.1/setup.cfg
--rw-r--r--   0 ok        (1000) ok        (1000)     1052 2023-02-16 19:35:29.000000 ncache-0.1.1/setup.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-02 09:33:09.215727 ncache-0.2/
+-rw-r--r--   0 ok        (1000) ok        (1000)     1798 2023-05-02 09:33:09.215727 ncache-0.2/PKG-INFO
+-rw-r--r--   0 ok        (1000) ok        (1000)      988 2023-02-13 21:10:03.000000 ncache-0.2/README.md
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-02 09:33:09.213727 ncache-0.2/ncache/
+-rw-r--r--   0 ok        (1000) ok        (1000)       21 2023-02-16 19:17:55.000000 ncache-0.2/ncache/__init__.py
+-rw-r--r--   0 ok        (1000) ok        (1000)     2443 2023-05-02 09:32:46.000000 ncache-0.2/ncache/ncache.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-02 09:33:09.215727 ncache-0.2/ncache.egg-info/
+-rw-r--r--   0 ok        (1000) ok        (1000)     1798 2023-05-02 09:33:08.000000 ncache-0.2/ncache.egg-info/PKG-INFO
+-rw-r--r--   0 ok        (1000) ok        (1000)      178 2023-05-02 09:33:09.000000 ncache-0.2/ncache.egg-info/SOURCES.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)        1 2023-05-02 09:33:08.000000 ncache-0.2/ncache.egg-info/dependency_links.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)        7 2023-05-02 09:33:08.000000 ncache-0.2/ncache.egg-info/top_level.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)       38 2023-05-02 09:33:09.215727 ncache-0.2/setup.cfg
+-rw-r--r--   0 ok        (1000) ok        (1000)     1052 2023-02-16 19:35:29.000000 ncache-0.2/setup.py
```

### Comparing `ncache-0.1.1/PKG-INFO` & `ncache-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncache
-Version: 0.1.1
+Version: 0.2
 Summary: A simple and lightweight dictionary-based persistent cache for storing python objects.
 Home-page: https://github.com/rsusik/ncache
 Author: Robert Susik
 Author-email: robert.susik@gmail.com
 License: GPLv3
 Description: # Nano cache
```

### Comparing `ncache-0.1.1/README.md` & `ncache-0.2/README.md`

 * *Files identical despite different names*

### Comparing `ncache-0.1.1/ncache/ncache.py` & `ncache-0.2/ncache/ncache.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 import hashlib
 import pickle
 from typing import Any
 import os
 
-__version__ = '0.1.1'
+__version__ = '0.2'
 
 class Cache:
-    def __init__(self, filename:str, nocache:bool=False):
+    def __init__(self, 
+        filename:str, 
+        nocache:bool=False, 
+        tmpfilename:str=None # if None no temp file is created
+    ):
         self.filename = filename
+        if tmpfilename is None:
+            self.tmpfilename = self.filename
+        else:
+            self.tmpfilename = tmpfilename
         self.nocache = nocache
         self.cache = {}
     
     def if_cache_on(alt_exception=None, alt_value=None):
         def wrapper(fun):
             def inner(self, *args, **kwargs):
                 if self.nocache == False:
@@ -41,16 +49,17 @@
                 self.cache = pickle.load(f)
         else:
             print('Cache does not exists. Creating new one.')
             self.cache = {}
     
     @if_cache_on()
     def save_cache(self):
-        with open(self.filename, 'wb') as f:
-                pickle.dump(self.cache, f)
+        with open(self.tmpfilename, 'wb') as f:
+            pickle.dump(self.cache, f)
+            os.rename(self.tmpfilename, self.filename)
 
     class NoCacheValue(Exception):
         pass
 
     @if_cache_on(alt_exception=NoCacheValue())
     def get_value(self, obj:Any)->Any:
         _hash = self.get_hash(obj)
```

### Comparing `ncache-0.1.1/ncache.egg-info/PKG-INFO` & `ncache-0.2/ncache.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncache
-Version: 0.1.1
+Version: 0.2
 Summary: A simple and lightweight dictionary-based persistent cache for storing python objects.
 Home-page: https://github.com/rsusik/ncache
 Author: Robert Susik
 Author-email: robert.susik@gmail.com
 License: GPLv3
 Description: # Nano cache
```

### Comparing `ncache-0.1.1/setup.py` & `ncache-0.2/setup.py`

 * *Files identical despite different names*

