# Comparing `tmp/EverLoguru-1.1.1.tar.gz` & `tmp/EverLoguru-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EverLoguru-1.1.1.tar", last modified: Tue May  2 07:26:15 2023, max compression
+gzip compressed data, was "EverLoguru-1.1.2.tar", last modified: Tue May  2 07:40:37 2023, max compression
```

## Comparing `EverLoguru-1.1.1.tar` & `EverLoguru-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:14.998401 EverLoguru-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:14.998401 EverLoguru-1.1.1/EverLoguru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-02 07:26:14.000000 EverLoguru-1.1.1/EverLoguru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-02 07:26:14.000000 EverLoguru-1.1.1/EverLoguru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:26:14.000000 EverLoguru-1.1.1/EverLoguru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 07:26:14.000000 EverLoguru-1.1.1/EverLoguru.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-02 07:26:14.998401 EverLoguru-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-02 07:26:00.000000 EverLoguru-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:14.998401 EverLoguru-1.1.1/ever_loguru/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 07:26:00.000000 EverLoguru-1.1.1/ever_loguru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-02 07:26:00.000000 EverLoguru-1.1.1/ever_loguru/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-02 07:26:00.000000 EverLoguru-1.1.1/ever_loguru/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-02 07:26:00.000000 EverLoguru-1.1.1/ever_loguru/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-02 07:26:00.000000 EverLoguru-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 07:26:14.998401 EverLoguru-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-02 07:26:00.000000 EverLoguru-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:40:37.443535 EverLoguru-1.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:40:37.443535 EverLoguru-1.1.2/EverLoguru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-02 07:40:37.000000 EverLoguru-1.1.2/EverLoguru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-02 07:40:37.000000 EverLoguru-1.1.2/EverLoguru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:40:37.000000 EverLoguru-1.1.2/EverLoguru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 07:40:37.000000 EverLoguru-1.1.2/EverLoguru.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-02 07:40:37.443535 EverLoguru-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-02 07:40:26.000000 EverLoguru-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:40:37.443535 EverLoguru-1.1.2/ever_loguru/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 07:40:26.000000 EverLoguru-1.1.2/ever_loguru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-02 07:40:26.000000 EverLoguru-1.1.2/ever_loguru/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-02 07:40:26.000000 EverLoguru-1.1.2/ever_loguru/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-02 07:40:26.000000 EverLoguru-1.1.2/ever_loguru/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-02 07:40:26.000000 EverLoguru-1.1.2/ever_loguru/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-02 07:40:26.000000 EverLoguru-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 07:40:37.443535 EverLoguru-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-02 07:40:26.000000 EverLoguru-1.1.2/setup.py
```

### Comparing `EverLoguru-1.1.1/EverLoguru.egg-info/PKG-INFO` & `EverLoguru-1.1.2/EverLoguru.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EverLoguru
-Version: 1.1.1
+Version: 1.1.2
 Summary: Loguru all over the world. | 全世界都在用 Lo~guru~~
 Home-page: 
 Author: cyan
 Author-email: Cyan <lc_shizuku@outlook.com>
 Project-URL: Homepage, https://github.com/Chinese-Cyq20100313/loguruEverywhere
 Project-URL: Bug Tracker, https://github.com/Chinese-Cyq20100313/loguruEverywhere/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EverLoguru-1.1.1/PKG-INFO` & `EverLoguru-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EverLoguru
-Version: 1.1.1
+Version: 1.1.2
 Summary: Loguru all over the world. | 全世界都在用 Lo~guru~~
 Home-page: 
 Author: cyan
 Author-email: Cyan <lc_shizuku@outlook.com>
 Project-URL: Homepage, https://github.com/Chinese-Cyq20100313/loguruEverywhere
 Project-URL: Bug Tracker, https://github.com/Chinese-Cyq20100313/loguruEverywhere/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EverLoguru-1.1.1/README.md` & `EverLoguru-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `EverLoguru-1.1.1/ever_loguru/handler.py` & `EverLoguru-1.1.2/ever_loguru/handler.py`

 * *Files identical despite different names*

### Comparing `EverLoguru-1.1.1/ever_loguru/install.py` & `EverLoguru-1.1.2/ever_loguru/install.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     :param replace_exist: replace_exist
     :return: 
     """
     _Logger = getattr(sys.modules['logging'], "Logger")
     setattr(sys.modules['logging'], "Logger", LoggingLoguruWrapper)
     setattr(sys.modules['logging'].Logger, "manager", _Logger.manager)
     setattr(sys.modules['logging'].Logger.manager, "loggerClass", LoggingLoguruWrapper)
+
     if replace_exist:
         update_exist()
 
 
 # noinspection PyPep8Naming
 def install_force(replace_exist: bool = False):
     """
```

### Comparing `EverLoguru-1.1.1/ever_loguru/wrapper.py` & `EverLoguru-1.1.2/ever_loguru/wrapper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from loguru import logger
-from logging import PlaceHolder
 
+from .mask import FakeLogger
 
-class LoggingLoguruWrapper(PlaceHolder):
+
+class LoggingLoguruWrapper(FakeLogger):
     def __init__(self, name: str = None, _depth=0):
         self.name = name
         self._depth = _depth
 
     def __getattr__(self, item):
         return getattr(logger.opt(depth=self._depth), item)
 
 
-class AsyncLoggingLoguruWrapper(PlaceHolder):
+class AsyncLoggingLoguruWrapper(FakeLogger):
     def __init__(self, name: str = None, _depth=2):
         self.name = name
         self._depth = _depth
 
     @staticmethod
     def _async_wrapper(func):
         async def __logger_wrapper(*args, **kwargs):
```

### Comparing `EverLoguru-1.1.1/pyproject.toml` & `EverLoguru-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EverLoguru"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
     { name = "Cyan", email = "lc_shizuku@outlook.com" }
 ]
 description = "Loguru all over the world. | 全世界都在用 Lo~guru~~"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

