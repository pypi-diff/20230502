# Comparing `tmp/TuoTuo-0.1.3.tar.gz` & `tmp/TuoTuo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TuoTuo-0.1.3.tar", last modified: Tue May  2 13:09:02 2023, max compression
+gzip compressed data, was "TuoTuo-0.1.4.tar", last modified: Tue May  2 13:10:26 2023, max compression
```

## Comparing `TuoTuo-0.1.3.tar` & `TuoTuo-0.1.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:09:02.517346 TuoTuo-0.1.3/
--rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.1.3/.DS_Store
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:09:02.506558 TuoTuo-0.1.3/.github/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:09:02.510115 TuoTuo-0.1.3/.github/workflows/
--rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.1.3/.github/workflows/python-package.yml
--rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.1.3/.gitignore
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:09:02.510413 TuoTuo-0.1.3/.vscode/
--rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.1.3/.vscode/c_cpp_properties.json
--rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.1.3/LICENSE
--rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 13:09:02.517491 TuoTuo-0.1.3/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.1.3/README.md
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:09:02.511441 TuoTuo-0.1.3/TuoTuo.egg-info/
--rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 13:09:02.000000 TuoTuo-0.1.3/TuoTuo.egg-info/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      879 2023-05-02 13:09:02.000000 TuoTuo-0.1.3/TuoTuo.egg-info/SOURCES.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-02 13:09:02.000000 TuoTuo-0.1.3/TuoTuo.egg-info/dependency_links.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       45 2023-05-02 13:09:02.000000 TuoTuo-0.1.3/TuoTuo.egg-info/requires.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       21 2023-05-02 13:09:02.000000 TuoTuo-0.1.3/TuoTuo.egg-info/top_level.txt
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 TuoTuo-0.1.3/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:09:02.512107 TuoTuo-0.1.3/notebook/
--rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.1.3/notebook/Our Model vs SKLearn.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.1.3/notebook/__init__.py
--rw-r--r--   0 ericliu    (501) staff       (20)      123 2023-05-02 13:08:32.000000 TuoTuo-0.1.3/project.toml
--rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.1.3/requirements.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-02 13:09:02.517838 TuoTuo-0.1.3/setup.cfg
--rw-r--r--   0 ericliu    (501) staff       (20)     1683 2023-05-02 13:08:59.000000 TuoTuo-0.1.3/setup.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:09:02.514658 TuoTuo-0.1.3/tuotuo/
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.1.3/tuotuo/__init__.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:09:02.507065 TuoTuo-0.1.3/tuotuo/build/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:09:02.514936 TuoTuo-0.1.3/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.3/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:09:02.515722 TuoTuo-0.1.3/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
--rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.1.3/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
--rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.1.3/tuotuo/cutils.c
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.3/tuotuo/cutils.cpython-38-darwin.so
--rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.1.3/tuotuo/cutils.pyx
--rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.1.3/tuotuo/generator.py
--rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.1.3/tuotuo/lda_model.py
--rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.1.3/tuotuo/text_pre_processor.py
--rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.1.3/tuotuo/utils.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.728253 TuoTuo-0.1.4/
+-rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.1.4/.DS_Store
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.713308 TuoTuo-0.1.4/.github/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.717345 TuoTuo-0.1.4/.github/workflows/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.1.4/.github/workflows/python-package.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.1.4/.gitignore
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.717820 TuoTuo-0.1.4/.vscode/
+-rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.1.4/.vscode/c_cpp_properties.json
+-rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.1.4/LICENSE
+-rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 13:10:26.728402 TuoTuo-0.1.4/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.1.4/README.md
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.718936 TuoTuo-0.1.4/TuoTuo.egg-info/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 13:10:26.000000 TuoTuo-0.1.4/TuoTuo.egg-info/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      879 2023-05-02 13:10:26.000000 TuoTuo-0.1.4/TuoTuo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-02 13:10:26.000000 TuoTuo-0.1.4/TuoTuo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       45 2023-05-02 13:10:26.000000 TuoTuo-0.1.4/TuoTuo.egg-info/requires.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       21 2023-05-02 13:10:26.000000 TuoTuo-0.1.4/TuoTuo.egg-info/top_level.txt
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 TuoTuo-0.1.4/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.719837 TuoTuo-0.1.4/notebook/
+-rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.1.4/notebook/Our Model vs SKLearn.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.1.4/notebook/__init__.py
+-rw-r--r--   0 ericliu    (501) staff       (20)      123 2023-05-02 13:10:01.000000 TuoTuo-0.1.4/project.toml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.1.4/requirements.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-02 13:10:26.728705 TuoTuo-0.1.4/setup.cfg
+-rw-r--r--   0 ericliu    (501) staff       (20)     1684 2023-05-02 13:10:11.000000 TuoTuo-0.1.4/setup.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.723798 TuoTuo-0.1.4/tuotuo/
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.1.4/tuotuo/__init__.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.713789 TuoTuo-0.1.4/tuotuo/build/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.724226 TuoTuo-0.1.4/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.4/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.725583 TuoTuo-0.1.4/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
+-rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.1.4/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
+-rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.1.4/tuotuo/cutils.c
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.4/tuotuo/cutils.cpython-38-darwin.so
+-rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.1.4/tuotuo/cutils.pyx
+-rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.1.4/tuotuo/generator.py
+-rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.1.4/tuotuo/lda_model.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.1.4/tuotuo/text_pre_processor.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.1.4/tuotuo/utils.py
```

### Comparing `TuoTuo-0.1.3/.DS_Store` & `TuoTuo-0.1.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/.github/workflows/python-package.yml` & `TuoTuo-0.1.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/.github/workflows/python-publish.yml` & `TuoTuo-0.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/.vscode/c_cpp_properties.json` & `TuoTuo-0.1.4/.vscode/c_cpp_properties.json`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/LICENSE` & `TuoTuo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/PKG-INFO` & `TuoTuo-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.1.3
+Version: 0.1.4
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
 Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.0.5.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
```

