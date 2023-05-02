# Comparing `tmp/foliantcontrib.includes-1.1.8.tar.gz` & `tmp/foliantcontrib.includes-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/foliantcontrib.includes-1.1.8.tar", last modified: Thu Nov 21 13:17:08 2019, max compression
+gzip compressed data, was "dist/foliantcontrib.includes-1.1.9.tar", last modified: Tue Feb  4 08:00:28 2020, max compression
```

## Comparing `foliantcontrib.includes-1.1.8.tar` & `foliantcontrib.includes-1.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 lomov     (1000) lomov     (1000)        0 2019-11-21 13:17:08.000000 foliantcontrib.includes-1.1.8/
-drwxrwxr-x   0 lomov     (1000) lomov     (1000)        0 2019-11-21 13:17:08.000000 foliantcontrib.includes-1.1.8/foliant/
-drwxrwxr-x   0 lomov     (1000) lomov     (1000)        0 2019-11-21 13:17:08.000000 foliantcontrib.includes-1.1.8/foliant/preprocessors/
--rw-r--r--   0 lomov     (1000) lomov     (1000)    35805 2019-11-21 13:15:39.000000 foliantcontrib.includes-1.1.8/foliant/preprocessors/includes.py
-drwxrwxr-x   0 lomov     (1000) lomov     (1000)        0 2019-11-21 13:17:08.000000 foliantcontrib.includes-1.1.8/foliantcontrib.includes.egg-info/
--rw-rw-r--   0 lomov     (1000) lomov     (1000)    12062 2019-11-21 13:17:07.000000 foliantcontrib.includes-1.1.8/foliantcontrib.includes.egg-info/PKG-INFO
--rw-rw-r--   0 lomov     (1000) lomov     (1000)      286 2019-11-21 13:17:07.000000 foliantcontrib.includes-1.1.8/foliantcontrib.includes.egg-info/SOURCES.txt
--rw-rw-r--   0 lomov     (1000) lomov     (1000)        1 2019-11-21 13:17:07.000000 foliantcontrib.includes-1.1.8/foliantcontrib.includes.egg-info/dependency_links.txt
--rw-rw-r--   0 lomov     (1000) lomov     (1000)       76 2019-11-21 13:17:07.000000 foliantcontrib.includes-1.1.8/foliantcontrib.includes.egg-info/requires.txt
--rw-rw-r--   0 lomov     (1000) lomov     (1000)        8 2019-11-21 13:17:07.000000 foliantcontrib.includes-1.1.8/foliantcontrib.includes.egg-info/top_level.txt
--rw-r--r--   0 lomov     (1000) lomov     (1000)     9362 2019-08-14 11:09:53.000000 foliantcontrib.includes-1.1.8/README.md
--rw-r--r--   0 lomov     (1000) lomov     (1000)     1173 2019-11-21 13:15:39.000000 foliantcontrib.includes-1.1.8/setup.py
--rw-rw-r--   0 lomov     (1000) lomov     (1000)    12062 2019-11-21 13:17:08.000000 foliantcontrib.includes-1.1.8/PKG-INFO
--rw-rw-r--   0 lomov     (1000) lomov     (1000)       38 2019-11-21 13:17:08.000000 foliantcontrib.includes-1.1.8/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2020-02-04 08:00:28.000000 foliantcontrib.includes-1.1.9/
+-rw-r--r--   0 user       (501) staff       (20)    12062 2020-02-04 08:00:28.000000 foliantcontrib.includes-1.1.9/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     9362 2019-09-26 07:29:54.000000 foliantcontrib.includes-1.1.9/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2020-02-04 08:00:28.000000 foliantcontrib.includes-1.1.9/foliant/
+drwxr-xr-x   0 user       (501) staff       (20)        0 2020-02-04 08:00:28.000000 foliantcontrib.includes-1.1.9/foliant/preprocessors/
+-rw-r--r--   0 user       (501) staff       (20)    35801 2020-02-04 07:33:53.000000 foliantcontrib.includes-1.1.9/foliant/preprocessors/includes.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2020-02-04 08:00:28.000000 foliantcontrib.includes-1.1.9/foliantcontrib.includes.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)    12062 2020-02-04 08:00:28.000000 foliantcontrib.includes-1.1.9/foliantcontrib.includes.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      286 2020-02-04 08:00:28.000000 foliantcontrib.includes-1.1.9/foliantcontrib.includes.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2020-02-04 08:00:28.000000 foliantcontrib.includes-1.1.9/foliantcontrib.includes.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       76 2020-02-04 08:00:28.000000 foliantcontrib.includes-1.1.9/foliantcontrib.includes.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2020-02-04 08:00:28.000000 foliantcontrib.includes-1.1.9/foliantcontrib.includes.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)       38 2020-02-04 08:00:28.000000 foliantcontrib.includes-1.1.9/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)     1173 2020-02-04 07:33:53.000000 foliantcontrib.includes-1.1.9/setup.py
```

### Comparing `foliantcontrib.includes-1.1.8/foliant/preprocessors/includes.py` & `foliantcontrib.includes-1.1.9/foliant/preprocessors/includes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from io import StringIO
 from pathlib import Path
 from subprocess import run, CalledProcessError, PIPE, STDOUT
 
 from foliant.preprocessors.base import BasePreprocessor
 from foliant.preprocessors import escapecode
-from foliant.cli.meta.utils import remove_meta
+from foliant.meta.tools import remove_meta
 
 
 class Preprocessor(BasePreprocessor):
     defaults = {
         'recursive': True,
         'cache_dir': Path('.includescache'),
         'aliases': {}
```

### Comparing `foliantcontrib.includes-1.1.8/foliantcontrib.includes.egg-info/PKG-INFO` & `foliantcontrib.includes-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliantcontrib.includes
-Version: 1.1.8
+Version: 1.1.9
 Summary: Powerful includes for Foliant doc maker.
 Home-page: https://github.com/foliant-docs/foliantcontrib.includes
 Author: Konstantin Molchanov
 Author-email: moigagoo@live.com
 License: MIT
 Description: # Includes for Foliant
```

### Comparing `foliantcontrib.includes-1.1.8/README.md` & `foliantcontrib.includes-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `foliantcontrib.includes-1.1.8/setup.py` & `foliantcontrib.includes-1.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 
 setup(
     name='foliantcontrib.includes',
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
-    version='1.1.8',
+    version='1.1.9',
     author='Konstantin Molchanov',
     author_email='moigagoo@live.com',
     url='https://github.com/foliant-docs/foliantcontrib.includes',
     packages=['foliant.preprocessors'],
     license='MIT',
     platforms='any',
     install_requires=[
         'foliant>=1.0.10',
         'foliantcontrib.escapecode>=1.0.0',
-        'foliantcontrib.meta>=1.2.0'
+        'foliantcontrib.meta>=1.3.0'
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `foliantcontrib.includes-1.1.8/PKG-INFO` & `foliantcontrib.includes-1.1.9/foliantcontrib.includes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliantcontrib.includes
-Version: 1.1.8
+Version: 1.1.9
 Summary: Powerful includes for Foliant doc maker.
 Home-page: https://github.com/foliant-docs/foliantcontrib.includes
 Author: Konstantin Molchanov
 Author-email: moigagoo@live.com
 License: MIT
 Description: # Includes for Foliant
```

