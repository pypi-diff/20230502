# Comparing `tmp/python-voi-0.0.1.tar.gz` & `tmp/python-voi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-voi-0.0.1.tar", last modified: Tue May  2 16:37:45 2023, max compression
+gzip compressed data, was "python-voi-0.0.2.tar", last modified: Tue May  2 16:40:06 2023, max compression
```

## Comparing `python-voi-0.0.1.tar` & `python-voi-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 cfpark00  (1000) cfpark00  (1000)        0 2023-05-02 16:37:45.080489 python-voi-0.0.1/
--rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)     2164 2023-05-02 16:37:45.080489 python-voi-0.0.1/PKG-INFO
--rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)     1936 2023-05-02 16:17:24.000000 python-voi-0.0.1/README.md
-drwxrwxr-x   0 cfpark00  (1000) cfpark00  (1000)        0 2023-05-02 16:37:45.080489 python-voi-0.0.1/python_voi.egg-info/
--rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)     2164 2023-05-02 16:37:45.000000 python-voi-0.0.1/python_voi.egg-info/PKG-INFO
--rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)      196 2023-05-02 16:37:45.000000 python-voi-0.0.1/python_voi.egg-info/SOURCES.txt
--rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)        1 2023-05-02 16:37:45.000000 python-voi-0.0.1/python_voi.egg-info/dependency_links.txt
--rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)       12 2023-05-02 16:37:45.000000 python-voi-0.0.1/python_voi.egg-info/requires.txt
--rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)        6 2023-05-02 16:37:45.000000 python-voi-0.0.1/python_voi.egg-info/top_level.txt
--rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)     5142 2023-05-02 14:14:30.000000 python-voi-0.0.1/pyvoi.py
--rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)       38 2023-05-02 16:37:45.080489 python-voi-0.0.1/setup.cfg
--rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)      501 2023-05-02 16:34:30.000000 python-voi-0.0.1/setup.py
+drwxrwxr-x   0 cfpark00  (1000) cfpark00  (1000)        0 2023-05-02 16:40:06.828824 python-voi-0.0.2/
+-rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)     2169 2023-05-02 16:40:06.824823 python-voi-0.0.2/PKG-INFO
+-rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)     1941 2023-05-02 16:39:18.000000 python-voi-0.0.2/README.md
+drwxrwxr-x   0 cfpark00  (1000) cfpark00  (1000)        0 2023-05-02 16:40:06.824823 python-voi-0.0.2/python_voi.egg-info/
+-rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)     2169 2023-05-02 16:40:06.000000 python-voi-0.0.2/python_voi.egg-info/PKG-INFO
+-rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)      196 2023-05-02 16:40:06.000000 python-voi-0.0.2/python_voi.egg-info/SOURCES.txt
+-rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)        1 2023-05-02 16:40:06.000000 python-voi-0.0.2/python_voi.egg-info/dependency_links.txt
+-rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)       12 2023-05-02 16:40:06.000000 python-voi-0.0.2/python_voi.egg-info/requires.txt
+-rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)        6 2023-05-02 16:40:06.000000 python-voi-0.0.2/python_voi.egg-info/top_level.txt
+-rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)     5142 2023-05-02 14:14:30.000000 python-voi-0.0.2/pyvoi.py
+-rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)       38 2023-05-02 16:40:06.828824 python-voi-0.0.2/setup.cfg
+-rw-rw-r--   0 cfpark00  (1000) cfpark00  (1000)      501 2023-05-02 16:39:57.000000 python-voi-0.0.2/setup.py
```

### Comparing `python-voi-0.0.1/PKG-INFO` & `python-voi-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-voi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python implementation of Variation of Information
 Author: Core Francisco Park
 Author-email: cfpark00@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # pyvoi: Variation of Information in numpy/torch
@@ -12,15 +12,15 @@
 Calculate the Variation of Information for two clusterings
 
 References:
 Meila, Marina (2003). Comparing Clusterings by the Variation of Information. Learning Theory and Kernel Machines: 173–187
 
 ## Installation
 
-    pip install pyvoi
+    pip install python-voi
 
 ## Usage
 
 By default, pyvoi uses torch to compute the variation of information.
 
 ### To get VI values only
     import pyvoi
```

### Comparing `python-voi-0.0.1/README.md` & `python-voi-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Calculate the Variation of Information for two clusterings
 
 References:
 Meila, Marina (2003). Comparing Clusterings by the Variation of Information. Learning Theory and Kernel Machines: 173–187
 
 ## Installation
 
-    pip install pyvoi
+    pip install python-voi
 
 ## Usage
 
 By default, pyvoi uses torch to compute the variation of information.
 
 ### To get VI values only
     import pyvoi
```

### Comparing `python-voi-0.0.1/python_voi.egg-info/PKG-INFO` & `python-voi-0.0.2/python_voi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-voi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python implementation of Variation of Information
 Author: Core Francisco Park
 Author-email: cfpark00@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # pyvoi: Variation of Information in numpy/torch
@@ -12,15 +12,15 @@
 Calculate the Variation of Information for two clusterings
 
 References:
 Meila, Marina (2003). Comparing Clusterings by the Variation of Information. Learning Theory and Kernel Machines: 173–187
 
 ## Installation
 
-    pip install pyvoi
+    pip install python-voi
 
 ## Usage
 
 By default, pyvoi uses torch to compute the variation of information.
 
 ### To get VI values only
     import pyvoi
```

### Comparing `python-voi-0.0.1/pyvoi.py` & `python-voi-0.0.2/pyvoi.py`

 * *Files identical despite different names*

