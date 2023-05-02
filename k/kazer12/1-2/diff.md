# Comparing `tmp/kazer12-1.tar.gz` & `tmp/kazer12-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kazer12-1.tar", last modified: Tue May  2 21:34:32 2023, max compression
+gzip compressed data, was "kazer12-2.tar", last modified: Tue May  2 21:37:10 2023, max compression
```

## Comparing `kazer12-1.tar` & `kazer12-2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 21:34:32.029558 kazer12-1/
--rw-rw-rw-   0        0        0    14722 2023-05-02 21:34:32.030558 kazer12-1/PKG-INFO
--rw-rw-rw-   0        0        0    13715 2023-03-04 16:03:05.000000 kazer12-1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 21:34:31.993570 kazer12-1/kazer12/
--rw-rw-rw-   0        0        0       69 2023-03-04 16:06:10.000000 kazer12-1/kazer12/__init__.py
--rw-rw-rw-   0        0        0    12024 2023-03-04 15:48:27.000000 kazer12-1/kazer12/bettercolor_file.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:34:32.027559 kazer12-1/kazer12.egg-info/
--rw-rw-rw-   0        0        0    14722 2023-05-02 21:34:31.000000 kazer12-1/kazer12.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-05-02 21:34:31.000000 kazer12-1/kazer12.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 21:34:31.000000 kazer12-1/kazer12.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-02 21:34:31.000000 kazer12-1/kazer12.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 21:34:31.000000 kazer12-1/kazer12.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-05-02 21:34:32.037556 kazer12-1/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-05-02 21:34:03.000000 kazer12-1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:37:10.485605 kazer12-2/
+-rw-rw-rw-   0        0        0    14722 2023-05-02 21:37:10.486619 kazer12-2/PKG-INFO
+-rw-rw-rw-   0        0        0    13715 2023-03-04 16:03:05.000000 kazer12-2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 21:37:10.458633 kazer12-2/kazer12/
+-rw-rw-rw-   0        0        0       69 2023-03-04 16:06:10.000000 kazer12-2/kazer12/__init__.py
+-rw-rw-rw-   0        0        0    12024 2023-03-04 15:48:27.000000 kazer12-2/kazer12/bettercolor_file.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:37:10.484606 kazer12-2/kazer12.egg-info/
+-rw-rw-rw-   0        0        0    14722 2023-05-02 21:37:10.000000 kazer12-2/kazer12.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-05-02 21:37:10.000000 kazer12-2/kazer12.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 21:37:10.000000 kazer12-2/kazer12.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-02 21:37:10.000000 kazer12-2/kazer12.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 21:37:10.000000 kazer12-2/kazer12.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-05-02 21:37:10.488606 kazer12-2/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-05-02 21:36:24.000000 kazer12-2/setup.py
```

### Comparing `kazer12-1/PKG-INFO` & `kazer12-2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kazer12
-Version: 1
+Version: 2
 Summary: Pure-python Colors implementation
 Home-page: https://github.com/tartley/colorama
 Author: Jonathan Hartley
 Author-email: tartley@tartley.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kazer12-1/README.md` & `kazer12-2/README.md`

 * *Files identical despite different names*

### Comparing `kazer12-1/kazer12/bettercolor_file.py` & `kazer12-2/kazer12/bettercolor_file.py`

 * *Files identical despite different names*

### Comparing `kazer12-1/kazer12.egg-info/PKG-INFO` & `kazer12-2/kazer12.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kazer12
-Version: 1
+Version: 2
 Summary: Pure-python Colors implementation
 Home-page: https://github.com/tartley/colorama
 Author: Jonathan Hartley
 Author-email: tartley@tartley.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kazer12-1/setup.py` & `kazer12-2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kazer12',
-    version='1',
+    version='2',
     author='Jonathan Hartley',
     author_email='tartley@tartley.com',
     description='Pure-python Colors implementation',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/tartley/colorama',
     packages=find_packages(),
```

