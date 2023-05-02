# Comparing `tmp/dhuolib-0.1.0.tar.gz` & `tmp/dhuolib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuolib-0.1.0.tar", last modified: Thu Apr 27 03:59:59 2023, max compression
+gzip compressed data, was "dhuolib-0.1.1.tar", last modified: Tue May  2 19:37:13 2023, max compression
```

## Comparing `dhuolib-0.1.0.tar` & `dhuolib-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 ac        (1000) ac        (1000)        0 2023-04-27 03:59:59.324152 dhuolib-0.1.0/
--rw-rw-r--   0 ac        (1000) ac        (1000)     1319 2023-04-27 03:59:59.324152 dhuolib-0.1.0/PKG-INFO
--rw-rw-r--   0 ac        (1000) ac        (1000)      769 2023-04-27 03:13:47.000000 dhuolib-0.1.0/README.md
-drwxrwxr-x   0 ac        (1000) ac        (1000)        0 2023-04-27 03:59:59.320152 dhuolib-0.1.0/dhuolib/
--rw-rw-r--   0 ac        (1000) ac        (1000)        0 2023-04-27 01:07:16.000000 dhuolib-0.1.0/dhuolib/__init__.py
-drwxrwxr-x   0 ac        (1000) ac        (1000)        0 2023-04-27 03:59:59.324152 dhuolib-0.1.0/dhuolib/auth/
--rw-rw-r--   0 ac        (1000) ac        (1000)        0 2023-04-27 03:19:21.000000 dhuolib-0.1.0/dhuolib/auth/__init__.py
--rw-rw-r--   0 ac        (1000) ac        (1000)      562 2023-04-27 03:37:02.000000 dhuolib-0.1.0/dhuolib/auth/login.py
--rw-rw-r--   0 ac        (1000) ac        (1000)     2454 2023-04-27 03:54:29.000000 dhuolib-0.1.0/dhuolib/auth/openid.py
--rw-rw-r--   0 ac        (1000) ac        (1000)     1115 2023-04-27 03:58:09.000000 dhuolib-0.1.0/dhuolib/cli.py
-drwxrwxr-x   0 ac        (1000) ac        (1000)        0 2023-04-27 03:59:59.324152 dhuolib-0.1.0/dhuolib/utils/
--rw-rw-r--   0 ac        (1000) ac        (1000)        0 2023-04-27 03:21:21.000000 dhuolib-0.1.0/dhuolib/utils/__init__.py
--rw-rw-r--   0 ac        (1000) ac        (1000)     4622 2023-04-27 03:36:23.000000 dhuolib-0.1.0/dhuolib/utils/persistence.py
--rw-rw-r--   0 ac        (1000) ac        (1000)      426 2023-04-27 03:20:15.000000 dhuolib-0.1.0/dhuolib/utils/utils.py
-drwxrwxr-x   0 ac        (1000) ac        (1000)        0 2023-04-27 03:59:59.324152 dhuolib-0.1.0/dhuolib.egg-info/
--rw-rw-r--   0 ac        (1000) ac        (1000)     1319 2023-04-27 03:59:59.000000 dhuolib-0.1.0/dhuolib.egg-info/PKG-INFO
--rw-rw-r--   0 ac        (1000) ac        (1000)      399 2023-04-27 03:59:59.000000 dhuolib-0.1.0/dhuolib.egg-info/SOURCES.txt
--rw-rw-r--   0 ac        (1000) ac        (1000)        1 2023-04-27 03:59:59.000000 dhuolib-0.1.0/dhuolib.egg-info/dependency_links.txt
--rw-rw-r--   0 ac        (1000) ac        (1000)       40 2023-04-27 03:59:59.000000 dhuolib-0.1.0/dhuolib.egg-info/entry_points.txt
--rw-rw-r--   0 ac        (1000) ac        (1000)      104 2023-04-27 03:59:59.000000 dhuolib-0.1.0/dhuolib.egg-info/requires.txt
--rw-rw-r--   0 ac        (1000) ac        (1000)        8 2023-04-27 03:59:59.000000 dhuolib-0.1.0/dhuolib.egg-info/top_level.txt
--rw-rw-r--   0 ac        (1000) ac        (1000)       95 2023-04-27 03:59:59.324152 dhuolib-0.1.0/setup.cfg
--rw-rw-r--   0 ac        (1000) ac        (1000)     1308 2023-04-27 03:17:23.000000 dhuolib-0.1.0/setup.py
+drwxrwxr-x   0 ac        (1000) ac        (1000)        0 2023-05-02 19:37:13.709538 dhuolib-0.1.1/
+-rw-rw-r--   0 ac        (1000) ac        (1000)     1356 2023-05-02 19:37:13.709538 dhuolib-0.1.1/PKG-INFO
+-rw-rw-r--   0 ac        (1000) ac        (1000)      769 2023-05-02 19:37:04.000000 dhuolib-0.1.1/README.md
+drwxrwxr-x   0 ac        (1000) ac        (1000)        0 2023-05-02 19:37:13.709538 dhuolib-0.1.1/dhuolib/
+-rw-rw-r--   0 ac        (1000) ac        (1000)        0 2023-04-27 01:07:16.000000 dhuolib-0.1.1/dhuolib/__init__.py
+drwxrwxr-x   0 ac        (1000) ac        (1000)        0 2023-05-02 19:37:13.709538 dhuolib-0.1.1/dhuolib/auth/
+-rw-rw-r--   0 ac        (1000) ac        (1000)        0 2023-04-27 03:19:21.000000 dhuolib-0.1.1/dhuolib/auth/__init__.py
+-rw-rw-r--   0 ac        (1000) ac        (1000)      562 2023-04-27 03:37:02.000000 dhuolib-0.1.1/dhuolib/auth/login.py
+-rw-rw-r--   0 ac        (1000) ac        (1000)     2454 2023-04-27 03:54:29.000000 dhuolib-0.1.1/dhuolib/auth/openid.py
+-rw-rw-r--   0 ac        (1000) ac        (1000)     1115 2023-04-27 03:58:09.000000 dhuolib-0.1.1/dhuolib/cli.py
+-rw-rw-r--   0 ac        (1000) ac        (1000)      574 2023-04-28 19:11:32.000000 dhuolib-0.1.1/dhuolib/config.py
+drwxrwxr-x   0 ac        (1000) ac        (1000)        0 2023-05-02 19:37:13.709538 dhuolib-0.1.1/dhuolib/utils/
+-rw-rw-r--   0 ac        (1000) ac        (1000)        0 2023-04-27 03:21:21.000000 dhuolib-0.1.1/dhuolib/utils/__init__.py
+-rw-rw-r--   0 ac        (1000) ac        (1000)     4622 2023-04-27 03:36:23.000000 dhuolib-0.1.1/dhuolib/utils/persistence.py
+-rw-rw-r--   0 ac        (1000) ac        (1000)      426 2023-04-27 03:20:15.000000 dhuolib-0.1.1/dhuolib/utils/utils.py
+drwxrwxr-x   0 ac        (1000) ac        (1000)        0 2023-05-02 19:37:13.709538 dhuolib-0.1.1/dhuolib.egg-info/
+-rw-rw-r--   0 ac        (1000) ac        (1000)     1356 2023-05-02 19:37:13.000000 dhuolib-0.1.1/dhuolib.egg-info/PKG-INFO
+-rw-rw-r--   0 ac        (1000) ac        (1000)      417 2023-05-02 19:37:13.000000 dhuolib-0.1.1/dhuolib.egg-info/SOURCES.txt
+-rw-rw-r--   0 ac        (1000) ac        (1000)        1 2023-05-02 19:37:13.000000 dhuolib-0.1.1/dhuolib.egg-info/dependency_links.txt
+-rw-rw-r--   0 ac        (1000) ac        (1000)       41 2023-05-02 19:37:13.000000 dhuolib-0.1.1/dhuolib.egg-info/entry_points.txt
+-rw-rw-r--   0 ac        (1000) ac        (1000)      104 2023-05-02 19:37:13.000000 dhuolib-0.1.1/dhuolib.egg-info/requires.txt
+-rw-rw-r--   0 ac        (1000) ac        (1000)        8 2023-05-02 19:37:13.000000 dhuolib-0.1.1/dhuolib.egg-info/top_level.txt
+-rw-rw-r--   0 ac        (1000) ac        (1000)       95 2023-05-02 19:37:13.713538 dhuolib-0.1.1/setup.cfg
+-rw-rw-r--   0 ac        (1000) ac        (1000)     1308 2023-05-02 19:36:55.000000 dhuolib-0.1.1/setup.py
```

### Comparing `dhuolib-0.1.0/PKG-INFO` & `dhuolib-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: dhuolib
-Version: 0.1.0
+Version: 0.1.1
+Summary: UNKNOWN
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: Antonio Carlos de Lima Junior
 Author-email: antonio.lima@engdb.com.br
 License: MIT
 Keywords: datascience datapipeline mlops
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 
 # dhuolib
 
