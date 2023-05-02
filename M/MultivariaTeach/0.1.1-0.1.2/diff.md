# Comparing `tmp/MultivariaTeach-0.1.1.tar.gz` & `tmp/MultivariaTeach-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MultivariaTeach-0.1.1.tar", last modified: Tue May  2 20:37:58 2023, max compression
+gzip compressed data, was "MultivariaTeach-0.1.2.tar", last modified: Tue May  2 20:46:12 2023, max compression
```

## Comparing `MultivariaTeach-0.1.1.tar` & `MultivariaTeach-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 20:37:58.044016 MultivariaTeach-0.1.1/
--rw-------   0 ben        (501) staff       (20)      743 2023-04-25 22:03:04.000000 MultivariaTeach-0.1.1/LICENSE
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 20:37:58.043212 MultivariaTeach-0.1.1/MultivariaTeach.egg-info/
--rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 20:37:58.000000 MultivariaTeach-0.1.1/MultivariaTeach.egg-info/PKG-INFO
--rw-------   0 ben        (501) staff       (20)      267 2023-05-02 20:37:58.000000 MultivariaTeach-0.1.1/MultivariaTeach.egg-info/SOURCES.txt
--rw-------   0 ben        (501) staff       (20)        1 2023-05-02 20:37:58.000000 MultivariaTeach-0.1.1/MultivariaTeach.egg-info/dependency_links.txt
--rw-------   0 ben        (501) staff       (20)       41 2023-05-02 20:37:58.000000 MultivariaTeach-0.1.1/MultivariaTeach.egg-info/requires.txt
--rw-------   0 ben        (501) staff       (20)        6 2023-05-02 20:37:58.000000 MultivariaTeach-0.1.1/MultivariaTeach.egg-info/top_level.txt
--rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 20:37:58.043708 MultivariaTeach-0.1.1/PKG-INFO
--rw-------   0 ben        (501) staff       (20)    14698 2023-05-02 00:18:49.000000 MultivariaTeach-0.1.1/README.md
--rw-------   0 ben        (501) staff       (20)       38 2023-05-02 20:37:58.044055 MultivariaTeach-0.1.1/setup.cfg
--rw-------   0 ben        (501) staff       (20)      932 2023-05-02 20:35:08.000000 MultivariaTeach-0.1.1/setup.py
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 20:37:58.043422 MultivariaTeach-0.1.1/tests/
--rw-------   0 ben        (501) staff       (20)        0 2023-04-25 22:05:08.000000 MultivariaTeach-0.1.1/tests/__init__.py
--rw-------   0 ben        (501) staff       (20)     7016 2023-05-01 22:22:43.000000 MultivariaTeach-0.1.1/tests/test_multivariteach.py
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 20:46:12.875620 MultivariaTeach-0.1.2/
+-rw-------   0 ben        (501) staff       (20)      743 2023-04-25 22:03:04.000000 MultivariaTeach-0.1.2/LICENSE
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 20:46:12.874508 MultivariaTeach-0.1.2/MultivariaTeach.egg-info/
+-rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 20:46:12.000000 MultivariaTeach-0.1.2/MultivariaTeach.egg-info/PKG-INFO
+-rw-------   0 ben        (501) staff       (20)      267 2023-05-02 20:46:12.000000 MultivariaTeach-0.1.2/MultivariaTeach.egg-info/SOURCES.txt
+-rw-------   0 ben        (501) staff       (20)        1 2023-05-02 20:46:12.000000 MultivariaTeach-0.1.2/MultivariaTeach.egg-info/dependency_links.txt
+-rw-------   0 ben        (501) staff       (20)       41 2023-05-02 20:46:12.000000 MultivariaTeach-0.1.2/MultivariaTeach.egg-info/requires.txt
+-rw-------   0 ben        (501) staff       (20)        6 2023-05-02 20:46:12.000000 MultivariaTeach-0.1.2/MultivariaTeach.egg-info/top_level.txt
+-rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 20:46:12.875364 MultivariaTeach-0.1.2/PKG-INFO
+-rw-------   0 ben        (501) staff       (20)    14698 2023-05-02 00:18:49.000000 MultivariaTeach-0.1.2/README.md
+-rw-------   0 ben        (501) staff       (20)       38 2023-05-02 20:46:12.875660 MultivariaTeach-0.1.2/setup.cfg
+-rw-------   0 ben        (501) staff       (20)      932 2023-05-02 20:45:28.000000 MultivariaTeach-0.1.2/setup.py
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 20:46:12.874853 MultivariaTeach-0.1.2/tests/
+-rw-------   0 ben        (501) staff       (20)        0 2023-04-25 22:05:08.000000 MultivariaTeach-0.1.2/tests/__init__.py
+-rw-------   0 ben        (501) staff       (20)     7016 2023-05-01 22:22:43.000000 MultivariaTeach-0.1.2/tests/test_multivariteach.py
```

### Comparing `MultivariaTeach-0.1.1/LICENSE` & `MultivariaTeach-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MultivariaTeach-0.1.1/MultivariaTeach.egg-info/PKG-INFO` & `MultivariaTeach-0.1.2/MultivariaTeach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultivariaTeach
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of tools intended for students of multivariate analysis
 Home-page: https://github.com/Ben-Goren/MultivariaTeach
 Author: Ben Goren
 Author-email: bgoren@asu.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `MultivariaTeach-0.1.1/PKG-INFO` & `MultivariaTeach-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultivariaTeach
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of tools intended for students of multivariate analysis
 Home-page: https://github.com/Ben-Goren/MultivariaTeach
 Author: Ben Goren
 Author-email: bgoren@asu.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `MultivariaTeach-0.1.1/README.md` & `MultivariaTeach-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `MultivariaTeach-0.1.1/setup.py` & `MultivariaTeach-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MultivariaTeach",
-    version="0.1.1",
+    version="0.1.2",
     description="A collection of tools intended for students of multivariate analysis",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Ben Goren",
     author_email="bgoren@asu.edu",
     url="https://github.com/Ben-Goren/MultivariaTeach",
     packages=find_packages(),
```

### Comparing `MultivariaTeach-0.1.1/tests/test_multivariteach.py` & `MultivariaTeach-0.1.2/tests/test_multivariteach.py`

 * *Files identical despite different names*

