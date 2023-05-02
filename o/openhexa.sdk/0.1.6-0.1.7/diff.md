# Comparing `tmp/openhexa.sdk-0.1.6.tar.gz` & `tmp/openhexa.sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhexa.sdk-0.1.6.tar", last modified: Thu Apr 27 13:41:32 2023, max compression
+gzip compressed data, was "openhexa.sdk-0.1.7.tar", last modified: Tue May  2 10:28:08 2023, max compression
```

## Comparing `openhexa.sdk-0.1.6.tar` & `openhexa.sdk-0.1.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:41:32.619593 openhexa.sdk-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-27 13:41:32.619593 openhexa.sdk-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:41:32.603593 openhexa.sdk-0.1.6/openhexa/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:41:32.607593 openhexa.sdk-0.1.6/openhexa/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/cli/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:41:32.611593 openhexa.sdk-0.1.6/openhexa/cli/skeleton/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/cli/skeleton/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/cli/skeleton/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/cli/skeleton/workspace.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:41:32.611593 openhexa.sdk-0.1.6/openhexa/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:41:32.615593 openhexa.sdk-0.1.6/openhexa/sdk/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/sdk/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/sdk/pipelines/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/sdk/pipelines/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/sdk/pipelines/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/sdk/pipelines/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/sdk/pipelines/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/sdk/pipelines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:41:32.615593 openhexa.sdk-0.1.6/openhexa/sdk/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/sdk/workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/sdk/workspaces/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/openhexa/sdk/workspaces/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:41:32.607593 openhexa.sdk-0.1.6/openhexa.sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-27 13:41:32.000000 openhexa.sdk-0.1.6/openhexa.sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-27 13:41:32.000000 openhexa.sdk-0.1.6/openhexa.sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:41:32.000000 openhexa.sdk-0.1.6/openhexa.sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-27 13:41:32.000000 openhexa.sdk-0.1.6/openhexa.sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-27 13:41:32.000000 openhexa.sdk-0.1.6/openhexa.sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 13:41:32.000000 openhexa.sdk-0.1.6/openhexa.sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:41:17.000000 openhexa.sdk-0.1.6/openhexa.sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-27 13:41:32.619593 openhexa.sdk-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:41:32.619593 openhexa.sdk-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/tests/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-27 13:41:09.000000 openhexa.sdk-0.1.6/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:28:08.683038 openhexa.sdk-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-02 10:28:08.683038 openhexa.sdk-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:28:08.679037 openhexa.sdk-0.1.7/openhexa/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:28:08.679037 openhexa.sdk-0.1.7/openhexa/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/cli/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:28:08.679037 openhexa.sdk-0.1.7/openhexa/cli/skeleton/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/cli/skeleton/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/cli/skeleton/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/cli/skeleton/workspace.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:28:08.679037 openhexa.sdk-0.1.7/openhexa/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:28:08.679037 openhexa.sdk-0.1.7/openhexa/sdk/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/sdk/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/sdk/pipelines/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/sdk/pipelines/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/sdk/pipelines/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/sdk/pipelines/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/sdk/pipelines/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/sdk/pipelines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:28:08.679037 openhexa.sdk-0.1.7/openhexa/sdk/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/sdk/workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/sdk/workspaces/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/openhexa/sdk/workspaces/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:28:08.679037 openhexa.sdk-0.1.7/openhexa.sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-02 10:28:08.000000 openhexa.sdk-0.1.7/openhexa.sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-02 10:28:08.000000 openhexa.sdk-0.1.7/openhexa.sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:28:08.000000 openhexa.sdk-0.1.7/openhexa.sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 10:28:08.000000 openhexa.sdk-0.1.7/openhexa.sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-02 10:28:08.000000 openhexa.sdk-0.1.7/openhexa.sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 10:28:08.000000 openhexa.sdk-0.1.7/openhexa.sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:27:55.000000 openhexa.sdk-0.1.7/openhexa.sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-02 10:28:08.683038 openhexa.sdk-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:28:08.679037 openhexa.sdk-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-02 10:27:51.000000 openhexa.sdk-0.1.7/tests/test_pipeline.py
```

### Comparing `openhexa.sdk-0.1.6/LICENCE` & `openhexa.sdk-0.1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.6/PKG-INFO` & `openhexa.sdk-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: OpenHexa SDK
 Home-page: https://github.com/BLSQ/openhexa-sdk-python
 Author: Bluesquare
 Author-email: dev@bluesquarehub.com
 License: MIT License
 Keywords: openhexa,pipelines
 Classifier: Programming Language :: Python :: 3
```

### Comparing `openhexa.sdk-0.1.6/README.md` & `openhexa.sdk-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.6/openhexa/cli/api.py` & `openhexa.sdk-0.1.7/openhexa/cli/api.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.6/openhexa/cli/cli.py` & `openhexa.sdk-0.1.7/openhexa/cli/cli.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.6/openhexa/sdk/pipelines/parameter.py` & `openhexa.sdk-0.1.7/openhexa/sdk/pipelines/parameter.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.6/openhexa/sdk/pipelines/pipeline.py` & `openhexa.sdk-0.1.7/openhexa/sdk/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.6/openhexa/sdk/pipelines/run.py` & `openhexa.sdk-0.1.7/openhexa/sdk/pipelines/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                     "uri": f"gs://{os.environ['WORKSPACE_BUCKET_NAME']}{stripped_path}",
                     "type": "file",
                     "name": name,
                 }
             }
             self._graphql_query(query, variables)
         else:
-            print(f"Sending output with path {path} and name: {name}")
+            print(f"Sending output with path {stripped_path}")
 
     def add_database_output(self, table_name: str):
         if self.connected:
             query = """
                                 mutation addPipelineOutput ($input: AddPipelineOutputInput!) {
                                     addPipelineOutput(input: $input) { success errors }
                                 }"""
```

### Comparing `openhexa.sdk-0.1.6/openhexa/sdk/pipelines/runtime.py` & `openhexa.sdk-0.1.7/openhexa/sdk/pipelines/runtime.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.6/openhexa/sdk/pipelines/task.py` & `openhexa.sdk-0.1.7/openhexa/sdk/pipelines/task.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.6/openhexa/sdk/pipelines/utils.py` & `openhexa.sdk-0.1.7/openhexa/sdk/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.6/openhexa/sdk/workspaces/workspace.py` & `openhexa.sdk-0.1.7/openhexa/sdk/workspaces/workspace.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.6/openhexa.sdk.egg-info/PKG-INFO` & `openhexa.sdk-0.1.7/openhexa.sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: OpenHexa SDK
 Home-page: https://github.com/BLSQ/openhexa-sdk-python
 Author: Bluesquare
 Author-email: dev@bluesquarehub.com
 License: MIT License
 Keywords: openhexa,pipelines
 Classifier: Programming Language :: Python :: 3
```

### Comparing `openhexa.sdk-0.1.6/openhexa.sdk.egg-info/SOURCES.txt` & `openhexa.sdk-0.1.7/openhexa.sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.6/pyproject.toml` & `openhexa.sdk-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.6/setup.cfg` & `openhexa.sdk-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.6/tests/test_parameter.py` & `openhexa.sdk-0.1.7/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `openhexa.sdk-0.1.6/tests/test_pipeline.py` & `openhexa.sdk-0.1.7/tests/test_pipeline.py`

 * *Files identical despite different names*

