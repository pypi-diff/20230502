# Comparing `tmp/cdk-stacksets-0.0.91.tar.gz` & `tmp/cdk-stacksets-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-stacksets-0.0.91.tar", last modified: Mon May  1 00:15:47 2023, max compression
+gzip compressed data, was "cdk-stacksets-0.0.92.tar", last modified: Tue May  2 00:14:53 2023, max compression
```

## Comparing `cdk-stacksets-0.0.91.tar` & `cdk-stacksets-0.0.92.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:15:47.539839 cdk-stacksets-0.0.91/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-01 00:15:32.000000 cdk-stacksets-0.0.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 00:15:32.000000 cdk-stacksets-0.0.91/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-01 00:15:47.539839 cdk-stacksets-0.0.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-01 00:15:32.000000 cdk-stacksets-0.0.91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-01 00:15:32.000000 cdk-stacksets-0.0.91/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 00:15:47.539839 cdk-stacksets-0.0.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-01 00:15:32.000000 cdk-stacksets-0.0.91/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:15:47.539839 cdk-stacksets-0.0.91/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:15:47.539839 cdk-stacksets-0.0.91/src/cdk_stacksets/
--rw-r--r--   0 runner    (1001) docker     (123)    83981 2023-05-01 00:15:32.000000 cdk-stacksets-0.0.91/src/cdk_stacksets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:15:47.539839 cdk-stacksets-0.0.91/src/cdk_stacksets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-01 00:15:32.000000 cdk-stacksets-0.0.91/src/cdk_stacksets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71057 2023-05-01 00:15:32.000000 cdk-stacksets-0.0.91/src/cdk_stacksets/_jsii/cdk-stacksets@0.0.91.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:15:32.000000 cdk-stacksets-0.0.91/src/cdk_stacksets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:15:47.539839 cdk-stacksets-0.0.91/src/cdk_stacksets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-01 00:15:47.000000 cdk-stacksets-0.0.91/src/cdk_stacksets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-01 00:15:47.000000 cdk-stacksets-0.0.91/src/cdk_stacksets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:15:47.000000 cdk-stacksets-0.0.91/src/cdk_stacksets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-01 00:15:47.000000 cdk-stacksets-0.0.91/src/cdk_stacksets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 00:15:47.000000 cdk-stacksets-0.0.91/src/cdk_stacksets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:14:53.459162 cdk-stacksets-0.0.92/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 00:14:37.000000 cdk-stacksets-0.0.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 00:14:37.000000 cdk-stacksets-0.0.92/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-02 00:14:53.459162 cdk-stacksets-0.0.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-02 00:14:37.000000 cdk-stacksets-0.0.92/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 00:14:37.000000 cdk-stacksets-0.0.92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 00:14:53.459162 cdk-stacksets-0.0.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-02 00:14:37.000000 cdk-stacksets-0.0.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:14:53.459162 cdk-stacksets-0.0.92/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:14:53.459162 cdk-stacksets-0.0.92/src/cdk_stacksets/
+-rw-r--r--   0 runner    (1001) docker     (123)    83981 2023-05-02 00:14:37.000000 cdk-stacksets-0.0.92/src/cdk_stacksets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:14:53.459162 cdk-stacksets-0.0.92/src/cdk_stacksets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-02 00:14:37.000000 cdk-stacksets-0.0.92/src/cdk_stacksets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71058 2023-05-02 00:14:37.000000 cdk-stacksets-0.0.92/src/cdk_stacksets/_jsii/cdk-stacksets@0.0.92.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:14:37.000000 cdk-stacksets-0.0.92/src/cdk_stacksets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:14:53.459162 cdk-stacksets-0.0.92/src/cdk_stacksets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-02 00:14:53.000000 cdk-stacksets-0.0.92/src/cdk_stacksets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-02 00:14:53.000000 cdk-stacksets-0.0.92/src/cdk_stacksets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:14:53.000000 cdk-stacksets-0.0.92/src/cdk_stacksets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-02 00:14:53.000000 cdk-stacksets-0.0.92/src/cdk_stacksets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 00:14:53.000000 cdk-stacksets-0.0.92/src/cdk_stacksets.egg-info/top_level.txt
```

### Comparing `cdk-stacksets-0.0.91/LICENSE` & `cdk-stacksets-0.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.91/PKG-INFO` & `cdk-stacksets-0.0.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-stacksets
-Version: 0.0.91
+Version: 0.0.92
 Summary: cdk-stacksets
 Home-page: https://github.com/cdklabs/cdk-stacksets.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-stacksets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-stacksets-0.0.91/README.md` & `cdk-stacksets-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.91/setup.py` & `cdk-stacksets-0.0.92/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-stacksets",
-    "version": "0.0.91",
+    "version": "0.0.92",
     "description": "cdk-stacksets",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-stacksets.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_stacksets",
         "cdk_stacksets._jsii"
     ],
     "package_data": {
         "cdk_stacksets._jsii": [
-            "cdk-stacksets@0.0.91.jsii.tgz"
+            "cdk-stacksets@0.0.92.jsii.tgz"
         ],
         "cdk_stacksets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-stacksets-0.0.91/src/cdk_stacksets/__init__.py` & `cdk-stacksets-0.0.92/src/cdk_stacksets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.91/src/cdk_stacksets.egg-info/PKG-INFO` & `cdk-stacksets-0.0.92/src/cdk_stacksets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-stacksets
-Version: 0.0.91
+Version: 0.0.92
 Summary: cdk-stacksets
 Home-page: https://github.com/cdklabs/cdk-stacksets.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-stacksets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