### Comparing `TuoTuo-0.1.3/README.md` & `TuoTuo-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/TuoTuo.egg-info/PKG-INFO` & `TuoTuo-0.1.4/TuoTuo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.1.3
+Version: 0.1.4
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
 Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.0.5.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
```

### Comparing `TuoTuo-0.1.3/TuoTuo.egg-info/SOURCES.txt` & `TuoTuo-0.1.4/TuoTuo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.4/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/notebook/Our Model vs SKLearn.ipynb` & `TuoTuo-0.1.4/notebook/Our Model vs SKLearn.ipynb`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/requirements.txt` & `TuoTuo-0.1.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/setup.py` & `TuoTuo-0.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import Extension, setup
 from setuptools import dist
 from distutils.core import setup
 
-dist.Distribution().fetch_build_eggs(['Cython>=0.15.1', 'numpy>=1.10'])
+#dist.Distribution().fetch_build_eggs(['Cython>=0.15.1', 'numpy>=1.10'])
 
 import numpy as np 
 from Cython.Build import cythonize
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 
@@ -20,15 +20,15 @@
     ["tuotuo/cutils.pyx"],
     include_dirs=[np.get_include()], 
 )
 
 setup(
     name = 'TuoTuo',
     packages = ['tuotuo'],
-    version = '0.1.3',  
+    version = '0.1.4',  
     license='MIT',
     description = 'LDA & Neura based topic modelling library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'tuotuo Superman',
     author_email = 'tuotuo@HanwellSquare.BigForce.com',
     url = 'https://github.com/RobbenRibery/TuoTuo',
```

### Comparing `TuoTuo-0.1.3/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.4/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o` & `TuoTuo-0.1.4/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/tuotuo/cutils.c` & `TuoTuo-0.1.4/tuotuo/cutils.c`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/tuotuo/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.4/tuotuo/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/tuotuo/cutils.pyx` & `TuoTuo-0.1.4/tuotuo/cutils.pyx`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/tuotuo/generator.py` & `TuoTuo-0.1.4/tuotuo/generator.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/tuotuo/lda_model.py` & `TuoTuo-0.1.4/tuotuo/lda_model.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/tuotuo/text_pre_processor.py` & `TuoTuo-0.1.4/tuotuo/text_pre_processor.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.3/tuotuo/utils.py` & `TuoTuo-0.1.4/tuotuo/utils.py`

 * *Files identical despite different names*

