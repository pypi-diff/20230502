# Comparing `tmp/MultivariaTeach-0.1.4.tar.gz` & `tmp/MultivariaTeach-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MultivariaTeach-0.1.4.tar", last modified: Tue May  2 21:14:27 2023, max compression
+gzip compressed data, was "MultivariaTeach-0.1.5.tar", last modified: Tue May  2 21:22:32 2023, max compression
```

## Comparing `MultivariaTeach-0.1.4.tar` & `MultivariaTeach-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:14:27.796776 MultivariaTeach-0.1.4/
--rw-------   0 ben        (501) staff       (20)      743 2023-04-25 22:03:04.000000 MultivariaTeach-0.1.4/LICENSE
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:14:27.795134 MultivariaTeach-0.1.4/MultivariaTeach.egg-info/
--rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 21:14:27.000000 MultivariaTeach-0.1.4/MultivariaTeach.egg-info/PKG-INFO
--rw-------   0 ben        (501) staff       (20)      330 2023-05-02 21:14:27.000000 MultivariaTeach-0.1.4/MultivariaTeach.egg-info/SOURCES.txt
--rw-------   0 ben        (501) staff       (20)        1 2023-05-02 21:14:27.000000 MultivariaTeach-0.1.4/MultivariaTeach.egg-info/dependency_links.txt
--rw-------   0 ben        (501) staff       (20)       41 2023-05-02 21:14:27.000000 MultivariaTeach-0.1.4/MultivariaTeach.egg-info/requires.txt
--rw-------   0 ben        (501) staff       (20)       22 2023-05-02 21:14:27.000000 MultivariaTeach-0.1.4/MultivariaTeach.egg-info/top_level.txt
--rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 21:14:27.796475 MultivariaTeach-0.1.4/PKG-INFO
--rw-------   0 ben        (501) staff       (20)    14698 2023-05-02 00:18:49.000000 MultivariaTeach-0.1.4/README.md
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:14:27.795542 MultivariaTeach-0.1.4/multivariateach/
--rw-------   0 ben        (501) staff       (20)       31 2023-05-02 20:33:56.000000 MultivariaTeach-0.1.4/multivariateach/__init__.py
--rw-------   0 ben        (501) staff       (20)    11161 2023-05-01 19:52:12.000000 MultivariaTeach-0.1.4/multivariateach/multivariateach.py
--rw-------   0 ben        (501) staff       (20)       38 2023-05-02 21:14:27.796841 MultivariaTeach-0.1.4/setup.cfg
--rw-------   0 ben        (501) staff       (20)      932 2023-05-02 21:13:48.000000 MultivariaTeach-0.1.4/setup.py
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:14:27.795932 MultivariaTeach-0.1.4/tests/
--rw-------   0 ben        (501) staff       (20)        0 2023-04-25 22:05:08.000000 MultivariaTeach-0.1.4/tests/__init__.py
--rw-------   0 ben        (501) staff       (20)     7016 2023-05-01 22:22:43.000000 MultivariaTeach-0.1.4/tests/test_multivariteach.py
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:22:32.421158 MultivariaTeach-0.1.5/
+-rw-------   0 ben        (501) staff       (20)      743 2023-04-25 22:03:04.000000 MultivariaTeach-0.1.5/LICENSE
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:22:32.419844 MultivariaTeach-0.1.5/MultivariaTeach.egg-info/
+-rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 21:22:32.000000 MultivariaTeach-0.1.5/MultivariaTeach.egg-info/PKG-INFO
+-rw-------   0 ben        (501) staff       (20)      330 2023-05-02 21:22:32.000000 MultivariaTeach-0.1.5/MultivariaTeach.egg-info/SOURCES.txt
+-rw-------   0 ben        (501) staff       (20)        1 2023-05-02 21:22:32.000000 MultivariaTeach-0.1.5/MultivariaTeach.egg-info/dependency_links.txt
+-rw-------   0 ben        (501) staff       (20)       41 2023-05-02 21:22:32.000000 MultivariaTeach-0.1.5/MultivariaTeach.egg-info/requires.txt
+-rw-------   0 ben        (501) staff       (20)       22 2023-05-02 21:22:32.000000 MultivariaTeach-0.1.5/MultivariaTeach.egg-info/top_level.txt
+-rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 21:22:32.421013 MultivariaTeach-0.1.5/PKG-INFO
+-rw-------   0 ben        (501) staff       (20)    14698 2023-05-02 21:22:03.000000 MultivariaTeach-0.1.5/README.md
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:22:32.420164 MultivariaTeach-0.1.5/multivariateach/
+-rw-------   0 ben        (501) staff       (20)       31 2023-05-02 20:33:56.000000 MultivariaTeach-0.1.5/multivariateach/__init__.py
+-rw-------   0 ben        (501) staff       (20)    11161 2023-05-01 19:52:12.000000 MultivariaTeach-0.1.5/multivariateach/multivariateach.py
+-rw-------   0 ben        (501) staff       (20)       38 2023-05-02 21:22:32.421193 MultivariaTeach-0.1.5/setup.cfg
+-rw-------   0 ben        (501) staff       (20)      932 2023-05-02 21:22:26.000000 MultivariaTeach-0.1.5/setup.py
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:22:32.420628 MultivariaTeach-0.1.5/tests/
+-rw-------   0 ben        (501) staff       (20)        0 2023-04-25 22:05:08.000000 MultivariaTeach-0.1.5/tests/__init__.py
+-rw-------   0 ben        (501) staff       (20)     7016 2023-05-01 22:22:43.000000 MultivariaTeach-0.1.5/tests/test_multivariteach.py
```

### Comparing `MultivariaTeach-0.1.4/LICENSE` & `MultivariaTeach-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MultivariaTeach-0.1.4/MultivariaTeach.egg-info/PKG-INFO` & `MultivariaTeach-0.1.5/MultivariaTeach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultivariaTeach
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of tools intended for students of multivariate analysis
 Home-page: https://github.com/Ben-Goren/MultivariaTeach
 Author: Ben Goren
 Author-email: bgoren@asu.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: ISC License (ISCL)
