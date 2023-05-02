# Comparing `tmp/coupml-0.1.0.tar.gz` & `tmp/coupml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coupml-0.1.0.tar", last modified: Mon May  1 10:07:24 2023, max compression
+gzip compressed data, was "coupml-0.1.1.tar", last modified: Tue May  2 07:24:12 2023, max compression
```

## Comparing `coupml-0.1.0.tar` & `coupml-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 cbrown     (502) staff       (20)        0 2023-05-01 10:07:24.712935 coupml-0.1.0/
--rw-r--r--   0 cbrown     (502) staff       (20)      551 2023-05-01 07:54:35.000000 coupml-0.1.0/LICENSE
--rw-r--r--   0 cbrown     (502) staff       (20)     4447 2023-05-01 10:07:24.712666 coupml-0.1.0/PKG-INFO
--rw-r--r--   0 cbrown     (502) staff       (20)     3463 2023-05-01 08:29:27.000000 coupml-0.1.0/README.md
-drwxr-xr-x   0 cbrown     (502) staff       (20)        0 2023-05-01 10:07:24.698683 coupml-0.1.0/coupml/
--rw-r--r--   0 cbrown     (502) staff       (20)     7724 2023-05-01 08:28:55.000000 coupml-0.1.0/coupml/__init__.py
--rw-r--r--   0 cbrown     (502) staff       (20)    28820 2023-04-30 16:03:23.000000 coupml-0.1.0/coupml/actions.py
--rw-r--r--   0 cbrown     (502) staff       (20)     2717 2023-04-30 15:49:37.000000 coupml-0.1.0/coupml/constants.py
--rw-r--r--   0 cbrown     (502) staff       (20)     2232 2023-04-30 15:23:08.000000 coupml-0.1.0/coupml/dealer.py
--rw-r--r--   0 cbrown     (502) staff       (20)    19287 2023-05-01 08:18:41.000000 coupml-0.1.0/coupml/game.py
--rw-r--r--   0 cbrown     (502) staff       (20)     7997 2023-04-30 16:11:38.000000 coupml-0.1.0/coupml/observer.py
--rw-r--r--   0 cbrown     (502) staff       (20)     1926 2023-04-30 15:23:13.000000 coupml-0.1.0/coupml/player.py
--rw-r--r--   0 cbrown     (502) staff       (20)     4855 2023-04-30 15:50:19.000000 coupml-0.1.0/coupml/utils.py
--rw-r--r--   0 cbrown     (502) staff       (20)     5345 2023-04-30 15:39:45.000000 coupml-0.1.0/coupml/view.py
-drwxr-xr-x   0 cbrown     (502) staff       (20)        0 2023-05-01 10:07:24.701930 coupml-0.1.0/coupml.egg-info/
--rw-r--r--   0 cbrown     (502) staff       (20)     4447 2023-05-01 10:07:24.000000 coupml-0.1.0/coupml.egg-info/PKG-INFO
--rw-r--r--   0 cbrown     (502) staff       (20)      395 2023-05-01 10:07:24.000000 coupml-0.1.0/coupml.egg-info/SOURCES.txt
--rw-r--r--   0 cbrown     (502) staff       (20)        1 2023-05-01 10:07:24.000000 coupml-0.1.0/coupml.egg-info/dependency_links.txt
--rw-r--r--   0 cbrown     (502) staff       (20)       24 2023-05-01 10:07:24.000000 coupml-0.1.0/coupml.egg-info/requires.txt
--rw-r--r--   0 cbrown     (502) staff       (20)        7 2023-05-01 10:07:24.000000 coupml-0.1.0/coupml.egg-info/top_level.txt
--rw-r--r--   0 cbrown     (502) staff       (20)      394 2023-05-01 10:04:13.000000 coupml-0.1.0/pyproject.toml
--rw-r--r--   0 cbrown     (502) staff       (20)       38 2023-05-01 10:07:24.712979 coupml-0.1.0/setup.cfg
-drwxr-xr-x   0 cbrown     (502) staff       (20)        0 2023-05-01 10:07:24.712154 coupml-0.1.0/test/
--rw-r--r--   0 cbrown     (502) staff       (20)    34301 2023-05-01 08:19:07.000000 coupml-0.1.0/test/test_game.py
--rw-r--r--   0 cbrown     (502) staff       (20)    21490 2023-05-01 07:55:13.000000 coupml-0.1.0/test/test_observer.py
--rw-r--r--   0 cbrown     (502) staff       (20)     9435 2023-05-01 08:19:25.000000 coupml-0.1.0/test/test_view.py
+drwxr-xr-x   0 cbrown     (502) staff       (20)        0 2023-05-02 07:24:12.591190 coupml-0.1.1/
+-rw-r--r--   0 cbrown     (502) staff       (20)      551 2023-05-01 07:54:35.000000 coupml-0.1.1/LICENSE
+-rw-r--r--   0 cbrown     (502) staff       (20)     4447 2023-05-02 07:24:12.590896 coupml-0.1.1/PKG-INFO
+-rw-r--r--   0 cbrown     (502) staff       (20)     3463 2023-05-01 08:29:27.000000 coupml-0.1.1/README.md
+drwxr-xr-x   0 cbrown     (502) staff       (20)        0 2023-05-02 07:24:12.576242 coupml-0.1.1/coupml/
+-rw-r--r--   0 cbrown     (502) staff       (20)     7724 2023-05-01 08:28:55.000000 coupml-0.1.1/coupml/__init__.py
+-rw-r--r--   0 cbrown     (502) staff       (20)    28820 2023-04-30 16:03:23.000000 coupml-0.1.1/coupml/actions.py
+-rw-r--r--   0 cbrown     (502) staff       (20)     2717 2023-04-30 15:49:37.000000 coupml-0.1.1/coupml/constants.py
+-rw-r--r--   0 cbrown     (502) staff       (20)     2232 2023-04-30 15:23:08.000000 coupml-0.1.1/coupml/dealer.py
+-rw-r--r--   0 cbrown     (502) staff       (20)    19287 2023-05-01 08:18:41.000000 coupml-0.1.1/coupml/game.py
+-rw-r--r--   0 cbrown     (502) staff       (20)     7997 2023-04-30 16:11:38.000000 coupml-0.1.1/coupml/observer.py
+-rw-r--r--   0 cbrown     (502) staff       (20)     1926 2023-04-30 15:23:13.000000 coupml-0.1.1/coupml/player.py
+-rw-r--r--   0 cbrown     (502) staff       (20)    18858 2023-05-01 10:34:55.000000 coupml-0.1.1/coupml/rule_ai.py
+-rw-r--r--   0 cbrown     (502) staff       (20)     4855 2023-04-30 15:50:19.000000 coupml-0.1.1/coupml/utils.py
+-rw-r--r--   0 cbrown     (502) staff       (20)     5345 2023-04-30 15:39:45.000000 coupml-0.1.1/coupml/view.py
+drwxr-xr-x   0 cbrown     (502) staff       (20)        0 2023-05-02 07:24:12.578808 coupml-0.1.1/coupml.egg-info/
+-rw-r--r--   0 cbrown     (502) staff       (20)     4447 2023-05-02 07:24:12.000000 coupml-0.1.1/coupml.egg-info/PKG-INFO
+-rw-r--r--   0 cbrown     (502) staff       (20)      413 2023-05-02 07:24:12.000000 coupml-0.1.1/coupml.egg-info/SOURCES.txt
+-rw-r--r--   0 cbrown     (502) staff       (20)        1 2023-05-02 07:24:12.000000 coupml-0.1.1/coupml.egg-info/dependency_links.txt
+-rw-r--r--   0 cbrown     (502) staff       (20)       24 2023-05-02 07:24:12.000000 coupml-0.1.1/coupml.egg-info/requires.txt
+-rw-r--r--   0 cbrown     (502) staff       (20)        7 2023-05-02 07:24:12.000000 coupml-0.1.1/coupml.egg-info/top_level.txt
+-rw-r--r--   0 cbrown     (502) staff       (20)      394 2023-05-02 07:22:34.000000 coupml-0.1.1/pyproject.toml
+-rw-r--r--   0 cbrown     (502) staff       (20)       38 2023-05-02 07:24:12.591241 coupml-0.1.1/setup.cfg
+drwxr-xr-x   0 cbrown     (502) staff       (20)        0 2023-05-02 07:24:12.590408 coupml-0.1.1/test/
+-rw-r--r--   0 cbrown     (502) staff       (20)    34301 2023-05-01 08:19:07.000000 coupml-0.1.1/test/test_game.py
+-rw-r--r--   0 cbrown     (502) staff       (20)    21490 2023-05-01 07:55:13.000000 coupml-0.1.1/test/test_observer.py
+-rw-r--r--   0 cbrown     (502) staff       (20)     9435 2023-05-01 08:19:25.000000 coupml-0.1.1/test/test_view.py
```

### Comparing `coupml-0.1.0/LICENSE` & `coupml-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coupml-0.1.0/PKG-INFO` & `coupml-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coupml
-Version: 0.1.0
+Version: 0.1.1
 Summary: An implementation of the card game Coup intended for machine learning
 Author-email: Chris Brown <chris@thebrown.net>
 License: Copyright 2023 Chris Brown
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
```

### Comparing `coupml-0.1.0/README.md` & `coupml-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `coupml-0.1.0/coupml/__init__.py` & `coupml-0.1.1/coupml/__init__.py`

 * *Files identical despite different names*

