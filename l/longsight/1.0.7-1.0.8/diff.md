# Comparing `tmp/longsight-1.0.7.tar.gz` & `tmp/longsight-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longsight-1.0.7.tar", last modified: Thu Apr 27 09:05:51 2023, max compression
+gzip compressed data, was "longsight-1.0.8.tar", last modified: Tue May  2 10:29:24 2023, max compression
```

## Comparing `longsight-1.0.7.tar` & `longsight-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-27 09:05:51.772607 longsight-1.0.7/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 longsight-1.0.7/LICENSE.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     7922 2023-04-27 09:05:51.772607 longsight-1.0.7/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     6051 2023-04-24 10:53:59.000000 longsight-1.0.7/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     1029 2023-04-27 08:54:33.000000 longsight-1.0.7/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)     1011 2023-04-27 09:05:51.772607 longsight-1.0.7/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-27 09:05:51.772607 longsight-1.0.7/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-27 09:05:51.772607 longsight-1.0.7/src/longsight/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-29 16:56:16.000000 longsight-1.0.7/src/longsight/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    13846 2023-04-27 08:50:15.000000 longsight-1.0.7/src/longsight/instrumentation.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-27 09:05:51.772607 longsight-1.0.7/src/longsight.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     7922 2023-04-27 09:05:51.000000 longsight-1.0.7/src/longsight.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      318 2023-04-27 09:05:51.000000 longsight-1.0.7/src/longsight.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-27 09:05:51.000000 longsight-1.0.7/src/longsight.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      131 2023-04-27 09:05:51.000000 longsight-1.0.7/src/longsight.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       10 2023-04-27 09:05:51.000000 longsight-1.0.7/src/longsight.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-27 09:05:51.772607 longsight-1.0.7/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)     8180 2023-04-27 08:50:44.000000 longsight-1.0.7/tests/test_instrumentation.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:29:24.062202 longsight-1.0.8/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 longsight-1.0.8/LICENSE.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8536 2023-05-02 10:29:24.062202 longsight-1.0.8/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6665 2023-04-27 09:11:46.000000 longsight-1.0.8/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1029 2023-05-02 10:29:03.000000 longsight-1.0.8/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1011 2023-05-02 10:29:24.062202 longsight-1.0.8/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:29:24.062202 longsight-1.0.8/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:29:24.062202 longsight-1.0.8/src/longsight/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-29 16:56:16.000000 longsight-1.0.8/src/longsight/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    14169 2023-05-02 10:14:58.000000 longsight-1.0.8/src/longsight/instrumentation.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:29:24.062202 longsight-1.0.8/src/longsight.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8536 2023-05-02 10:29:24.000000 longsight-1.0.8/src/longsight.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      318 2023-05-02 10:29:24.000000 longsight-1.0.8/src/longsight.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-02 10:29:24.000000 longsight-1.0.8/src/longsight.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      131 2023-05-02 10:29:24.000000 longsight-1.0.8/src/longsight.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       10 2023-05-02 10:29:24.000000 longsight-1.0.8/src/longsight.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:29:24.062202 longsight-1.0.8/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8180 2023-04-27 08:50:44.000000 longsight-1.0.8/tests/test_instrumentation.py
```

### Comparing `longsight-1.0.7/LICENSE.md` & `longsight-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `longsight-1.0.7/PKG-INFO` & `longsight-1.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longsight
-Version: 1.0.7
+Version: 1.0.8
 Summary: This library implements a range of common logging functions.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
         
@@ -89,14 +89,31 @@
 
     @instrument(create_aws=True, bucket="my-bucket")
     def a_function(instrumentation):
         instrumentation.logger.info("Hello, World!")
         s3_client = instrumentation.aws_connector.s3_client
         return
 
+## Easy counters
+The instrumentation class also provides a simple counter function to increment a counter in CloudWatch:
+
+    from longsight.instrumentation import instrument
+
+    @instrumentation.instrument(
+    cloudwatch_push=True,
+    log_stream_name="martin-test-stream-name",
+    log_group_name="martin-test-group-name",
+    namespace="martin-test-namespace",
+    )
+    def a_function(instrumentation):
+        instrumentation.add_counter(
+            metric_name="test_counter", status_code=200, member_id=None, 
+            additional_dimensions=[{"Name": "Environment", "Value": "Production"}]
+        )
+
 ## Correlation ID Middleware
 The AWSCorrelationIdMiddleware middleware automatically generates or loads a correlation ID for each incoming request, and attaches it to the request headers and logs. To use the middleware, create an instance of the AWSCorrelationIdMiddleware class and add it to your FastAPI application:
 
     from fastapi import FastAPI
     from longsight.instrumentation import AWSCorrelationIdMiddleware
     
     app = FastAPI()
```

