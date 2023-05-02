# Comparing `tmp/roboweb-extension-0.1.8.tar.gz` & `tmp/roboweb_extension-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboweb-extension-0.1.8.tar", last modified: Sun Apr  9 03:17:20 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `roboweb-extension-0.1.8.tar` & `roboweb_extension-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,25 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 03:17:20.066654 roboweb-extension-0.1.8/
--rw-r--r--   0 hamel      (501) staff       (20)        0 2023-04-09 03:10:44.000000 roboweb-extension-0.1.8/LICENSE
--rw-r--r--   0 hamel      (501) staff       (20)      389 2023-04-09 03:10:44.000000 roboweb-extension-0.1.8/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     4511 2023-04-09 03:17:20.066383 roboweb-extension-0.1.8/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     3469 2023-04-09 03:10:44.000000 roboweb-extension-0.1.8/README.md
--rw-r--r--   0 hamel      (501) staff       (20)      195 2023-04-09 03:10:44.000000 roboweb-extension-0.1.8/install.json
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 03:17:20.063497 roboweb-extension-0.1.8/lib/
--rw-r--r--   0 hamel      (501) staff       (20)     9805 2023-04-09 03:10:44.000000 roboweb-extension-0.1.8/lib/index.js
--rw-r--r--   0 hamel      (501) staff       (20)     1684 2023-04-09 03:10:44.000000 roboweb-extension-0.1.8/package.json
--rw-r--r--   0 hamel      (501) staff       (20)     2626 2023-04-09 03:16:14.000000 roboweb-extension-0.1.8/pyproject.toml
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 03:17:20.063820 roboweb-extension-0.1.8/roboweb-extension/
--rw-r--r--   0 hamel      (501) staff       (20)      318 2023-04-09 03:10:44.000000 roboweb-extension-0.1.8/roboweb-extension/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)       23 2023-04-09 03:10:44.000000 roboweb-extension-0.1.8/roboweb-extension/_version.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 03:17:20.064004 roboweb-extension-0.1.8/roboweb-extension/labextension/
--rw-r--r--   0 hamel      (501) staff       (20)     1800 2023-04-09 03:12:01.000000 roboweb-extension-0.1.8/roboweb-extension/labextension/package.json
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 03:17:20.064792 roboweb-extension-0.1.8/roboweb-extension/labextension/static/
--rw-r--r--   0 hamel      (501) staff       (20)     4442 2023-04-09 03:12:01.000000 roboweb-extension-0.1.8/roboweb-extension/labextension/static/568.aeca1ad98987afd7f02f.js
--rw-r--r--   0 hamel      (501) staff       (20)     6380 2023-04-09 03:12:01.000000 roboweb-extension-0.1.8/roboweb-extension/labextension/static/remoteEntry.ef66e4e5d4f3238e004f.js
--rw-r--r--   0 hamel      (501) staff       (20)      118 2023-04-09 03:11:59.000000 roboweb-extension-0.1.8/roboweb-extension/labextension/static/style.js
--rw-r--r--   0 hamel      (501) staff       (20)       20 2023-04-09 03:12:01.000000 roboweb-extension-0.1.8/roboweb-extension/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 03:17:20.065677 roboweb-extension-0.1.8/roboweb_extension.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     4511 2023-04-09 03:17:20.000000 roboweb-extension-0.1.8/roboweb_extension.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      737 2023-04-09 03:17:20.000000 roboweb-extension-0.1.8/roboweb_extension.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-09 03:17:20.000000 roboweb-extension-0.1.8/roboweb_extension.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-04-09 03:17:20.000000 roboweb-extension-0.1.8/roboweb_extension.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       15 2023-04-09 03:17:20.000000 roboweb-extension-0.1.8/roboweb_extension.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)       18 2023-04-09 03:17:20.000000 roboweb-extension-0.1.8/roboweb_extension.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-04-09 03:17:20.066694 roboweb-extension-0.1.8/setup.cfg
--rw-r--r--   0 hamel      (501) staff       (20)     2826 2023-04-09 03:14:36.000000 roboweb-extension-0.1.8/setup.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-04-09 03:17:20.066147 roboweb-extension-0.1.8/style/
--rw-r--r--   0 hamel      (501) staff       (20)        0 2023-04-09 03:10:44.000000 roboweb-extension-0.1.8/style/base.css
--rw-r--r--   0 hamel      (501) staff       (20)       25 2023-04-09 03:10:44.000000 roboweb-extension-0.1.8/style/index.css
--rw-r--r--   0 hamel      (501) staff       (20)       21 2023-04-09 03:10:44.000000 roboweb-extension-0.1.8/style/index.js
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/MANIFEST.in
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/Makefile
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/install.json
+-rw-r--r--   0        0        0   170064 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/package-lock.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/package.json
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/settings.ini
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/setup.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/binder/environment.yml
+-rwxr-xr-x   0        0        0     1262 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/binder/postBuild
+-rw-r--r--   0        0        0     9805 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/lib/index.js
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/roboweb-extension/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/roboweb-extension/_version.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/roboweb-extension/labextension/package.json
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/roboweb-extension/labextension/static/568.aeca1ad98987afd7f02f.js
+-rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/roboweb-extension/labextension/static/remoteEntry.ef66e4e5d4f3238e004f.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/roboweb-extension/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/roboweb-extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/style/index.js
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/README.md
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 roboweb_extension-0.1.9/PKG-INFO
```

### Comparing `roboweb-extension-0.1.8/PKG-INFO` & `roboweb_extension-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: roboweb-extension
-Version: 0.1.8
+Version: 0.1.9
 Summary: Roboweb extension
