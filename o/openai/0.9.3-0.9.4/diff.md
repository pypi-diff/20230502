# Comparing `tmp/openai-0.9.3.tar.gz` & `tmp/openai-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openai-0.9.3.tar", last modified: Wed Jun 30 19:42:44 2021, max compression
+gzip compressed data, was "dist/openai-0.9.4.tar", last modified: Mon Jul 12 22:30:04 2021, max compression
```

## Comparing `openai-0.9.3.tar` & `openai-0.9.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-06-30 19:42:44.000000 openai-0.9.3/
--rw-r--r--   0 rachel     (502) staff       (20)     1083 2021-03-18 23:38:07.000000 openai-0.9.3/LICENSE
--rw-r--r--   0 rachel     (502) staff       (20)      309 2021-06-30 19:42:44.000000 openai-0.9.3/PKG-INFO
--rw-r--r--   0 rachel     (502) staff       (20)     1955 2021-06-30 19:35:24.000000 openai-0.9.3/README.md
-drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-06-30 19:42:43.000000 openai-0.9.3/bin/
--rwxr-xr-x   0 rachel     (502) staff       (20)     1904 2021-06-30 04:04:32.000000 openai-0.9.3/bin/openai
-drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-06-30 19:42:43.000000 openai-0.9.3/openai/
--rw-r--r--   0 rachel     (502) staff       (20)      932 2021-06-11 23:02:33.000000 openai-0.9.3/openai/__init__.py
--rw-r--r--   0 rachel     (502) staff       (20)    13692 2021-06-24 17:05:10.000000 openai-0.9.3/openai/api_requestor.py
-drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-06-30 19:42:44.000000 openai-0.9.3/openai/api_resources/
--rw-r--r--   0 rachel     (502) staff       (20)      528 2021-06-11 23:02:33.000000 openai-0.9.3/openai/api_resources/__init__.py
-drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-06-30 19:42:44.000000 openai-0.9.3/openai/api_resources/abstract/
--rw-r--r--   0 rachel     (502) staff       (20)      696 2021-06-11 23:02:33.000000 openai-0.9.3/openai/api_resources/abstract/__init__.py
--rw-r--r--   0 rachel     (502) staff       (20)     2485 2021-06-11 23:02:33.000000 openai-0.9.3/openai/api_resources/abstract/api_resource.py
--rw-r--r--   0 rachel     (502) staff       (20)     1030 2021-06-11 23:02:33.000000 openai-0.9.3/openai/api_resources/abstract/createable_api_resource.py
--rw-r--r--   0 rachel     (502) staff       (20)     1488 2021-06-11 23:02:33.000000 openai-0.9.3/openai/api_resources/abstract/custom_method.py
--rw-r--r--   0 rachel     (502) staff       (20)      526 2021-06-11 23:02:33.000000 openai-0.9.3/openai/api_resources/abstract/deletable_api_resource.py
--rw-r--r--   0 rachel     (502) staff       (20)     4066 2021-06-24 17:05:10.000000 openai-0.9.3/openai/api_resources/abstract/engine_api_resource.py
--rw-r--r--   0 rachel     (502) staff       (20)     1106 2021-06-11 23:02:33.000000 openai-0.9.3/openai/api_resources/abstract/listable_api_resource.py
--rw-r--r--   0 rachel     (502) staff       (20)     3889 2021-06-11 23:02:33.000000 openai-0.9.3/openai/api_resources/abstract/nested_resource_class_methods.py
--rw-r--r--   0 rachel     (502) staff       (20)      890 2021-06-11 23:02:33.000000 openai-0.9.3/openai/api_resources/abstract/singleton_api_resource.py
--rw-r--r--   0 rachel     (502) staff       (20)      785 2021-06-11 23:02:33.000000 openai-0.9.3/openai/api_resources/abstract/updateable_api_resource.py
--rw-r--r--   0 rachel     (502) staff       (20)      341 2021-03-18 23:38:07.000000 openai-0.9.3/openai/api_resources/answer.py
--rw-r--r--   0 rachel     (502) staff       (20)      357 2021-03-18 23:38:07.000000 openai-0.9.3/openai/api_resources/classification.py
--rw-r--r--   0 rachel     (502) staff       (20)     1300 2021-06-30 04:04:32.000000 openai-0.9.3/openai/api_resources/completion.py
--rw-r--r--   0 rachel     (502) staff       (20)      945 2021-06-11 23:02:33.000000 openai-0.9.3/openai/api_resources/engine.py
--rw-r--r--   0 rachel     (502) staff       (20)      793 2021-03-18 23:38:07.000000 openai-0.9.3/openai/api_resources/error_object.py
-drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-06-30 19:42:44.000000 openai-0.9.3/openai/api_resources/experimental/
--rw-r--r--   0 rachel     (502) staff       (20)      104 2021-06-11 23:02:33.000000 openai-0.9.3/openai/api_resources/experimental/__init__.py
--rw-r--r--   0 rachel     (502) staff       (20)      273 2021-04-12 15:19:34.000000 openai-0.9.3/openai/api_resources/experimental/completion_config.py
--rw-r--r--   0 rachel     (502) staff       (20)     2876 2021-06-30 04:04:32.000000 openai-0.9.3/openai/api_resources/file.py
--rw-r--r--   0 rachel     (502) staff       (20)     1648 2021-06-11 23:02:33.000000 openai-0.9.3/openai/api_resources/fine_tune.py
--rw-r--r--   0 rachel     (502) staff       (20)      215 2021-06-11 23:02:33.000000 openai-0.9.3/openai/api_resources/snapshot.py
--rw-r--r--   0 rachel     (502) staff       (20)    27968 2021-06-30 19:40:58.000000 openai-0.9.3/openai/cli.py
-drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-06-30 19:42:44.000000 openai-0.9.3/openai/data/
--rw-r--r--   0 rachel     (502) staff       (20)   209309 2021-03-18 23:38:07.000000 openai-0.9.3/openai/data/ca-certificates.crt
--rw-r--r--   0 rachel     (502) staff       (20)     3808 2021-06-11 23:02:33.000000 openai-0.9.3/openai/error.py
--rw-r--r--   0 rachel     (502) staff       (20)     2294 2021-03-18 23:38:07.000000 openai-0.9.3/openai/gzip_stream.py
--rw-r--r--   0 rachel     (502) staff       (20)    12100 2021-06-11 23:02:33.000000 openai-0.9.3/openai/http_client.py
--rw-r--r--   0 rachel     (502) staff       (20)     2956 2021-06-11 23:02:33.000000 openai-0.9.3/openai/multipart_data_generator.py
--rw-r--r--   0 rachel     (502) staff       (20)      407 2021-04-12 15:19:34.000000 openai-0.9.3/openai/object_classes.py
--rw-r--r--   0 rachel     (502) staff       (20)    11699 2021-06-11 23:02:33.000000 openai-0.9.3/openai/openai_object.py
--rw-r--r--   0 rachel     (502) staff       (20)      581 2021-03-18 23:38:07.000000 openai-0.9.3/openai/openai_response.py
--rw-r--r--   0 rachel     (502) staff       (20)        0 2021-06-11 23:02:33.000000 openai-0.9.3/openai/py.typed
--rw-r--r--   0 rachel     (502) staff       (20)      401 2021-03-18 23:38:07.000000 openai-0.9.3/openai/request_metrics.py
--rw-r--r--   0 rachel     (502) staff       (20)     1190 2021-06-11 23:02:33.000000 openai-0.9.3/openai/upload_progress.py
--rw-r--r--   0 rachel     (502) staff       (20)     6111 2021-06-11 23:02:33.000000 openai-0.9.3/openai/util.py
--rw-r--r--   0 rachel     (502) staff       (20)    27122 2021-06-30 19:40:58.000000 openai-0.9.3/openai/validators.py
--rw-r--r--   0 rachel     (502) staff       (20)       18 2021-06-30 19:40:58.000000 openai-0.9.3/openai/version.py
-drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-06-30 19:42:44.000000 openai-0.9.3/openai.egg-info/
--rw-r--r--   0 rachel     (502) staff       (20)      309 2021-06-30 19:42:43.000000 openai-0.9.3/openai.egg-info/PKG-INFO
--rw-r--r--   0 rachel     (502) staff       (20)     1502 2021-06-30 19:42:43.000000 openai-0.9.3/openai.egg-info/SOURCES.txt
--rw-r--r--   0 rachel     (502) staff       (20)        1 2021-06-30 19:42:43.000000 openai-0.9.3/openai.egg-info/dependency_links.txt
--rw-r--r--   0 rachel     (502) staff       (20)      106 2021-06-30 19:42:43.000000 openai-0.9.3/openai.egg-info/requires.txt
--rw-r--r--   0 rachel     (502) staff       (20)        7 2021-06-30 19:42:43.000000 openai-0.9.3/openai.egg-info/top_level.txt
--rw-r--r--   0 rachel     (502) staff       (20)       38 2021-06-30 19:42:44.000000 openai-0.9.3/setup.cfg
--rw-r--r--   0 rachel     (502) staff       (20)     1163 2021-06-30 04:04:32.000000 openai-0.9.3/setup.py
+drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-07-12 22:30:04.000000 openai-0.9.4/
+-rw-r--r--   0 rachel     (502) staff       (20)     1083 2021-03-18 23:38:07.000000 openai-0.9.4/LICENSE
+-rw-r--r--   0 rachel     (502) staff       (20)      309 2021-07-12 22:30:04.000000 openai-0.9.4/PKG-INFO
+-rw-r--r--   0 rachel     (502) staff       (20)     1955 2021-07-12 22:28:20.000000 openai-0.9.4/README.md
+drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-07-12 22:30:04.000000 openai-0.9.4/bin/
+-rwxr-xr-x   0 rachel     (502) staff       (20)     1904 2021-06-30 04:04:32.000000 openai-0.9.4/bin/openai
+drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-07-12 22:30:04.000000 openai-0.9.4/openai/
+-rw-r--r--   0 rachel     (502) staff       (20)      932 2021-06-11 23:02:33.000000 openai-0.9.4/openai/__init__.py
+-rw-r--r--   0 rachel     (502) staff       (20)    13692 2021-06-24 17:05:10.000000 openai-0.9.4/openai/api_requestor.py
+drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-07-12 22:30:04.000000 openai-0.9.4/openai/api_resources/
+-rw-r--r--   0 rachel     (502) staff       (20)      528 2021-06-11 23:02:33.000000 openai-0.9.4/openai/api_resources/__init__.py
+drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-07-12 22:30:04.000000 openai-0.9.4/openai/api_resources/abstract/
+-rw-r--r--   0 rachel     (502) staff       (20)      696 2021-06-11 23:02:33.000000 openai-0.9.4/openai/api_resources/abstract/__init__.py
+-rw-r--r--   0 rachel     (502) staff       (20)     2485 2021-06-11 23:02:33.000000 openai-0.9.4/openai/api_resources/abstract/api_resource.py
+-rw-r--r--   0 rachel     (502) staff       (20)     1030 2021-06-11 23:02:33.000000 openai-0.9.4/openai/api_resources/abstract/createable_api_resource.py
+-rw-r--r--   0 rachel     (502) staff       (20)     1488 2021-06-11 23:02:33.000000 openai-0.9.4/openai/api_resources/abstract/custom_method.py
+-rw-r--r--   0 rachel     (502) staff       (20)      526 2021-06-11 23:02:33.000000 openai-0.9.4/openai/api_resources/abstract/deletable_api_resource.py
+-rw-r--r--   0 rachel     (502) staff       (20)     4066 2021-06-24 17:05:10.000000 openai-0.9.4/openai/api_resources/abstract/engine_api_resource.py
+-rw-r--r--   0 rachel     (502) staff       (20)     1106 2021-06-11 23:02:33.000000 openai-0.9.4/openai/api_resources/abstract/listable_api_resource.py
+-rw-r--r--   0 rachel     (502) staff       (20)     3889 2021-06-11 23:02:33.000000 openai-0.9.4/openai/api_resources/abstract/nested_resource_class_methods.py
+-rw-r--r--   0 rachel     (502) staff       (20)      890 2021-06-11 23:02:33.000000 openai-0.9.4/openai/api_resources/abstract/singleton_api_resource.py
+-rw-r--r--   0 rachel     (502) staff       (20)      785 2021-06-11 23:02:33.000000 openai-0.9.4/openai/api_resources/abstract/updateable_api_resource.py
+-rw-r--r--   0 rachel     (502) staff       (20)      341 2021-03-18 23:38:07.000000 openai-0.9.4/openai/api_resources/answer.py
+-rw-r--r--   0 rachel     (502) staff       (20)      357 2021-03-18 23:38:07.000000 openai-0.9.4/openai/api_resources/classification.py
+-rw-r--r--   0 rachel     (502) staff       (20)     1300 2021-06-30 04:04:32.000000 openai-0.9.4/openai/api_resources/completion.py
+-rw-r--r--   0 rachel     (502) staff       (20)      945 2021-06-11 23:02:33.000000 openai-0.9.4/openai/api_resources/engine.py
+-rw-r--r--   0 rachel     (502) staff       (20)      793 2021-03-18 23:38:07.000000 openai-0.9.4/openai/api_resources/error_object.py
+drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-07-12 22:30:04.000000 openai-0.9.4/openai/api_resources/experimental/
+-rw-r--r--   0 rachel     (502) staff       (20)      104 2021-06-11 23:02:33.000000 openai-0.9.4/openai/api_resources/experimental/__init__.py
+-rw-r--r--   0 rachel     (502) staff       (20)      273 2021-04-12 15:19:34.000000 openai-0.9.4/openai/api_resources/experimental/completion_config.py
+-rw-r--r--   0 rachel     (502) staff       (20)     2876 2021-06-30 04:04:32.000000 openai-0.9.4/openai/api_resources/file.py
+-rw-r--r--   0 rachel     (502) staff       (20)     1648 2021-06-11 23:02:33.000000 openai-0.9.4/openai/api_resources/fine_tune.py
+-rw-r--r--   0 rachel     (502) staff       (20)      215 2021-06-11 23:02:33.000000 openai-0.9.4/openai/api_resources/snapshot.py
+-rw-r--r--   0 rachel     (502) staff       (20)    27968 2021-06-30 19:40:58.000000 openai-0.9.4/openai/cli.py
+drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-07-12 22:30:04.000000 openai-0.9.4/openai/data/
+-rw-r--r--   0 rachel     (502) staff       (20)   209309 2021-03-18 23:38:07.000000 openai-0.9.4/openai/data/ca-certificates.crt
+-rw-r--r--   0 rachel     (502) staff       (20)     3808 2021-06-11 23:02:33.000000 openai-0.9.4/openai/error.py
+-rw-r--r--   0 rachel     (502) staff       (20)     2294 2021-03-18 23:38:07.000000 openai-0.9.4/openai/gzip_stream.py
+-rw-r--r--   0 rachel     (502) staff       (20)    12100 2021-06-11 23:02:33.000000 openai-0.9.4/openai/http_client.py
+-rw-r--r--   0 rachel     (502) staff       (20)     2956 2021-06-11 23:02:33.000000 openai-0.9.4/openai/multipart_data_generator.py
+-rw-r--r--   0 rachel     (502) staff       (20)      407 2021-04-12 15:19:34.000000 openai-0.9.4/openai/object_classes.py
+-rw-r--r--   0 rachel     (502) staff       (20)    11699 2021-06-11 23:02:33.000000 openai-0.9.4/openai/openai_object.py
+-rw-r--r--   0 rachel     (502) staff       (20)      581 2021-03-18 23:38:07.000000 openai-0.9.4/openai/openai_response.py
+-rw-r--r--   0 rachel     (502) staff       (20)        0 2021-06-11 23:02:33.000000 openai-0.9.4/openai/py.typed
+-rw-r--r--   0 rachel     (502) staff       (20)      401 2021-03-18 23:38:07.000000 openai-0.9.4/openai/request_metrics.py
+-rw-r--r--   0 rachel     (502) staff       (20)     1190 2021-06-11 23:02:33.000000 openai-0.9.4/openai/upload_progress.py
+-rw-r--r--   0 rachel     (502) staff       (20)     6111 2021-06-11 23:02:33.000000 openai-0.9.4/openai/util.py
+-rw-r--r--   0 rachel     (502) staff       (20)    27648 2021-07-12 22:28:23.000000 openai-0.9.4/openai/validators.py
+-rw-r--r--   0 rachel     (502) staff       (20)       18 2021-07-12 22:28:23.000000 openai-0.9.4/openai/version.py
+drwxr-xr-x   0 rachel     (502) staff       (20)        0 2021-07-12 22:30:04.000000 openai-0.9.4/openai.egg-info/
+-rw-r--r--   0 rachel     (502) staff       (20)      309 2021-07-12 22:30:04.000000 openai-0.9.4/openai.egg-info/PKG-INFO
+-rw-r--r--   0 rachel     (502) staff       (20)     1502 2021-07-12 22:30:04.000000 openai-0.9.4/openai.egg-info/SOURCES.txt
+-rw-r--r--   0 rachel     (502) staff       (20)        1 2021-07-12 22:30:04.000000 openai-0.9.4/openai.egg-info/dependency_links.txt
+-rw-r--r--   0 rachel     (502) staff       (20)      106 2021-07-12 22:30:04.000000 openai-0.9.4/openai.egg-info/requires.txt
+-rw-r--r--   0 rachel     (502) staff       (20)        7 2021-07-12 22:30:04.000000 openai-0.9.4/openai.egg-info/top_level.txt
+-rw-r--r--   0 rachel     (502) staff       (20)       38 2021-07-12 22:30:04.000000 openai-0.9.4/setup.cfg
+-rw-r--r--   0 rachel     (502) staff       (20)     1163 2021-06-30 04:04:32.000000 openai-0.9.4/setup.py
```

### Comparing `openai-0.9.3/LICENSE` & `openai-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/README.md` & `openai-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/bin/openai` & `openai-0.9.4/bin/openai`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/__init__.py` & `openai-0.9.4/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_requestor.py` & `openai-0.9.4/openai/api_requestor.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/__init__.py` & `openai-0.9.4/openai/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/abstract/__init__.py` & `openai-0.9.4/openai/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/abstract/api_resource.py` & `openai-0.9.4/openai/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/abstract/createable_api_resource.py` & `openai-0.9.4/openai/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/abstract/custom_method.py` & `openai-0.9.4/openai/api_resources/abstract/custom_method.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/abstract/deletable_api_resource.py` & `openai-0.9.4/openai/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/abstract/engine_api_resource.py` & `openai-0.9.4/openai/api_resources/abstract/engine_api_resource.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/abstract/listable_api_resource.py` & `openai-0.9.4/openai/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/abstract/nested_resource_class_methods.py` & `openai-0.9.4/openai/api_resources/abstract/nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/abstract/singleton_api_resource.py` & `openai-0.9.4/openai/api_resources/abstract/singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/abstract/updateable_api_resource.py` & `openai-0.9.4/openai/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/completion.py` & `openai-0.9.4/openai/api_resources/completion.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/engine.py` & `openai-0.9.4/openai/api_resources/engine.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/error_object.py` & `openai-0.9.4/openai/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/file.py` & `openai-0.9.4/openai/api_resources/file.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/api_resources/fine_tune.py` & `openai-0.9.4/openai/api_resources/fine_tune.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/cli.py` & `openai-0.9.4/openai/cli.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/data/ca-certificates.crt` & `openai-0.9.4/openai/data/ca-certificates.crt`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/error.py` & `openai-0.9.4/openai/error.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/gzip_stream.py` & `openai-0.9.4/openai/gzip_stream.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/http_client.py` & `openai-0.9.4/openai/http_client.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/multipart_data_generator.py` & `openai-0.9.4/openai/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/openai_object.py` & `openai-0.9.4/openai/openai_object.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/openai_response.py` & `openai-0.9.4/openai/openai_response.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/upload_progress.py` & `openai-0.9.4/openai/upload_progress.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/util.py` & `openai-0.9.4/openai/util.py`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/openai/validators.py` & `openai-0.9.4/openai/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         "\n\n===>\n\n",
         "\n\n--->\n\n",
     ]
     for suffix_option in suffix_options:
         if suffix_option == " ->":
             if df.prompt.str.contains("\n").any():
                 continue
-        if df.prompt.str.contains(suffix_option).any():
+        if df.prompt.str.contains(suffix_option, regex=False).any():
             continue
         suggested_suffix = suffix_option
         break
     display_suggested_suffix = suggested_suffix.replace("\n", "\\n")
 
     ft_type = infer_task_type(df)
     if ft_type == "open-ended generation":
@@ -198,15 +198,19 @@
     if common_suffix != "":
         common_suffix_new_line_handled = common_suffix.replace("\n", "\\n")
         immediate_msg = (
             f"\n- All prompts end with suffix `{common_suffix_new_line_handled}`"
         )
         if len(common_suffix) > 10:
             immediate_msg += f". This suffix seems very long. Consider replacing with a shorter suffix, such as `{display_suggested_suffix}`"
-        if df.prompt.str[: -len(common_suffix)].str.contains(common_suffix).any():
+        if (
+            df.prompt.str[: -len(common_suffix)]
+            .str.contains(common_suffix, regex=False)
+            .any()
+        ):
             immediate_msg += f"\n  WARNING: Some of your prompts contain the suffix `{common_suffix}` more than once. We strongly suggest that you review your prompts and add a unique suffix"
 
     else:
         immediate_msg = "\n- Your data does not contain a common separator at the end of your prompts. Having a separator string appended to the end of the prompt makes it clearer to the fine-tuned model where the completion should begin. See `Fine Tuning How to Guide` for more detail and examples. If you intend to do open-ended generation, then you should leave the prompts empty"
 
     if common_suffix == "":
         optional_msg = (
@@ -267,30 +271,34 @@
 def common_completion_prefix_validator(df):
     """
     This validator will suggest to remove a common prefix from the completion if a long one exist.
     """
     MAX_PREFIX_LEN = 5
 
     common_prefix = get_common_xfix(df.completion, xfix="prefix")
+    ws_prefix = len(common_prefix) > 0 and common_prefix[0] == " "
     if len(common_prefix) < MAX_PREFIX_LEN:
         return Remediation(name="common_prefix")
 
-    def remove_common_prefix(x, prefix):
+    def remove_common_prefix(x, prefix, ws_prefix):
         x["completion"] = x["completion"].str[len(prefix) :]
+        if ws_prefix:
+            # keep the single whitespace as prefix
+            x["completion"] = " " + x["completion"]
         return x
 
     if (df.completion == common_prefix).all():
         # already handled by common_suffix_validator
         return Remediation(name="common_prefix")
 
     immediate_msg = f"\n- All completions start with prefix `{common_prefix}`. Most of the time you should only add the output data into the completion, without any prefix"
     optional_msg = f"Remove prefix `{common_prefix}` from all completions"
 
     def optional_fn(x):
-        return remove_common_prefix(x, common_prefix)
+        return remove_common_prefix(x, common_prefix, ws_prefix)
 
     return Remediation(
         name="common_completion_prefix",
         immediate_msg=immediate_msg,
         optional_msg=optional_msg,
         optional_fn=optional_fn,
     )
@@ -301,55 +309,59 @@
     This validator will suggest to add a common suffix to the completion if one doesn't already exist in case of classification or conditional generation.
     """
     error_msg = None
     immediate_msg = None
     optional_msg = None
     optional_fn = None
 
+    ft_type = infer_task_type(df)
+    if ft_type == "open-ended generation" or ft_type == "classification":
+        return Remediation(name="common_suffix")
+
+    common_suffix = get_common_xfix(df.completion, xfix="suffix")
+    if (df.completion == common_suffix).all():
+        error_msg = f"All completions are identical: `{common_suffix}`\nEnsure completions are different, otherwise the model will just repeat `{common_suffix}`"
+        return Remediation(name="common_suffix", error_msg=error_msg)
+
     # Find a suffix which is not contained within the completion otherwise
     suggested_suffix = " [END]"
     suffix_options = [
         "\n",
         ".",
         " END",
         "***",
         "+++",
         "&&&",
         "$$$",
         "@@@",
         "%%%",
     ]
     for suffix_option in suffix_options:
-        if df.completion.str.contains(suffix_option).any():
+        if df.completion.str.contains(suffix_option, regex=False).any():
             continue
         suggested_suffix = suffix_option
         break
     display_suggested_suffix = suggested_suffix.replace("\n", "\\n")
 
-    ft_type = infer_task_type(df)
-    if ft_type == "open-ended generation" or ft_type == "classification":
-        return Remediation(name="common_suffix")
-
     def add_suffix(x, suffix):
         x["completion"] += suffix
         return x
 
-    common_suffix = get_common_xfix(df.completion, xfix="suffix")
-    if (df.completion == common_suffix).all():
-        error_msg = f"All completions are identical: `{common_suffix}`\nEnsure completions are different, otherwise the model will just repeat `{common_suffix}`"
-        return Remediation(name="common_suffix", error_msg=error_msg)
-
     if common_suffix != "":
         common_suffix_new_line_handled = common_suffix.replace("\n", "\\n")
         immediate_msg = (
             f"\n- All completions end with suffix `{common_suffix_new_line_handled}`"
         )
         if len(common_suffix) > 10:
             immediate_msg += f". This suffix seems very long. Consider replacing with a shorter suffix, such as `{display_suggested_suffix}`"
-        if df.completion.str[: -len(common_suffix)].str.contains(common_suffix).any():
+        if (
+            df.completion.str[: -len(common_suffix)]
+            .str.contains(common_suffix, regex=False)
+            .any()
+        ):
             immediate_msg += f"\n  WARNING: Some of your completions contain the suffix `{common_suffix}` more than once. We suggest that you review your completions and add a unique ending"
 
     else:
         immediate_msg = "\n- Your data does not contain a common ending at the end of your completions. Having a common ending string appended to the end of the completion makes it clearer to the fine-tuned model where the completion should end. See `Fine Tuning How to Guide` for more detail and examples."
 
     if common_suffix == "":
         optional_msg = (
@@ -613,16 +625,21 @@
             df_out[["prompt", "completion"]].to_json(
                 out_fname, lines=True, orient="records"
             )
 
         # Add -v VALID_FILE if we split the file into train / valid
         files_string = ("s" if split else "") + " to `" + ("` and `".join(outfnames))
         valid_string = f' -v "{outfnames[1]}"' if split else ""
