# Comparing `tmp/mpopt_lulav-0.2.tar.gz` & `tmp/mpopt_lulav-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpopt_lulav-0.2.tar", last modified: Tue May  2 11:19:13 2023, max compression
+gzip compressed data, was "mpopt_lulav-0.3.tar", last modified: Tue May  2 11:23:37 2023, max compression
```

## Comparing `mpopt_lulav-0.2.tar` & `mpopt_lulav-0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxr-xr-x   0 glebteplov   (501) staff       (20)        0 2023-05-02 11:19:13.456266 mpopt_lulav-0.2/
--rw-r--r--   0 glebteplov   (501) staff       (20)      757 2023-05-02 11:19:13.456415 mpopt_lulav-0.2/PKG-INFO
-drwxr-xr-x   0 glebteplov   (501) staff       (20)        0 2023-05-02 11:19:13.456153 mpopt_lulav-0.2/mpopt_lulav/
--rw-r--r--   0 glebteplov   (501) staff       (20)       30 2023-05-02 11:16:40.274757 mpopt_lulav-0.2/mpopt_lulav/__init__.py
--rw-r--r--   0 glebteplov   (501) staff       (20)   130904 2023-04-25 08:47:09.109647 mpopt_lulav-0.2/mpopt_lulav/mpopt_lulav.py
--rw-r--r--   0 glebteplov   (501) staff       (20)       39 2023-05-02 09:29:09.632076 mpopt_lulav-0.2/setup.cfg
--rw-r--r--   0 glebteplov   (501) staff       (20)      938 2023-05-02 11:19:00.288527 mpopt_lulav-0.2/setup.py
+drwxr-xr-x   0 glebteplov   (501) staff       (20)        0 2023-05-02 11:23:37.244911 mpopt_lulav-0.3/
+-rw-r--r--   0 glebteplov   (501) staff       (20)      757 2023-05-02 11:23:37.245054 mpopt_lulav-0.3/PKG-INFO
+drwxr-xr-x   0 glebteplov   (501) staff       (20)        0 2023-05-02 11:23:37.244325 mpopt_lulav-0.3/mpopt_lulav/
+-rw-r--r--   0 glebteplov   (501) staff       (20)      343 2023-05-02 11:22:34.655909 mpopt_lulav-0.3/mpopt_lulav/__init__.py
+-rw-r--r--   0 glebteplov   (501) staff       (20)   130904 2023-04-25 08:47:09.109647 mpopt_lulav-0.3/mpopt_lulav/mpopt_lulav.py
+-rw-r--r--   0 glebteplov   (501) staff       (20)       39 2023-05-02 09:29:09.632076 mpopt_lulav-0.3/setup.cfg
+-rw-r--r--   0 glebteplov   (501) staff       (20)      938 2023-05-02 11:23:24.014193 mpopt_lulav-0.3/setup.py
```

### Comparing `mpopt_lulav-0.2/PKG-INFO` & `mpopt_lulav-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mpopt_lulav
-Version: 0.2
+Version: 0.3
 Summary: Optimal control lib modified by Lulav Space
 Home-page: https://github.com/lulav/mpopt_lulav
 Author: gtep
 Author-email: gleb@lulav.space
 License: MIT
 Download-URL: https://github.com/lulav/mpopt_lulav/archive/refs/tags/v0.1.tar.gz
 Description: UNKNOWN
```

### Comparing `mpopt_lulav-0.2/mpopt_lulav/mpopt_lulav.py` & `mpopt_lulav-0.3/mpopt_lulav/mpopt_lulav.py`

 * *Files identical despite different names*

### Comparing `mpopt_lulav-0.2/setup.py` & `mpopt_lulav-0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'mpopt_lulav',   
   packages = ['mpopt_lulav'], 
-  version = '0.2', 
+  version = '0.3', 
   license='MIT',   
   description = 'Optimal control lib modified by Lulav Space', 
   author = 'gtep',   
   author_email = 'gleb@lulav.space', 
   url = 'https://github.com/lulav/mpopt_lulav',
   download_url = 'https://github.com/lulav/mpopt_lulav/archive/refs/tags/v0.1.tar.gz', 
   keywords = ['Optimal', 'Control', 'Lulav'],
```

