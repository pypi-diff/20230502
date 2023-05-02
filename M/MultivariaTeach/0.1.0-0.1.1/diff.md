# Comparing `tmp/MultivariaTeach-0.1.0.tar.gz` & `tmp/MultivariaTeach-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MultivariaTeach-0.1.0.tar", last modified: Tue May  2 00:51:36 2023, max compression
+gzip compressed data, was "MultivariaTeach-0.1.1.tar", last modified: Tue May  2 20:37:58 2023, max compression
```

## Comparing `MultivariaTeach-0.1.0.tar` & `MultivariaTeach-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 00:51:36.832119 MultivariaTeach-0.1.0/
--rw-------   0 ben        (501) staff       (20)      743 2023-04-25 22:03:04.000000 MultivariaTeach-0.1.0/LICENSE
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 00:51:36.830675 MultivariaTeach-0.1.0/MultivariaTeach.egg-info/
--rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 00:51:36.000000 MultivariaTeach-0.1.0/MultivariaTeach.egg-info/PKG-INFO
--rw-------   0 ben        (501) staff       (20)      330 2023-05-02 00:51:36.000000 MultivariaTeach-0.1.0/MultivariaTeach.egg-info/SOURCES.txt
--rw-------   0 ben        (501) staff       (20)        1 2023-05-02 00:51:36.000000 MultivariaTeach-0.1.0/MultivariaTeach.egg-info/dependency_links.txt
--rw-------   0 ben        (501) staff       (20)       41 2023-05-02 00:51:36.000000 MultivariaTeach-0.1.0/MultivariaTeach.egg-info/requires.txt
--rw-------   0 ben        (501) staff       (20)       22 2023-05-02 00:51:36.000000 MultivariaTeach-0.1.0/MultivariaTeach.egg-info/top_level.txt
--rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 00:51:36.831719 MultivariaTeach-0.1.0/PKG-INFO
--rw-------   0 ben        (501) staff       (20)    14698 2023-05-02 00:18:49.000000 MultivariaTeach-0.1.0/README.md
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 00:51:36.830891 MultivariaTeach-0.1.0/multivariateach/
--rw-------   0 ben        (501) staff       (20)        0 2023-05-01 18:04:20.000000 MultivariaTeach-0.1.0/multivariateach/__init__.py
--rw-------   0 ben        (501) staff       (20)    11161 2023-05-01 19:52:12.000000 MultivariaTeach-0.1.0/multivariateach/multivariateach.py
--rw-------   0 ben        (501) staff       (20)       38 2023-05-02 00:51:36.832158 MultivariaTeach-0.1.0/setup.cfg
--rw-------   0 ben        (501) staff       (20)      932 2023-05-02 00:40:11.000000 MultivariaTeach-0.1.0/setup.py
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 00:51:36.831323 MultivariaTeach-0.1.0/tests/
--rw-------   0 ben        (501) staff       (20)        0 2023-04-25 22:05:08.000000 MultivariaTeach-0.1.0/tests/__init__.py
--rw-------   0 ben        (501) staff       (20)     7016 2023-05-01 22:22:43.000000 MultivariaTeach-0.1.0/tests/test_multivariteach.py
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 20:37:58.044016 MultivariaTeach-0.1.1/
+-rw-------   0 ben        (501) staff       (20)      743 2023-04-25 22:03:04.000000 MultivariaTeach-0.1.1/LICENSE
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 20:37:58.043212 MultivariaTeach-0.1.1/MultivariaTeach.egg-info/
+-rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 20:37:58.000000 MultivariaTeach-0.1.1/MultivariaTeach.egg-info/PKG-INFO
+-rw-------   0 ben        (501) staff       (20)      267 2023-05-02 20:37:58.000000 MultivariaTeach-0.1.1/MultivariaTeach.egg-info/SOURCES.txt
+-rw-------   0 ben        (501) staff       (20)        1 2023-05-02 20:37:58.000000 MultivariaTeach-0.1.1/MultivariaTeach.egg-info/dependency_links.txt
+-rw-------   0 ben        (501) staff       (20)       41 2023-05-02 20:37:58.000000 MultivariaTeach-0.1.1/MultivariaTeach.egg-info/requires.txt
+-rw-------   0 ben        (501) staff       (20)        6 2023-05-02 20:37:58.000000 MultivariaTeach-0.1.1/MultivariaTeach.egg-info/top_level.txt
+-rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 20:37:58.043708 MultivariaTeach-0.1.1/PKG-INFO
+-rw-------   0 ben        (501) staff       (20)    14698 2023-05-02 00:18:49.000000 MultivariaTeach-0.1.1/README.md
+-rw-------   0 ben        (501) staff       (20)       38 2023-05-02 20:37:58.044055 MultivariaTeach-0.1.1/setup.cfg
+-rw-------   0 ben        (501) staff       (20)      932 2023-05-02 20:35:08.000000 MultivariaTeach-0.1.1/setup.py
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 20:37:58.043422 MultivariaTeach-0.1.1/tests/
+-rw-------   0 ben        (501) staff       (20)        0 2023-04-25 22:05:08.000000 MultivariaTeach-0.1.1/tests/__init__.py
+-rw-------   0 ben        (501) staff       (20)     7016 2023-05-01 22:22:43.000000 MultivariaTeach-0.1.1/tests/test_multivariteach.py
```

### Comparing `MultivariaTeach-0.1.0/LICENSE` & `MultivariaTeach-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MultivariaTeach-0.1.0/MultivariaTeach.egg-info/PKG-INFO` & `MultivariaTeach-0.1.1/MultivariaTeach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultivariaTeach
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of tools intended for students of multivariate analysis
 Home-page: https://github.com/Ben-Goren/MultivariaTeach
 Author: Ben Goren
 Author-email: bgoren@asu.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `MultivariaTeach-0.1.0/PKG-INFO` & `MultivariaTeach-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultivariaTeach
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of tools intended for students of multivariate analysis
 Home-page: https://github.com/Ben-Goren/MultivariaTeach
 Author: Ben Goren
 Author-email: bgoren@asu.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `MultivariaTeach-0.1.0/README.md` & `MultivariaTeach-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `MultivariaTeach-0.1.0/setup.py` & `MultivariaTeach-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MultivariaTeach",
-    version="0.1.0",
+    version="0.1.1",
     description="A collection of tools intended for students of multivariate analysis",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Ben Goren",
     author_email="bgoren@asu.edu",
     url="https://github.com/Ben-Goren/MultivariaTeach",
     packages=find_packages(),
```

### Comparing `MultivariaTeach-0.1.0/tests/test_multivariteach.py` & `MultivariaTeach-0.1.1/tests/test_multivariteach.py`

 * *Files identical despite different names*

