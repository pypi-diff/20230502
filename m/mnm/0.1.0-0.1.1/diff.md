# Comparing `tmp/mnm-0.1.0.tar.gz` & `tmp/mnm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnm-0.1.0.tar", last modified: Mon May  1 13:02:41 2023, max compression
+gzip compressed data, was "mnm-0.1.1.tar", last modified: Tue May  2 00:19:04 2023, max compression
```

## Comparing `mnm-0.1.0.tar` & `mnm-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-01 13:02:41.552071 mnm-0.1.0/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1067 2023-05-01 04:28:16.000000 mnm-0.1.0/LICENSE
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      926 2023-05-01 13:02:41.552071 mnm-0.1.0/PKG-INFO
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      403 2023-05-01 12:59:53.000000 mnm-0.1.0/README.md
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      636 2023-05-01 13:02:31.000000 mnm-0.1.0/pyproject.toml
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       38 2023-05-01 13:02:41.552071 mnm-0.1.0/setup.cfg
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-01 13:02:41.542071 mnm-0.1.0/src/
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-01 13:02:41.552071 mnm-0.1.0/src/mnm/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     4061 2023-05-01 12:57:05.000000 mnm-0.1.0/src/mnm/__init__.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      183 2023-05-01 12:58:39.000000 mnm-0.1.0/src/mnm/example.py
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-01 13:02:41.552071 mnm-0.1.0/src/mnm.egg-info/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      926 2023-05-01 13:02:41.000000 mnm-0.1.0/src/mnm.egg-info/PKG-INFO
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      225 2023-05-01 13:02:41.000000 mnm-0.1.0/src/mnm.egg-info/SOURCES.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        1 2023-05-01 13:02:41.000000 mnm-0.1.0/src/mnm.egg-info/dependency_links.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       29 2023-05-01 13:02:41.000000 mnm-0.1.0/src/mnm.egg-info/requires.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        4 2023-05-01 13:02:41.000000 mnm-0.1.0/src/mnm.egg-info/top_level.txt
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-02 00:19:04.252639 mnm-0.1.1/
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1067 2023-05-01 04:28:16.000000 mnm-0.1.1/LICENSE
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      926 2023-05-02 00:19:04.252639 mnm-0.1.1/PKG-INFO
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      403 2023-05-01 12:59:53.000000 mnm-0.1.1/README.md
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      636 2023-05-02 00:18:54.000000 mnm-0.1.1/pyproject.toml
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       38 2023-05-02 00:19:04.252639 mnm-0.1.1/setup.cfg
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-02 00:19:04.252639 mnm-0.1.1/src/
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-02 00:19:04.252639 mnm-0.1.1/src/mnm/
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     4061 2023-05-01 12:57:05.000000 mnm-0.1.1/src/mnm/__init__.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      183 2023-05-01 13:05:36.000000 mnm-0.1.1/src/mnm/example.py
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-02 00:19:04.252639 mnm-0.1.1/src/mnm.egg-info/
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      926 2023-05-02 00:19:04.000000 mnm-0.1.1/src/mnm.egg-info/PKG-INFO
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      225 2023-05-02 00:19:04.000000 mnm-0.1.1/src/mnm.egg-info/SOURCES.txt
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        1 2023-05-02 00:19:04.000000 mnm-0.1.1/src/mnm.egg-info/dependency_links.txt
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       29 2023-05-02 00:19:04.000000 mnm-0.1.1/src/mnm.egg-info/requires.txt
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        4 2023-05-02 00:19:04.000000 mnm-0.1.1/src/mnm.egg-info/top_level.txt
```

### Comparing `mnm-0.1.0/LICENSE` & `mnm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mnm-0.1.0/PKG-INFO` & `mnm-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnm
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple python library for pentesting firewall protected webapp
 Author-email: ohk990102 <ohk990102@gmail.com>
 Project-URL: Homepage, https://github.com/ohk990102/mnm
 Project-URL: Bug Tracker, https://github.com/ohk990102/mnm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `mnm-0.1.0/pyproject.toml` & `mnm-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mnm"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="ohk990102", email="ohk990102@gmail.com" },
 ]
 description = "A simple python library for pentesting firewall protected webapp"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `mnm-0.1.0/src/mnm/__init__.py` & `mnm-0.1.1/src/mnm/__init__.py`

 * *Files identical despite different names*

### Comparing `mnm-0.1.0/src/mnm.egg-info/PKG-INFO` & `mnm-0.1.1/src/mnm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnm
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple python library for pentesting firewall protected webapp
 Author-email: ohk990102 <ohk990102@gmail.com>
 Project-URL: Homepage, https://github.com/ohk990102/mnm
 Project-URL: Bug Tracker, https://github.com/ohk990102/mnm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

