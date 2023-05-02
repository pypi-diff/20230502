# Comparing `tmp/eyes_soatra-0.0.4.macosx-10.9-universal2.tar.gz` & `tmp/eyes_soatra-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.4.macosx-10.9-universal2.tar", last modified: Tue May  2 05:07:47 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.5.tar", last modified: Tue May  2 05:09:51 2023, max compression
```

## Comparing `eyes_soatra-0.0.4.macosx-10.9-universal2.tar` & `eyes_soatra-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,13 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:07:47.915240 ./
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:07:47.915290 ./Library/
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:07:47.915344 ./Library/Frameworks/
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:07:47.915392 ./Library/Frameworks/Python.framework/
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:07:47.915440 ./Library/Frameworks/Python.framework/Versions/
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:07:47.915488 ./Library/Frameworks/Python.framework/Versions/3.10/
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:07:47.915541 ./Library/Frameworks/Python.framework/Versions/3.10/lib/
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:07:47.915588 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:07:47.923517 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:07:47.916746 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes/
--rw-r--r--   0 soatra     (501) staff       (20)       21 2023-05-02 03:45:03.000000 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:07:47.917992 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes/__pycache__/
--rw-r--r--   0 soatra     (501) staff       (20)      214 2023-05-02 05:07:47.916873 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 soatra     (501) staff       (20)     5691 2023-05-02 05:07:47.917935 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes/__pycache__/eyes.cpython-310.pyc
--rw-r--r--   0 soatra     (501) staff       (20)    10973 2023-05-02 03:40:32.000000 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:07:47.924197 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes_soatra-0.0.4-py3.10.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      543 2023-05-02 05:07:47.847620 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes_soatra-0.0.4-py3.10.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)      188 2023-05-02 05:07:47.862609 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes_soatra-0.0.4-py3.10.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-02 05:07:47.847742 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes_soatra-0.0.4-py3.10.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)        5 2023-05-02 05:07:47.847904 ./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes_soatra-0.0.4-py3.10.egg-info/top_level.txt
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:09:51.370940 eyes_soatra-0.0.5/
+-rw-r--r--   0 soatra     (501) staff       (20)      543 2023-05-02 05:09:51.370816 eyes_soatra-0.0.5/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)       47 2023-05-02 03:38:24.000000 eyes_soatra-0.0.5/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:09:51.369881 eyes_soatra-0.0.5/eyes/
+-rw-r--r--   0 soatra     (501) staff       (20)       21 2023-05-02 03:45:03.000000 eyes_soatra-0.0.5/eyes/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)    10973 2023-05-02 03:40:32.000000 eyes_soatra-0.0.5/eyes/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:09:51.370621 eyes_soatra-0.0.5/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      543 2023-05-02 05:09:51.000000 eyes_soatra-0.0.5/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)      188 2023-05-02 05:09:51.000000 eyes_soatra-0.0.5/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-02 05:09:51.000000 eyes_soatra-0.0.5/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        5 2023-05-02 05:09:51.000000 eyes_soatra-0.0.5/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-02 05:09:51.370989 eyes_soatra-0.0.5/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1062 2023-05-02 05:09:47.000000 eyes_soatra-0.0.5/setup.py
```

### Comparing `./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes/eyes.py` & `eyes_soatra-0.0.5/eyes/eyes.py`

 * *Files identical despite different names*

### Comparing `./Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/site-packages/eyes_soatra-0.0.4-py3.10.egg-info/PKG-INFO` & `eyes_soatra-0.0.5/eyes_soatra.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes-soatra
-Version: 0.0.4
+Version: 0.0.5
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: requests,requests_html,jellyfish,translate,re
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

