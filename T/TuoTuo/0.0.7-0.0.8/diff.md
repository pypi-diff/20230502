# Comparing `tmp/TuoTuo-0.0.7.tar.gz` & `tmp/TuoTuo-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TuoTuo-0.0.7.tar", last modified: Tue May  2 12:13:36 2023, max compression
+gzip compressed data, was "TuoTuo-0.0.8.tar", last modified: Tue May  2 12:17:03 2023, max compression
```

## Comparing `TuoTuo-0.0.7.tar` & `TuoTuo-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:13:36.343191 TuoTuo-0.0.7/
--rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.0.7/.DS_Store
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:13:36.328744 TuoTuo-0.0.7/.github/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:13:36.332649 TuoTuo-0.0.7/.github/workflows/
--rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.0.7/.github/workflows/python-package.yml
--rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.0.7/.gitignore
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:13:36.333050 TuoTuo-0.0.7/.vscode/
--rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.0.7/.vscode/c_cpp_properties.json
--rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.0.7/LICENSE
--rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 12:13:36.343326 TuoTuo-0.0.7/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.0.7/README.md
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:13:36.333953 TuoTuo-0.0.7/TuoTuo.egg-info/
--rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 12:13:36.000000 TuoTuo-0.0.7/TuoTuo.egg-info/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      866 2023-05-02 12:13:36.000000 TuoTuo-0.0.7/TuoTuo.egg-info/SOURCES.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-02 12:13:36.000000 TuoTuo-0.0.7/TuoTuo.egg-info/dependency_links.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       32 2023-05-02 12:13:36.000000 TuoTuo-0.0.7/TuoTuo.egg-info/requires.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        7 2023-05-02 12:13:36.000000 TuoTuo-0.0.7/TuoTuo.egg-info/top_level.txt
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 TuoTuo-0.0.7/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:13:36.334749 TuoTuo-0.0.7/notebook/
--rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.0.7/notebook/Our Model vs SKLearn.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.0.7/notebook/__init__.py
--rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.0.7/requirements.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-02 12:13:36.343593 TuoTuo-0.0.7/setup.cfg
--rw-r--r--   0 ericliu    (501) staff       (20)     1384 2023-05-02 12:13:26.000000 TuoTuo-0.0.7/setup.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:13:36.338759 TuoTuo-0.0.7/tuotuo/
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.0.7/tuotuo/__init__.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:13:36.329242 TuoTuo-0.0.7/tuotuo/build/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:13:36.339178 TuoTuo-0.0.7/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.0.7/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:13:36.340470 TuoTuo-0.0.7/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
--rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.0.7/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
--rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.0.7/tuotuo/cutils.c
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.0.7/tuotuo/cutils.cpython-38-darwin.so
--rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.0.7/tuotuo/cutils.pyx
--rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.0.7/tuotuo/generator.py
--rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.0.7/tuotuo/lda_model.py
--rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.0.7/tuotuo/text_pre_processor.py
--rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.0.7/tuotuo/utils.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:17:03.717971 TuoTuo-0.0.8/
+-rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.0.8/.DS_Store
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:17:03.704702 TuoTuo-0.0.8/.github/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:17:03.708373 TuoTuo-0.0.8/.github/workflows/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.0.8/.github/workflows/python-package.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.0.8/.gitignore
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:17:03.708624 TuoTuo-0.0.8/.vscode/
+-rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.0.8/.vscode/c_cpp_properties.json
+-rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.0.8/LICENSE
+-rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 12:17:03.718086 TuoTuo-0.0.8/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.0.8/README.md
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:17:03.709574 TuoTuo-0.0.8/TuoTuo.egg-info/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 12:17:03.000000 TuoTuo-0.0.8/TuoTuo.egg-info/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      866 2023-05-02 12:17:03.000000 TuoTuo-0.0.8/TuoTuo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-02 12:17:03.000000 TuoTuo-0.0.8/TuoTuo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       32 2023-05-02 12:17:03.000000 TuoTuo-0.0.8/TuoTuo.egg-info/requires.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        7 2023-05-02 12:17:03.000000 TuoTuo-0.0.8/TuoTuo.egg-info/top_level.txt
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 TuoTuo-0.0.8/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:17:03.710271 TuoTuo-0.0.8/notebook/
+-rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.0.8/notebook/Our Model vs SKLearn.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.0.8/notebook/__init__.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.0.8/requirements.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-02 12:17:03.718382 TuoTuo-0.0.8/setup.cfg
+-rw-r--r--   0 ericliu    (501) staff       (20)     1343 2023-05-02 12:16:59.000000 TuoTuo-0.0.8/setup.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:17:03.713684 TuoTuo-0.0.8/tuotuo/
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.0.8/tuotuo/__init__.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:17:03.705180 TuoTuo-0.0.8/tuotuo/build/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:17:03.714141 TuoTuo-0.0.8/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.0.8/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:17:03.715443 TuoTuo-0.0.8/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
+-rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.0.8/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
+-rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.0.8/tuotuo/cutils.c
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.0.8/tuotuo/cutils.cpython-38-darwin.so
+-rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.0.8/tuotuo/cutils.pyx
+-rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.0.8/tuotuo/generator.py
+-rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.0.8/tuotuo/lda_model.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.0.8/tuotuo/text_pre_processor.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.0.8/tuotuo/utils.py
```

### Comparing `TuoTuo-0.0.7/.DS_Store` & `TuoTuo-0.0.8/.DS_Store`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/.github/workflows/python-package.yml` & `TuoTuo-0.0.8/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/.github/workflows/python-publish.yml` & `TuoTuo-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/.vscode/c_cpp_properties.json` & `TuoTuo-0.0.8/.vscode/c_cpp_properties.json`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/LICENSE` & `TuoTuo-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/PKG-INFO` & `TuoTuo-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.0.7
+Version: 0.0.8
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
 Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.0.5.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
