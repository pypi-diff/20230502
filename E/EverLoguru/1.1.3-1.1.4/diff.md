# Comparing `tmp/EverLoguru-1.1.3.tar.gz` & `tmp/EverLoguru-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EverLoguru-1.1.3.tar", last modified: Tue May  2 07:48:54 2023, max compression
+gzip compressed data, was "EverLoguru-1.1.4.tar", last modified: Tue May  2 07:56:45 2023, max compression
```

## Comparing `EverLoguru-1.1.3.tar` & `EverLoguru-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:48:54.806527 EverLoguru-1.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:48:54.802527 EverLoguru-1.1.3/EverLoguru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-02 07:48:54.000000 EverLoguru-1.1.3/EverLoguru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-02 07:48:54.000000 EverLoguru-1.1.3/EverLoguru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:48:54.000000 EverLoguru-1.1.3/EverLoguru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 07:48:54.000000 EverLoguru-1.1.3/EverLoguru.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-02 07:48:54.806527 EverLoguru-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-02 07:48:43.000000 EverLoguru-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:48:54.806527 EverLoguru-1.1.3/ever_loguru/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 07:48:43.000000 EverLoguru-1.1.3/ever_loguru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-02 07:48:43.000000 EverLoguru-1.1.3/ever_loguru/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-02 07:48:43.000000 EverLoguru-1.1.3/ever_loguru/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-02 07:48:43.000000 EverLoguru-1.1.3/ever_loguru/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-02 07:48:43.000000 EverLoguru-1.1.3/ever_loguru/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-02 07:48:43.000000 EverLoguru-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 07:48:54.806527 EverLoguru-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-02 07:48:43.000000 EverLoguru-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:56:45.157849 EverLoguru-1.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:56:45.153849 EverLoguru-1.1.4/EverLoguru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-02 07:56:45.000000 EverLoguru-1.1.4/EverLoguru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-02 07:56:45.000000 EverLoguru-1.1.4/EverLoguru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:56:45.000000 EverLoguru-1.1.4/EverLoguru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 07:56:45.000000 EverLoguru-1.1.4/EverLoguru.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-02 07:56:45.157849 EverLoguru-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-02 07:56:31.000000 EverLoguru-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:56:45.157849 EverLoguru-1.1.4/ever_loguru/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 07:56:31.000000 EverLoguru-1.1.4/ever_loguru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-02 07:56:31.000000 EverLoguru-1.1.4/ever_loguru/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-02 07:56:31.000000 EverLoguru-1.1.4/ever_loguru/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-02 07:56:31.000000 EverLoguru-1.1.4/ever_loguru/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-02 07:56:31.000000 EverLoguru-1.1.4/ever_loguru/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-02 07:56:31.000000 EverLoguru-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 07:56:45.157849 EverLoguru-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-02 07:56:31.000000 EverLoguru-1.1.4/setup.py
```

### Comparing `EverLoguru-1.1.3/EverLoguru.egg-info/PKG-INFO` & `EverLoguru-1.1.4/EverLoguru.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EverLoguru
-Version: 1.1.3
+Version: 1.1.4
 Summary: Loguru all over the world. | 全世界都在用 Lo~guru~~
 Home-page: 
 Author: cyan
 Author-email: Cyan <lc_shizuku@outlook.com>
 Project-URL: Homepage, https://github.com/Chinese-Cyq20100313/loguruEverywhere
 Project-URL: Bug Tracker, https://github.com/Chinese-Cyq20100313/loguruEverywhere/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EverLoguru-1.1.3/PKG-INFO` & `EverLoguru-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EverLoguru
-Version: 1.1.3
+Version: 1.1.4
 Summary: Loguru all over the world. | 全世界都在用 Lo~guru~~
 Home-page: 
 Author: cyan
 Author-email: Cyan <lc_shizuku@outlook.com>
 Project-URL: Homepage, https://github.com/Chinese-Cyq20100313/loguruEverywhere
 Project-URL: Bug Tracker, https://github.com/Chinese-Cyq20100313/loguruEverywhere/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EverLoguru-1.1.3/README.md` & `EverLoguru-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `EverLoguru-1.1.3/ever_loguru/handler.py` & `EverLoguru-1.1.4/ever_loguru/handler.py`

 * *Files identical despite different names*

### Comparing `EverLoguru-1.1.3/ever_loguru/install.py` & `EverLoguru-1.1.4/ever_loguru/install.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     Install for manager.getLogger, manager.loggerClass that may break some modules
     :param replace_exist: Replace exist logger
     :return:
     """
     install()
     sys.modules['logging'].Logger.manager.getLogger = LoggingLoguruWrapper
     sys.modules['logging'].Logger.manager.loggerClass = LoggingLoguruWrapper
-    setattr(sys.modules['logging'].Logger.manager, "_loggerClass", LoggingLoguruWrapper)
+    setattr(sys.modules['logging'].Logger.manager, "loggerClass", LoggingLoguruWrapper)
     if replace_exist:
         update_exist()
 
 
 # noinspection PyPep8Naming
 def remove():
     sys.modules['logging'].Logger.callHandlers = callHandlers_func
```

### Comparing `EverLoguru-1.1.3/ever_loguru/wrapper.py` & `EverLoguru-1.1.4/ever_loguru/wrapper.py`

 * *Files identical despite different names*

### Comparing `EverLoguru-1.1.3/pyproject.toml` & `EverLoguru-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EverLoguru"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
     { name = "Cyan", email = "lc_shizuku@outlook.com" }
 ]
 description = "Loguru all over the world. | 全世界都在用 Lo~guru~~"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

