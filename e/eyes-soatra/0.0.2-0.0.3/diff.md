# Comparing `tmp/eyes_soatra-0.0.2.tar.gz` & `tmp/eyes_soatra-0.0.3.macosx-10.9-universal2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.2.tar", last modified: Tue May  2 04:57:46 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.3.macosx-10.9-universal2.tar", last modified: Tue May  2 05:05:08 2023, max compression
```

## Comparing `eyes_soatra-0.0.2.tar` & `eyes_soatra-0.0.3.macosx-10.9-universal2.tar`

### file list

```diff
@@ -1,13 +1,20 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 04:57:46.951774 eyes_soatra-0.0.2/
--rw-r--r--   0 soatra     (501) staff       (20)      543 2023-05-02 04:57:46.951600 eyes_soatra-0.0.2/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)       47 2023-05-02 03:38:24.000000 eyes_soatra-0.0.2/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 04:57:46.950764 eyes_soatra-0.0.2/eyes/
--rw-r--r--   0 soatra     (501) staff       (20)       21 2023-05-02 03:45:03.000000 eyes_soatra-0.0.2/eyes/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)    10973 2023-05-02 03:40:32.000000 eyes_soatra-0.0.2/eyes/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 04:57:46.951399 eyes_soatra-0.0.2/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      543 2023-05-02 04:57:46.000000 eyes_soatra-0.0.2/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)      188 2023-05-02 04:57:46.000000 eyes_soatra-0.0.2/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-02 04:57:46.000000 eyes_soatra-0.0.2/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)        5 2023-05-02 04:57:46.000000 eyes_soatra-0.0.2/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-02 04:57:46.951836 eyes_soatra-0.0.2/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1062 2023-05-02 04:57:30.000000 eyes_soatra-0.0.2/setup.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:05:08.910757 ./
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:05:08.910811 ./Library/
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:05:08.910867 ./Library/Frameworks/
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:05:08.910915 ./Library/Frameworks/Python.framework/
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:05:08.910962 ./Library/Frameworks/Python.framework/Versions/
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:05:08.911008 ./Library/Frameworks/Python.framework/Versions/3.10/
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:05:08.911056 ./Library/Frameworks/Python.framework/Versions/3.10/lib/
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:05:08.911104 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:05:08.919113 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:05:08.912434 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes/
+-rw-r--r--   0 soatra     (501) staff       (20)       21 2023-05-02 03:45:03.000000 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:05:08.913667 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes/__pycache__/
+-rw-r--r--   0 soatra     (501) staff       (20)      214 2023-05-02 05:05:08.912541 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 soatra     (501) staff       (20)     5691 2023-05-02 05:05:08.913607 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes/__pycache__/eyes.cpython-310.pyc
+-rw-r--r--   0 soatra     (501) staff       (20)    10973 2023-05-02 03:40:32.000000 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:05:08.919794 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes_soatra-0.0.3-py3.10.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      543 2023-05-02 05:05:08.848751 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes_soatra-0.0.3-py3.10.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)      188 2023-05-02 05:05:08.864363 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes_soatra-0.0.3-py3.10.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-02 05:05:08.848888 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes_soatra-0.0.3-py3.10.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        5 2023-05-02 05:05:08.849047 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes_soatra-0.0.3-py3.10.egg-info/top_level.txt
```

### Comparing `eyes_soatra-0.0.2/PKG-INFO` & `./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes_soatra-0.0.3-py3.10.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eyes_soatra
-Version: 0.0.2
+Name: eyes-soatra
+Version: 0.0.3
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: requests,requests_html,jellyfish,translate,re
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.2/eyes/eyes.py` & `./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes/eyes.py`

 * *Files identical despite different names*

