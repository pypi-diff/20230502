# Comparing `tmp/neulabs-cdk-constructs-0.2.4.tar.gz` & `tmp/neulabs-cdk-constructs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neulabs-cdk-constructs-0.2.4.tar", last modified: Fri Apr 21 14:18:07 2023, max compression
+gzip compressed data, was "neulabs-cdk-constructs-0.3.0.tar", last modified: Tue May  2 15:15:24 2023, max compression
```

## Comparing `neulabs-cdk-constructs-0.2.4.tar` & `neulabs-cdk-constructs-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:18:07.281666 neulabs-cdk-constructs-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 14:17:55.000000 neulabs-cdk-constructs-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 14:17:55.000000 neulabs-cdk-constructs-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-21 14:18:07.281666 neulabs-cdk-constructs-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-21 14:17:55.000000 neulabs-cdk-constructs-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-21 14:17:55.000000 neulabs-cdk-constructs-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:18:07.281666 neulabs-cdk-constructs-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-21 14:17:55.000000 neulabs-cdk-constructs-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:18:07.277666 neulabs-cdk-constructs-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:18:07.281666 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-21 14:17:55.000000 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:18:07.281666 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-21 14:17:55.000000 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   325953 2023-04-21 14:17:55.000000 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.2.4.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:18:07.281666 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)   221164 2023-04-21 14:17:55.000000 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/aws_lambda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:18:07.281666 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)    40775 2023-04-21 14:17:55.000000 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:18:07.281666 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    38906 2023-04-21 14:17:55.000000 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:17:55.000000 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:18:07.281666 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/stack/
--rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-04-21 14:17:55.000000 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:18:07.281666 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-21 14:17:55.000000 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:18:07.281666 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-21 14:18:06.000000 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-21 14:18:07.000000 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:18:06.000000 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-21 14:18:07.000000 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 14:18:07.000000 neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.047906 neulabs-cdk-constructs-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   325919 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.3.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)   221164 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/aws_lambda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)    40775 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    38906 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-02 15:15:11.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:15:24.051906 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-02 15:15:24.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-02 15:15:24.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:15:24.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-02 15:15:24.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 15:15:24.000000 neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/top_level.txt
```

### Comparing `neulabs-cdk-constructs-0.2.4/LICENSE` & `neulabs-cdk-constructs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.4/PKG-INFO` & `neulabs-cdk-constructs-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.2.4
+Version: 0.3.0
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -101,9 +101,7 @@
 ### Contributors
 
 <a href="https://github.com/neulabscom/neulabs-cdk-constructs/graphs/contributors"> <img src="https://contrib.rocks/image?repo=neulabscom/neulabs-cdk-constructs" /> </a>
 
 ### License
 
 See the `LICENSE` file for more information.
-
-
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: neulabs-cdk-constructs Version: 0.2.4 Summary:
+Metadata-Version: 2.1 Name: neulabs-cdk-constructs Version: 0.3.0 Summary:
 neulabs-cdk-constructs Home-page: https://github.com/neulabscom/neulabs-cdk-
 constructs.git Author: Neulabs
 neulabs.com> License: Apache-2.0 Project-URL: Source, https://github.com/
-neulabscom/neulabs-cdk-constructs.git Platform: UNKNOWN Classifier: Intended
-Audience :: Developers Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: JavaScript Classifier: Programming Language
-:: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Typing :: Typed Classifier: Development Status :: 5 - Production/
-Stable Classifier: License :: OSI Approved Requires-Python: ~=3.7 Description-
-Content-Type: text/markdown License-File: LICENSE # Neulabs CDK Constructs [!
-[NPM](https://img.shields.io/npm/v/neulabs-cdk-
-constructs?color=blue&label=npm+cdk)](https://www.npmjs.com/package/neulabs-
-cdk-constructs) [![PyPI](https://img.shields.io/pypi/v/neulabs-cdk-
+neulabscom/neulabs-cdk-constructs.git Classifier: Intended Audience ::
+Developers Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: JavaScript Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Typing :: Typed Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+Requires-Python: ~=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE # Neulabs CDK Constructs [![NPM](https://img.shields.io/npm/v/neulabs-
+cdk-constructs?color=blue&label=npm+cdk)](https://www.npmjs.com/package/
+neulabs-cdk-constructs) [![PyPI](https://img.shields.io/pypi/v/neulabs-cdk-
 constructs?color=blue&label=pypi+cdk)](https://pypi.org/project/neulabs-cdk-
 constructs/) [![PyPI](https://img.shields.io/github/last-commit/neulabscom/
 neulabs-cdk-constructs/main)](https://github.com/neulabscom/neulabs-cdk-
 constructs/commits/main) [![License](https://img.shields.io/badge/license-
 Apache--2.0-blue)](https://github.com/neulabscom/neulabs-cdk-constructs/blob/
 main/LICENSE) The neulabs-cdk-constructs library contains CDK-based constructs
 and stacks to allow the creation of cloud infrastructure on AWS. The purpose of
