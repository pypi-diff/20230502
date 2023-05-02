# Comparing `tmp/TuoTuo-0.1.4.tar.gz` & `tmp/TuoTuo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TuoTuo-0.1.4.tar", last modified: Tue May  2 13:10:26 2023, max compression
+gzip compressed data, was "TuoTuo-0.1.5.tar", last modified: Tue May  2 13:14:15 2023, max compression
```

## Comparing `TuoTuo-0.1.4.tar` & `TuoTuo-0.1.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.728253 TuoTuo-0.1.4/
--rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.1.4/.DS_Store
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.713308 TuoTuo-0.1.4/.github/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.717345 TuoTuo-0.1.4/.github/workflows/
--rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.1.4/.github/workflows/python-package.yml
--rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.1.4/.gitignore
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.717820 TuoTuo-0.1.4/.vscode/
--rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.1.4/.vscode/c_cpp_properties.json
--rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.1.4/LICENSE
--rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 13:10:26.728402 TuoTuo-0.1.4/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.1.4/README.md
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.718936 TuoTuo-0.1.4/TuoTuo.egg-info/
--rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 13:10:26.000000 TuoTuo-0.1.4/TuoTuo.egg-info/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      879 2023-05-02 13:10:26.000000 TuoTuo-0.1.4/TuoTuo.egg-info/SOURCES.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-02 13:10:26.000000 TuoTuo-0.1.4/TuoTuo.egg-info/dependency_links.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       45 2023-05-02 13:10:26.000000 TuoTuo-0.1.4/TuoTuo.egg-info/requires.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       21 2023-05-02 13:10:26.000000 TuoTuo-0.1.4/TuoTuo.egg-info/top_level.txt
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 TuoTuo-0.1.4/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.719837 TuoTuo-0.1.4/notebook/
--rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.1.4/notebook/Our Model vs SKLearn.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.1.4/notebook/__init__.py
--rw-r--r--   0 ericliu    (501) staff       (20)      123 2023-05-02 13:10:01.000000 TuoTuo-0.1.4/project.toml
--rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.1.4/requirements.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-02 13:10:26.728705 TuoTuo-0.1.4/setup.cfg
--rw-r--r--   0 ericliu    (501) staff       (20)     1684 2023-05-02 13:10:11.000000 TuoTuo-0.1.4/setup.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.723798 TuoTuo-0.1.4/tuotuo/
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.1.4/tuotuo/__init__.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.713789 TuoTuo-0.1.4/tuotuo/build/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.724226 TuoTuo-0.1.4/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.4/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:10:26.725583 TuoTuo-0.1.4/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
--rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.1.4/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
--rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.1.4/tuotuo/cutils.c
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.4/tuotuo/cutils.cpython-38-darwin.so
--rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.1.4/tuotuo/cutils.pyx
--rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.1.4/tuotuo/generator.py
--rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.1.4/tuotuo/lda_model.py
--rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.1.4/tuotuo/text_pre_processor.py
--rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.1.4/tuotuo/utils.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:14:15.504887 TuoTuo-0.1.5/
+-rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 TuoTuo-0.1.5/.DS_Store
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:14:15.493754 TuoTuo-0.1.5/.github/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:14:15.497151 TuoTuo-0.1.5/.github/workflows/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 TuoTuo-0.1.5/.github/workflows/python-package.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 TuoTuo-0.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 TuoTuo-0.1.5/.gitignore
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:14:15.497415 TuoTuo-0.1.5/.vscode/
+-rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 TuoTuo-0.1.5/.vscode/c_cpp_properties.json
+-rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 TuoTuo-0.1.5/LICENSE
+-rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 13:14:15.505030 TuoTuo-0.1.5/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 TuoTuo-0.1.5/README.md
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:14:15.498643 TuoTuo-0.1.5/TuoTuo.egg-info/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1514 2023-05-02 13:14:15.000000 TuoTuo-0.1.5/TuoTuo.egg-info/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      879 2023-05-02 13:14:15.000000 TuoTuo-0.1.5/TuoTuo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-02 13:14:15.000000 TuoTuo-0.1.5/TuoTuo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       45 2023-05-02 13:14:15.000000 TuoTuo-0.1.5/TuoTuo.egg-info/requires.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       21 2023-05-02 13:14:15.000000 TuoTuo-0.1.5/TuoTuo.egg-info/top_level.txt
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 TuoTuo-0.1.5/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:14:15.499389 TuoTuo-0.1.5/notebook/
+-rw-r--r--   0 ericliu    (501) staff       (20)    56829 2023-05-02 09:53:49.000000 TuoTuo-0.1.5/notebook/Our Model vs SKLearn.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 TuoTuo-0.1.5/notebook/__init__.py
+-rw-r--r--   0 ericliu    (501) staff       (20)      123 2023-05-02 13:10:01.000000 TuoTuo-0.1.5/project.toml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 TuoTuo-0.1.5/requirements.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-02 13:14:15.505362 TuoTuo-0.1.5/setup.cfg
+-rw-r--r--   0 ericliu    (501) staff       (20)     1845 2023-05-02 13:14:12.000000 TuoTuo-0.1.5/setup.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:14:15.501978 TuoTuo-0.1.5/tuotuo/
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 TuoTuo-0.1.5/tuotuo/__init__.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:14:15.494248 TuoTuo-0.1.5/tuotuo/build/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:14:15.502259 TuoTuo-0.1.5/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.5/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 13:14:15.503040 TuoTuo-0.1.5/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/
+-rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 TuoTuo-0.1.5/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
+-rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 TuoTuo-0.1.5/tuotuo/cutils.c
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 TuoTuo-0.1.5/tuotuo/cutils.cpython-38-darwin.so
+-rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 TuoTuo-0.1.5/tuotuo/cutils.pyx
+-rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 TuoTuo-0.1.5/tuotuo/generator.py
+-rw-r--r--   0 ericliu    (501) staff       (20)    16225 2023-05-02 09:53:34.000000 TuoTuo-0.1.5/tuotuo/lda_model.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 TuoTuo-0.1.5/tuotuo/text_pre_processor.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     9792 2023-05-02 09:53:39.000000 TuoTuo-0.1.5/tuotuo/utils.py
```

### Comparing `TuoTuo-0.1.4/.DS_Store` & `TuoTuo-0.1.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/.github/workflows/python-package.yml` & `TuoTuo-0.1.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/.github/workflows/python-publish.yml` & `TuoTuo-0.1.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/.vscode/c_cpp_properties.json` & `TuoTuo-0.1.5/.vscode/c_cpp_properties.json`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/LICENSE` & `TuoTuo-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/PKG-INFO` & `TuoTuo-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.1.4
+Version: 0.1.5
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
 Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.0.5.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
```

