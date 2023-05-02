# Comparing `tmp/longsight-1.0.8.tar.gz` & `tmp/longsight-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longsight-1.0.8.tar", last modified: Tue May  2 10:29:24 2023, max compression
+gzip compressed data, was "longsight-1.0.9.tar", last modified: Tue May  2 10:36:43 2023, max compression
```

## Comparing `longsight-1.0.8.tar` & `longsight-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:29:24.062202 longsight-1.0.8/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 longsight-1.0.8/LICENSE.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     8536 2023-05-02 10:29:24.062202 longsight-1.0.8/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     6665 2023-04-27 09:11:46.000000 longsight-1.0.8/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     1029 2023-05-02 10:29:03.000000 longsight-1.0.8/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)     1011 2023-05-02 10:29:24.062202 longsight-1.0.8/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:29:24.062202 longsight-1.0.8/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:29:24.062202 longsight-1.0.8/src/longsight/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-29 16:56:16.000000 longsight-1.0.8/src/longsight/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    14169 2023-05-02 10:14:58.000000 longsight-1.0.8/src/longsight/instrumentation.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:29:24.062202 longsight-1.0.8/src/longsight.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     8536 2023-05-02 10:29:24.000000 longsight-1.0.8/src/longsight.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      318 2023-05-02 10:29:24.000000 longsight-1.0.8/src/longsight.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-02 10:29:24.000000 longsight-1.0.8/src/longsight.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      131 2023-05-02 10:29:24.000000 longsight-1.0.8/src/longsight.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       10 2023-05-02 10:29:24.000000 longsight-1.0.8/src/longsight.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:29:24.062202 longsight-1.0.8/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)     8180 2023-04-27 08:50:44.000000 longsight-1.0.8/tests/test_instrumentation.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:36:43.251808 longsight-1.0.9/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 longsight-1.0.9/LICENSE.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8536 2023-05-02 10:36:43.251808 longsight-1.0.9/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6665 2023-04-27 09:11:46.000000 longsight-1.0.9/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1029 2023-05-02 10:36:34.000000 longsight-1.0.9/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1011 2023-05-02 10:36:43.251808 longsight-1.0.9/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:36:43.251808 longsight-1.0.9/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:36:43.251808 longsight-1.0.9/src/longsight/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-29 16:56:16.000000 longsight-1.0.9/src/longsight/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    14317 2023-05-02 10:36:34.000000 longsight-1.0.9/src/longsight/instrumentation.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:36:43.251808 longsight-1.0.9/src/longsight.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8536 2023-05-02 10:36:43.000000 longsight-1.0.9/src/longsight.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      318 2023-05-02 10:36:43.000000 longsight-1.0.9/src/longsight.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-02 10:36:43.000000 longsight-1.0.9/src/longsight.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      131 2023-05-02 10:36:43.000000 longsight-1.0.9/src/longsight.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       10 2023-05-02 10:36:43.000000 longsight-1.0.9/src/longsight.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-02 10:36:43.251808 longsight-1.0.9/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8180 2023-04-27 08:50:44.000000 longsight-1.0.9/tests/test_instrumentation.py
```

### Comparing `longsight-1.0.8/LICENSE.md` & `longsight-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `longsight-1.0.8/PKG-INFO` & `longsight-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longsight
-Version: 1.0.8
+Version: 1.0.9
 Summary: This library implements a range of common logging functions.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `longsight-1.0.8/README.md` & `longsight-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `longsight-1.0.8/pyproject.toml` & `longsight-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "longsight"
-version = "1.0.8"
+version = "1.0.9"
 description = "This library implements a range of common logging functions."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.md"}
 keywords = ["distributed computing"]
 authors = [
   {email = "meve@crossref.org"},
```

### Comparing `longsight-1.0.8/setup.cfg` & `longsight-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = longsight
-version = 1.0.8
+version = 1.0.9
 description = This library implements a range of common logging functions.
 url = https://gitlab.com/crossref/labs/distrunner
 author = Martin Paul Eve
 author_email = meve@crossref.org
 license = MIT
 classifiers = 
 	Intended Audience :: Developers
```

### Comparing `longsight-1.0.8/src/longsight/instrumentation.py` & `longsight-1.0.9/src/longsight/instrumentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,25 +124,27 @@
 def instrument(
     bucket: str = "",
     create_aws=False,
     cloudwatch_push=False,
     log_group_name: str = "",
     log_stream_name: str = "",
     namespace: str = "namespace",
+    sign_aws_requests: bool = False,
 ):
     """
     This is a decorator that will instrument a method and provide AWS access
     if desired.
     :param bucket: the bucket for the AWSClient to use.
     :param create_aws: whether to create an AWSClient
     :param cloudwatch_push: whether to push metrics to CloudWatch. Note that
     setting this to true will create an AWSClient
     :param log_group_name: the log group name to use for the logger
     :param log_stream_name: the log stream name to use for the logger
     :param namespace: the namespace to use for the metrics
+    :param sign_aws_requests: whether to sign AWS requests
     :return: the wrapped function
     """
 
     def wrap(f):
         @contextmanager
         def wrapping_logic(*args, **kwargs):
             from claws import aws_utils
@@ -151,14 +153,15 @@
                 # create the boto3 objects
                 aws_access_key_id = os.environ.get("AWS_ACCESS_KEY_ID")
                 aws_secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY")
                 aws_connector = aws_utils.AWSConnector(
                     bucket=bucket,
                     aws_access_key_id=aws_access_key_id,
                     aws_secret_access_key=aws_secret_access_key,
+                    unsigned=not sign_aws_requests,
                 )
             else:
                 aws_connector = None
 
             fastapi_request = kwargs.get("request", None)
             fastapi_app = fastapi_request.app if fastapi_request else None
```

### Comparing `longsight-1.0.8/src/longsight.egg-info/PKG-INFO` & `longsight-1.0.9/src/longsight.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longsight
-Version: 1.0.8
+Version: 1.0.9
 Summary: This library implements a range of common logging functions.
 Home-page: https://gitlab.com/crossref/labs/distrunner
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `longsight-1.0.8/tests/test_instrumentation.py` & `longsight-1.0.9/tests/test_instrumentation.py`

 * *Files identical despite different names*

