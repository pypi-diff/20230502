# Comparing `tmp/cdk-image-pipeline-0.2.1.tar.gz` & `tmp/cdk-image-pipeline-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-image-pipeline-0.2.1.tar", last modified: Mon Apr 24 15:27:31 2023, max compression
+gzip compressed data, was "cdk-image-pipeline-0.3.0.tar", last modified: Mon May  1 17:12:56 2023, max compression
```

## Comparing `cdk-image-pipeline-0.2.1.tar` & `cdk-image-pipeline-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:27:31.948847 cdk-image-pipeline-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-24 15:27:31.948847 cdk-image-pipeline-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:27:31.948847 cdk-image-pipeline-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:27:31.944847 cdk-image-pipeline-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:27:31.948847 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)    39572 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:27:31.948847 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27727 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline/_jsii/cdk-image-pipeline@0.2.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:27:31.948847 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-24 15:27:31.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-24 15:27:31.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:27:31.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-24 15:27:31.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 15:27:31.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:12:56.455348 cdk-image-pipeline-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-01 17:12:42.000000 cdk-image-pipeline-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 17:12:42.000000 cdk-image-pipeline-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-01 17:12:56.455348 cdk-image-pipeline-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-05-01 17:12:42.000000 cdk-image-pipeline-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-01 17:12:42.000000 cdk-image-pipeline-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 17:12:56.455348 cdk-image-pipeline-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-01 17:12:42.000000 cdk-image-pipeline-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:12:56.455348 cdk-image-pipeline-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:12:56.455348 cdk-image-pipeline-0.3.0/src/cdk_image_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)    39572 2023-05-01 17:12:42.000000 cdk-image-pipeline-0.3.0/src/cdk_image_pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:12:56.455348 cdk-image-pipeline-0.3.0/src/cdk_image_pipeline/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-01 17:12:42.000000 cdk-image-pipeline-0.3.0/src/cdk_image_pipeline/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28100 2023-05-01 17:12:42.000000 cdk-image-pipeline-0.3.0/src/cdk_image_pipeline/_jsii/cdk-image-pipeline@0.3.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:12:42.000000 cdk-image-pipeline-0.3.0/src/cdk_image_pipeline/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:12:56.455348 cdk-image-pipeline-0.3.0/src/cdk_image_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-01 17:12:56.000000 cdk-image-pipeline-0.3.0/src/cdk_image_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-01 17:12:56.000000 cdk-image-pipeline-0.3.0/src/cdk_image_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:12:56.000000 cdk-image-pipeline-0.3.0/src/cdk_image_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-01 17:12:56.000000 cdk-image-pipeline-0.3.0/src/cdk_image_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 17:12:56.000000 cdk-image-pipeline-0.3.0/src/cdk_image_pipeline.egg-info/top_level.txt
```

### Comparing `cdk-image-pipeline-0.2.1/LICENSE` & `cdk-image-pipeline-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-image-pipeline-0.2.1/PKG-INFO` & `cdk-image-pipeline-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-image-pipeline
-Version: 0.2.1
+Version: 0.3.0
 Summary: Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK
 Home-page: https://github.com/aws-samples/cdk-image-pipeline.git
 Author: Cameron Magee<magcamer@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/cdk-image-pipeline.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-image-pipeline-0.2.1/README.md` & `cdk-image-pipeline-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-image-pipeline-0.2.1/setup.py` & `cdk-image-pipeline-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-image-pipeline",
-    "version": "0.2.1",
+    "version": "0.3.0",
     "description": "Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK",
     "license": "MIT-0",
     "url": "https://github.com/aws-samples/cdk-image-pipeline.git",
     "long_description_content_type": "text/markdown",
     "author": "Cameron Magee<magcamer@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_image_pipeline",
         "cdk_image_pipeline._jsii"
     ],
     "package_data": {
         "cdk_image_pipeline._jsii": [
-            "cdk-image-pipeline@0.2.1.jsii.tgz"
+            "cdk-image-pipeline@0.3.0.jsii.tgz"
         ],
         "cdk_image_pipeline": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-image-pipeline-0.2.1/src/cdk_image_pipeline/__init__.py` & `cdk-image-pipeline-0.3.0/src/cdk_image_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-image-pipeline-0.2.1/src/cdk_image_pipeline.egg-info/PKG-INFO` & `cdk-image-pipeline-0.3.0/src/cdk_image_pipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-image-pipeline
-Version: 0.2.1
+Version: 0.3.0
 Summary: Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK
 Home-page: https://github.com/aws-samples/cdk-image-pipeline.git
 Author: Cameron Magee<magcamer@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/cdk-image-pipeline.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

