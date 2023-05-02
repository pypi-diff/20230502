# Comparing `tmp/maharashtra_forts-0.3.1.macosx-10.9-x86_64.tar.gz` & `tmp/maharashtra-forts-0.3.2.macosx-10.9-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maharashtra_forts-0.3.1.macosx-10.9-x86_64.tar", last modified: Tue May  2 07:42:52 2023, max compression
+gzip compressed data, was "maharashtra-forts-0.3.2.macosx-10.9-x86_64.tar", last modified: Tue May  2 12:00:57 2023, max compression
```

## Comparing `maharashtra_forts-0.3.1.macosx-10.9-x86_64.tar` & `maharashtra-forts-0.3.2.macosx-10.9-x86_64.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:42:52.477071 ./
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:42:52.477126 ./Library/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:42:52.477183 ./Library/Frameworks/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:42:52.477237 ./Library/Frameworks/Python.framework/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:42:52.477290 ./Library/Frameworks/Python.framework/Versions/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:42:52.477346 ./Library/Frameworks/Python.framework/Versions/3.8/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:42:52.477403 ./Library/Frameworks/Python.framework/Versions/3.8/lib/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:42:52.477458 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:42:52.488738 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:42:52.478924 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.544891 ./
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.544948 ./Library/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.545002 ./Library/Frameworks/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.545055 ./Library/Frameworks/Python.framework/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.545111 ./Library/Frameworks/Python.framework/Versions/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.545165 ./Library/Frameworks/Python.framework/Versions/3.8/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.545218 ./Library/Frameworks/Python.framework/Versions/3.8/lib/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.545273 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.558908 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.547723 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra-forts/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:22:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra-forts/__init__.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.548954 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra-forts/__pycache__/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      198 2023-05-02 12:00:57.548874 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra-forts/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      591 2023-05-02 12:00:57.548537 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra-forts/__pycache__/get_forts.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      487 2023-05-02 07:41:41.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra-forts/get_forts.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.549180 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/
 -rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:22:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__init__.py
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:42:52.479394 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      198 2023-05-02 07:42:52.479330 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      591 2023-05-02 07:42:52.479040 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/get_forts.cpython-38.pyc
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.549599 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      198 2023-05-02 12:00:57.549546 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      591 2023-05-02 12:00:57.549294 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/get_forts.cpython-38.pyc
 -rw-r--r--   0 rahulbhoyar   (501) staff       (20)      487 2023-05-02 07:41:41.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/get_forts.py
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:42:52.489712 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.1-py3.8.egg-info/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)     2369 2023-05-02 07:42:52.485984 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.1-py3.8.egg-info/PKG-INFO
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      243 2023-05-02 07:42:52.488572 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.1-py3.8.egg-info/SOURCES.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        1 2023-05-02 07:42:52.486361 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.1-py3.8.egg-info/dependency_links.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)       18 2023-05-02 07:42:52.486789 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.1-py3.8.egg-info/top_level.txt
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:00:57.563251 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.2-py3.8.egg-info/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     2386 2023-05-02 12:00:57.557086 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.2-py3.8.egg-info/PKG-INFO
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      243 2023-05-02 12:00:57.558763 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.2-py3.8.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        1 2023-05-02 12:00:57.557224 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.2-py3.8.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)       18 2023-05-02 12:00:57.557389 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.2-py3.8.egg-info/top_level.txt
```

### Comparing `./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.1-py3.8.egg-info/PKG-INFO` & `./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.3.2-py3.8.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: maharashtra-forts
-Version: 0.3.1
+Version: 0.3.2
 Summary: This is library created for all Fort Lovers in Maharashtra
 Home-page: https://github.com/rahulbhoyar1995/maharashtra-forts-library
 Author: Rahul Bhoyar
 Author-email: rahulbhoyaroffice@gmail.com
 License: UNKNOWN
 Description: # Maharashtra Forts
         
         This Python package provides information about the forts in the state of Maharashtra, India. The data has been collected from various sources and compiled into a convenient package for easy access and use.
         
         ## Installation
         
         To install Maharashtra Forts, simply use `pip`:
         
-        pip install maharashtra-forts
+        `pip install maharashtra-forts`
         
         ## Usage
         
         To use Maharashtra Forts, first import the package:
         
-        import maharashtra_forts
+        `import maharashtra_forts`
         
         Then, you can access the information about the forts using the `get_forts()` function:
         
-        all_forts = maharashtra_forts.all_forts()
-        print(all_forts)
+        `all_forts = maharashtra_forts.all_forts()`
+        
+        `print(all_forts)`
         
         This will print a list of dictionaries, with each dictionary containing information about a fort, including its name, location, and historical significance.
         
         ## Data
         
         The data in Maharashtra Forts has been collected from various sources, including historical texts, government archives, and local historians. We have done our best to ensure the accuracy of the data, but please note that some information may be incomplete or outdated.
```

