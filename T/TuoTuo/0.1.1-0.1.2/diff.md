# Comparing `tmp/TuoTuo-0.1.1.tar.gz` & `tmp/TuoTuo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TuoTuo-0.1.1.tar", last modified: Tue May  2 12:50:49 2023, max compression
+gzip compressed data, was "TuoTuo-0.1.2.tar", last modified: Tue May  2 12:59:12 2023, max compression
```

## Comparing `TuoTuo-0.1.1.tar` & `TuoTuo-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:50:49.022075 TuoTuo-0.1.1/
--rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.1.1/.DS_Store
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:50:48.999416 TuoTuo-0.1.1/.github/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:50:49.004090 TuoTuo-0.1.1/.github/workflows/
--rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.1.1/.github/workflows/python-package.yml
--rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.1.1/.gitignore
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:50:49.004588 TuoTuo-0.1.1/.vscode/
--rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.1.1/.vscode/c_cpp_properties.json
--rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.1.1/LICENSE
--rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 12:50:49.022251 TuoTuo-0.1.1/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.1.1/README.md
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:50:49.005514 TuoTuo-0.1.1/TuoTuo.egg-info/
--rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 12:50:48.000000 TuoTuo-0.1.1/TuoTuo.egg-info/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      866 2023-05-02 12:50:48.000000 TuoTuo-0.1.1/TuoTuo.egg-info/SOURCES.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-02 12:50:48.000000 TuoTuo-0.1.1/TuoTuo.egg-info/dependency_links.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       45 2023-05-02 12:50:48.000000 TuoTuo-0.1.1/TuoTuo.egg-info/requires.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       21 2023-05-02 12:50:48.000000 TuoTuo-0.1.1/TuoTuo.egg-info/top_level.txt
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 TuoTuo-0.1.1/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:50:49.006474 TuoTuo-0.1.1/notebook/
--rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.1.1/notebook/Our Model vs SKLearn.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.1.1/notebook/__init__.py
--rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.1.1/requirements.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-02 12:50:49.022672 TuoTuo-0.1.1/setup.cfg
--rw-r--r--   0 ericliu    (501) staff       (20)     1601 2023-05-02 12:50:46.000000 TuoTuo-0.1.1/setup.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:50:49.017533 TuoTuo-0.1.1/tuotuo/
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.1.1/tuotuo/__init__.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:50:48.999936 TuoTuo-0.1.1/tuotuo/build/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:50:49.017997 TuoTuo-0.1.1/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.1/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:50:49.019318 TuoTuo-0.1.1/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
--rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.1.1/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
--rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.1.1/tuotuo/cutils.c
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.1/tuotuo/cutils.cpython-38-darwin.so
--rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.1.1/tuotuo/cutils.pyx
--rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.1.1/tuotuo/generator.py
--rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.1.1/tuotuo/lda_model.py
--rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.1.1/tuotuo/text_pre_processor.py
--rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.1.1/tuotuo/utils.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:59:12.501051 TuoTuo-0.1.2/
+-rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.1.2/.DS_Store
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:59:12.486651 TuoTuo-0.1.2/.github/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:59:12.490533 TuoTuo-0.1.2/.github/workflows/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.1.2/.github/workflows/python-package.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.1.2/.gitignore
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:59:12.490880 TuoTuo-0.1.2/.vscode/
+-rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.1.2/.vscode/c_cpp_properties.json
+-rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.1.2/LICENSE
+-rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 12:59:12.501182 TuoTuo-0.1.2/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.1.2/README.md
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:59:12.491810 TuoTuo-0.1.2/TuoTuo.egg-info/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 12:59:12.000000 TuoTuo-0.1.2/TuoTuo.egg-info/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      866 2023-05-02 12:59:12.000000 TuoTuo-0.1.2/TuoTuo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-02 12:59:12.000000 TuoTuo-0.1.2/TuoTuo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       45 2023-05-02 12:59:12.000000 TuoTuo-0.1.2/TuoTuo.egg-info/requires.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       21 2023-05-02 12:59:12.000000 TuoTuo-0.1.2/TuoTuo.egg-info/top_level.txt
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 TuoTuo-0.1.2/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:59:12.492797 TuoTuo-0.1.2/notebook/
+-rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.1.2/notebook/Our Model vs SKLearn.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.1.2/notebook/__init__.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.1.2/requirements.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-02 12:59:12.501459 TuoTuo-0.1.2/setup.cfg
+-rw-r--r--   0 ericliu    (501) staff       (20)     1683 2023-05-02 12:59:07.000000 TuoTuo-0.1.2/setup.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:59:12.496590 TuoTuo-0.1.2/tuotuo/
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.1.2/tuotuo/__init__.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:59:12.487141 TuoTuo-0.1.2/tuotuo/build/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:59:12.496981 TuoTuo-0.1.2/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.2/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:59:12.498156 TuoTuo-0.1.2/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
+-rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.1.2/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
+-rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.1.2/tuotuo/cutils.c
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.2/tuotuo/cutils.cpython-38-darwin.so
+-rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.1.2/tuotuo/cutils.pyx
+-rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.1.2/tuotuo/generator.py
+-rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.1.2/tuotuo/lda_model.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.1.2/tuotuo/text_pre_processor.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.1.2/tuotuo/utils.py
```

### Comparing `TuoTuo-0.1.1/.DS_Store` & `TuoTuo-0.1.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/.github/workflows/python-package.yml` & `TuoTuo-0.1.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/.github/workflows/python-publish.yml` & `TuoTuo-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/.vscode/c_cpp_properties.json` & `TuoTuo-0.1.2/.vscode/c_cpp_properties.json`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/LICENSE` & `TuoTuo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/PKG-INFO` & `TuoTuo-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.1.1
+Version: 0.1.2
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
 Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.0.5.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
```

