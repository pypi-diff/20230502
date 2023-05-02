# Comparing `tmp/maharashtra_forts-0.2.macosx-10.9-x86_64.tar.gz` & `tmp/maharashtra_forts-0.3.macosx-10.9-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maharashtra_forts-0.2.macosx-10.9-x86_64.tar", last modified: Tue May  2 07:25:37 2023, max compression
+gzip compressed data, was "maharashtra_forts-0.3.macosx-10.9-x86_64.tar", last modified: Tue May  2 07:29:54 2023, max compression
```

## Comparing `maharashtra_forts-0.2.macosx-10.9-x86_64.tar` & `maharashtra_forts-0.3.macosx-10.9-x86_64.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.912671 ./
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.912725 ./Library/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.912782 ./Library/Frameworks/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.912835 ./Library/Frameworks/Python.framework/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.912890 ./Library/Frameworks/Python.framework/Versions/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.912944 ./Library/Frameworks/Python.framework/Versions/3.8/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.912997 ./Library/Frameworks/Python.framework/Versions/3.8/lib/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.913053 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.922626 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.913918 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:29:54.805413 ./
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:29:54.805475 ./Library/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:29:54.805536 ./Library/Frameworks/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:29:54.805734 ./Library/Frameworks/Python.framework/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:29:54.805821 ./Library/Frameworks/Python.framework/Versions/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:29:54.805887 ./Library/Frameworks/Python.framework/Versions/3.8/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:29:54.805947 ./Library/Frameworks/Python.framework/Versions/3.8/lib/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:29:54.806006 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:29:54.816548 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:29:54.807023 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/
 -rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:22:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__init__.py
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.914105 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      198 2023-05-02 07:25:37.914033 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.926825 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.2-py3.8.egg-info/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)     2373 2023-05-02 07:25:37.921044 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.2-py3.8.egg-info/PKG-INFO
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      212 2023-05-02 07:25:37.922498 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.2-py3.8.egg-info/SOURCES.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        1 2023-05-02 07:25:37.921175 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.2-py3.8.egg-info/dependency_links.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)       18 2023-05-02 07:25:37.921360 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.2-py3.8.egg-info/top_level.txt
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:29:54.807230 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      198 2023-05-02 07:29:54.807154 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:29:54.820137 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3-py3.8.egg-info/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     2373 2023-05-02 07:29:54.814826 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3-py3.8.egg-info/PKG-INFO
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      212 2023-05-02 07:29:54.816384 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3-py3.8.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        1 2023-05-02 07:29:54.814966 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3-py3.8.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)       18 2023-05-02 07:29:54.815126 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3-py3.8.egg-info/top_level.txt
```

### Comparing `./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.2-py3.8.egg-info/PKG-INFO` & `./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3-py3.8.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maharashtra-forts
-Version: 0.2
+Version: 0.3
 Summary: This is library created for all Fort Lovers in Maharashtra
 Home-page: https://github.com/rahulbhoyar1995/maharashtra-forts-library
 Author: Rahul Bhoyar
 Author-email: rahulbhoyaroffice@gmail.com
 License: UNKNOWN
 Description: # Maharashtra Forts
         
@@ -39,15 +39,15 @@
         
         ## License
         
         Maharashtra Forts is distributed under the MIT license. Please see the LICENSE file for more information.
         
         ## Contact
         
-        If you have any questions, comments, or concerns about Maharashtra Forts, please feel free to contact us at rahulbhoyaroffice[@gmail.co](mailto:maharashtra_forts@gmail.com)m
+        If you have any questions, comments, or concerns about Maharashtra Forts, please feel free to contact us at [maharashtra_forts@gmail.com](mailto:maharashtra_forts@gmail.com)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

