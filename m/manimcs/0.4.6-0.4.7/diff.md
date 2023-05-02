# Comparing `tmp/manimcs-0.4.6.tar.gz` & `tmp/manimcs-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manimcs-0.4.6.tar", last modified: Tue May  2 21:40:04 2023, max compression
+gzip compressed data, was "manimcs-0.4.7.tar", last modified: Tue May  2 21:43:22 2023, max compression
```

## Comparing `manimcs-0.4.6.tar` & `manimcs-0.4.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:40:04.838382 manimcs-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-02 21:40:04.838382 manimcs-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-02 21:39:45.000000 manimcs-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:40:04.834382 manimcs-0.4.6/manimcs/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 21:39:45.000000 manimcs-0.4.6/manimcs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:40:04.834382 manimcs-0.4.6/manimcs/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 21:39:45.000000 manimcs-0.4.6/manimcs/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-05-02 21:39:45.000000 manimcs-0.4.6/manimcs/algorithms/array_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:40:04.834382 manimcs-0.4.6/manimcs/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 21:39:45.000000 manimcs-0.4.6/manimcs/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-02 21:39:45.000000 manimcs-0.4.6/manimcs/engine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:40:04.834382 manimcs-0.4.6/manimcs/mobjs/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 21:39:45.000000 manimcs-0.4.6/manimcs/mobjs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-02 21:39:45.000000 manimcs-0.4.6/manimcs/mobjs/sort_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-02 21:39:45.000000 manimcs-0.4.6/manimcs/mobjs/sortable_mobject.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-02 21:39:45.000000 manimcs-0.4.6/manimcs/mobjs/svg_mobject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:40:04.834382 manimcs-0.4.6/manimcs/renderer/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 21:39:45.000000 manimcs-0.4.6/manimcs/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 21:39:45.000000 manimcs-0.4.6/manimcs/renderer/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:40:04.838382 manimcs-0.4.6/manimcs/scene/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-02 21:39:45.000000 manimcs-0.4.6/manimcs/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 21:39:45.000000 manimcs-0.4.6/manimcs/scene/array_sort_scene.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:40:04.834382 manimcs-0.4.6/manimcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-02 21:40:04.000000 manimcs-0.4.6/manimcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-02 21:40:04.000000 manimcs-0.4.6/manimcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:40:04.000000 manimcs-0.4.6/manimcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 21:40:04.000000 manimcs-0.4.6/manimcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 21:40:04.000000 manimcs-0.4.6/manimcs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 21:39:45.000000 manimcs-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:40:04.838382 manimcs-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-02 21:39:45.000000 manimcs-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:43:22.276899 manimcs-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-02 21:43:22.276899 manimcs-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-02 21:43:07.000000 manimcs-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:43:22.272899 manimcs-0.4.7/manimcs/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 21:43:07.000000 manimcs-0.4.7/manimcs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:43:22.276899 manimcs-0.4.7/manimcs/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 21:43:07.000000 manimcs-0.4.7/manimcs/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-05-02 21:43:07.000000 manimcs-0.4.7/manimcs/algorithms/array_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:43:22.276899 manimcs-0.4.7/manimcs/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 21:43:07.000000 manimcs-0.4.7/manimcs/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-02 21:43:07.000000 manimcs-0.4.7/manimcs/engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:43:22.276899 manimcs-0.4.7/manimcs/mobjs/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 21:43:07.000000 manimcs-0.4.7/manimcs/mobjs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-02 21:43:07.000000 manimcs-0.4.7/manimcs/mobjs/sort_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-02 21:43:07.000000 manimcs-0.4.7/manimcs/mobjs/sortable_mobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-02 21:43:07.000000 manimcs-0.4.7/manimcs/mobjs/svg_mobject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:43:22.276899 manimcs-0.4.7/manimcs/renderer/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 21:43:07.000000 manimcs-0.4.7/manimcs/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 21:43:07.000000 manimcs-0.4.7/manimcs/renderer/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:43:22.276899 manimcs-0.4.7/manimcs/scene/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-02 21:43:07.000000 manimcs-0.4.7/manimcs/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 21:43:07.000000 manimcs-0.4.7/manimcs/scene/array_sort_scene.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:43:22.276899 manimcs-0.4.7/manimcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-02 21:43:22.000000 manimcs-0.4.7/manimcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-02 21:43:22.000000 manimcs-0.4.7/manimcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:43:22.000000 manimcs-0.4.7/manimcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 21:43:22.000000 manimcs-0.4.7/manimcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 21:43:22.000000 manimcs-0.4.7/manimcs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 21:43:07.000000 manimcs-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:43:22.280899 manimcs-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-02 21:43:07.000000 manimcs-0.4.7/setup.py
```

### Comparing `manimcs-0.4.6/PKG-INFO` & `manimcs-0.4.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manimcs
-Version: 0.4.6
+Version: 0.4.7
 Summary: An Animation Library for Explanitory Computer Science Videos
 Home-page: https://github.com/CadenScharpf/manim-cs
 Author: Caden Scharpf
 Author-email: caden.scharpf@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: manimcs Version: 0.4.6 Summary: An Animation