-Home-page: https://github.com/jlewi/roboweb
-Author: Jeremy Lewi
-Author-email: Francisco Uribe <francisco.uribe@gmail.com>
 Project-URL: Homepage, https://github.com/github_username/roboweb-extension
+Author-email: Francisco Uribe <francisco.uribe@gmail.com>
+License-File: LICENSE
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: License :: OSI Approved :: BSD License
@@ -17,16 +16,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
 
 # roboweb-extension
 
 ![Github Actions Status](https://github.com/github_username/roboweb-extension/workflows/Build/badge.svg)
 
 Roboweb extension
```

### Comparing `roboweb-extension-0.1.8/README.md` & `roboweb_extension-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `roboweb-extension-0.1.8/lib/index.js` & `roboweb_extension-0.1.9/lib/index.js`

 * *Files identical despite different names*

### Comparing `roboweb-extension-0.1.8/package.json` & `roboweb_extension-0.1.9/package.json`

 * *Files identical despite different names*

### Comparing `roboweb-extension-0.1.8/pyproject.toml` & `roboweb_extension-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
-version = "0.1.8"
+version = "0.1.9"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/github_username/roboweb-extension"
```

### Comparing `roboweb-extension-0.1.8/roboweb-extension/labextension/package.json` & `roboweb_extension-0.1.9/roboweb-extension/labextension/package.json`

 * *Files identical despite different names*

### Comparing `roboweb-extension-0.1.8/roboweb-extension/labextension/static/568.aeca1ad98987afd7f02f.js` & `roboweb_extension-0.1.9/roboweb-extension/labextension/static/568.aeca1ad98987afd7f02f.js`

 * *Files identical despite different names*

### Comparing `roboweb-extension-0.1.8/roboweb-extension/labextension/static/remoteEntry.ef66e4e5d4f3238e004f.js` & `roboweb_extension-0.1.9/roboweb-extension/labextension/static/remoteEntry.ef66e4e5d4f3238e004f.js`

 * *Files identical despite different names*

### Comparing `roboweb-extension-0.1.8/setup.py` & `roboweb_extension-0.1.9/setup.py`

 * *Files identical despite different names*

