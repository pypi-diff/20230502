# Comparing `tmp/echostream-node-0.3.8.tar.gz` & `tmp/echostream-node-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echostream-node-0.3.8.tar", last modified: Fri Apr  7 16:23:31 2023, max compression
+gzip compressed data, was "echostream-node-0.3.9.tar", last modified: Mon May  1 23:48:39 2023, max compression
```

## Comparing `echostream-node-0.3.8.tar` & `echostream-node-0.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:23:31.703426 echostream-node-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-07 16:22:52.000000 echostream-node-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 16:22:52.000000 echostream-node-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-07 16:23:31.703426 echostream-node-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-07 16:22:52.000000 echostream-node-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:23:31.703426 echostream-node-0.3.8/echostream_node/
--rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-04-07 16:22:52.000000 echostream-node-0.3.8/echostream_node/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:23:31.703426 echostream-node-0.3.8/echostream_node/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)    34186 2023-04-07 16:22:52.000000 echostream-node-0.3.8/echostream_node/asyncio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:23:31.703426 echostream-node-0.3.8/echostream_node/threading/
--rw-r--r--   0 runner    (1001) docker     (123)    29306 2023-04-07 16:22:52.000000 echostream-node-0.3.8/echostream_node/threading/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:23:31.703426 echostream-node-0.3.8/echostream_node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-07 16:23:31.000000 echostream-node-0.3.8/echostream_node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-07 16:23:31.000000 echostream-node-0.3.8/echostream_node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:23:31.000000 echostream-node-0.3.8/echostream_node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-07 16:23:31.000000 echostream-node-0.3.8/echostream_node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-07 16:23:31.000000 echostream-node-0.3.8/echostream_node.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-07 16:22:52.000000 echostream-node-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-07 16:23:31.703426 echostream-node-0.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:48:39.895714 echostream-node-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 23:47:50.000000 echostream-node-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 23:47:50.000000 echostream-node-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-05-01 23:48:39.895714 echostream-node-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-05-01 23:47:50.000000 echostream-node-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:48:39.891714 echostream-node-0.3.9/echostream_node/
+-rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-05-01 23:47:50.000000 echostream-node-0.3.9/echostream_node/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:48:39.891714 echostream-node-0.3.9/echostream_node/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)    34186 2023-05-01 23:47:50.000000 echostream-node-0.3.9/echostream_node/asyncio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:48:39.895714 echostream-node-0.3.9/echostream_node/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)    29306 2023-05-01 23:47:50.000000 echostream-node-0.3.9/echostream_node/threading/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:48:39.891714 echostream-node-0.3.9/echostream_node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-05-01 23:48:39.000000 echostream-node-0.3.9/echostream_node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-01 23:48:39.000000 echostream-node-0.3.9/echostream_node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:48:39.000000 echostream-node-0.3.9/echostream_node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-01 23:48:39.000000 echostream-node-0.3.9/echostream_node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 23:48:39.000000 echostream-node-0.3.9/echostream_node.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-01 23:47:50.000000 echostream-node-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-01 23:48:39.895714 echostream-node-0.3.9/setup.cfg
```

### Comparing `echostream-node-0.3.8/LICENSE` & `echostream-node-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `echostream-node-0.3.8/PKG-INFO` & `echostream-node-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echostream-node
-Version: 0.3.8
+Version: 0.3.9
 Summary: EchoStream library for implementing remote nodes
 Author: EchoStream
 Author-email: pypi@echo.stream
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echostream-node-0.3.8/README.md` & `echostream-node-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `echostream-node-0.3.8/echostream_node/__init__.py` & `echostream-node-0.3.9/echostream_node/__init__.py`

 * *Files identical despite different names*

### Comparing `echostream-node-0.3.8/echostream_node/asyncio/__init__.py` & `echostream-node-0.3.9/echostream_node/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `echostream-node-0.3.8/echostream_node/threading/__init__.py` & `echostream-node-0.3.9/echostream_node/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `echostream-node-0.3.8/echostream_node.egg-info/PKG-INFO` & `echostream-node-0.3.9/echostream_node.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echostream-node
-Version: 0.3.8
+Version: 0.3.9
 Summary: EchoStream library for implementing remote nodes
 Author: EchoStream
 Author-email: pypi@echo.stream
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echostream-node-0.3.8/setup.cfg` & `echostream-node-0.3.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [metadata]
 name = echostream-node
 author = EchoStream
 author_email = pypi@echo.stream
-version = 0.3.8
+version = 0.3.9
 description = EchoStream library for implementing remote nodes
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 packages = find:
 include_package_data = true
 install_requires = 
 	aws-error-utils==2.7.0
 	awsserviceendpoints==0.0.2
 	dynamic-function-loader==0.0.3
 	echostream-botocore==0.0.2
 	gql[aiohttp,requests]==3.4.0
 	gql-appsync-cognito-authentication==0.0.1
-	httpx==0.23.3
-	httpx-auth==0.15.0
+	httpx==0.24.0
+	httpx-auth==0.17.0
 	pycognito==2022.12.0
 	simplejson==3.19.1
 python_requires = >=3.9
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

