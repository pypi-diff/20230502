# Comparing `tmp/TuoTuo-0.0.9.tar.gz` & `tmp/TuoTuo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TuoTuo-0.0.9.tar", last modified: Tue May  2 12:40:45 2023, max compression
+gzip compressed data, was "TuoTuo-0.1.0.tar", last modified: Tue May  2 12:42:29 2023, max compression
```

## Comparing `TuoTuo-0.0.9.tar` & `TuoTuo-0.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:40:45.542676 TuoTuo-0.0.9/
--rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.0.9/.DS_Store
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:40:45.526615 TuoTuo-0.0.9/.github/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:40:45.530920 TuoTuo-0.0.9/.github/workflows/
--rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.0.9/.github/workflows/python-package.yml
--rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.0.9/.github/workflows/python-publish.yml
--rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.0.9/.gitignore
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:40:45.531375 TuoTuo-0.0.9/.vscode/
--rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.0.9/.vscode/c_cpp_properties.json
--rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.0.9/LICENSE
--rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 12:40:45.542781 TuoTuo-0.0.9/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.0.9/README.md
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:40:45.532277 TuoTuo-0.0.9/TuoTuo.egg-info/
--rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 12:40:45.000000 TuoTuo-0.0.9/TuoTuo.egg-info/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      866 2023-05-02 12:40:45.000000 TuoTuo-0.0.9/TuoTuo.egg-info/SOURCES.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-02 12:40:45.000000 TuoTuo-0.0.9/TuoTuo.egg-info/dependency_links.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       39 2023-05-02 12:40:45.000000 TuoTuo-0.0.9/TuoTuo.egg-info/requires.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        7 2023-05-02 12:40:45.000000 TuoTuo-0.0.9/TuoTuo.egg-info/top_level.txt
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 TuoTuo-0.0.9/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:40:45.533181 TuoTuo-0.0.9/notebook/
--rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.0.9/notebook/Our Model vs SKLearn.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.0.9/notebook/__init__.py
--rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.0.9/requirements.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-02 12:40:45.545063 TuoTuo-0.0.9/setup.cfg
--rw-r--r--   0 ericliu    (501) staff       (20)     1361 2023-05-02 12:40:40.000000 TuoTuo-0.0.9/setup.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:40:45.538071 TuoTuo-0.0.9/tuotuo/
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.0.9/tuotuo/__init__.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:40:45.527214 TuoTuo-0.0.9/tuotuo/build/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:40:45.538456 TuoTuo-0.0.9/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.0.9/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:40:45.540254 TuoTuo-0.0.9/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
--rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.0.9/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
--rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.0.9/tuotuo/cutils.c
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.0.9/tuotuo/cutils.cpython-38-darwin.so
--rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.0.9/tuotuo/cutils.pyx
--rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.0.9/tuotuo/generator.py
--rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.0.9/tuotuo/lda_model.py
--rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.0.9/tuotuo/text_pre_processor.py
--rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.0.9/tuotuo/utils.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:42:29.198328 TuoTuo-0.1.0/
+-rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.1.0/.DS_Store
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:42:29.177079 TuoTuo-0.1.0/.github/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:42:29.181125 TuoTuo-0.1.0/.github/workflows/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.1.0/.github/workflows/python-package.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.1.0/.gitignore
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:42:29.181678 TuoTuo-0.1.0/.vscode/
+-rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.1.0/.vscode/c_cpp_properties.json
+-rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.1.0/LICENSE
+-rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 12:42:29.198465 TuoTuo-0.1.0/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.1.0/README.md
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:42:29.182797 TuoTuo-0.1.0/TuoTuo.egg-info/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 12:42:29.000000 TuoTuo-0.1.0/TuoTuo.egg-info/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      866 2023-05-02 12:42:29.000000 TuoTuo-0.1.0/TuoTuo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-02 12:42:29.000000 TuoTuo-0.1.0/TuoTuo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       45 2023-05-02 12:42:29.000000 TuoTuo-0.1.0/TuoTuo.egg-info/requires.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        7 2023-05-02 12:42:29.000000 TuoTuo-0.1.0/TuoTuo.egg-info/top_level.txt
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 TuoTuo-0.1.0/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:42:29.183794 TuoTuo-0.1.0/notebook/
+-rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.1.0/notebook/Our Model vs SKLearn.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.1.0/notebook/__init__.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.1.0/requirements.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-02 12:42:29.198793 TuoTuo-0.1.0/setup.cfg
+-rw-r--r--   0 ericliu    (501) staff       (20)     1378 2023-05-02 12:42:24.000000 TuoTuo-0.1.0/setup.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:42:29.188027 TuoTuo-0.1.0/tuotuo/
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.1.0/tuotuo/__init__.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:42:29.177574 TuoTuo-0.1.0/tuotuo/build/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:42:29.188439 TuoTuo-0.1.0/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.0/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 12:42:29.189778 TuoTuo-0.1.0/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
+-rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.1.0/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
+-rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.1.0/tuotuo/cutils.c
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.0/tuotuo/cutils.cpython-38-darwin.so
+-rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.1.0/tuotuo/cutils.pyx
+-rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.1.0/tuotuo/generator.py
+-rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.1.0/tuotuo/lda_model.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.1.0/tuotuo/text_pre_processor.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.1.0/tuotuo/utils.py
```

### Comparing `TuoTuo-0.0.9/.DS_Store` & `TuoTuo-0.1.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/.github/workflows/python-package.yml` & `TuoTuo-0.1.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/.github/workflows/python-publish.yml` & `TuoTuo-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/.vscode/c_cpp_properties.json` & `TuoTuo-0.1.0/.vscode/c_cpp_properties.json`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/LICENSE` & `TuoTuo-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/PKG-INFO` & `TuoTuo-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.0.9
+Version: 0.1.0
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
 Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.0.5.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
```

