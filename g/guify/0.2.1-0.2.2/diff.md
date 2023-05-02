# Comparing `tmp/guify-0.2.1.tar.gz` & `tmp/guify-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guify-0.2.1.tar", last modified: Tue May  2 08:48:17 2023, max compression
+gzip compressed data, was "guify-0.2.2.tar", last modified: Tue May  2 10:29:37 2023, max compression
```

## Comparing `guify-0.2.1.tar` & `guify-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:48:17.593559 guify-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 08:47:19.000000 guify-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 08:47:19.000000 guify-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-02 08:48:17.593559 guify-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-02 08:47:19.000000 guify-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 08:47:19.000000 guify-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-02 08:48:17.593559 guify-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:48:17.593559 guify-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:48:17.593559 guify-0.2.1/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:48:17.593559 guify-0.2.1/src/python/guify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-02 08:48:17.000000 guify-0.2.1/src/python/guify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-02 08:48:17.000000 guify-0.2.1/src/python/guify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 08:48:17.000000 guify-0.2.1/src/python/guify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-02 08:48:17.000000 guify-0.2.1/src/python/guify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 08:48:17.000000 guify-0.2.1/src/python/guify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:29:37.224868 guify-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-02 10:28:28.000000 guify-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 10:28:28.000000 guify-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-02 10:29:37.224868 guify-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-02 10:28:28.000000 guify-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 10:28:28.000000 guify-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-02 10:29:37.224868 guify-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:29:37.224868 guify-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:29:37.224868 guify-0.2.2/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:29:37.224868 guify-0.2.2/src/python/guify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-02 10:29:37.000000 guify-0.2.2/src/python/guify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-02 10:29:37.000000 guify-0.2.2/src/python/guify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:29:37.000000 guify-0.2.2/src/python/guify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-02 10:29:37.000000 guify-0.2.2/src/python/guify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:29:37.000000 guify-0.2.2/src/python/guify.egg-info/top_level.txt
```

### Comparing `guify-0.2.1/LICENSE` & `guify-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `guify-0.2.1/PKG-INFO` & `guify-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guify
-Version: 0.2.1
+Version: 0.2.2
 Summary: A tool that will GUI-ify your functions
 Author: Michael Druyan
 Author-email: michael@druyan.net
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `guify-0.2.1/README.md` & `guify-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `guify-0.2.1/setup.cfg` & `guify-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = guify
-version = 0.2.1
+version = 0.2.2
 author = Michael Druyan
 author_email = michael@druyan.net
 description = A tool that will GUI-ify your functions
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `guify-0.2.1/src/python/guify.egg-info/PKG-INFO` & `guify-0.2.2/src/python/guify.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guify
-Version: 0.2.1
+Version: 0.2.2
 Summary: A tool that will GUI-ify your functions
 Author: Michael Druyan
 Author-email: michael@druyan.net
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `guify-0.2.1/src/python/guify.egg-info/requires.txt` & `guify-0.2.2/src/python/guify.egg-info/requires.txt`

 * *Files identical despite different names*

