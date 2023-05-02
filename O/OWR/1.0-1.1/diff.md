# Comparing `tmp/OWR-1.0.tar.gz` & `tmp/OWR-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OWR-1.0.tar", last modified: Mon May  1 15:18:10 2023, max compression
+gzip compressed data, was "OWR-1.1.tar", last modified: Tue May  2 15:53:32 2023, max compression
```

## Comparing `OWR-1.0.tar` & `OWR-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 15:18:10.633934 OWR-1.0/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-1.0/LICENSE
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 15:18:10.633934 OWR-1.0/OWR/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6365 2023-05-01 15:17:25.000000 OWR-1.0/OWR/__init__.py
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-01 15:18:10.633934 OWR-1.0/OWR.egg-info/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-01 15:18:10.000000 OWR-1.0/OWR.egg-info/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      176 2023-05-01 15:18:10.000000 OWR-1.0/OWR.egg-info/SOURCES.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-01 15:18:10.000000 OWR-1.0/OWR.egg-info/dependency_links.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       74 2023-05-01 15:18:10.000000 OWR-1.0/OWR.egg-info/requires.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-01 15:18:10.000000 OWR-1.0/OWR.egg-info/top_level.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-01 15:18:10.633934 OWR-1.0/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-1.0/README.md
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-01 15:18:10.633934 OWR-1.0/setup.cfg
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      594 2023-05-01 15:18:04.000000 OWR-1.0/setup.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-02 15:53:32.049386 OWR-1.1/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-1.1/LICENSE
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-02 15:53:32.049386 OWR-1.1/OWR/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6365 2023-05-01 15:17:25.000000 OWR-1.1/OWR/__init__.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-02 15:53:32.049386 OWR-1.1/OWR.egg-info/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-02 15:53:32.000000 OWR-1.1/OWR.egg-info/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      176 2023-05-02 15:53:32.000000 OWR-1.1/OWR.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-02 15:53:32.000000 OWR-1.1/OWR.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-02 15:53:32.000000 OWR-1.1/OWR.egg-info/requires.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-02 15:53:32.000000 OWR-1.1/OWR.egg-info/top_level.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-02 15:53:32.049386 OWR-1.1/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-1.1/README.md
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-02 15:53:32.049386 OWR-1.1/setup.cfg
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      632 2023-05-02 15:53:13.000000 OWR-1.1/setup.py
```

### Comparing `OWR-1.0/LICENSE` & `OWR-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `OWR-1.0/OWR/__init__.py` & `OWR-1.1/OWR/__init__.py`

 * *Files identical despite different names*

### Comparing `OWR-1.0/setup.py` & `OWR-1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 setup(
     name='OWR',
-    version='1.0',
+    version='1.1',
     description='Obscene word recognition package',
     url='https://github.com/VladVslv/OWR',
     author='Vlad Vasilev',
     author_email='vpvasilev.work@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['OWR'],
     install_requires=['huggingsound',
                       'librosa',
-                      'Levenshtein',
+                      'scikit-learn',
+                      'levenshtein',
                       'soundfile',
                       'fonetika',
                       'numpy',
                       'playsound',
                       'pylcs'],
 )
```