### Comparing `longsight-1.0.7/README.md` & `longsight-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,31 @@
 
     @instrument(create_aws=True, bucket="my-bucket")
     def a_function(instrumentation):
         instrumentation.logger.info("Hello, World!")
         s3_client = instrumentation.aws_connector.s3_client
         return
 
+## Easy counters
+The instrumentation class also provides a simple counter function to increment a counter in CloudWatch:
+
+    from longsight.instrumentation import instrument
+
+    @instrumentation.instrument(
+    cloudwatch_push=True,
+    log_stream_name="martin-test-stream-name",
+    log_group_name="martin-test-group-name",
+    namespace="martin-test-namespace",
+    )
+    def a_function(instrumentation):
+        instrumentation.add_counter(
+            metric_name="test_counter", status_code=200, member_id=None, 
+            additional_dimensions=[{"Name": "Environment", "Value": "Production"}]
+        )
+
 ## Correlation ID Middleware
 The AWSCorrelationIdMiddleware middleware automatically generates or loads a correlation ID for each incoming request, and attaches it to the request headers and logs. To use the middleware, create an instance of the AWSCorrelationIdMiddleware class and add it to your FastAPI application:
 
     from fastapi import FastAPI
     from longsight.instrumentation import AWSCorrelationIdMiddleware
     
     app = FastAPI()
```

### Comparing `longsight-1.0.7/pyproject.toml` & `longsight-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "longsight"
-version = "1.0.7"
+version = "1.0.8"
 description = "This library implements a range of common logging functions."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.md"}
 keywords = ["distributed computing"]
 authors = [
   {email = "meve@crossref.org"},
```

### Comparing `longsight-1.0.7/setup.cfg` & `longsight-1.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = longsight
-version = 1.0.7
+version = 1.0.8
 description = This library implements a range of common logging functions.
 url = https://gitlab.com/crossref/labs/distrunner
 author = Martin Paul Eve
 author_email = meve@crossref.org
 license = MIT
 classifiers = 
 	Intended Audience :: Developers
```

### Comparing `longsight-1.0.7/src/longsight/instrumentation.py` & `longsight-1.0.8/src/longsight/instrumentation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import functools
 import inspect
 import logging
+import os
 from contextlib import AbstractContextManager, contextmanager
 from contextvars import ContextVar
 from datetime import datetime
 from logging import LogRecord
 from types import TracebackType
 from typing import Callable
 from typing import Optional
@@ -144,15 +145,21 @@
     def wrap(f):
         @contextmanager
         def wrapping_logic(*args, **kwargs):
             from claws import aws_utils
 
             if create_aws or cloudwatch_push:
                 # create the boto3 objects
-                aws_connector = aws_utils.AWSConnector(bucket=bucket)
+                aws_access_key_id = os.environ.get("AWS_ACCESS_KEY_ID")
+                aws_secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY")
+                aws_connector = aws_utils.AWSConnector(
+                    bucket=bucket,
+                    aws_access_key_id=aws_access_key_id,
+                    aws_secret_access_key=aws_secret_access_key,
+                )
             else:
                 aws_connector = None
 
             fastapi_request = kwargs.get("request", None)
             fastapi_app = fastapi_request.app if fastapi_request else None
 
             aws_context = (
```

### Comparing `longsight-1.0.7/src/longsight.egg-info/PKG-INFO` & `longsight-1.0.8/src/longsight.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longsight
-Version: 1.0.7
+Version: 1.0.8
 Summary: This library implements a range of common logging functions.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
         
@@ -89,14 +89,31 @@
 
     @instrument(create_aws=True, bucket="my-bucket")
     def a_function(instrumentation):
         instrumentation.logger.info("Hello, World!")
         s3_client = instrumentation.aws_connector.s3_client
         return
 
+## Easy counters
+The instrumentation class also provides a simple counter function to increment a counter in CloudWatch:
+
+    from longsight.instrumentation import instrument
+
+    @instrumentation.instrument(
+    cloudwatch_push=True,
+    log_stream_name="martin-test-stream-name",
+    log_group_name="martin-test-group-name",
+    namespace="martin-test-namespace",
+    )
+    def a_function(instrumentation):
+        instrumentation.add_counter(
+            metric_name="test_counter", status_code=200, member_id=None, 
+            additional_dimensions=[{"Name": "Environment", "Value": "Production"}]
+        )
+
 ## Correlation ID Middleware
 The AWSCorrelationIdMiddleware middleware automatically generates or loads a correlation ID for each incoming request, and attaches it to the request headers and logs. To use the middleware, create an instance of the AWSCorrelationIdMiddleware class and add it to your FastAPI application:
 
     from fastapi import FastAPI
     from longsight.instrumentation import AWSCorrelationIdMiddleware
     
     app = FastAPI()
```

### Comparing `longsight-1.0.7/tests/test_instrumentation.py` & `longsight-1.0.8/tests/test_instrumentation.py`

 * *Files identical despite different names*

