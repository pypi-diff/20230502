# Comparing `tmp/ImageStack SVG-0.2.6.tar.gz` & `tmp/ImageStack SVG-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImageStack SVG-0.2.6.tar", last modified: Tue Apr 19 09:55:18 2022, max compression
+gzip compressed data, was "ImageStack SVG-1.0.0.tar", last modified: Tue May  2 12:23:04 2023, max compression
```

## Comparing `ImageStack SVG-0.2.6.tar` & `ImageStack SVG-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 09:55:18.745895 ImageStack SVG-0.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 09:55:18.741895 ImageStack SVG-0.2.6/ImageStack_SVG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-04-19 09:55:18.000000 ImageStack SVG-0.2.6/ImageStack_SVG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-04-19 09:55:18.000000 ImageStack SVG-0.2.6/ImageStack_SVG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-19 09:55:18.000000 ImageStack SVG-0.2.6/ImageStack_SVG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-19 09:55:18.000000 ImageStack SVG-0.2.6/ImageStack_SVG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-19 09:55:18.000000 ImageStack SVG-0.2.6/ImageStack_SVG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-04-19 09:55:00.000000 ImageStack SVG-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-04-19 09:55:18.745895 ImageStack SVG-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-04-19 09:55:00.000000 ImageStack SVG-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 09:55:18.745895 ImageStack SVG-0.2.6/imagestack_svg/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-19 09:55:00.000000 ImageStack SVG-0.2.6/imagestack_svg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-04-19 09:55:00.000000 ImageStack SVG-0.2.6/imagestack_svg/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3591 2022-04-19 09:55:00.000000 ImageStack SVG-0.2.6/imagestack_svg/imagecreator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-04-19 09:55:00.000000 ImageStack SVG-0.2.6/imagestack_svg/imageresolve.py
--rw-r--r--   0 runner    (1001) docker     (121)     3206 2022-04-19 09:55:00.000000 ImageStack SVG-0.2.6/imagestack_svg/imagestack.py
--rw-r--r--   0 runner    (1001) docker     (121)     4945 2022-04-19 09:55:00.000000 ImageStack SVG-0.2.6/imagestack_svg/loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-19 09:55:18.745895 ImageStack SVG-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-04-19 09:55:17.000000 ImageStack SVG-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:23:04.960415 ImageStack SVG-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:23:04.960415 ImageStack SVG-1.0.0/ImageStack_SVG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-02 12:23:04.000000 ImageStack SVG-1.0.0/ImageStack_SVG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-02 12:23:04.000000 ImageStack SVG-1.0.0/ImageStack_SVG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:23:04.000000 ImageStack SVG-1.0.0/ImageStack_SVG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 12:23:04.000000 ImageStack SVG-1.0.0/ImageStack_SVG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 12:23:04.000000 ImageStack SVG-1.0.0/ImageStack_SVG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-02 12:22:43.000000 ImageStack SVG-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-02 12:23:04.960415 ImageStack SVG-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-02 12:22:43.000000 ImageStack SVG-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:23:04.960415 ImageStack SVG-1.0.0/imagestack_svg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:22:43.000000 ImageStack SVG-1.0.0/imagestack_svg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-02 12:22:43.000000 ImageStack SVG-1.0.0/imagestack_svg/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-02 12:22:43.000000 ImageStack SVG-1.0.0/imagestack_svg/imagecreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-02 12:22:43.000000 ImageStack SVG-1.0.0/imagestack_svg/imageresolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-02 12:22:43.000000 ImageStack SVG-1.0.0/imagestack_svg/imagestack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-02 12:22:43.000000 ImageStack SVG-1.0.0/imagestack_svg/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:23:04.960415 ImageStack SVG-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-02 12:23:02.000000 ImageStack SVG-1.0.0/setup.py
```

### Comparing `ImageStack SVG-0.2.6/ImageStack_SVG.egg-info/PKG-INFO` & `ImageStack SVG-1.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,33 @@
-Metadata-Version: 2.1
-Name: ImageStack-SVG
-Version: 0.2.6
-Summary: Create Images by Stacking them
-Home-page: https://github.com/skillor/imagestack-svg-python
-Author: skillor
-Author-email: skillor@gmx.net
-License: MIT
-Keywords: image,imagestack,imagestack-svg,imagestack_svg,svg
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Multimedia :: Graphics
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# ImageStack Python
 
-# - ImageStack Python -
-
-### A simple way to create images
+### A simple way to create images using svg and jinja2 templating
 
 [![Build Status](https://github.com/skillor/imagestack-svg-python/actions/workflows/test-python.yml/badge.svg)](https://github.com/skillor/imagestack-svg-python/actions/workflows/test-python.yml) [![PyPi version](https://badgen.net/pypi/v/ImageStack-SVG/)](https://pypi.org/project/ImageStack-SVG)
 
-for terminal users you need to ```xvfb-run python3 {your application}```
+## Installation
+
+### Install with pip
+
+    pip install imagestack-svg
+
+### Running without display
+
+    xvfb-run python3 {your application}
+    
+## Test Design
+
+You can test your SVG Design here: https://skillor.github.io/imagestack-svg-python/
+
+## Usage
+
+    from imagestack_svg.imagecreator import ImageCreator
+    from imagestack_svg.imageresolve import ImageStackResolveString
+    ig = ImageCreator()
+    s = ImageStackResolveString('<text>{{ dummy }}</text>')
+    s(dummy='Hello World!')
+    print(await ig.create_inner_svg(s))
+    with open('test.png', 'wb') as f:
+        f.write((await ig.create_bytes(s)).read())
 
 
+more examples here: https://github.com/skillor/imagestack-svg-python/blob/master/test.py
```

### Comparing `ImageStack SVG-0.2.6/LICENSE` & `ImageStack SVG-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ImageStack SVG-0.2.6/imagestack_svg/helpers.py` & `ImageStack SVG-1.0.0/imagestack_svg/helpers.py`

 * *Files identical despite different names*

### Comparing `ImageStack SVG-0.2.6/imagestack_svg/imagecreator.py` & `ImageStack SVG-1.0.0/imagestack_svg/imagecreator.py`

 * *Files identical despite different names*

### Comparing `ImageStack SVG-0.2.6/imagestack_svg/imageresolve.py` & `ImageStack SVG-1.0.0/imagestack_svg/imageresolve.py`

 * *Files identical despite different names*

### Comparing `ImageStack SVG-0.2.6/imagestack_svg/imagestack.py` & `ImageStack SVG-1.0.0/imagestack_svg/imagestack.py`

 * *Files identical despite different names*

### Comparing `ImageStack SVG-0.2.6/imagestack_svg/loaders.py` & `ImageStack SVG-1.0.0/imagestack_svg/loaders.py`

 * *Files identical despite different names*

### Comparing `ImageStack SVG-0.2.6/setup.py` & `ImageStack SVG-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = [x for x in fh.read().splitlines() if x]
 
 setup(name='ImageStack SVG',
       packages=['imagestack_svg'],
-      version='0.2.6',
+      version='1.0.0',
       description='Create Images by Stacking them',
       author='skillor',
       author_email='skillor@gmx.net',
       long_description=long_description,
       long_description_content_type="text/markdown",
       license='MIT',
       url='https://github.com/skillor/imagestack-svg-python',
```