### Comparing `TuoTuo-0.0.9/README.md` & `TuoTuo-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/TuoTuo.egg-info/PKG-INFO` & `TuoTuo-0.1.0/TuoTuo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.0.9
+Version: 0.1.0
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
 Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.0.5.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
```

### Comparing `TuoTuo-0.0.9/TuoTuo.egg-info/SOURCES.txt` & `TuoTuo-0.1.0/TuoTuo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.0/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/notebook/Our Model vs SKLearn.ipynb` & `TuoTuo-0.1.0/notebook/Our Model vs SKLearn.ipynb`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/requirements.txt` & `TuoTuo-0.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/setup.py` & `TuoTuo-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 this_directory = Path(__file__).parent
 
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = 'TuoTuo',
     packages = ['tuotuo'],
-    version = '0.0.9',  
+    version = '0.1.0',  
     license='MIT',
     description = 'LDA & Neura based topic modelling library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'tuotuo Superman',
     author_email = 'tuotuo@HanwellSquare.BigForce.com',
     url = 'https://github.com/RobbenRibery/TuoTuo',
@@ -24,14 +24,15 @@
     install_requires=[            
         'numpy',
         'torch',
         'scipy',
         'pyro-ppl',
         'pandas',
         'nltk',
+        'spacy',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha', 
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'License :: OSI Approved :: MIT License',  
         'Programming Language :: Python :: 3.8',
```

### Comparing `TuoTuo-0.0.9/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.0/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o` & `TuoTuo-0.1.0/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/tuotuo/cutils.c` & `TuoTuo-0.1.0/tuotuo/cutils.c`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/tuotuo/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.0/tuotuo/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/tuotuo/cutils.pyx` & `TuoTuo-0.1.0/tuotuo/cutils.pyx`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/tuotuo/generator.py` & `TuoTuo-0.1.0/tuotuo/generator.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/tuotuo/lda_model.py` & `TuoTuo-0.1.0/tuotuo/lda_model.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/tuotuo/text_pre_processor.py` & `TuoTuo-0.1.0/tuotuo/text_pre_processor.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.0.9/tuotuo/utils.py` & `TuoTuo-0.1.0/tuotuo/utils.py`

 * *Files identical despite different names*

