# Comparing `tmp/tiny_ai_helper-0.1.7.tar.gz` & `tmp/tiny_ai_helper-0.1.7.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_ai_helper-0.1.7.tar", last modified: Tue May  2 09:09:50 2023, max compression
+gzip compressed data, was "tiny_ai_helper-0.1.7.post1.tar", last modified: Tue May  2 09:20:17 2023, max compression
```

## Comparing `tiny_ai_helper-0.1.7.tar` & `tiny_ai_helper-0.1.7.post1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-02 09:09:50.948392 tiny_ai_helper-0.1.7/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     1103 2023-03-09 17:46:27.000000 tiny_ai_helper-0.1.7/LICENSE
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-05-02 09:09:50.948392 tiny_ai_helper-0.1.7/PKG-INFO
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       74 2022-09-27 15:48:25.000000 tiny_ai_helper-0.1.7/README.md
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       38 2023-05-02 09:09:50.948392 tiny_ai_helper-0.1.7/setup.cfg
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     1029 2023-05-02 08:38:57.000000 tiny_ai_helper-0.1.7/setup.py
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-02 09:09:50.944392 tiny_ai_helper-0.1.7/tiny_ai_helper/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    14107 2023-05-01 18:50:11.000000 tiny_ai_helper-0.1.7/tiny_ai_helper/Model.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    10452 2023-04-30 10:47:53.000000 tiny_ai_helper-0.1.7/tiny_ai_helper/Trainer.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      367 2023-05-02 08:39:07.000000 tiny_ai_helper-0.1.7/tiny_ai_helper/__init__.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     6232 2023-03-23 11:28:02.000000 tiny_ai_helper-0.1.7/tiny_ai_helper/layers.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     9071 2023-03-15 18:42:46.000000 tiny_ai_helper-0.1.7/tiny_ai_helper/mp.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    19836 2023-05-02 09:06:06.000000 tiny_ai_helper-0.1.7/tiny_ai_helper/utils.py
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-02 09:09:50.948392 tiny_ai_helper-0.1.7/tiny_ai_helper.egg-info/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-05-02 09:09:50.000000 tiny_ai_helper-0.1.7/tiny_ai_helper.egg-info/PKG-INFO
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      325 2023-05-02 09:09:50.000000 tiny_ai_helper-0.1.7/tiny_ai_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 www-data  (1000) www-data  (1000)        1 2023-05-02 09:09:50.000000 tiny_ai_helper-0.1.7/tiny_ai_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       15 2023-05-02 09:09:50.000000 tiny_ai_helper-0.1.7/tiny_ai_helper.egg-info/top_level.txt
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-02 09:20:17.308942 tiny_ai_helper-0.1.7.post1/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     1103 2023-03-09 17:46:27.000000 tiny_ai_helper-0.1.7.post1/LICENSE
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      790 2023-05-02 09:20:17.308942 tiny_ai_helper-0.1.7.post1/PKG-INFO
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       74 2022-09-27 15:48:25.000000 tiny_ai_helper-0.1.7.post1/README.md
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       38 2023-05-02 09:20:17.308942 tiny_ai_helper-0.1.7.post1/setup.cfg
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     1031 2023-05-02 09:19:12.000000 tiny_ai_helper-0.1.7.post1/setup.py
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-02 09:20:17.308942 tiny_ai_helper-0.1.7.post1/tiny_ai_helper/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    14107 2023-05-01 18:50:11.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper/Model.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    10452 2023-04-30 10:47:53.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper/Trainer.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      369 2023-05-02 09:19:24.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper/__init__.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     6232 2023-03-23 11:28:02.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper/layers.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     9071 2023-03-15 18:42:46.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper/mp.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    19915 2023-05-02 09:14:39.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper/utils.py
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-02 09:20:17.308942 tiny_ai_helper-0.1.7.post1/tiny_ai_helper.egg-info/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      790 2023-05-02 09:20:17.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      325 2023-05-02 09:20:17.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)        1 2023-05-02 09:20:17.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       15 2023-05-02 09:20:17.000000 tiny_ai_helper-0.1.7.post1/tiny_ai_helper.egg-info/top_level.txt
```

### Comparing `tiny_ai_helper-0.1.7/LICENSE` & `tiny_ai_helper-0.1.7.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.7/PKG-INFO` & `tiny_ai_helper-0.1.7.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny_ai_helper
-Version: 0.1.7
+Version: 0.1.7.post1
 Summary: Tiny AI Helper for PyTorch
 Home-page: https://github.com/bayrell/ai_helper
 Author: Ildar Bikmamatov
 Author-email: support@bayrell.org
 License: MIT License
 Keywords: ai helper,pytorch
 Platform: UNKNOWN
```

### Comparing `tiny_ai_helper-0.1.7/setup.py` & `tiny_ai_helper-0.1.7.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 from setuptools import setup, find_packages
 from os.path import abspath, dirname, join
 
 setup(
 	name="tiny_ai_helper",
-	version="0.1.7",
+	version="0.1.7-1",
 	description="Tiny AI Helper for PyTorch",
 	long_description=open(join(abspath(dirname(__file__)), 'README.md'), encoding='utf-8').read(),
 	long_description_content_type='text/markdown',
 	author="Ildar Bikmamatov",
 	author_email="support@bayrell.org",
 	license="MIT License",
 	url = "https://github.com/bayrell/ai_helper",
```

### Comparing `tiny_ai_helper-0.1.7/tiny_ai_helper/Model.py` & `tiny_ai_helper-0.1.7.post1/tiny_ai_helper/Model.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.7/tiny_ai_helper/Trainer.py` & `tiny_ai_helper-0.1.7.post1/tiny_ai_helper/Trainer.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.7/tiny_ai_helper/layers.py` & `tiny_ai_helper-0.1.7.post1/tiny_ai_helper/layers.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.7/tiny_ai_helper/mp.py` & `tiny_ai_helper-0.1.7.post1/tiny_ai_helper/mp.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.7/tiny_ai_helper/utils.py` & `tiny_ai_helper-0.1.7.post1/tiny_ai_helper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -604,18 +604,18 @@
             for i in range(4):
                 sz = len(str(value[i]))
                 if info_sizes[i] < sz:
                     info_sizes[i] = sz
             
         def format_row(arr, size):
             s = "{:<"+str(size[0] + 1)+"} {:>"+str(size[1] + 2)+"}" + \
-                "{:>"+str(size[2] + 3)+"} {:>"+str(size[3] + 2)+"}"
+                "{:>"+str(size[2] + 5)+"} {:>"+str(size[3] + 5)+"}"
             return s.format(*arr)
         
-        width = 63
+        width = info_sizes[0] + 1 + info_sizes[1] + 2 + info_sizes[2] + 5 + info_sizes[3] + 5 + 2
         print( "=" * width )
         print( format_row(["", "Layer", "Output", "Params"], info_sizes) )
         print( "-" * width )
         
         for _, value in enumerate(values):
             print( format_row(value, info_sizes) )
```

### Comparing `tiny_ai_helper-0.1.7/tiny_ai_helper.egg-info/PKG-INFO` & `tiny_ai_helper-0.1.7.post1/tiny_ai_helper.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-ai-helper
-Version: 0.1.7
+Version: 0.1.7.post1
 Summary: Tiny AI Helper for PyTorch
 Home-page: https://github.com/bayrell/ai_helper
 Author: Ildar Bikmamatov
 Author-email: support@bayrell.org
 License: MIT License
 Keywords: ai helper,pytorch
 Platform: UNKNOWN
```