```

### Comparing `neulabs-cdk-constructs-0.2.4/README.md` & `neulabs-cdk-constructs-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.4/setup.py` & `neulabs-cdk-constructs-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "neulabs-cdk-constructs",
-    "version": "0.2.4",
+    "version": "0.3.0",
     "description": "neulabs-cdk-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/neulabscom/neulabs-cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Neulabs<tech@neulabs.com>",
     "bdist_wheel": {
         "universal": true
@@ -27,39 +27,40 @@
         "neulabs_cdk_constructs.newrelic",
         "neulabs_cdk_constructs.oidc",
         "neulabs_cdk_constructs.stack",
         "neulabs_cdk_constructs.utils"
     ],
     "package_data": {
         "neulabs_cdk_constructs._jsii": [
-            "neulabs-cdk-constructs@0.2.4.jsii.tgz"
+            "neulabs-cdk-constructs@0.3.0.jsii.tgz"
         ],
         "neulabs_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.68.0",
-        "aws-cdk.aws-apigatewayv2-alpha==2.68.0.a0",
-        "aws-cdk.aws-apigatewayv2-integrations-alpha==2.68.0.a0",
+        "aws-cdk-lib==2.77.0",
+        "aws-cdk.aws-apigatewayv2-alpha==2.77.0.a0",
+        "aws-cdk.aws-apigatewayv2-integrations-alpha==2.77.0.a0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.74.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/__init__.py` & `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/_jsii/__init__.py` & `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/_jsii/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aws_cdk._jsii
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_apigatewayv2_integrations_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "neulabs-cdk-constructs",
-    "0.2.4",
+    "0.3.0",
     __name__[0:-6],
-    "neulabs-cdk-constructs@0.2.4.jsii.tgz",
+    "neulabs-cdk-constructs@0.3.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/aws_lambda/__init__.py` & `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/aws_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/newrelic/__init__.py` & `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/oidc/__init__.py` & `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/stack/__init__.py` & `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs/utils/__init__.py` & `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs.egg-info/PKG-INFO` & `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.2.4
+Version: 0.3.0
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -101,9 +101,7 @@
 ### Contributors
 
 <a href="https://github.com/neulabscom/neulabs-cdk-constructs/graphs/contributors"> <img src="https://contrib.rocks/image?repo=neulabscom/neulabs-cdk-constructs" /> </a>
 
 ### License
 
 See the `LICENSE` file for more information.
-
-
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: neulabs-cdk-constructs Version: 0.2.4 Summary:
+Metadata-Version: 2.1 Name: neulabs-cdk-constructs Version: 0.3.0 Summary:
 neulabs-cdk-constructs Home-page: https://github.com/neulabscom/neulabs-cdk-
 constructs.git Author: Neulabs
 neulabs.com> License: Apache-2.0 Project-URL: Source, https://github.com/
-neulabscom/neulabs-cdk-constructs.git Platform: UNKNOWN Classifier: Intended
-Audience :: Developers Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: JavaScript Classifier: Programming Language
-:: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Typing :: Typed Classifier: Development Status :: 5 - Production/
-Stable Classifier: License :: OSI Approved Requires-Python: ~=3.7 Description-
-Content-Type: text/markdown License-File: LICENSE # Neulabs CDK Constructs [!
-[NPM](https://img.shields.io/npm/v/neulabs-cdk-
-constructs?color=blue&label=npm+cdk)](https://www.npmjs.com/package/neulabs-
-cdk-constructs) [![PyPI](https://img.shields.io/pypi/v/neulabs-cdk-
+neulabscom/neulabs-cdk-constructs.git Classifier: Intended Audience ::
+Developers Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: JavaScript Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Typing :: Typed Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+Requires-Python: ~=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE # Neulabs CDK Constructs [![NPM](https://img.shields.io/npm/v/neulabs-
+cdk-constructs?color=blue&label=npm+cdk)](https://www.npmjs.com/package/
+neulabs-cdk-constructs) [![PyPI](https://img.shields.io/pypi/v/neulabs-cdk-
 constructs?color=blue&label=pypi+cdk)](https://pypi.org/project/neulabs-cdk-
 constructs/) [![PyPI](https://img.shields.io/github/last-commit/neulabscom/
 neulabs-cdk-constructs/main)](https://github.com/neulabscom/neulabs-cdk-
 constructs/commits/main) [![License](https://img.shields.io/badge/license-
 Apache--2.0-blue)](https://github.com/neulabscom/neulabs-cdk-constructs/blob/
 main/LICENSE) The neulabs-cdk-constructs library contains CDK-based constructs
 and stacks to allow the creation of cloud infrastructure on AWS. The purpose of
```

### Comparing `neulabs-cdk-constructs-0.2.4/src/neulabs_cdk_constructs.egg-info/SOURCES.txt` & `neulabs-cdk-constructs-0.3.0/src/neulabs_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/neulabs_cdk_constructs/py.typed
 src/neulabs_cdk_constructs.egg-info/PKG-INFO
 src/neulabs_cdk_constructs.egg-info/SOURCES.txt
 src/neulabs_cdk_constructs.egg-info/dependency_links.txt
 src/neulabs_cdk_constructs.egg-info/requires.txt
 src/neulabs_cdk_constructs.egg-info/top_level.txt
 src/neulabs_cdk_constructs/_jsii/__init__.py
-src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.2.4.jsii.tgz
+src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.3.0.jsii.tgz
 src/neulabs_cdk_constructs/aws_lambda/__init__.py
 src/neulabs_cdk_constructs/newrelic/__init__.py
 src/neulabs_cdk_constructs/oidc/__init__.py
 src/neulabs_cdk_constructs/stack/__init__.py
 src/neulabs_cdk_constructs/utils/__init__.py
```

