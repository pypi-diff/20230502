# Comparing `tmp/manimcs-0.2.tar.gz` & `tmp/manimcs-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manimcs-0.2.tar", last modified: Tue May  2 18:37:26 2023, max compression
+gzip compressed data, was "manimcs-0.3.tar", last modified: Tue May  2 19:29:29 2023, max compression
```

## Comparing `manimcs-0.2.tar` & `manimcs-0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:37:26.079413 manimcs-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-02 18:37:26.079413 manimcs-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-02 18:37:13.000000 manimcs-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:37:26.075413 manimcs-0.2/manimcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-02 18:37:26.000000 manimcs-0.2/manimcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-02 18:37:26.000000 manimcs-0.2/manimcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 18:37:26.000000 manimcs-0.2/manimcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 18:37:26.000000 manimcs-0.2/manimcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 18:37:26.000000 manimcs-0.2/manimcs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 18:37:13.000000 manimcs-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 18:37:26.079413 manimcs-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-02 18:37:13.000000 manimcs-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:37:26.075413 manimcs-0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 18:37:13.000000 manimcs-0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:37:26.075413 manimcs-0.2/src/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 18:37:13.000000 manimcs-0.2/src/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-05-02 18:37:13.000000 manimcs-0.2/src/algorithms/array_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:37:26.075413 manimcs-0.2/src/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 18:37:13.000000 manimcs-0.2/src/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-02 18:37:13.000000 manimcs-0.2/src/engine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:37:26.079413 manimcs-0.2/src/mobjs/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 18:37:13.000000 manimcs-0.2/src/mobjs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-02 18:37:13.000000 manimcs-0.2/src/mobjs/sort_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-02 18:37:13.000000 manimcs-0.2/src/mobjs/sortable_mobject.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-02 18:37:13.000000 manimcs-0.2/src/mobjs/svg_mobject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:37:26.079413 manimcs-0.2/src/renderer/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 18:37:13.000000 manimcs-0.2/src/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 18:37:13.000000 manimcs-0.2/src/renderer/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 18:37:26.079413 manimcs-0.2/src/scene/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-02 18:37:13.000000 manimcs-0.2/src/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 18:37:13.000000 manimcs-0.2/src/scene/array_sort_scene.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:29:29.067632 manimcs-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-02 19:29:29.067632 manimcs-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-02 19:29:18.000000 manimcs-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:29:29.063632 manimcs-0.3/manimcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-02 19:29:29.000000 manimcs-0.3/manimcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-02 19:29:29.000000 manimcs-0.3/manimcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:29:29.000000 manimcs-0.3/manimcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 19:29:29.000000 manimcs-0.3/manimcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 19:29:29.000000 manimcs-0.3/manimcs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 19:29:18.000000 manimcs-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:29:29.067632 manimcs-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-02 19:29:18.000000 manimcs-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:29:29.063632 manimcs-0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 19:29:18.000000 manimcs-0.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:29:29.063632 manimcs-0.3/src/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 19:29:18.000000 manimcs-0.3/src/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-05-02 19:29:18.000000 manimcs-0.3/src/algorithms/array_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:29:29.063632 manimcs-0.3/src/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 19:29:18.000000 manimcs-0.3/src/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-02 19:29:18.000000 manimcs-0.3/src/engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:29:29.063632 manimcs-0.3/src/mobjs/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 19:29:18.000000 manimcs-0.3/src/mobjs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-02 19:29:18.000000 manimcs-0.3/src/mobjs/sort_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-02 19:29:18.000000 manimcs-0.3/src/mobjs/sortable_mobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-02 19:29:18.000000 manimcs-0.3/src/mobjs/svg_mobject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:29:29.063632 manimcs-0.3/src/renderer/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 19:29:18.000000 manimcs-0.3/src/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 19:29:18.000000 manimcs-0.3/src/renderer/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:29:29.063632 manimcs-0.3/src/scene/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-02 19:29:18.000000 manimcs-0.3/src/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 19:29:18.000000 manimcs-0.3/src/scene/array_sort_scene.py
```

### Comparing `manimcs-0.2/PKG-INFO` & `manimcs-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manimcs
-Version: 0.2
+Version: 0.3
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
-Metadata-Version: 2.1 Name: manimcs Version: 0.2 Summary: An Animation Library
+Metadata-Version: 2.1 Name: manimcs Version: 0.3 Summary: An Animation Library
 for Explanitory Computer Science Videos Home-page: https://github.com/
 CadenScharpf/manim-cs Author: Caden Scharpf Author-email:
 caden.scharpf@icloud.com Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `manimcs-0.2/README.md` & `manimcs-0.3/README.md`

 * *Files identical despite different names*

### Comparing `manimcs-0.2/manimcs.egg-info/PKG-INFO` & `manimcs-0.3/manimcs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manimcs
-Version: 0.2
+Version: 0.3
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
-Metadata-Version: 2.1 Name: manimcs Version: 0.2 Summary: An Animation Library
+Metadata-Version: 2.1 Name: manimcs Version: 0.3 Summary: An Animation Library
 for Explanitory Computer Science Videos Home-page: https://github.com/
 CadenScharpf/manim-cs Author: Caden Scharpf Author-email:
 caden.scharpf@icloud.com Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `manimcs-0.2/manimcs.egg-info/SOURCES.txt` & `manimcs-0.3/manimcs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manimcs-0.2/setup.py` & `manimcs-0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='manimcs',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     install_requires=[
         'manim==0.17.3',
         # Add any other dependencies here
     ],
     author='Caden Scharpf',
     author_email='caden.scharpf@icloud.com',
```

### Comparing `manimcs-0.2/src/algorithms/array_sort.py` & `manimcs-0.3/src/algorithms/array_sort.py`

 * *Files identical despite different names*

### Comparing `manimcs-0.2/src/engine/engine.py` & `manimcs-0.3/src/engine/engine.py`

 * *Files identical despite different names*

### Comparing `manimcs-0.2/src/mobjs/sort_set.py` & `manimcs-0.3/src/mobjs/sort_set.py`

 * *Files identical despite different names*

### Comparing `manimcs-0.2/src/mobjs/sortable_mobject.py` & `manimcs-0.3/src/mobjs/sortable_mobject.py`

 * *Files identical despite different names*

