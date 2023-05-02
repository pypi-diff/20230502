# Comparing `tmp/eyes_soatra-0.0.5.tar.gz` & `tmp/eyes_soatra-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.5.tar", last modified: Tue May  2 05:09:51 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.6.tar", last modified: Tue May  2 05:26:18 2023, max compression
```

## Comparing `eyes_soatra-0.0.5.tar` & `eyes_soatra-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:09:51.370940 eyes_soatra-0.0.5/
--rw-r--r--   0 soatra     (501) staff       (20)      543 2023-05-02 05:09:51.370816 eyes_soatra-0.0.5/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)       47 2023-05-02 03:38:24.000000 eyes_soatra-0.0.5/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:09:51.369881 eyes_soatra-0.0.5/eyes/
--rw-r--r--   0 soatra     (501) staff       (20)       21 2023-05-02 03:45:03.000000 eyes_soatra-0.0.5/eyes/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)    10973 2023-05-02 03:40:32.000000 eyes_soatra-0.0.5/eyes/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:09:51.370621 eyes_soatra-0.0.5/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      543 2023-05-02 05:09:51.000000 eyes_soatra-0.0.5/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)      188 2023-05-02 05:09:51.000000 eyes_soatra-0.0.5/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-02 05:09:51.000000 eyes_soatra-0.0.5/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)        5 2023-05-02 05:09:51.000000 eyes_soatra-0.0.5/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-02 05:09:51.370989 eyes_soatra-0.0.5/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1062 2023-05-02 05:09:47.000000 eyes_soatra-0.0.5/setup.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:26:18.799571 eyes_soatra-0.0.6/
+-rw-r--r--   0 soatra     (501) staff       (20)      543 2023-05-02 05:26:18.799443 eyes_soatra-0.0.6/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)       47 2023-05-02 03:38:24.000000 eyes_soatra-0.0.6/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:26:18.798261 eyes_soatra-0.0.6/eyes/
+-rw-r--r--   0 soatra     (501) staff       (20)       46 2023-05-02 05:26:03.000000 eyes_soatra-0.0.6/eyes/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:26:18.798621 eyes_soatra-0.0.6/eyes/depends/
+-rw-r--r--   0 soatra     (501) staff       (20)       67 2023-05-02 05:25:18.000000 eyes_soatra-0.0.6/eyes/depends/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     7664 2023-05-02 03:37:05.000000 eyes_soatra-0.0.6/eyes/depends/depends_404.py
+-rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.6/eyes/depends/depends_no_data.py
+-rw-r--r--   0 soatra     (501) staff       (20)    10981 2023-05-02 05:25:49.000000 eyes_soatra-0.0.6/eyes/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-02 05:26:18.799229 eyes_soatra-0.0.6/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      543 2023-05-02 05:26:18.000000 eyes_soatra-0.0.6/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)      273 2023-05-02 05:26:18.000000 eyes_soatra-0.0.6/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-02 05:26:18.000000 eyes_soatra-0.0.6/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        5 2023-05-02 05:26:18.000000 eyes_soatra-0.0.6/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-02 05:26:18.799617 eyes_soatra-0.0.6/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1062 2023-05-02 05:26:17.000000 eyes_soatra-0.0.6/setup.py
```

### Comparing `eyes_soatra-0.0.5/PKG-INFO` & `eyes_soatra-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes_soatra
-Version: 0.0.5
+Version: 0.0.6
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: requests,requests_html,jellyfish,translate,re
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.5/eyes/eyes.py` & `eyes_soatra-0.0.6/eyes/eyes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!python3
-from .depends.depends_no_data import depends as depends_no_data
-from .depends.depends_404 import depends as depends_404
+from eyes.depends.depends_no_data import depends as depends_no_data
+from eyes.depends.depends_404 import depends as depends_404
 from translate import Translator
 from requests_html import HTML
 import requests
 import jellyfish
 import re
 
 # Suppress only the single warning from urllib3 needed.
```

### Comparing `eyes_soatra-0.0.5/eyes_soatra.egg-info/PKG-INFO` & `eyes_soatra-0.0.6/eyes_soatra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyes-soatra
-Version: 0.0.5
+Version: 0.0.6
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: requests,requests_html,jellyfish,translate,re
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.5/setup.py` & `eyes_soatra-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 NAME = 'eyes_soatra'
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Eyes'
 
 AUTHOR_NAME = 'Soatra'
 AUTHOR_EMAIL = 'johnsoatra@gmail.com'
 
 # Setting up
 setup(
```

