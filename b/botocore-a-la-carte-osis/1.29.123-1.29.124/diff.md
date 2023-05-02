# Comparing `tmp/botocore-a-la-carte-osis-1.29.123.tar.gz` & `tmp/botocore-a-la-carte-osis-1.29.124.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-osis-1.29.123.tar", last modified: Sat Apr 29 01:15:59 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-osis-1.29.124.tar", last modified: Tue May  2 01:16:34 2023, max compression
```

## Comparing `botocore-a-la-carte-osis-1.29.123.tar` & `botocore-a-la-carte-osis-1.29.124.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:15:59.156077 botocore-a-la-carte-osis-1.29.123/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-29 01:15:58.000000 botocore-a-la-carte-osis-1.29.123/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-29 01:15:59.156077 botocore-a-la-carte-osis-1.29.123/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:15:59.152076 botocore-a-la-carte-osis-1.29.123/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:15:59.152076 botocore-a-la-carte-osis-1.29.123/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:15:59.152076 botocore-a-la-carte-osis-1.29.123/botocore/data/osis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:15:59.156077 botocore-a-la-carte-osis-1.29.123/botocore/data/osis/2022-01-01/
--rw-r--r--   0 runner    (1001) docker     (123)    17616 2023-04-29 01:15:24.000000 botocore-a-la-carte-osis-1.29.123/botocore/data/osis/2022-01-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-29 01:15:24.000000 botocore-a-la-carte-osis-1.29.123/botocore/data/osis/2022-01-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-04-29 01:15:24.000000 botocore-a-la-carte-osis-1.29.123/botocore/data/osis/2022-01-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:15:59.156077 botocore-a-la-carte-osis-1.29.123/botocore_a_la_carte_osis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-29 01:15:59.000000 botocore-a-la-carte-osis-1.29.123/botocore_a_la_carte_osis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-29 01:15:59.000000 botocore-a-la-carte-osis-1.29.123/botocore_a_la_carte_osis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 01:15:59.000000 botocore-a-la-carte-osis-1.29.123/botocore_a_la_carte_osis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 01:15:59.000000 botocore-a-la-carte-osis-1.29.123/botocore_a_la_carte_osis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 01:15:59.156077 botocore-a-la-carte-osis-1.29.123/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-29 01:15:58.000000 botocore-a-la-carte-osis-1.29.123/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:16:34.406768 botocore-a-la-carte-osis-1.29.124/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-02 01:16:34.000000 botocore-a-la-carte-osis-1.29.124/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-02 01:16:34.406768 botocore-a-la-carte-osis-1.29.124/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:16:34.402768 botocore-a-la-carte-osis-1.29.124/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:16:34.402768 botocore-a-la-carte-osis-1.29.124/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:16:34.402768 botocore-a-la-carte-osis-1.29.124/botocore/data/osis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:16:34.402768 botocore-a-la-carte-osis-1.29.124/botocore/data/osis/2022-01-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17616 2023-05-02 01:15:57.000000 botocore-a-la-carte-osis-1.29.124/botocore/data/osis/2022-01-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 01:15:57.000000 botocore-a-la-carte-osis-1.29.124/botocore/data/osis/2022-01-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-05-02 01:15:57.000000 botocore-a-la-carte-osis-1.29.124/botocore/data/osis/2022-01-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:16:34.406768 botocore-a-la-carte-osis-1.29.124/botocore_a_la_carte_osis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-02 01:16:34.000000 botocore-a-la-carte-osis-1.29.124/botocore_a_la_carte_osis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-02 01:16:34.000000 botocore-a-la-carte-osis-1.29.124/botocore_a_la_carte_osis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 01:16:34.000000 botocore-a-la-carte-osis-1.29.124/botocore_a_la_carte_osis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 01:16:34.000000 botocore-a-la-carte-osis-1.29.124/botocore_a_la_carte_osis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 01:16:34.406768 botocore-a-la-carte-osis-1.29.124/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-02 01:16:34.000000 botocore-a-la-carte-osis-1.29.124/setup.py
```

### Comparing `botocore-a-la-carte-osis-1.29.123/LICENSE.txt` & `botocore-a-la-carte-osis-1.29.124/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-osis-1.29.123/PKG-INFO` & `botocore-a-la-carte-osis-1.29.124/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-osis
-Version: 1.29.123
+Version: 1.29.124
 Summary: osis data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-osis-1.29.123/botocore/data/osis/2022-01-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-osis-1.29.124/botocore/data/osis/2022-01-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-osis-1.29.123/botocore/data/osis/2022-01-01/service-2.json` & `botocore-a-la-carte-osis-1.29.124/botocore/data/osis/2022-01-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-osis-1.29.123/botocore_a_la_carte_osis.egg-info/PKG-INFO` & `botocore-a-la-carte-osis-1.29.124/botocore_a_la_carte_osis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-osis
-Version: 1.29.123
+Version: 1.29.124
 Summary: osis data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-osis-1.29.123/setup.py` & `botocore-a-la-carte-osis-1.29.124/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-osis',
-    version="1.29.123",
+    version="1.29.124",
     description='osis data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/osis/*/*.json'],
```

