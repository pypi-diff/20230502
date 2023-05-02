# Comparing `tmp/guify-0.2.2.tar.gz` & `tmp/guify-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guify-0.2.2.tar", last modified: Tue May  2 10:29:37 2023, max compression
+gzip compressed data, was "guify-0.2.4.tar", last modified: Tue May  2 10:59:37 2023, max compression
```

## Comparing `guify-0.2.2.tar` & `guify-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:29:37.224868 guify-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 10:28:28.000000 guify-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 10:28:28.000000 guify-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-02 10:29:37.224868 guify-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-02 10:28:28.000000 guify-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 10:28:28.000000 guify-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-02 10:29:37.224868 guify-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:29:37.224868 guify-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:29:37.224868 guify-0.2.2/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:29:37.224868 guify-0.2.2/src/python/guify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-02 10:29:37.000000 guify-0.2.2/src/python/guify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-02 10:29:37.000000 guify-0.2.2/src/python/guify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:29:37.000000 guify-0.2.2/src/python/guify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-02 10:29:37.000000 guify-0.2.2/src/python/guify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:29:37.000000 guify-0.2.2/src/python/guify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:59:37.644190 guify-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 10:58:24.000000 guify-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 10:58:24.000000 guify-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-02 10:59:37.644190 guify-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-02 10:58:24.000000 guify-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:59:37.644190 guify-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-02 10:58:24.000000 guify-0.2.4/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 10:58:24.000000 guify-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-02 10:59:37.644190 guify-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:59:37.640190 guify-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:59:37.644190 guify-0.2.4/src/guify/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-02 10:58:24.000000 guify-0.2.4/src/guify/App.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-02 10:58:24.000000 guify-0.2.4/src/guify/BaseTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-02 10:58:24.000000 guify-0.2.4/src/guify/ConfigTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-02 10:58:24.000000 guify-0.2.4/src/guify/Monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-02 10:58:24.000000 guify-0.2.4/src/guify/TestPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-02 10:58:24.000000 guify-0.2.4/src/guify/TestWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-02 10:58:24.000000 guify-0.2.4/src/guify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 10:58:24.000000 guify-0.2.4/src/guify/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-02 10:58:24.000000 guify-0.2.4/src/guify/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:59:37.644190 guify-0.2.4/src/guify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-02 10:59:37.000000 guify-0.2.4/src/guify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-02 10:59:37.000000 guify-0.2.4/src/guify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:59:37.000000 guify-0.2.4/src/guify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-02 10:59:37.000000 guify-0.2.4/src/guify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 10:59:37.000000 guify-0.2.4/src/guify.egg-info/top_level.txt
```

### Comparing `guify-0.2.2/LICENSE` & `guify-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `guify-0.2.2/README.md` & `guify-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `guify-0.2.2/setup.cfg` & `guify-0.2.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [metadata]
 name = guify
-version = 0.2.2
+version = 0.2.4
 author = Michael Druyan
 author_email = michael@druyan.net
 description = A tool that will GUI-ify your functions
-long_description = file: README.md
+long_description = file: docs/README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
 package_dir = 
-	= src/python
+	= src
 packages = find:
 include_package_data = true
 install_requires = 
 	bottle==0.12.25
 	bottle-websocket==0.2.9
 	cffi==1.15.1 ; platform_python_implementation == 'CPython' and sys_platform == 'win32'
 	eel==0.16.0
@@ -28,15 +28,15 @@
 	pyparsing==3.0.9 ; python_full_version >= '3.6.8'
 	setuptools==67.7.2 ; python_version >= '3.7'
 	whichcraft==0.6.1
 	zope.event==4.6
 	zope.interface==6.0 ; python_version >= '3.7'
 
 [options.packages.find]
-where = src/python
+where = src
 
 [options.package_data]
 guify = build/*
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `guify-0.2.2/src/python/guify.egg-info/requires.txt` & `guify-0.2.4/src/guify.egg-info/requires.txt`

 * *Files identical despite different names*

