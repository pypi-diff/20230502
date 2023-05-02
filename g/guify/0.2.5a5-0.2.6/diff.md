# Comparing `tmp/guify-0.2.5a5.tar.gz` & `tmp/guify-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guify-0.2.5a5.tar", last modified: Tue May  2 13:28:40 2023, max compression
+gzip compressed data, was "guify-0.2.6.tar", last modified: Tue May  2 13:42:11 2023, max compression
```

## Comparing `guify-0.2.5a5.tar` & `guify-0.2.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:28:40.245940 guify-0.2.5a5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 13:27:14.000000 guify-0.2.5a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-02 13:27:14.000000 guify-0.2.5a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-02 13:28:40.245940 guify-0.2.5a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-02 13:27:14.000000 guify-0.2.5a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:28:40.237940 guify-0.2.5a5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-02 13:27:14.000000 guify-0.2.5a5/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 13:27:14.000000 guify-0.2.5a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-02 13:28:40.245940 guify-0.2.5a5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:28:40.237940 guify-0.2.5a5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:28:40.237940 guify-0.2.5a5/src/guify/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-02 13:27:14.000000 guify-0.2.5a5/src/guify/App.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-02 13:27:14.000000 guify-0.2.5a5/src/guify/BaseTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-02 13:27:14.000000 guify-0.2.5a5/src/guify/ConfigTab.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-02 13:27:14.000000 guify-0.2.5a5/src/guify/Monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-02 13:27:14.000000 guify-0.2.5a5/src/guify/TestPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-02 13:27:14.000000 guify-0.2.5a5/src/guify/TestWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-02 13:27:14.000000 guify-0.2.5a5/src/guify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 13:27:14.000000 guify-0.2.5a5/src/guify/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-02 13:27:14.000000 guify-0.2.5a5/src/guify/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:28:40.241940 guify-0.2.5a5/src/guify/web/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-02 13:28:32.000000 guify-0.2.5a5/src/guify/web/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-02 13:28:17.000000 guify-0.2.5a5/src/guify/web/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-02 13:28:32.000000 guify-0.2.5a5/src/guify/web/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 13:28:17.000000 guify-0.2.5a5/src/guify/web/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:28:40.237940 guify-0.2.5a5/src/guify/web/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:28:40.241940 guify-0.2.5a5/src/guify/web/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   144117 2023-05-02 13:28:32.000000 guify-0.2.5a5/src/guify/web/static/css/main.c779b13f.css
--rw-r--r--   0 runner    (1001) docker     (123)   481735 2023-05-02 13:28:32.000000 guify-0.2.5a5/src/guify/web/static/css/main.c779b13f.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:28:40.241940 guify-0.2.5a5/src/guify/web/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   207756 2023-05-02 13:28:32.000000 guify-0.2.5a5/src/guify/web/static/js/main.bf3c494e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-02 13:28:32.000000 guify-0.2.5a5/src/guify/web/static/js/main.bf3c494e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   660257 2023-05-02 13:28:32.000000 guify-0.2.5a5/src/guify/web/static/js/main.bf3c494e.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:28:40.241940 guify-0.2.5a5/src/guify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-02 13:28:40.000000 guify-0.2.5a5/src/guify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-02 13:28:40.000000 guify-0.2.5a5/src/guify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:28:40.000000 guify-0.2.5a5/src/guify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-02 13:28:40.000000 guify-0.2.5a5/src/guify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 13:28:40.000000 guify-0.2.5a5/src/guify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:42:11.709524 guify-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 13:40:33.000000 guify-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-02 13:40:33.000000 guify-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-02 13:42:11.709524 guify-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-02 13:40:33.000000 guify-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:42:11.701525 guify-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-02 13:40:33.000000 guify-0.2.6/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 13:40:33.000000 guify-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-02 13:42:11.709524 guify-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:42:11.697524 guify-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:42:11.701525 guify-0.2.6/src/guify/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-02 13:40:33.000000 guify-0.2.6/src/guify/App.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-02 13:40:33.000000 guify-0.2.6/src/guify/BaseTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-02 13:40:33.000000 guify-0.2.6/src/guify/ConfigTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-02 13:40:33.000000 guify-0.2.6/src/guify/Monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-02 13:40:33.000000 guify-0.2.6/src/guify/TestPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-02 13:40:33.000000 guify-0.2.6/src/guify/TestWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-02 13:40:33.000000 guify-0.2.6/src/guify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 13:40:33.000000 guify-0.2.6/src/guify/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-02 13:40:33.000000 guify-0.2.6/src/guify/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:42:11.705525 guify-0.2.6/src/guify/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-02 13:42:02.000000 guify-0.2.6/src/guify/web/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-02 13:41:45.000000 guify-0.2.6/src/guify/web/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-02 13:42:03.000000 guify-0.2.6/src/guify/web/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 13:41:45.000000 guify-0.2.6/src/guify/web/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:42:11.701525 guify-0.2.6/src/guify/web/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:42:11.705525 guify-0.2.6/src/guify/web/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   144117 2023-05-02 13:42:02.000000 guify-0.2.6/src/guify/web/static/css/main.c779b13f.css
+-rw-r--r--   0 runner    (1001) docker     (123)   481735 2023-05-02 13:42:02.000000 guify-0.2.6/src/guify/web/static/css/main.c779b13f.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:42:11.705525 guify-0.2.6/src/guify/web/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   207756 2023-05-02 13:42:02.000000 guify-0.2.6/src/guify/web/static/js/main.bf3c494e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-02 13:42:02.000000 guify-0.2.6/src/guify/web/static/js/main.bf3c494e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   660257 2023-05-02 13:42:02.000000 guify-0.2.6/src/guify/web/static/js/main.bf3c494e.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:42:11.705525 guify-0.2.6/src/guify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-02 13:42:11.000000 guify-0.2.6/src/guify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-02 13:42:11.000000 guify-0.2.6/src/guify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:42:11.000000 guify-0.2.6/src/guify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-02 13:42:11.000000 guify-0.2.6/src/guify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 13:42:11.000000 guify-0.2.6/src/guify.egg-info/top_level.txt
```

### Comparing `guify-0.2.5a5/LICENSE` & `guify-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/PKG-INFO` & `guify-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guify
-Version: 0.2.5a5
+Version: 0.2.6
 Summary: A tool that will GUI-ify your functions
 Author: Michael Druyan
 Author-email: michael@druyan.net
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `guify-0.2.5a5/README.md` & `guify-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/docs/README.md` & `guify-0.2.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/setup.cfg` & `guify-0.2.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = guify
-version = 0.2.5a5
+version = 0.2.6
 author = Michael Druyan
 author_email = michael@druyan.net
 description = A tool that will GUI-ify your functions
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `guify-0.2.5a5/src/guify/App.py` & `guify-0.2.6/src/guify/App.py`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify/BaseTest.py` & `guify-0.2.6/src/guify/BaseTest.py`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify/ConfigTab.py` & `guify-0.2.6/src/guify/ConfigTab.py`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify/TestPool.py` & `guify-0.2.6/src/guify/TestPool.py`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify/TestWorker.py` & `guify-0.2.6/src/guify/TestWorker.py`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify/__init__.py` & `guify-0.2.6/src/guify/__init__.py`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify/utils.py` & `guify-0.2.6/src/guify/utils.py`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify/web/favicon.ico` & `guify-0.2.6/src/guify/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify/web/index.html` & `guify-0.2.6/src/guify/web/index.html`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify/web/static/css/main.c779b13f.css` & `guify-0.2.6/src/guify/web/static/css/main.c779b13f.css`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify/web/static/css/main.c779b13f.css.map` & `guify-0.2.6/src/guify/web/static/css/main.c779b13f.css.map`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify/web/static/js/main.bf3c494e.js` & `guify-0.2.6/src/guify/web/static/js/main.bf3c494e.js`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify/web/static/js/main.bf3c494e.js.LICENSE.txt` & `guify-0.2.6/src/guify/web/static/js/main.bf3c494e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify/web/static/js/main.bf3c494e.js.map` & `guify-0.2.6/src/guify/web/static/js/main.bf3c494e.js.map`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify.egg-info/PKG-INFO` & `guify-0.2.6/src/guify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guify
-Version: 0.2.5a5
+Version: 0.2.6
 Summary: A tool that will GUI-ify your functions
 Author: Michael Druyan
 Author-email: michael@druyan.net
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `guify-0.2.5a5/src/guify.egg-info/SOURCES.txt` & `guify-0.2.6/src/guify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `guify-0.2.5a5/src/guify.egg-info/requires.txt` & `guify-0.2.6/src/guify.egg-info/requires.txt`

 * *Files identical despite different names*

