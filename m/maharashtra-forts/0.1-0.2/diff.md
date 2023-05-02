# Comparing `tmp/maharashtra_forts-0.1.macosx-10.9-x86_64.tar.gz` & `tmp/maharashtra_forts-0.2.macosx-10.9-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maharashtra_forts-0.1.macosx-10.9-x86_64.tar", last modified: Tue May  2 07:06:31 2023, max compression
+gzip compressed data, was "maharashtra_forts-0.2.macosx-10.9-x86_64.tar", last modified: Tue May  2 07:25:37 2023, max compression
```

## Comparing `maharashtra_forts-0.1.macosx-10.9-x86_64.tar` & `maharashtra_forts-0.2.macosx-10.9-x86_64.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:06:31.328844 ./
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:06:31.328897 ./Library/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:06:31.328953 ./Library/Frameworks/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:06:31.329008 ./Library/Frameworks/Python.framework/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:06:31.329062 ./Library/Frameworks/Python.framework/Versions/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:06:31.329115 ./Library/Frameworks/Python.framework/Versions/3.8/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:06:31.329168 ./Library/Frameworks/Python.framework/Versions/3.8/lib/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:06:31.329222 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:06:31.336635 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:06:31.330310 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.912671 ./
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.912725 ./Library/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.912782 ./Library/Frameworks/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.912835 ./Library/Frameworks/Python.framework/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.912890 ./Library/Frameworks/Python.framework/Versions/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.912944 ./Library/Frameworks/Python.framework/Versions/3.8/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.912997 ./Library/Frameworks/Python.framework/Versions/3.8/lib/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.913053 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.922626 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.913918 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/
 -rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:22:46.000000 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__init__.py
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:06:31.330497 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      198 2023-05-02 07:06:31.330428 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:06:31.342571 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.1-py3.8.egg-info/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)     4454 2023-05-02 07:06:31.335327 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.1-py3.8.egg-info/PKG-INFO
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      212 2023-05-02 07:06:31.336523 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.1-py3.8.egg-info/SOURCES.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        1 2023-05-02 07:06:31.335425 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.1-py3.8.egg-info/dependency_links.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)       18 2023-05-02 07:06:31.335580 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.1-py3.8.egg-info/top_level.txt
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.914105 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      198 2023-05-02 07:25:37.914033 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:25:37.926825 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.2-py3.8.egg-info/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     2373 2023-05-02 07:25:37.921044 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.2-py3.8.egg-info/PKG-INFO
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      212 2023-05-02 07:25:37.922498 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.2-py3.8.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        1 2023-05-02 07:25:37.921175 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.2-py3.8.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)       18 2023-05-02 07:25:37.921360 ./Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/maharashtra_forts-0.2-py3.8.egg-info/top_level.txt
```