+Metadata-Version: 2.1 Name: manimcs Version: 0.4.7 Summary: An Animation
 Library for Explanitory Computer Science Videos Home-page: https://github.com/
 CadenScharpf/manim-cs Author: Caden Scharpf Author-email:
 caden.scharpf@icloud.com Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `manimcs-0.4.6/README.md` & `manimcs-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `manimcs-0.4.6/manimcs/algorithms/array_sort.py` & `manimcs-0.4.7/manimcs/algorithms/array_sort.py`

 * *Files identical despite different names*

### Comparing `manimcs-0.4.6/manimcs/engine/engine.py` & `manimcs-0.4.7/manimcs/engine/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             "bucket-sort": ArraySort.unImplementedAlgorithm},
         "tree" : {
             
         }
     }
     def __init__(self, command, *args, **kwargs):
         if command in self.commands.get("array"):
-            if not 'inputValue' in kwargs:
+            if not 'inputValues' in kwargs:
                 print("MANIM-CS-ERR: Please enter a list of integers to sort")
                 raise ValueError("MANIM-CS-ERR: Please enter a list of integers to sort")
             if 'output_dir' in kwargs:
                 self.output_dir = kwargs.get('output_dir')
             self.init_config(self.output_dir)
```

### Comparing `manimcs-0.4.6/manimcs/mobjs/sort_set.py` & `manimcs-0.4.7/manimcs/mobjs/sort_set.py`

 * *Files identical despite different names*

### Comparing `manimcs-0.4.6/manimcs/mobjs/sortable_mobject.py` & `manimcs-0.4.7/manimcs/mobjs/sortable_mobject.py`

 * *Files identical despite different names*

### Comparing `manimcs-0.4.6/manimcs.egg-info/PKG-INFO` & `manimcs-0.4.7/manimcs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manimcs
-Version: 0.4.6
+Version: 0.4.7
 Summary: An Animation Library for Explanitory Computer Science Videos
 Home-page: https://github.com/CadenScharpf/manim-cs
 Author: Caden Scharpf
 Author-email: caden.scharpf@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: manimcs Version: 0.4.6 Summary: An Animation
+Metadata-Version: 2.1 Name: manimcs Version: 0.4.7 Summary: An Animation
 Library for Explanitory Computer Science Videos Home-page: https://github.com/
 CadenScharpf/manim-cs Author: Caden Scharpf Author-email:
 caden.scharpf@icloud.com Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `manimcs-0.4.6/manimcs.egg-info/SOURCES.txt` & `manimcs-0.4.7/manimcs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manimcs-0.4.6/setup.py` & `manimcs-0.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='manimcs',
-    version='0.4.6',
+    version='0.4.7',
     packages=find_packages(),
     install_requires=[
         'manim==0.17.3',
         # Add any other dependencies here
     ],
     author='Caden Scharpf',
     author_email='caden.scharpf@icloud.com',
```

