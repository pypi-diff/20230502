# Comparing `tmp/MediaLib-3.0.1.4.tar.gz` & `tmp/MediaLib-3.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MediaLib-3.0.1.4.tar", last modified: Tue May  2 15:47:16 2023, max compression
+gzip compressed data, was "MediaLib-3.0.1.5.tar", last modified: Tue May  2 15:49:50 2023, max compression
```

## Comparing `MediaLib-3.0.1.4.tar` & `MediaLib-3.0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 15:47:16.735073 MediaLib-3.0.1.4/
--rw-r--r--   0 adamwynn   (501) staff       (20)      181 2023-05-02 15:47:16.735196 MediaLib-3.0.1.4/PKG-INFO
--rw-r--r--   0 adamwynn   (501) staff       (20)       13 2023-05-02 13:38:19.000000 MediaLib-3.0.1.4/README.rst
--rw-r--r--   0 adamwynn   (501) staff       (20)      107 2023-05-02 15:47:16.735579 MediaLib-3.0.1.4/setup.cfg
--rw-r--r--   0 adamwynn   (501) staff       (20)      367 2023-05-02 15:26:47.000000 MediaLib-3.0.1.4/setup.py
-drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 15:47:16.731955 MediaLib-3.0.1.4/src/
-drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 15:47:16.734376 MediaLib-3.0.1.4/src/MediaLib.egg-info/
--rw-r--r--   0 adamwynn   (501) staff       (20)      181 2023-05-02 15:47:16.000000 MediaLib-3.0.1.4/src/MediaLib.egg-info/PKG-INFO
--rw-r--r--   0 adamwynn   (501) staff       (20)      260 2023-05-02 15:47:16.000000 MediaLib-3.0.1.4/src/MediaLib.egg-info/SOURCES.txt
--rw-r--r--   0 adamwynn   (501) staff       (20)        1 2023-05-02 15:47:16.000000 MediaLib-3.0.1.4/src/MediaLib.egg-info/dependency_links.txt
--rw-r--r--   0 adamwynn   (501) staff       (20)        7 2023-05-02 15:47:16.000000 MediaLib-3.0.1.4/src/MediaLib.egg-info/requires.txt
--rw-r--r--   0 adamwynn   (501) staff       (20)       10 2023-05-02 15:47:16.000000 MediaLib-3.0.1.4/src/MediaLib.egg-info/top_level.txt
-drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 15:47:16.734777 MediaLib-3.0.1.4/src/medlialib/
--rw-r--r--   0 adamwynn   (501) staff       (20)       15 2023-05-02 15:47:06.000000 MediaLib-3.0.1.4/src/medlialib/__init__.py
--rw-r--r--   0 adamwynn   (501) staff       (20)     9122 2022-12-10 16:29:45.000000 MediaLib-3.0.1.4/src/medlialib/medialib.py
+drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 15:49:50.493654 MediaLib-3.0.1.5/
+-rw-r--r--   0 adamwynn   (501) staff       (20)      181 2023-05-02 15:49:50.493756 MediaLib-3.0.1.5/PKG-INFO
+-rw-r--r--   0 adamwynn   (501) staff       (20)       13 2023-05-02 13:38:19.000000 MediaLib-3.0.1.5/README.rst
+-rw-r--r--   0 adamwynn   (501) staff       (20)      107 2023-05-02 15:49:50.494140 MediaLib-3.0.1.5/setup.cfg
+-rw-r--r--   0 adamwynn   (501) staff       (20)      367 2023-05-02 15:49:26.000000 MediaLib-3.0.1.5/setup.py
+drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 15:49:50.490521 MediaLib-3.0.1.5/src/
+drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 15:49:50.492880 MediaLib-3.0.1.5/src/MediaLib.egg-info/
+-rw-r--r--   0 adamwynn   (501) staff       (20)      181 2023-05-02 15:49:50.000000 MediaLib-3.0.1.5/src/MediaLib.egg-info/PKG-INFO
+-rw-r--r--   0 adamwynn   (501) staff       (20)      260 2023-05-02 15:49:50.000000 MediaLib-3.0.1.5/src/MediaLib.egg-info/SOURCES.txt
+-rw-r--r--   0 adamwynn   (501) staff       (20)        1 2023-05-02 15:49:50.000000 MediaLib-3.0.1.5/src/MediaLib.egg-info/dependency_links.txt
+-rw-r--r--   0 adamwynn   (501) staff       (20)        7 2023-05-02 15:49:50.000000 MediaLib-3.0.1.5/src/MediaLib.egg-info/requires.txt
+-rw-r--r--   0 adamwynn   (501) staff       (20)       10 2023-05-02 15:49:50.000000 MediaLib-3.0.1.5/src/MediaLib.egg-info/top_level.txt
+drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 15:49:50.493258 MediaLib-3.0.1.5/src/medlialib/
+-rw-r--r--   0 adamwynn   (501) staff       (20)       23 2023-05-02 15:49:43.000000 MediaLib-3.0.1.5/src/medlialib/__init__.py
+-rw-r--r--   0 adamwynn   (501) staff       (20)     9122 2022-12-10 16:29:45.000000 MediaLib-3.0.1.5/src/medlialib/medialib.py
```

### Comparing `MediaLib-3.0.1.4/src/medlialib/medialib.py` & `MediaLib-3.0.1.5/src/medlialib/medialib.py`

 * *Files identical despite different names*

