# Comparing `tmp/croto-2.1.tar.gz` & `tmp/croto-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croto-2.1.tar", last modified: Mon May  1 21:24:03 2023, max compression
+gzip compressed data, was "croto-2.2.tar", last modified: Mon May  1 21:30:21 2023, max compression
```

## Comparing `croto-2.1.tar` & `croto-2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:24:03.464523 croto-2.1/
--rw-r--r--   0 defeee     (501) staff       (20)      299 2023-05-01 21:24:03.464587 croto-2.1/PKG-INFO
--rw-r--r--   0 defeee     (501) staff       (20)       28 2023-05-01 00:44:38.000000 croto-2.1/README.rst
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:24:03.463461 croto-2.1/coppado/
--rw-r--r--   0 defeee     (501) staff       (20)      846 2023-05-01 14:49:50.000000 croto-2.1/coppado/strings_with_arrows.py
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:24:03.463818 croto-2.1/croto/
--rw-r--r--   0 defeee     (501) staff       (20)        0 2023-05-01 21:20:56.000000 croto-2.1/croto/__init__.py
--rw-r--r--   0 defeee     (501) staff       (20)     8858 2023-05-01 21:18:17.000000 croto-2.1/croto/croto.py
-drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:24:03.464412 croto-2.1/croto.egg-info/
--rw-r--r--   0 defeee     (501) staff       (20)      299 2023-05-01 21:24:03.000000 croto-2.1/croto.egg-info/PKG-INFO
--rw-r--r--   0 defeee     (501) staff       (20)      209 2023-05-01 21:24:03.000000 croto-2.1/croto.egg-info/SOURCES.txt
--rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 21:24:03.000000 croto-2.1/croto.egg-info/dependency_links.txt
--rw-r--r--   0 defeee     (501) staff       (20)       14 2023-05-01 21:24:03.000000 croto-2.1/croto.egg-info/top_level.txt
--rw-r--r--   0 defeee     (501) staff       (20)      107 2023-05-01 21:24:03.464794 croto-2.1/setup.cfg
--rw-r--r--   0 defeee     (501) staff       (20)      394 2023-05-01 21:24:00.000000 croto-2.1/setup.py
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:30:21.748205 croto-2.2/
+-rw-r--r--   0 defeee     (501) staff       (20)      299 2023-05-01 21:30:21.748263 croto-2.2/PKG-INFO
+-rw-r--r--   0 defeee     (501) staff       (20)       28 2023-05-01 00:44:38.000000 croto-2.2/README.rst
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:30:21.746846 croto-2.2/coppado/
+-rw-r--r--   0 defeee     (501) staff       (20)      846 2023-05-01 14:49:50.000000 croto-2.2/coppado/strings_with_arrows.py
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:30:21.747266 croto-2.2/croto/
+-rw-r--r--   0 defeee     (501) staff       (20)        0 2023-05-01 21:20:56.000000 croto-2.2/croto/__init__.py
+-rw-r--r--   0 defeee     (501) staff       (20)     8858 2023-05-01 21:18:17.000000 croto-2.2/croto/croto.py
+drwxr-xr-x   0 defeee     (501) staff       (20)        0 2023-05-01 21:30:21.748054 croto-2.2/croto.egg-info/
+-rw-r--r--   0 defeee     (501) staff       (20)      299 2023-05-01 21:30:21.000000 croto-2.2/croto.egg-info/PKG-INFO
+-rw-r--r--   0 defeee     (501) staff       (20)      209 2023-05-01 21:30:21.000000 croto-2.2/croto.egg-info/SOURCES.txt
+-rw-r--r--   0 defeee     (501) staff       (20)        1 2023-05-01 21:30:21.000000 croto-2.2/croto.egg-info/dependency_links.txt
+-rw-r--r--   0 defeee     (501) staff       (20)       20 2023-05-01 21:30:21.000000 croto-2.2/croto.egg-info/top_level.txt
+-rw-r--r--   0 defeee     (501) staff       (20)      107 2023-05-01 21:30:21.748590 croto-2.2/setup.cfg
+-rw-r--r--   0 defeee     (501) staff       (20)      416 2023-05-01 21:30:13.000000 croto-2.2/setup.py
```

### Comparing `croto-2.1/coppado/strings_with_arrows.py` & `croto-2.2/coppado/strings_with_arrows.py`

 * *Files identical despite different names*

### Comparing `croto-2.1/croto/croto.py` & `croto-2.2/croto/croto.py`

 * *Files identical despite different names*