-![Version](https://img.shields.io/badge/version-0.1.0-blue.svg?cacheSeconds=2592000)
+![Version](https://img.shields.io/badge/version-0.1.1-blue.svg?cacheSeconds=2592000)
 [![License: MIT](https://img.shields.io/badge/License-MIT-grenn.svg)](#)
 
 > Library for data science on DHuO Data 
 
 ### 🏠 [Homepage](https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib)
 
 ## Install
@@ -57,7 +59,9 @@
 $ dh status
 ```
 
 Clone project
 ```sh
 $ dh get [project_id]
 ```
+
+
```

### Comparing `dhuolib-0.1.0/README.md` & `dhuolib-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # dhuolib
 
-![Version](https://img.shields.io/badge/version-0.1.0-blue.svg?cacheSeconds=2592000)
+![Version](https://img.shields.io/badge/version-0.1.1-blue.svg?cacheSeconds=2592000)
 [![License: MIT](https://img.shields.io/badge/License-MIT-grenn.svg)](#)
 
 > Library for data science on DHuO Data 
 
 ### 🏠 [Homepage](https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib)
 
 ## Install
```

### Comparing `dhuolib-0.1.0/dhuolib/auth/login.py` & `dhuolib-0.1.1/dhuolib/auth/login.py`

 * *Files identical despite different names*

### Comparing `dhuolib-0.1.0/dhuolib/auth/openid.py` & `dhuolib-0.1.1/dhuolib/auth/openid.py`

 * *Files identical despite different names*

### Comparing `dhuolib-0.1.0/dhuolib/cli.py` & `dhuolib-0.1.1/dhuolib/cli.py`

 * *Files identical despite different names*

### Comparing `dhuolib-0.1.0/dhuolib/utils/persistence.py` & `dhuolib-0.1.1/dhuolib/utils/persistence.py`

 * *Files identical despite different names*

### Comparing `dhuolib-0.1.0/dhuolib.egg-info/PKG-INFO` & `dhuolib-0.1.1/dhuolib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: dhuolib
-Version: 0.1.0
+Version: 0.1.1
+Summary: UNKNOWN
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: Antonio Carlos de Lima Junior
 Author-email: antonio.lima@engdb.com.br
 License: MIT
 Keywords: datascience datapipeline mlops
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 
 # dhuolib
 
-![Version](https://img.shields.io/badge/version-0.1.0-blue.svg?cacheSeconds=2592000)
+![Version](https://img.shields.io/badge/version-0.1.1-blue.svg?cacheSeconds=2592000)
 [![License: MIT](https://img.shields.io/badge/License-MIT-grenn.svg)](#)
 
 > Library for data science on DHuO Data 
 
 ### 🏠 [Homepage](https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib)
 
 ## Install
@@ -57,7 +59,9 @@
 $ dh status
 ```
 
 Clone project
 ```sh
 $ dh get [project_id]
 ```
+
+
```

### Comparing `dhuolib-0.1.0/setup.py` & `dhuolib-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                 'scikit-learn==1.2']
 
 SETUP_REQUIRES = ['flake8', 'pytest-runner']
 
 
 setup(
     name='dhuolib',
-    version='0.1.0',
+    version='0.1.1',
     long_description=readme(),
     long_description_content_type="text/markdown",
     author='Antonio Carlos de Lima Junior',
     author_email='antonio.lima@engdb.com.br',
     url='https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib',
     packages=find_packages(include=['dhuolib', 'dhuolib.*']),
     install_requires=REQUIREMENTS,
```

