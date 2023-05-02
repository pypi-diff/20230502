# Comparing `tmp/TuoTuo-0.1.6.tar.gz` & `tmp/TuoTuo-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TuoTuo-0.1.6.tar", last modified: Tue May  2 13:24:07 2023, max compression
+gzip compressed data, was "TuoTuo-0.1.7.tar", last modified: Tue May  2 13:35:10 2023, max compression
```

## Comparing `TuoTuo-0.1.6.tar` & `TuoTuo-0.1.7.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:24:07.172293 TuoTuo-0.1.6/
--rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.1.6/.DS_Store
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:24:07.151540 TuoTuo-0.1.6/.github/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:24:07.158914 TuoTuo-0.1.6/.github/workflows/
--rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.1.6/.github/workflows/python-package.yml
--rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.1.6/.github/workflows/python-publish.yml
--rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.1.6/.gitignore
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:24:07.159413 TuoTuo-0.1.6/.vscode/
--rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.1.6/.vscode/c_cpp_properties.json
--rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.1.6/LICENSE
--rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 13:24:07.172442 TuoTuo-0.1.6/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.1.6/README.md
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:24:07.160385 TuoTuo-0.1.6/TuoTuo.egg-info/
--rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 13:24:07.000000 TuoTuo-0.1.6/TuoTuo.egg-info/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      879 2023-05-02 13:24:07.000000 TuoTuo-0.1.6/TuoTuo.egg-info/SOURCES.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-02 13:24:07.000000 TuoTuo-0.1.6/TuoTuo.egg-info/dependency_links.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       45 2023-05-02 13:24:07.000000 TuoTuo-0.1.6/TuoTuo.egg-info/requires.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       21 2023-05-02 13:24:07.000000 TuoTuo-0.1.6/TuoTuo.egg-info/top_level.txt
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 TuoTuo-0.1.6/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:24:07.161292 TuoTuo-0.1.6/notebook/
--rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.1.6/notebook/Our Model vs SKLearn.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.1.6/notebook/__init__.py
--rw-r--r--   0 ericliu    (501) staff       (20)      123 2023-05-02 13:10:01.000000 TuoTuo-0.1.6/project.toml
--rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.1.6/requirements.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-02 13:24:07.172746 TuoTuo-0.1.6/setup.cfg
--rw-r--r--   0 ericliu    (501) staff       (20)     1977 2023-05-02 13:24:05.000000 TuoTuo-0.1.6/setup.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:24:07.164761 TuoTuo-0.1.6/tuotuo/
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.1.6/tuotuo/__init__.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:24:07.152044 TuoTuo-0.1.6/tuotuo/build/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:24:07.165174 TuoTuo-0.1.6/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.6/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:24:07.166493 TuoTuo-0.1.6/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
--rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.1.6/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
--rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.1.6/tuotuo/cutils.c
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.6/tuotuo/cutils.cpython-38-darwin.so
--rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.1.6/tuotuo/cutils.pyx
--rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.1.6/tuotuo/generator.py
--rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.1.6/tuotuo/lda_model.py
--rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.1.6/tuotuo/text_pre_processor.py
--rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.1.6/tuotuo/utils.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:35:10.562073 TuoTuo-0.1.7/
+-rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.1.7/.DS_Store
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:35:10.543306 TuoTuo-0.1.7/.github/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:35:10.548048 TuoTuo-0.1.7/.github/workflows/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.1.7/.github/workflows/python-package.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.1.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.1.7/.gitignore
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:35:10.548518 TuoTuo-0.1.7/.vscode/
+-rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.1.7/.vscode/c_cpp_properties.json
+-rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.1.7/LICENSE
+-rw-r--r--   0 ericliu    (501) staff       (20)       24 2023-05-02 13:32:32.000000 TuoTuo-0.1.7/MANIFEST.in
+-rw-r--r--   0 ericliu    (501) staff       (20)     1534 2023-05-02 13:35:10.562268 TuoTuo-0.1.7/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.1.7/README.md
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:35:10.549463 TuoTuo-0.1.7/TuoTuo.egg-info/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1534 2023-05-02 13:35:10.000000 TuoTuo-0.1.7/TuoTuo.egg-info/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      907 2023-05-02 13:35:10.000000 TuoTuo-0.1.7/TuoTuo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-02 13:35:10.000000 TuoTuo-0.1.7/TuoTuo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       59 2023-05-02 13:35:10.000000 TuoTuo-0.1.7/TuoTuo.egg-info/requires.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       21 2023-05-02 13:35:10.000000 TuoTuo-0.1.7/TuoTuo.egg-info/top_level.txt
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 TuoTuo-0.1.7/cutils.cpython-38-darwin.so
+-rw-r--r--   0 ericliu    (501) staff       (20)    13943 2023-05-02 13:32:32.000000 TuoTuo-0.1.7/cysetuptools.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:35:10.550330 TuoTuo-0.1.7/notebook/
+-rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.1.7/notebook/Our Model vs SKLearn.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.1.7/notebook/__init__.py
+-rw-r--r--   0 ericliu    (501) staff       (20)      123 2023-05-02 13:10:01.000000 TuoTuo-0.1.7/project.toml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.1.7/requirements.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)      197 2023-05-02 13:35:10.565938 TuoTuo-0.1.7/setup.cfg
+-rw-r--r--   0 ericliu    (501) staff       (20)     2028 2023-05-02 13:35:08.000000 TuoTuo-0.1.7/setup.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:35:10.554186 TuoTuo-0.1.7/tuotuo/
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.1.7/tuotuo/__init__.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:35:10.543796 TuoTuo-0.1.7/tuotuo/build/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:35:10.554589 TuoTuo-0.1.7/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.7/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:35:10.555769 TuoTuo-0.1.7/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
+-rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.1.7/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
+-rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.1.7/tuotuo/cutils.c
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.7/tuotuo/cutils.cpython-38-darwin.so
+-rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.1.7/tuotuo/cutils.pyx
+-rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.1.7/tuotuo/generator.py
+-rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.1.7/tuotuo/lda_model.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.1.7/tuotuo/text_pre_processor.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.1.7/tuotuo/utils.py
```

### Comparing `TuoTuo-0.1.6/.DS_Store` & `TuoTuo-0.1.7/.DS_Store`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/.github/workflows/python-package.yml` & `TuoTuo-0.1.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/.github/workflows/python-publish.yml` & `TuoTuo-0.1.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/.vscode/c_cpp_properties.json` & `TuoTuo-0.1.7/.vscode/c_cpp_properties.json`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/LICENSE` & `TuoTuo-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/PKG-INFO` & `TuoTuo-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.1.6
+Version: 0.1.7
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
 Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.0.5.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 Implemented the Smoothed Varational Inference version of Latent Dirichlet Allocation, following David M. Blei et al. 2003
 
 1. Complete the Varitaional Inference version for batch & online LDA [80%]
     - Following the original LDA Paper: [https://www.jmlr.org/papers/volume3/blei03a/blei03a.pdf]
     - Folloing the Online LDA Papaer: [https://papers.nips.cc/paper_files/paper/2010/file/71f6278d140af599e06ad9bf1ba03cb0-Paper.pdf]
```

### Comparing `TuoTuo-0.1.6/README.md` & `TuoTuo-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/TuoTuo.egg-info/PKG-INFO` & `TuoTuo-0.1.7/TuoTuo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.1.6
+Version: 0.1.7
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
 Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.0.5.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 Implemented the Smoothed Varational Inference version of Latent Dirichlet Allocation, following David M. Blei et al. 2003
 
 1. Complete the Varitaional Inference version for batch & online LDA [80%]
     - Following the original LDA Paper: [https://www.jmlr.org/papers/volume3/blei03a/blei03a.pdf]
     - Folloing the Online LDA Papaer: [https://papers.nips.cc/paper_files/paper/2010/file/71f6278d140af599e06ad9bf1ba03cb0-Paper.pdf]
```

### Comparing `TuoTuo-0.1.6/TuoTuo.egg-info/SOURCES.txt` & `TuoTuo-0.1.7/TuoTuo.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .DS_Store
 .gitignore
 LICENSE
+MANIFEST.in
 README.md
 cutils.cpython-38-darwin.so
+cysetuptools.py
 project.toml
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
 .vscode/c_cpp_properties.json
```

### Comparing `TuoTuo-0.1.6/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.7/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/notebook/Our Model vs SKLearn.ipynb` & `TuoTuo-0.1.7/notebook/Our Model vs SKLearn.ipynb`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/requirements.txt` & `TuoTuo-0.1.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/setup.py` & `TuoTuo-0.1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import Extension, setup
 from setuptools import dist
 from distutils.core import setup
 from pathlib import Path
+from setuptools.command.build_ext import build_ext
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 class NumpyExtension(Extension):
     # setuptools calls this function after installing dependencies
     def _convert_pyx_sources_to_lang(self):
@@ -28,15 +29,15 @@
         extensions, 
         annotate = True,
     )
 
 setup(
     name = 'TuoTuo',
     packages = ['tuotuo'],
-    version = '0.1.6',  
+    version = '0.1.7',  
     license='MIT',
     description = 'LDA & Neura based topic modelling library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'tuotuo Superman',
     author_email = 'tuotuo@HanwellSquare.BigForce.com',
     url = 'https://github.com/RobbenRibery/TuoTuo',
```

### Comparing `TuoTuo-0.1.6/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.7/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o` & `TuoTuo-0.1.7/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/tuotuo/cutils.c` & `TuoTuo-0.1.7/tuotuo/cutils.c`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/tuotuo/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.7/tuotuo/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/tuotuo/cutils.pyx` & `TuoTuo-0.1.7/tuotuo/cutils.pyx`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/tuotuo/generator.py` & `TuoTuo-0.1.7/tuotuo/generator.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/tuotuo/lda_model.py` & `TuoTuo-0.1.7/tuotuo/lda_model.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/tuotuo/text_pre_processor.py` & `TuoTuo-0.1.7/tuotuo/text_pre_processor.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.6/tuotuo/utils.py` & `TuoTuo-0.1.7/tuotuo/utils.py`

 * *Files identical despite different names*

