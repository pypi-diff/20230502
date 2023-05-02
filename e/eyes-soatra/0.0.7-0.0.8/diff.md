# Comparing `tmp/eyes_soatra-0.0.7.tar.gz` & `tmp/eyes_soatra-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.7.tar", last modified: Tue May  2 05:28:38 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.8.tar", last modified: Tue May  2 05:30:52 2023, max compression
```

## Comparing `eyes_soatra-0.0.7.tar` & `eyes_soatra-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:28:38.774205 eyes_soatra-0.0.7/
--rw-r--r--   0 soatra     (501) staff       (20)      543 2023-05-02 05:28:38.774087 eyes_soatra-0.0.7/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)       47 2023-05-02 03:38:24.000000 eyes_soatra-0.0.7/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:28:38.773041 eyes_soatra-0.0.7/eyes/
--rw-r--r--   0 soatra     (501) staff       (20)       46 2023-05-02 05:26:03.000000 eyes_soatra-0.0.7/eyes/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:28:38.773394 eyes_soatra-0.0.7/eyes/depends/
--rw-r--r--   0 soatra     (501) staff       (20)     7664 2023-05-02 03:37:05.000000 eyes_soatra-0.0.7/eyes/depends/depends_404.py
--rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.7/eyes/depends/depends_no_data.py
--rw-r--r--   0 soatra     (501) staff       (20)    10981 2023-05-02 05:25:49.000000 eyes_soatra-0.0.7/eyes/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:28:38.773908 eyes_soatra-0.0.7/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      543 2023-05-02 05:28:38.000000 eyes_soatra-0.0.7/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)      248 2023-05-02 05:28:38.000000 eyes_soatra-0.0.7/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-02 05:28:38.000000 eyes_soatra-0.0.7/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)        5 2023-05-02 05:28:38.000000 eyes_soatra-0.0.7/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-02 05:28:38.774246 eyes_soatra-0.0.7/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1062 2023-05-02 05:28:35.000000 eyes_soatra-0.0.7/setup.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:30:52.945839 eyes_soatra-0.0.8/
+-rw-r--r--   0 soatra     (501) staff       (20)      543 2023-05-02 05:30:52.945712 eyes_soatra-0.0.8/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)       47 2023-05-02 03:38:24.000000 eyes_soatra-0.0.8/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:30:52.944824 eyes_soatra-0.0.8/eyes/
+-rw-r--r--   0 soatra     (501) staff       (20)       46 2023-05-02 05:26:03.000000 eyes_soatra-0.0.8/eyes/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:30:52.945066 eyes_soatra-0.0.8/eyes/depends/
+-rw-r--r--   0 soatra     (501) staff       (20)     7664 2023-05-02 03:37:05.000000 eyes_soatra-0.0.8/eyes/depends/depends_404.py
+-rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.8/eyes/depends/depends_no_data.py
+-rw-r--r--   0 soatra     (501) staff       (20)    10971 2023-05-02 05:30:16.000000 eyes_soatra-0.0.8/eyes/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:30:52.945527 eyes_soatra-0.0.8/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      543 2023-05-02 05:30:52.000000 eyes_soatra-0.0.8/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)      248 2023-05-02 05:30:52.000000 eyes_soatra-0.0.8/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-02 05:30:52.000000 eyes_soatra-0.0.8/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        5 2023-05-02 05:30:52.000000 eyes_soatra-0.0.8/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-02 05:30:52.945906 eyes_soatra-0.0.8/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1062 2023-05-02 05:30:50.000000 eyes_soatra-0.0.8/setup.py
```

### Comparing `eyes_soatra-0.0.7/PKG-INFO` & `eyes_soatra-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes_soatra
-Version: 0.0.7
+Version: 0.0.8
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: requests,requests_html,jellyfish,translate,re
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.7/eyes/depends/depends_404.py` & `eyes_soatra-0.0.8/eyes/depends/depends_404.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.7/eyes/eyes.py` & `eyes_soatra-0.0.8/eyes/eyes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!python3
-from eyes.depends.depends_no_data import depends as depends_no_data
-from eyes.depends.depends_404 import depends as depends_404
+from depends.depends_no_data import depends as depends_no_data
+from depends.depends_404 import depends as depends_404
 from translate import Translator
 from requests_html import HTML
 import requests
 import jellyfish
 import re
 
 # Suppress only the single warning from urllib3 needed.
```

### Comparing `eyes_soatra-0.0.7/eyes_soatra.egg-info/PKG-INFO` & `eyes_soatra-0.0.8/eyes_soatra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes-soatra
-Version: 0.0.7
+Version: 0.0.8
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: requests,requests_html,jellyfish,translate,re
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.7/setup.py` & `eyes_soatra-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 NAME = 'eyes_soatra'
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Eyes'
 
 AUTHOR_NAME = 'Soatra'
 AUTHOR_EMAIL = 'johnsoatra@gmail.com'
 
 # Setting up
 setup(
```

