# Comparing `tmp/dbt-rpc-0.4.0b1.tar.gz` & `tmp/dbt-rpc-0.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-rpc-0.4.0b1.tar", last modified: Tue Feb 28 22:29:50 2023, max compression
+gzip compressed data, was "dbt-rpc-0.4.0rc1.tar", last modified: Thu Apr 13 00:25:36 2023, max compression
```

## Comparing `dbt-rpc-0.4.0b1.tar` & `dbt-rpc-0.4.0rc1.tar`

### file list

```diff
@@ -1,41 +1,55 @@
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-02-28 22:29:50.328755 dbt-rpc-0.4.0b1/
--rw-r--r--   0 chenyuli   (502) staff       (20)    11344 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0b1/LICENSE.md
--rw-r--r--   0 chenyuli   (502) staff       (20)      862 2023-02-28 22:29:50.328589 dbt-rpc-0.4.0b1/PKG-INFO
--rw-r--r--   0 chenyuli   (502) staff       (20)     1864 2022-12-16 19:31:44.000000 dbt-rpc-0.4.0b1/README.md
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-02-28 22:29:50.322779 dbt-rpc-0.4.0b1/dbt_rpc/
--rw-r--r--   0 chenyuli   (502) staff       (20)        0 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0b1/dbt_rpc/__init__.py
--rw-r--r--   0 chenyuli   (502) staff       (20)    17375 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0b1/dbt_rpc/__main__.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-02-28 22:29:50.323990 dbt-rpc-0.4.0b1/dbt_rpc/contracts/
--rw-r--r--   0 chenyuli   (502) staff       (20)    22857 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0b1/dbt_rpc/contracts/rpc.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-02-28 22:29:50.324590 dbt-rpc-0.4.0b1/dbt_rpc/parser/
--rw-r--r--   0 chenyuli   (502) staff       (20)     1966 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0b1/dbt_rpc/parser/rpc.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-02-28 22:29:50.327359 dbt-rpc-0.4.0b1/dbt_rpc/rpc/
--rw-r--r--   0 chenyuli   (502) staff       (20)     1992 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0b1/dbt_rpc/rpc/__init__.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     8439 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0b1/dbt_rpc/rpc/builtins.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     2259 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0b1/dbt_rpc/rpc/error.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     3927 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0b1/dbt_rpc/rpc/gc.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     6024 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0b1/dbt_rpc/rpc/logger.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     5133 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0b1/dbt_rpc/rpc/method.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     4356 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0b1/dbt_rpc/rpc/node_runners.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     4870 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0b1/dbt_rpc/rpc/response_manager.py
--rw-r--r--   0 chenyuli   (502) staff       (20)    18829 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0b1/dbt_rpc/rpc/task_handler.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     2696 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0b1/dbt_rpc/rpc/task_handler_protocol.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     9512 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0b1/dbt_rpc/rpc/task_manager.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-02-28 22:29:50.328342 dbt-rpc-0.4.0b1/dbt_rpc/task/
--rw-r--r--   0 chenyuli   (502) staff       (20)        0 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0b1/dbt_rpc/task/__init__.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     1569 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0b1/dbt_rpc/task/base.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     5059 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0b1/dbt_rpc/task/cli.py
--rw-r--r--   0 chenyuli   (502) staff       (20)      976 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0b1/dbt_rpc/task/deps.py
--rw-r--r--   0 chenyuli   (502) staff       (20)    10644 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0b1/dbt_rpc/task/project_commands.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     6222 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0b1/dbt_rpc/task/server.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     7375 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0b1/dbt_rpc/task/sql_commands.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-02-28 22:29:50.323858 dbt-rpc-0.4.0b1/dbt_rpc.egg-info/
--rw-r--r--   0 chenyuli   (502) staff       (20)      862 2023-02-28 22:29:50.000000 dbt-rpc-0.4.0b1/dbt_rpc.egg-info/PKG-INFO
--rw-r--r--   0 chenyuli   (502) staff       (20)      790 2023-02-28 22:29:50.000000 dbt-rpc-0.4.0b1/dbt_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)        1 2023-02-28 22:29:50.000000 dbt-rpc-0.4.0b1/dbt_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)       50 2023-02-28 22:29:50.000000 dbt-rpc-0.4.0b1/dbt_rpc.egg-info/entry_points.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)        1 2022-07-20 22:27:25.000000 dbt-rpc-0.4.0b1/dbt_rpc.egg-info/not-zip-safe
--rw-r--r--   0 chenyuli   (502) staff       (20)       36 2023-02-28 22:29:50.000000 dbt-rpc-0.4.0b1/dbt_rpc.egg-info/requires.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)        8 2023-02-28 22:29:50.000000 dbt-rpc-0.4.0b1/dbt_rpc.egg-info/top_level.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)       38 2023-02-28 22:29:50.328802 dbt-rpc-0.4.0b1/setup.cfg
--rw-r--r--   0 chenyuli   (502) staff       (20)     1442 2023-02-28 22:29:45.000000 dbt-rpc-0.4.0b1/setup.py
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.066645 dbt-rpc-0.4.0rc1/
+-rw-r--r--   0 chenyuli   (502) staff       (20)    11344 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/LICENSE.md
+-rw-r--r--   0 chenyuli   (502) staff       (20)      863 2023-04-13 00:25:36.066500 dbt-rpc-0.4.0rc1/PKG-INFO
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1864 2022-12-16 19:31:44.000000 dbt-rpc-0.4.0rc1/README.md
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.056728 dbt-rpc-0.4.0rc1/dbt_rpc/
+-rw-r--r--   0 chenyuli   (502) staff       (20)        0 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/dbt_rpc/__init__.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)    17375 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc/__main__.py
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.058142 dbt-rpc-0.4.0rc1/dbt_rpc/contracts/
+-rw-r--r--   0 chenyuli   (502) staff       (20)    22857 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0rc1/dbt_rpc/contracts/rpc.py
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.058643 dbt-rpc-0.4.0rc1/dbt_rpc/parser/
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1966 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0rc1/dbt_rpc/parser/rpc.py
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.061640 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1992 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/__init__.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     8439 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/builtins.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     2259 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/error.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     3927 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/gc.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     6024 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/logger.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     5133 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/method.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     4374 2023-04-13 00:25:34.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/node_runners.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     4870 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/response_manager.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)    19107 2023-04-13 00:25:34.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/task_handler.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     2696 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/task_handler_protocol.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     9512 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc/rpc/task_manager.py
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.063322 dbt-rpc-0.4.0rc1/dbt_rpc/task/
+-rw-r--r--   0 chenyuli   (502) staff       (20)        0 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/dbt_rpc/task/__init__.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1569 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc/task/base.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     5059 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc/task/cli.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)      976 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc/task/deps.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)    10644 2023-02-28 18:49:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc/task/project_commands.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     6222 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0rc1/dbt_rpc/task/server.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     7375 2023-02-07 23:21:09.000000 dbt-rpc-0.4.0rc1/dbt_rpc/task/sql_commands.py
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.058003 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/
+-rw-r--r--   0 chenyuli   (502) staff       (20)      863 2023-04-13 00:25:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1089 2023-04-13 00:25:36.000000 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyuli   (502) staff       (20)        1 2023-04-13 00:25:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyuli   (502) staff       (20)       50 2023-04-13 00:25:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/entry_points.txt
+-rw-r--r--   0 chenyuli   (502) staff       (20)        1 2022-07-20 22:27:25.000000 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/not-zip-safe
+-rw-r--r--   0 chenyuli   (502) staff       (20)       36 2023-04-13 00:25:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/requires.txt
+-rw-r--r--   0 chenyuli   (502) staff       (20)        8 2023-04-13 00:25:35.000000 dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/top_level.txt
+-rw-r--r--   0 chenyuli   (502) staff       (20)       38 2023-04-13 00:25:36.066688 dbt-rpc-0.4.0rc1/setup.cfg
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1443 2023-04-13 00:25:34.000000 dbt-rpc-0.4.0rc1/setup.py
+drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-04-13 00:25:36.066285 dbt-rpc-0.4.0rc1/tests/
+-rw-r--r--   0 chenyuli   (502) staff       (20)     5803 2023-02-14 23:05:02.000000 dbt-rpc-0.4.0rc1/tests/test_build.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     2763 2023-04-06 22:01:40.000000 dbt-rpc-0.4.0rc1/tests/test_compile.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1284 2023-04-13 00:25:34.000000 dbt-rpc-0.4.0rc1/tests/test_compile_sql.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     1154 2022-07-23 23:11:05.000000 dbt-rpc-0.4.0rc1/tests/test_concurrency.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     5955 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/tests/test_deps.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)    12604 2022-12-30 20:30:27.000000 dbt-rpc-0.4.0rc1/tests/test_management.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     4500 2022-07-23 23:11:26.000000 dbt-rpc-0.4.0rc1/tests/test_run.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     3018 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/tests/test_run_operation.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)      562 2022-09-14 22:22:50.000000 dbt-rpc-0.4.0rc1/tests/test_run_sql.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     3517 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/tests/test_seed.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     4638 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/tests/test_snapshots.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     6387 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/tests/test_source_freshness.py
+-rw-r--r--   0 chenyuli   (502) staff       (20)     3242 2022-07-20 21:30:31.000000 dbt-rpc-0.4.0rc1/tests/test_test.py
```

### Comparing `dbt-rpc-0.4.0b1/LICENSE.md` & `dbt-rpc-0.4.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/PKG-INFO` & `dbt-rpc-0.4.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-rpc
-Version: 0.4.0b1
+Version: 0.4.0rc1
 Summary:  A JSON RPC server that provides an interface to programmically interact with dbt projects. 
 Home-page: https://github.com/dbt-labs/dbt-rpc
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-rpc-0.4.0b1/README.md` & `dbt-rpc-0.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/__main__.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/__main__.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/contracts/rpc.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/contracts/rpc.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/parser/rpc.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/parser/rpc.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/rpc/__init__.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/rpc/builtins.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/builtins.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/rpc/error.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/error.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/rpc/gc.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/gc.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/rpc/logger.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/logger.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/rpc/method.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/method.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/rpc/node_runners.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/node_runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,17 @@
         pass
 
     def after_execute(self, result):
         pass
 
     def compile(self, manifest):
         if not self.node.config.enabled:
-            raise dbt.exceptions.raise_compiler_error(
-                "Trying to compile a node that is disabled"
+            raise dbt.exceptions.CompilationError(
+                "Trying to compile a node that is disabled",
+                None
             )
         compiler = self.adapter.get_compiler()
         return compiler.compile_node(self.node, manifest, {}, write=False)
 
     @abstractmethod
     def execute(self, compiled_node, manifest) -> RPCSQLResult:
         pass
```

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/rpc/response_manager.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/response_manager.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/rpc/task_handler.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/task_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,19 @@
             if getattr(self.task.args, 'threads', None) is not None:
                 self.task.config.threads = self.task.args.threads
 
             # we previously always set a selector here
             if not hasattr(self.task.args, 'selector'):
                 object.__setattr__(self.task.args, "selector", None)
                 object.__setattr__(self.task.args, "SELECTOR", None)
+            # pre-1.5 we always set populate_cache to True. This represent parity
+            # with the old behavior, not parity with core
+            if not hasattr(self.task.args, 'populate_cache'):
+                object.__setattr__(self.task.args, "populate_cache", True)
+
             rpc_exception = None
             result = None
             try:
                 result = self.task.handle_request()
             except RPCException as exc:
                 rpc_exception = exc
             except dbt.exceptions.RPCKilledException as exc:
```

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/rpc/task_handler_protocol.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/task_handler_protocol.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/rpc/task_manager.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/rpc/task_manager.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/task/base.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/task/base.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/task/cli.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/task/cli.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/task/deps.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/task/deps.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/task/project_commands.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/task/project_commands.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/task/server.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/task/server.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc/task/sql_commands.py` & `dbt-rpc-0.4.0rc1/dbt_rpc/task/sql_commands.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.0b1/dbt_rpc.egg-info/PKG-INFO` & `dbt-rpc-0.4.0rc1/dbt_rpc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-rpc
-Version: 0.4.0b1
+Version: 0.4.0rc1
 Summary:  A JSON RPC server that provides an interface to programmically interact with dbt projects. 
 Home-page: https://github.com/dbt-labs/dbt-rpc
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-rpc-0.4.0b1/setup.py` & `dbt-rpc-0.4.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 package_name = "dbt-rpc"
-package_version = "0.4.0b1"
+package_version = "0.4.0rc1"
 description = """ A JSON RPC server that provides an interface to programmically interact with dbt projects. """
 
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