```

### Comparing `TuoTuo-0.0.7/README.md` & `TuoTuo-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/TuoTuo.egg-info/PKG-INFO` & `TuoTuo-0.0.8/TuoTuo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.0.7
+Version: 0.0.8
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
 Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.0.5.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
```

### Comparing `TuoTuo-0.0.7/TuoTuo.egg-info/SOURCES.txt` & `TuoTuo-0.0.8/TuoTuo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/cutils.cpython-38-darwin.so` & `TuoTuo-0.0.8/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/notebook/Our Model vs SKLearn.ipynb` & `TuoTuo-0.0.8/notebook/Our Model vs SKLearn.ipynb`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/requirements.txt` & `TuoTuo-0.0.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/setup.py` & `TuoTuo-0.0.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 # coding: utf-8
 import pkg_resources 
 from setuptools import Extension, setup
 from distutils.core import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 
-pkg_resources.require(['pip >= 23.1.2'])
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = 'TuoTuo',
     packages = ['tuotuo'],
-    version = '0.0.7',  
+    version = '0.0.8',  
     license='MIT',
     description = 'LDA & Neura based topic modelling library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'tuotuo Superman',
     author_email = 'tuotuo@HanwellSquare.BigForce.com',
     url = 'https://github.com/RobbenRibery/TuoTuo',
```

### Comparing `TuoTuo-0.0.7/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so` & `TuoTuo-0.0.8/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o` & `TuoTuo-0.0.8/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/tuotuo/cutils.c` & `TuoTuo-0.0.8/tuotuo/cutils.c`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/tuotuo/cutils.cpython-38-darwin.so` & `TuoTuo-0.0.8/tuotuo/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/tuotuo/cutils.pyx` & `TuoTuo-0.0.8/tuotuo/cutils.pyx`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/tuotuo/generator.py` & `TuoTuo-0.0.8/tuotuo/generator.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/tuotuo/lda_model.py` & `TuoTuo-0.0.8/tuotuo/lda_model.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/tuotuo/text_pre_processor.py` & `TuoTuo-0.0.8/tuotuo/text_pre_processor.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.7/tuotuo/utils.py` & `TuoTuo-0.0.8/tuotuo/utils.py`

 * *Files identical despite different names*

