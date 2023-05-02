# Comparing `tmp/pycozo-0.6.0.tar.gz` & `tmp/pycozo-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycozo-0.6.0.tar", last modified: Thu Apr 20 04:44:22 2023, max compression
+gzip compressed data, was "pycozo-0.7.0.tar", last modified: Tue May  2 15:48:58 2023, max compression
```

## Comparing `pycozo-0.6.0.tar` & `pycozo-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-04-20 04:44:22.197333 pycozo-0.6.0/
--rw-r--r--   0 zh217      (501) staff       (20)    16724 2022-11-30 04:19:19.000000 pycozo-0.6.0/LICENSE.txt
--rw-r--r--   0 zh217      (501) staff       (20)      469 2023-04-20 04:44:22.197204 pycozo-0.6.0/PKG-INFO
--rw-r--r--   0 zh217      (501) staff       (20)     7974 2023-01-21 11:49:23.000000 pycozo-0.6.0/README.md
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-04-20 04:44:22.196396 pycozo-0.6.0/pycozo/
--rw-r--r--   0 zh217      (501) staff       (20)      284 2022-11-30 04:32:35.000000 pycozo-0.6.0/pycozo/__init__.py
--rw-r--r--   0 zh217      (501) staff       (20)     9665 2023-01-21 11:49:23.000000 pycozo-0.6.0/pycozo/client.py
--rw-r--r--   0 zh217      (501) staff       (20)     4619 2022-12-28 04:03:29.000000 pycozo-0.6.0/pycozo/ext_impl.py
--rw-r--r--   0 zh217      (501) staff       (20)      378 2022-11-30 04:32:35.000000 pycozo-0.6.0/pycozo/ipyext.py
--rw-r--r--   0 zh217      (501) staff       (20)      677 2022-11-30 04:32:35.000000 pycozo-0.6.0/pycozo/ipyext_direct.py
--rw-r--r--   0 zh217      (501) staff       (20)     2046 2023-01-21 11:49:23.000000 pycozo-0.6.0/pycozo/test_client.py
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-04-20 04:44:22.197036 pycozo-0.6.0/pycozo.egg-info/
--rw-r--r--   0 zh217      (501) staff       (20)      469 2023-04-20 04:44:22.000000 pycozo-0.6.0/pycozo.egg-info/PKG-INFO
--rw-r--r--   0 zh217      (501) staff       (20)      297 2023-04-20 04:44:22.000000 pycozo-0.6.0/pycozo.egg-info/SOURCES.txt
--rw-r--r--   0 zh217      (501) staff       (20)        1 2023-04-20 04:44:22.000000 pycozo-0.6.0/pycozo.egg-info/dependency_links.txt
--rw-r--r--   0 zh217      (501) staff       (20)       77 2023-04-20 04:44:22.000000 pycozo-0.6.0/pycozo.egg-info/requires.txt
--rw-r--r--   0 zh217      (501) staff       (20)        7 2023-04-20 04:44:22.000000 pycozo-0.6.0/pycozo.egg-info/top_level.txt
--rw-r--r--   0 zh217      (501) staff       (20)       38 2023-04-20 04:44:22.197371 pycozo-0.6.0/setup.cfg
--rw-r--r--   0 zh217      (501) staff       (20)      920 2023-04-20 04:44:07.000000 pycozo-0.6.0/setup.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-02 15:48:58.860654 pycozo-0.7.0/
+-rw-r--r--   0 zh217      (501) staff       (20)    16724 2022-11-30 04:19:19.000000 pycozo-0.7.0/LICENSE.txt
+-rw-r--r--   0 zh217      (501) staff       (20)      469 2023-05-02 15:48:58.860538 pycozo-0.7.0/PKG-INFO
+-rw-r--r--   0 zh217      (501) staff       (20)     7974 2023-01-21 11:49:23.000000 pycozo-0.7.0/README.md
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-02 15:48:58.859782 pycozo-0.7.0/pycozo/
+-rw-r--r--   0 zh217      (501) staff       (20)      284 2022-11-30 04:32:35.000000 pycozo-0.7.0/pycozo/__init__.py
+-rw-r--r--   0 zh217      (501) staff       (20)     9665 2023-01-21 11:49:23.000000 pycozo-0.7.0/pycozo/client.py
+-rw-r--r--   0 zh217      (501) staff       (20)     4619 2022-12-28 04:03:29.000000 pycozo-0.7.0/pycozo/ext_impl.py
+-rw-r--r--   0 zh217      (501) staff       (20)      378 2022-11-30 04:32:35.000000 pycozo-0.7.0/pycozo/ipyext.py
+-rw-r--r--   0 zh217      (501) staff       (20)      677 2022-11-30 04:32:35.000000 pycozo-0.7.0/pycozo/ipyext_direct.py
+-rw-r--r--   0 zh217      (501) staff       (20)     2046 2023-01-21 11:49:23.000000 pycozo-0.7.0/pycozo/test_client.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-02 15:48:58.860372 pycozo-0.7.0/pycozo.egg-info/
+-rw-r--r--   0 zh217      (501) staff       (20)      469 2023-05-02 15:48:58.000000 pycozo-0.7.0/pycozo.egg-info/PKG-INFO
+-rw-r--r--   0 zh217      (501) staff       (20)      297 2023-05-02 15:48:58.000000 pycozo-0.7.0/pycozo.egg-info/SOURCES.txt
+-rw-r--r--   0 zh217      (501) staff       (20)        1 2023-05-02 15:48:58.000000 pycozo-0.7.0/pycozo.egg-info/dependency_links.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       77 2023-05-02 15:48:58.000000 pycozo-0.7.0/pycozo.egg-info/requires.txt
+-rw-r--r--   0 zh217      (501) staff       (20)        7 2023-05-02 15:48:58.000000 pycozo-0.7.0/pycozo.egg-info/top_level.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-02 15:48:58.860695 pycozo-0.7.0/setup.cfg
+-rw-r--r--   0 zh217      (501) staff       (20)      920 2023-05-02 15:29:42.000000 pycozo-0.7.0/setup.py
```

### Comparing `pycozo-0.6.0/LICENSE.txt` & `pycozo-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycozo-0.6.0/README.md` & `pycozo-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pycozo-0.6.0/pycozo/client.py` & `pycozo-0.7.0/pycozo/client.py`

 * *Files identical despite different names*

### Comparing `pycozo-0.6.0/pycozo/ext_impl.py` & `pycozo-0.7.0/pycozo/ext_impl.py`

 * *Files identical despite different names*

### Comparing `pycozo-0.6.0/pycozo/ipyext_direct.py` & `pycozo-0.7.0/pycozo/ipyext_direct.py`

 * *Files identical despite different names*

### Comparing `pycozo-0.6.0/pycozo/test_client.py` & `pycozo-0.7.0/pycozo/test_client.py`

 * *Files identical despite different names*

### Comparing `pycozo-0.6.0/setup.py` & `pycozo-0.7.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.
 #  If a copy of the MPL was not distributed with this file,
 #  You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from setuptools import setup
 
-VERSION = '0.6.0'
+VERSION = '0.7.0'
 
 setup(
     name='pycozo',
     version=VERSION,
     packages=['pycozo'],
     url='',
     license='MPL-2.0',
```