+        separator_reminder = (
+            ""
+            if len(common_prompt_suffix_new_line_handled) == 0
+            else f"After you’ve fine-tuned a model, remember that your prompt has to end with the indicator string `{common_prompt_suffix_new_line_handled}` for the model to start generating completions, rather than continuing with the prompt."
+        )
         sys.stdout.write(
-            f'\nWrote modified file{files_string}`\nFeel free to take a look!\n\nNow use that file when fine-tuning:\n> openai api fine_tunes.create -t "{outfnames[0]}"{valid_string}{packing_param}\n\nAfter you’ve fine-tuned a model, remember that your prompt has to end with the indicator string `{common_prompt_suffix_new_line_handled}` for the model to start generating completions, rather than continuing with the prompt.{optional_ending_string}\n'
+            f'\nWrote modified file{files_string}`\nFeel free to take a look!\n\nNow use that file when fine-tuning:\n> openai api fine_tunes.create -t "{outfnames[0]}"{valid_string}{packing_param}\n\n{separator_reminder}{optional_ending_string}\n'
         )
     else:
         sys.stdout.write("Aborting... did not write the file\n")
 
 
 def infer_task_type(df):
     """
```

### Comparing `openai-0.9.3/openai.egg-info/SOURCES.txt` & `openai-0.9.4/openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai-0.9.3/setup.py` & `openai-0.9.4/setup.py`

 * *Files identical despite different names*