@@ -81,15 +81,15 @@
 Finally, $\mathbf{H} = \mathbf{M}^\intercal \mathbf{B} \mathbf{M}$. The $\mathbf{E}$ and $\mathbf{H}$ matrices are then used to calculate the test statistics.
 
 While you are welcome to construct all four matrices by hand, MultivariaTeach provides tools to help construct them.
 
 First, as usual, make sure you load the package at the top of your Python file:
 
 ```python
-import MultivariaTeach as mt
+import multivariateach as mt
 ```
 
 This would typically be included with the lines above importing `pandas` and `sklearn`. We can now create our $\mathbf{X}$ and $\mathbf{Y}$ matrices:
 
 ```python
 X = mt.create_design_matrix(data, 'group')
 Y = mt.create_response_matrix(data, ['x1', 'x2', 'x3', 'x4'])
```

### Comparing `MultivariaTeach-0.1.4/PKG-INFO` & `MultivariaTeach-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultivariaTeach
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of tools intended for students of multivariate analysis
 Home-page: https://github.com/Ben-Goren/MultivariaTeach
 Author: Ben Goren
 Author-email: bgoren@asu.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: ISC License (ISCL)
@@ -81,15 +81,15 @@
 Finally, $\mathbf{H} = \mathbf{M}^\intercal \mathbf{B} \mathbf{M}$. The $\mathbf{E}$ and $\mathbf{H}$ matrices are then used to calculate the test statistics.
 
 While you are welcome to construct all four matrices by hand, MultivariaTeach provides tools to help construct them.
 
 First, as usual, make sure you load the package at the top of your Python file:
 
 ```python
-import MultivariaTeach as mt
+import multivariateach as mt
 ```
 
 This would typically be included with the lines above importing `pandas` and `sklearn`. We can now create our $\mathbf{X}$ and $\mathbf{Y}$ matrices:
 
 ```python
 X = mt.create_design_matrix(data, 'group')
 Y = mt.create_response_matrix(data, ['x1', 'x2', 'x3', 'x4'])
```

### Comparing `MultivariaTeach-0.1.4/README.md` & `MultivariaTeach-0.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 Finally, $\mathbf{H} = \mathbf{M}^\intercal \mathbf{B} \mathbf{M}$. The $\mathbf{E}$ and $\mathbf{H}$ matrices are then used to calculate the test statistics.
 
 While you are welcome to construct all four matrices by hand, MultivariaTeach provides tools to help construct them.
 
 First, as usual, make sure you load the package at the top of your Python file:
 
 ```python
-import MultivariaTeach as mt
+import multivariateach as mt
 ```
 
 This would typically be included with the lines above importing `pandas` and `sklearn`. We can now create our $\mathbf{X}$ and $\mathbf{Y}$ matrices:
 
 ```python
 X = mt.create_design_matrix(data, 'group')
 Y = mt.create_response_matrix(data, ['x1', 'x2', 'x3', 'x4'])
```

### Comparing `MultivariaTeach-0.1.4/multivariateach/multivariateach.py` & `MultivariaTeach-0.1.5/multivariateach/multivariateach.py`

 * *Files identical despite different names*

### Comparing `MultivariaTeach-0.1.4/setup.py` & `MultivariaTeach-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MultivariaTeach",
-    version="0.1.4",
+    version="0.1.5",
     description="A collection of tools intended for students of multivariate analysis",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Ben Goren",
     author_email="bgoren@asu.edu",
     url="https://github.com/Ben-Goren/MultivariaTeach",
     packages=find_packages(),
```

### Comparing `MultivariaTeach-0.1.4/tests/test_multivariteach.py` & `MultivariaTeach-0.1.5/tests/test_multivariteach.py`

 * *Files identical despite different names*