### Comparing `TuoTuo-0.1.1/README.md` & `TuoTuo-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/TuoTuo.egg-info/PKG-INFO` & `TuoTuo-0.1.2/TuoTuo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.1.1
+Version: 0.1.2
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
 Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.0.5.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
```

### Comparing `TuoTuo-0.1.1/TuoTuo.egg-info/SOURCES.txt` & `TuoTuo-0.1.2/TuoTuo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.2/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/notebook/Our Model vs SKLearn.ipynb` & `TuoTuo-0.1.2/notebook/Our Model vs SKLearn.ipynb`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/requirements.txt` & `TuoTuo-0.1.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/setup.py` & `TuoTuo-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 #!/usr/bin/env python
 # coding: utf-8
-import pkg_resources 
+
 from setuptools import Extension, setup
+from setuptools import dist
+from distutils.core import setup
+
+dist.Distribution().fetch_build_eggs(['Cython>=0.15.1', 'numpy>=1.10'])
+
 import numpy as np 
 from Cython.Build import cythonize
-from distutils.core import setup
+
 from pathlib import Path
 this_directory = Path(__file__).parent
 
 long_description = (this_directory / "README.md").read_text()
 
 extensions = Extension(
     "tuotuo/cutils", 
     ["tuotuo/cutils.pyx"],
     include_dirs=[np.get_include()], 
 )
 
 setup(
     name = 'TuoTuo',
     packages = ['tuotuo'],
-    version = '0.1.1',  
+    version = '0.1.2',  
     license='MIT',
     description = 'LDA & Neura based topic modelling library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'tuotuo Superman',
     author_email = 'tuotuo@HanwellSquare.BigForce.com',
     url = 'https://github.com/RobbenRibery/TuoTuo',
```

### Comparing `TuoTuo-0.1.1/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.2/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o` & `TuoTuo-0.1.2/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/tuotuo/cutils.c` & `TuoTuo-0.1.2/tuotuo/cutils.c`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/tuotuo/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.2/tuotuo/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/tuotuo/cutils.pyx` & `TuoTuo-0.1.2/tuotuo/cutils.pyx`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/tuotuo/generator.py` & `TuoTuo-0.1.2/tuotuo/generator.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/tuotuo/lda_model.py` & `TuoTuo-0.1.2/tuotuo/lda_model.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/tuotuo/text_pre_processor.py` & `TuoTuo-0.1.2/tuotuo/text_pre_processor.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.1/tuotuo/utils.py` & `TuoTuo-0.1.2/tuotuo/utils.py`

 * *Files identical despite different names*