### Comparing `coupml-0.1.0/coupml/actions.py` & `coupml-0.1.1/coupml/actions.py`

 * *Files identical despite different names*

### Comparing `coupml-0.1.0/coupml/constants.py` & `coupml-0.1.1/coupml/constants.py`

 * *Files identical despite different names*

### Comparing `coupml-0.1.0/coupml/dealer.py` & `coupml-0.1.1/coupml/dealer.py`

 * *Files identical despite different names*

### Comparing `coupml-0.1.0/coupml/game.py` & `coupml-0.1.1/coupml/game.py`

 * *Files identical despite different names*

### Comparing `coupml-0.1.0/coupml/observer.py` & `coupml-0.1.1/coupml/observer.py`

 * *Files identical despite different names*

### Comparing `coupml-0.1.0/coupml/player.py` & `coupml-0.1.1/coupml/player.py`

 * *Files identical despite different names*

### Comparing `coupml-0.1.0/coupml/utils.py` & `coupml-0.1.1/coupml/utils.py`

 * *Files identical despite different names*

### Comparing `coupml-0.1.0/coupml/view.py` & `coupml-0.1.1/coupml/view.py`

 * *Files identical despite different names*

### Comparing `coupml-0.1.0/coupml.egg-info/PKG-INFO` & `coupml-0.1.1/coupml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coupml
-Version: 0.1.0
+Version: 0.1.1
 Summary: An implementation of the card game Coup intended for machine learning
 Author-email: Chris Brown <chris@thebrown.net>
 License: Copyright 2023 Chris Brown
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
```

### Comparing `coupml-0.1.0/test/test_game.py` & `coupml-0.1.1/test/test_game.py`

 * *Files identical despite different names*

### Comparing `coupml-0.1.0/test/test_observer.py` & `coupml-0.1.1/test/test_observer.py`

 * *Files identical despite different names*

### Comparing `coupml-0.1.0/test/test_view.py` & `coupml-0.1.1/test/test_view.py`

 * *Files identical despite different names*