### Comparing `TuoTuo-0.1.4/README.md` & `TuoTuo-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/TuoTuo.egg-info/PKG-INFO` & `TuoTuo-0.1.5/TuoTuo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TuoTuo
-Version: 0.1.4
+Version: 0.1.5
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
 Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.0.5.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
```

### Comparing `TuoTuo-0.1.4/TuoTuo.egg-info/SOURCES.txt` & `TuoTuo-0.1.5/TuoTuo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.5/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/notebook/Our Model vs SKLearn.ipynb` & `TuoTuo-0.1.5/notebook/Our Model vs SKLearn.ipynb`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/requirements.txt` & `TuoTuo-0.1.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.5/tuotuo/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o` & `TuoTuo-0.1.5/tuotuo/build/temp.macosx-10.14-arm64-cpython-38/cutils.o`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/tuotuo/cutils.c` & `TuoTuo-0.1.5/tuotuo/cutils.c`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/tuotuo/cutils.cpython-38-darwin.so` & `TuoTuo-0.1.5/tuotuo/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/tuotuo/cutils.pyx` & `TuoTuo-0.1.5/tuotuo/cutils.pyx`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/tuotuo/generator.py` & `TuoTuo-0.1.5/tuotuo/generator.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/tuotuo/lda_model.py` & `TuoTuo-0.1.5/tuotuo/lda_model.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/tuotuo/text_pre_processor.py` & `TuoTuo-0.1.5/tuotuo/text_pre_processor.py`

 * *Files identical despite different names*

### Comparing `TuoTuo-0.1.4/tuotuo/utils.py` & `TuoTuo-0.1.5/tuotuo/utils.py`

 * *Files identical despite different names*

