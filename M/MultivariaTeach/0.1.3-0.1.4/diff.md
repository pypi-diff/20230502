# Comparing `tmp/MultivariaTeach-0.1.3.tar.gz` & `tmp/MultivariaTeach-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MultivariaTeach-0.1.3.tar", last modified: Tue May  2 20:56:48 2023, max compression
+gzip compressed data, was "MultivariaTeach-0.1.4.tar", last modified: Tue May  2 21:14:27 2023, max compression
```

## Comparing `MultivariaTeach-0.1.3.tar` & `MultivariaTeach-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 20:56:48.396335 MultivariaTeach-0.1.3/
--rw-------   0 ben        (501) staff       (20)      743 2023-04-25 22:03:04.000000 MultivariaTeach-0.1.3/LICENSE
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 20:56:48.395394 MultivariaTeach-0.1.3/MultivariaTeach.egg-info/
--rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 20:56:48.000000 MultivariaTeach-0.1.3/MultivariaTeach.egg-info/PKG-INFO
--rw-------   0 ben        (501) staff       (20)      267 2023-05-02 20:56:48.000000 MultivariaTeach-0.1.3/MultivariaTeach.egg-info/SOURCES.txt
--rw-------   0 ben        (501) staff       (20)        1 2023-05-02 20:56:48.000000 MultivariaTeach-0.1.3/MultivariaTeach.egg-info/dependency_links.txt
--rw-------   0 ben        (501) staff       (20)       41 2023-05-02 20:56:48.000000 MultivariaTeach-0.1.3/MultivariaTeach.egg-info/requires.txt
--rw-------   0 ben        (501) staff       (20)        6 2023-05-02 20:56:48.000000 MultivariaTeach-0.1.3/MultivariaTeach.egg-info/top_level.txt
--rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 20:56:48.396061 MultivariaTeach-0.1.3/PKG-INFO
--rw-------   0 ben        (501) staff       (20)    14698 2023-05-02 00:18:49.000000 MultivariaTeach-0.1.3/README.md
--rw-------   0 ben        (501) staff       (20)       38 2023-05-02 20:56:48.396368 MultivariaTeach-0.1.3/setup.cfg
--rw-------   0 ben        (501) staff       (20)      932 2023-05-02 20:56:38.000000 MultivariaTeach-0.1.3/setup.py
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 20:56:48.395607 MultivariaTeach-0.1.3/tests/
--rw-------   0 ben        (501) staff       (20)        0 2023-04-25 22:05:08.000000 MultivariaTeach-0.1.3/tests/__init__.py
--rw-------   0 ben        (501) staff       (20)     7016 2023-05-01 22:22:43.000000 MultivariaTeach-0.1.3/tests/test_multivariteach.py
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:14:27.796776 MultivariaTeach-0.1.4/
+-rw-------   0 ben        (501) staff       (20)      743 2023-04-25 22:03:04.000000 MultivariaTeach-0.1.4/LICENSE
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:14:27.795134 MultivariaTeach-0.1.4/MultivariaTeach.egg-info/
+-rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 21:14:27.000000 MultivariaTeach-0.1.4/MultivariaTeach.egg-info/PKG-INFO
+-rw-------   0 ben        (501) staff       (20)      330 2023-05-02 21:14:27.000000 MultivariaTeach-0.1.4/MultivariaTeach.egg-info/SOURCES.txt
+-rw-------   0 ben        (501) staff       (20)        1 2023-05-02 21:14:27.000000 MultivariaTeach-0.1.4/MultivariaTeach.egg-info/dependency_links.txt
+-rw-------   0 ben        (501) staff       (20)       41 2023-05-02 21:14:27.000000 MultivariaTeach-0.1.4/MultivariaTeach.egg-info/requires.txt
+-rw-------   0 ben        (501) staff       (20)       22 2023-05-02 21:14:27.000000 MultivariaTeach-0.1.4/MultivariaTeach.egg-info/top_level.txt
+-rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 21:14:27.796475 MultivariaTeach-0.1.4/PKG-INFO
+-rw-------   0 ben        (501) staff       (20)    14698 2023-05-02 00:18:49.000000 MultivariaTeach-0.1.4/README.md
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:14:27.795542 MultivariaTeach-0.1.4/multivariateach/
+-rw-------   0 ben        (501) staff       (20)       31 2023-05-02 20:33:56.000000 MultivariaTeach-0.1.4/multivariateach/__init__.py
+-rw-------   0 ben        (501) staff       (20)    11161 2023-05-01 19:52:12.000000 MultivariaTeach-0.1.4/multivariateach/multivariateach.py
+-rw-------   0 ben        (501) staff       (20)       38 2023-05-02 21:14:27.796841 MultivariaTeach-0.1.4/setup.cfg
+-rw-------   0 ben        (501) staff       (20)      932 2023-05-02 21:13:48.000000 MultivariaTeach-0.1.4/setup.py
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:14:27.795932 MultivariaTeach-0.1.4/tests/
+-rw-------   0 ben        (501) staff       (20)        0 2023-04-25 22:05:08.000000 MultivariaTeach-0.1.4/tests/__init__.py
+-rw-------   0 ben        (501) staff       (20)     7016 2023-05-01 22:22:43.000000 MultivariaTeach-0.1.4/tests/test_multivariteach.py
```

### Comparing `MultivariaTeach-0.1.3/LICENSE` & `MultivariaTeach-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MultivariaTeach-0.1.3/MultivariaTeach.egg-info/PKG-INFO` & `MultivariaTeach-0.1.4/MultivariaTeach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultivariaTeach
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of tools intended for students of multivariate analysis
 Home-page: https://github.com/Ben-Goren/MultivariaTeach
 Author: Ben Goren
 Author-email: bgoren@asu.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `MultivariaTeach-0.1.3/PKG-INFO` & `MultivariaTeach-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultivariaTeach
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of tools intended for students of multivariate analysis
 Home-page: https://github.com/Ben-Goren/MultivariaTeach
 Author: Ben Goren
 Author-email: bgoren@asu.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `MultivariaTeach-0.1.3/README.md` & `MultivariaTeach-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `MultivariaTeach-0.1.3/setup.py` & `MultivariaTeach-0.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MultivariaTeach",
-    version="0.1.3",
+    version="0.1.4",
     description="A collection of tools intended for students of multivariate analysis",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Ben Goren",
     author_email="bgoren@asu.edu",
     url="https://github.com/Ben-Goren/MultivariaTeach",
     packages=find_packages(),
```

### Comparing `MultivariaTeach-0.1.3/tests/test_multivariteach.py` & `MultivariaTeach-0.1.4/tests/test_multivariteach.py`

 * *Files identical despite different names*

