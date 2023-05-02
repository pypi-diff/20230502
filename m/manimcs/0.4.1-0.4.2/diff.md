# Comparing `tmp/manimcs-0.4.1.tar.gz` & `tmp/manimcs-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manimcs-0.4.1.tar", last modified: Tue May  2 19:47:52 2023, max compression
+gzip compressed data, was "manimcs-0.4.2.tar", last modified: Tue May  2 19:53:17 2023, max compression
```

## Comparing `manimcs-0.4.1.tar` & `manimcs-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:47:52.538694 manimcs-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-02 19:47:52.538694 manimcs-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-02 19:47:41.000000 manimcs-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:47:52.538694 manimcs-0.4.1/manimcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-02 19:47:52.000000 manimcs-0.4.1/manimcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-02 19:47:52.000000 manimcs-0.4.1/manimcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:47:52.000000 manimcs-0.4.1/manimcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 19:47:52.000000 manimcs-0.4.1/manimcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:47:52.000000 manimcs-0.4.1/manimcs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 19:47:41.000000 manimcs-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:47:52.538694 manimcs-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-02 19:47:41.000000 manimcs-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:17.199329 manimcs-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-02 19:53:17.199329 manimcs-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-02 19:53:03.000000 manimcs-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:17.199329 manimcs-0.4.2/manimcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-02 19:53:17.000000 manimcs-0.4.2/manimcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-02 19:53:17.000000 manimcs-0.4.2/manimcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:53:17.000000 manimcs-0.4.2/manimcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 19:53:17.000000 manimcs-0.4.2/manimcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 19:53:17.000000 manimcs-0.4.2/manimcs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-02 19:53:03.000000 manimcs-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:53:17.199329 manimcs-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-02 19:53:03.000000 manimcs-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:17.199329 manimcs-0.4.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 19:53:03.000000 manimcs-0.4.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:17.199329 manimcs-0.4.2/src/manimcs/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 19:53:03.000000 manimcs-0.4.2/src/manimcs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:17.199329 manimcs-0.4.2/src/manimcs/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 19:53:03.000000 manimcs-0.4.2/src/manimcs/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-05-02 19:53:03.000000 manimcs-0.4.2/src/manimcs/algorithms/array_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:17.199329 manimcs-0.4.2/src/manimcs/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 19:53:03.000000 manimcs-0.4.2/src/manimcs/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-02 19:53:03.000000 manimcs-0.4.2/src/manimcs/engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:17.199329 manimcs-0.4.2/src/manimcs/mobjs/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 19:53:03.000000 manimcs-0.4.2/src/manimcs/mobjs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-02 19:53:03.000000 manimcs-0.4.2/src/manimcs/mobjs/sort_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-02 19:53:03.000000 manimcs-0.4.2/src/manimcs/mobjs/sortable_mobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-02 19:53:03.000000 manimcs-0.4.2/src/manimcs/mobjs/svg_mobject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:17.199329 manimcs-0.4.2/src/manimcs/renderer/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 19:53:03.000000 manimcs-0.4.2/src/manimcs/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 19:53:03.000000 manimcs-0.4.2/src/manimcs/renderer/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:53:17.199329 manimcs-0.4.2/src/manimcs/scene/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-02 19:53:03.000000 manimcs-0.4.2/src/manimcs/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 19:53:03.000000 manimcs-0.4.2/src/manimcs/scene/array_sort_scene.py
```

### Comparing `manimcs-0.4.1/PKG-INFO` & `manimcs-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manimcs
-Version: 0.4.1
+Version: 0.4.2
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
-Metadata-Version: 2.1 Name: manimcs Version: 0.4.1 Summary: An Animation
+Metadata-Version: 2.1 Name: manimcs Version: 0.4.2 Summary: An Animation
 Library for Explanitory Computer Science Videos Home-page: https://github.com/
 CadenScharpf/manim-cs Author: Caden Scharpf Author-email:
 caden.scharpf@icloud.com Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `manimcs-0.4.1/README.md` & `manimcs-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `manimcs-0.4.1/manimcs.egg-info/PKG-INFO` & `manimcs-0.4.2/manimcs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manimcs
-Version: 0.4.1
+Version: 0.4.2
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
-Metadata-Version: 2.1 Name: manimcs Version: 0.4.1 Summary: An Animation
+Metadata-Version: 2.1 Name: manimcs Version: 0.4.2 Summary: An Animation
 Library for Explanitory Computer Science Videos Home-page: https://github.com/
 CadenScharpf/manim-cs Author: Caden Scharpf Author-email:
 caden.scharpf@icloud.com Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `manimcs-0.4.1/setup.py` & `manimcs-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='manimcs',
-    version='0.4.1',
+    version='0.4.2',
     packages=find_packages(),
     install_requires=[
         'manim==0.17.3',
         # Add any other dependencies here
     ],
     author='Caden Scharpf',
     author_email='caden.scharpf@icloud.com',
```

