# Comparing `tmp/maharashtra-forts-0.7.tar.gz` & `tmp/maharashtra-forts-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maharashtra-forts-0.7.tar", last modified: Tue May  2 12:37:32 2023, max compression
+gzip compressed data, was "maharashtra-forts-0.8.tar", last modified: Tue May  2 12:53:27 2023, max compression
```

## Comparing `maharashtra-forts-0.7.tar` & `maharashtra-forts-0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:37:32.143425 maharashtra-forts-0.7/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)     2367 2023-05-02 12:37:32.143264 maharashtra-forts-0.7/PKG-INFO
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)     1552 2023-05-02 07:47:39.000000 maharashtra-forts-0.7/README.md
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:37:32.140838 maharashtra-forts-0.7/maharashtra_forts/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:22:46.000000 maharashtra-forts-0.7/maharashtra_forts/__init__.py
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:37:32.143042 maharashtra-forts-0.7/maharashtra_forts/forts/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 06:48:51.000000 maharashtra-forts-0.7/maharashtra_forts/forts/__init__.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/harishchandragad_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/lohagad_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/pratapgad_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/purandar_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/raigad_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/rajgad_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/shivneri_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/sinhagad_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/tikona_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/torna_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      487 2023-05-02 07:41:41.000000 maharashtra-forts-0.7/maharashtra_forts/maharashtra_forts.py
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:37:32.141665 maharashtra-forts-0.7/maharashtra_forts.egg-info/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)     2367 2023-05-02 12:37:32.000000 maharashtra-forts-0.7/maharashtra_forts.egg-info/PKG-INFO
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      696 2023-05-02 12:37:32.000000 maharashtra-forts-0.7/maharashtra_forts.egg-info/SOURCES.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        1 2023-05-02 12:37:32.000000 maharashtra-forts-0.7/maharashtra_forts.egg-info/dependency_links.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)       18 2023-05-02 12:37:32.000000 maharashtra-forts-0.7/maharashtra_forts.egg-info/top_level.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)       38 2023-05-02 12:37:32.143485 maharashtra-forts-0.7/setup.cfg
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)     1072 2023-05-02 12:35:48.000000 maharashtra-forts-0.7/setup.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:53:27.105113 maharashtra-forts-0.8/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     2367 2023-05-02 12:53:27.104968 maharashtra-forts-0.8/PKG-INFO
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     1552 2023-05-02 07:47:39.000000 maharashtra-forts-0.8/README.md
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:53:27.102748 maharashtra-forts-0.8/maharashtra_forts/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:22:46.000000 maharashtra-forts-0.8/maharashtra_forts/__init__.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:53:27.104737 maharashtra-forts-0.8/maharashtra_forts/forts/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 06:48:51.000000 maharashtra-forts-0.8/maharashtra_forts/forts/__init__.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.8/maharashtra_forts/forts/harishchandragad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.8/maharashtra_forts/forts/lohagad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.8/maharashtra_forts/forts/pratapgad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.8/maharashtra_forts/forts/purandar_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.8/maharashtra_forts/forts/raigad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)       77 2023-05-02 12:52:51.000000 maharashtra-forts-0.8/maharashtra_forts/forts/rajgad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.8/maharashtra_forts/forts/shivneri_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.8/maharashtra_forts/forts/sinhagad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.8/maharashtra_forts/forts/tikona_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.8/maharashtra_forts/forts/torna_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      487 2023-05-02 07:41:41.000000 maharashtra-forts-0.8/maharashtra_forts/get_forts.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:53:27.103321 maharashtra-forts-0.8/maharashtra_forts.egg-info/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     2367 2023-05-02 12:53:27.000000 maharashtra-forts-0.8/maharashtra_forts.egg-info/PKG-INFO
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      688 2023-05-02 12:53:27.000000 maharashtra-forts-0.8/maharashtra_forts.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        1 2023-05-02 12:53:27.000000 maharashtra-forts-0.8/maharashtra_forts.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)       18 2023-05-02 12:53:27.000000 maharashtra-forts-0.8/maharashtra_forts.egg-info/top_level.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)       38 2023-05-02 12:53:27.105161 maharashtra-forts-0.8/setup.cfg
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     1072 2023-05-02 12:53:16.000000 maharashtra-forts-0.8/setup.py
```

### Comparing `maharashtra-forts-0.7/PKG-INFO` & `maharashtra-forts-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maharashtra-forts
-Version: 0.7
+Version: 0.8
 Summary: A Python library for exploring forts in Maharashtra
 Home-page: https://github.com/your-username/maharashtra-forts
 Author: Rahul Bhoyar
 Author-email: rahulbhoyaroffice@gmail.com
 License: UNKNOWN
 Description: # Maharashtra Forts
```

### Comparing `maharashtra-forts-0.7/README.md` & `maharashtra-forts-0.8/README.md`

 * *Files identical despite different names*

### Comparing `maharashtra-forts-0.7/maharashtra_forts.egg-info/PKG-INFO` & `maharashtra-forts-0.8/maharashtra_forts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maharashtra-forts
-Version: 0.7
+Version: 0.8
 Summary: A Python library for exploring forts in Maharashtra
 Home-page: https://github.com/your-username/maharashtra-forts
 Author: Rahul Bhoyar
 Author-email: rahulbhoyaroffice@gmail.com
 License: UNKNOWN
 Description: # Maharashtra Forts
```

### Comparing `maharashtra-forts-0.7/maharashtra_forts.egg-info/SOURCES.txt` & `maharashtra-forts-0.8/maharashtra_forts.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 README.md
 setup.py
 maharashtra_forts/__init__.py
-maharashtra_forts/maharashtra_forts.py
+maharashtra_forts/get_forts.py
 maharashtra_forts.egg-info/PKG-INFO
 maharashtra_forts.egg-info/SOURCES.txt
 maharashtra_forts.egg-info/dependency_links.txt
 maharashtra_forts.egg-info/top_level.txt
 maharashtra_forts/forts/__init__.py
 maharashtra_forts/forts/harishchandragad_fort.py
 maharashtra_forts/forts/lohagad_fort.py
```

### Comparing `maharashtra-forts-0.7/setup.py` & `maharashtra-forts-0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="maharashtra-forts", # Replace with the name of your package
-    version="0.7", # Replace with the version of your package
+    version="0.8", # Replace with the version of your package
     author="Rahul Bhoyar",
     author_email="rahulbhoyaroffice@gmail.com",
     description="A Python library for exploring forts in Maharashtra",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/your-username/maharashtra-forts",
     packages=setuptools.find_packages(),
```

