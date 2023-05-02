# Comparing `tmp/OWR-1.1.tar.gz` & `tmp/OWR-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OWR-1.1.tar", last modified: Tue May  2 15:53:32 2023, max compression
+gzip compressed data, was "OWR-1.2.tar", last modified: Tue May  2 15:55:27 2023, max compression
```

## Comparing `OWR-1.1.tar` & `OWR-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-02 15:53:32.049386 OWR-1.1/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-1.1/LICENSE
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-02 15:53:32.049386 OWR-1.1/OWR/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6365 2023-05-01 15:17:25.000000 OWR-1.1/OWR/__init__.py
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-02 15:53:32.049386 OWR-1.1/OWR.egg-info/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-02 15:53:32.000000 OWR-1.1/OWR.egg-info/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      176 2023-05-02 15:53:32.000000 OWR-1.1/OWR.egg-info/SOURCES.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-02 15:53:32.000000 OWR-1.1/OWR.egg-info/dependency_links.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-02 15:53:32.000000 OWR-1.1/OWR.egg-info/requires.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-02 15:53:32.000000 OWR-1.1/OWR.egg-info/top_level.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-02 15:53:32.049386 OWR-1.1/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-1.1/README.md
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-02 15:53:32.049386 OWR-1.1/setup.cfg
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      632 2023-05-02 15:53:13.000000 OWR-1.1/setup.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-02 15:55:27.031642 OWR-1.2/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-1.2/LICENSE
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-02 15:55:27.031642 OWR-1.2/OWR/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6365 2023-05-01 15:17:25.000000 OWR-1.2/OWR/__init__.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-02 15:55:27.031642 OWR-1.2/OWR.egg-info/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-02 15:55:27.000000 OWR-1.2/OWR.egg-info/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      176 2023-05-02 15:55:27.000000 OWR-1.2/OWR.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-02 15:55:27.000000 OWR-1.2/OWR.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-02 15:55:27.000000 OWR-1.2/OWR.egg-info/requires.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-02 15:55:27.000000 OWR-1.2/OWR.egg-info/top_level.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-02 15:55:27.031642 OWR-1.2/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-1.2/README.md
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-02 15:55:27.031642 OWR-1.2/setup.cfg
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      632 2023-05-02 15:55:21.000000 OWR-1.2/setup.py
```

### Comparing `OWR-1.1/LICENSE` & `OWR-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OWR-1.1/OWR/__init__.py` & `OWR-1.2/OWR/__init__.py`

 * *Files identical despite different names*

### Comparing `OWR-1.1/setup.py` & `OWR-1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 setup(
     name='OWR',
-    version='1.1',
+    version='1.2',
     description='Obscene word recognition package',
     url='https://github.com/VladVslv/OWR',
     author='Vlad Vasilev',
     author_email='vpvasilev.work@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['OWR'],
-    install_requires=['huggingsound',
+    install_requires=['scikit-learn',
+                      'huggingsound',
                       'librosa',
-                      'scikit-learn',
                       'levenshtein',
                       'soundfile',
                       'fonetika',
                       'numpy',
                       'playsound',
                       'pylcs'],
 )
```

