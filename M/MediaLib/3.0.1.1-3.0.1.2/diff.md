# Comparing `tmp/MediaLib-3.0.1.1.tar.gz` & `tmp/MediaLib-3.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MediaLib-3.0.1.1.tar", last modified: Tue May  2 13:54:44 2023, max compression
+gzip compressed data, was "MediaLib-3.0.1.2.tar", last modified: Tue May  2 14:00:20 2023, max compression
```

## Comparing `MediaLib-3.0.1.1.tar` & `MediaLib-3.0.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 13:54:44.303001 MediaLib-3.0.1.1/
--rw-r--r--   0 adamwynn   (501) staff       (20)      181 2023-05-02 13:54:44.303882 MediaLib-3.0.1.1/PKG-INFO
--rw-r--r--   0 adamwynn   (501) staff       (20)       13 2023-05-02 13:38:19.000000 MediaLib-3.0.1.1/README.rst
--rw-r--r--   0 adamwynn   (501) staff       (20)      107 2023-05-02 13:54:44.304311 MediaLib-3.0.1.1/setup.cfg
--rw-r--r--   0 adamwynn   (501) staff       (20)      366 2023-05-02 13:54:26.000000 MediaLib-3.0.1.1/setup.py
-drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 13:54:44.300864 MediaLib-3.0.1.1/src/
-drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 13:54:44.302409 MediaLib-3.0.1.1/src/MediaLib.egg-info/
--rw-r--r--   0 adamwynn   (501) staff       (20)      181 2023-05-02 13:54:44.000000 MediaLib-3.0.1.1/src/MediaLib.egg-info/PKG-INFO
--rw-r--r--   0 adamwynn   (501) staff       (20)      233 2023-05-02 13:54:44.000000 MediaLib-3.0.1.1/src/MediaLib.egg-info/SOURCES.txt
--rw-r--r--   0 adamwynn   (501) staff       (20)        1 2023-05-02 13:54:44.000000 MediaLib-3.0.1.1/src/MediaLib.egg-info/dependency_links.txt
--rw-r--r--   0 adamwynn   (501) staff       (20)        7 2023-05-02 13:54:44.000000 MediaLib-3.0.1.1/src/MediaLib.egg-info/requires.txt
--rw-r--r--   0 adamwynn   (501) staff       (20)        9 2023-05-02 13:54:44.000000 MediaLib-3.0.1.1/src/MediaLib.egg-info/top_level.txt
-drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 13:54:44.302715 MediaLib-3.0.1.1/src/medialib/
--rw-r--r--   0 adamwynn   (501) staff       (20)     9122 2022-12-10 16:29:45.000000 MediaLib-3.0.1.1/src/medialib/__init__.py
+drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 14:00:20.602046 MediaLib-3.0.1.2/
+-rw-r--r--   0 adamwynn   (501) staff       (20)      181 2023-05-02 14:00:20.602114 MediaLib-3.0.1.2/PKG-INFO
+-rw-r--r--   0 adamwynn   (501) staff       (20)       13 2023-05-02 13:38:19.000000 MediaLib-3.0.1.2/README.rst
+-rw-r--r--   0 adamwynn   (501) staff       (20)      107 2023-05-02 14:00:20.602374 MediaLib-3.0.1.2/setup.cfg
+-rw-r--r--   0 adamwynn   (501) staff       (20)      367 2023-05-02 13:58:44.000000 MediaLib-3.0.1.2/setup.py
+drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 14:00:20.599781 MediaLib-3.0.1.2/src/
+drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 14:00:20.601527 MediaLib-3.0.1.2/src/MediaLib.egg-info/
+-rw-r--r--   0 adamwynn   (501) staff       (20)      181 2023-05-02 14:00:20.000000 MediaLib-3.0.1.2/src/MediaLib.egg-info/PKG-INFO
+-rw-r--r--   0 adamwynn   (501) staff       (20)      258 2023-05-02 14:00:20.000000 MediaLib-3.0.1.2/src/MediaLib.egg-info/SOURCES.txt
+-rw-r--r--   0 adamwynn   (501) staff       (20)        1 2023-05-02 14:00:20.000000 MediaLib-3.0.1.2/src/MediaLib.egg-info/dependency_links.txt
+-rw-r--r--   0 adamwynn   (501) staff       (20)        7 2023-05-02 14:00:20.000000 MediaLib-3.0.1.2/src/MediaLib.egg-info/requires.txt
+-rw-r--r--   0 adamwynn   (501) staff       (20)        9 2023-05-02 14:00:20.000000 MediaLib-3.0.1.2/src/MediaLib.egg-info/top_level.txt
+drwxr-xr-x   0 adamwynn   (501) staff       (20)        0 2023-05-02 14:00:20.601784 MediaLib-3.0.1.2/src/medialib/
+-rw-r--r--   0 adamwynn   (501) staff       (20)        0 2023-05-02 13:58:27.000000 MediaLib-3.0.1.2/src/medialib/__init__.py
+-rw-r--r--   0 adamwynn   (501) staff       (20)     9122 2022-12-10 16:29:45.000000 MediaLib-3.0.1.2/src/medialib/medialib.py
```

### Comparing `MediaLib-3.0.1.1/src/medialib/__init__.py` & `MediaLib-3.0.1.2/src/medialib/medialib.py`

 * *Files identical despite different names*

