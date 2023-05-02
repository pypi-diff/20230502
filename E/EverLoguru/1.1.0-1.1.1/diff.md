# Comparing `tmp/EverLoguru-1.1.0.tar.gz` & `tmp/EverLoguru-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EverLoguru-1.1.0.tar", last modified: Tue May  2 07:07:23 2023, max compression
+gzip compressed data, was "EverLoguru-1.1.1.tar", last modified: Tue May  2 07:26:15 2023, max compression
```

## Comparing `EverLoguru-1.1.0.tar` & `EverLoguru-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cyan      (1000) cyan      (1000)        0 2023-05-02 07:07:23.571610 EverLoguru-1.1.0/
-drwxr-xr-x   0 cyan      (1000) cyan      (1000)        0 2023-05-02 07:07:23.571610 EverLoguru-1.1.0/EverLoguru.egg-info/
--rw-r--r--   0 cyan      (1000) cyan      (1000)     2002 2023-05-02 07:07:23.000000 EverLoguru-1.1.0/EverLoguru.egg-info/PKG-INFO
--rw-r--r--   0 cyan      (1000) cyan      (1000)      262 2023-05-02 07:07:23.000000 EverLoguru-1.1.0/EverLoguru.egg-info/SOURCES.txt
--rw-r--r--   0 cyan      (1000) cyan      (1000)        1 2023-05-02 07:07:23.000000 EverLoguru-1.1.0/EverLoguru.egg-info/dependency_links.txt
--rw-r--r--   0 cyan      (1000) cyan      (1000)       12 2023-05-02 07:07:23.000000 EverLoguru-1.1.0/EverLoguru.egg-info/top_level.txt
--rw-r--r--   0 cyan      (1000) cyan      (1000)     2002 2023-05-02 07:07:23.571610 EverLoguru-1.1.0/PKG-INFO
--rw-r--r--   0 cyan      (1000) cyan      (1000)     1468 2023-05-02 07:01:03.000000 EverLoguru-1.1.0/README.md
-drwxr-xr-x   0 cyan      (1000) cyan      (1000)        0 2023-05-02 07:07:23.571610 EverLoguru-1.1.0/ever_loguru/
--rw-r--r--   0 cyan      (1000) cyan      (1000)       46 2023-05-02 05:18:42.000000 EverLoguru-1.1.0/ever_loguru/__init__.py
--rw-r--r--   0 cyan      (1000) cyan      (1000)      916 2023-05-02 05:16:00.000000 EverLoguru-1.1.0/ever_loguru/handler.py
--rw-r--r--   0 cyan      (1000) cyan      (1000)     2066 2023-05-02 06:23:10.000000 EverLoguru-1.1.0/ever_loguru/install.py
--rw-r--r--   0 cyan      (1000) cyan      (1000)      727 2023-05-02 05:28:28.000000 EverLoguru-1.1.0/ever_loguru/wrapper.py
--rw-r--r--   0 cyan      (1000) cyan      (1000)      597 2023-05-02 07:06:19.000000 EverLoguru-1.1.0/pyproject.toml
--rw-r--r--   0 cyan      (1000) cyan      (1000)       38 2023-05-02 07:07:23.571610 EverLoguru-1.1.0/setup.cfg
--rw-r--r--   0 cyan      (1000) cyan      (1000)      407 2023-05-02 07:05:12.000000 EverLoguru-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:14.998401 EverLoguru-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:14.998401 EverLoguru-1.1.1/EverLoguru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-02 07:26:14.000000 EverLoguru-1.1.1/EverLoguru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-02 07:26:14.000000 EverLoguru-1.1.1/EverLoguru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:26:14.000000 EverLoguru-1.1.1/EverLoguru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 07:26:14.000000 EverLoguru-1.1.1/EverLoguru.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-02 07:26:14.998401 EverLoguru-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-02 07:26:00.000000 EverLoguru-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:26:14.998401 EverLoguru-1.1.1/ever_loguru/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 07:26:00.000000 EverLoguru-1.1.1/ever_loguru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-02 07:26:00.000000 EverLoguru-1.1.1/ever_loguru/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-02 07:26:00.000000 EverLoguru-1.1.1/ever_loguru/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-02 07:26:00.000000 EverLoguru-1.1.1/ever_loguru/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-02 07:26:00.000000 EverLoguru-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 07:26:14.998401 EverLoguru-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-02 07:26:00.000000 EverLoguru-1.1.1/setup.py
```

### Comparing `EverLoguru-1.1.0/EverLoguru.egg-info/PKG-INFO` & `EverLoguru-1.1.1/EverLoguru.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: EverLoguru
-Version: 1.1.0
+Version: 1.1.1
 Summary: Loguru all over the world. | 全世界都在用 Lo~guru~~
 Home-page: 
 Author: cyan
 Author-email: Cyan <lc_shizuku@outlook.com>
 Project-URL: Homepage, https://github.com/Chinese-Cyq20100313/loguruEverywhere
 Project-URL: Bug Tracker, https://github.com/Chinese-Cyq20100313/loguruEverywhere/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires: loguru
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Loguru Ever
 [![PyPI version](https://img.shields.io/pypi/v/EverLoguru.svg)](https://pypi.org/project/EverLoguru/)
-[![PyPI license](https://img.shields.io/pypi/l/EverLoguru.svg)](https://pypi.org/project/EverLoguru/)
-[![PyPI downloads](https://img.shields.io/pypi/dm/EverLoguru.svg)](https://pypi.org/project/EverLoguru/)
+[![GitHub Latest](https://img.shields.io/github/downloads/Chinese-Cyq20100313/loguruEverywhere/latest/total)](https://github.com/Chinese-Cyq20100313/loguruEverywhere/releases)
+  
 Use and replace logging to loguru everywhere!
 
 _**Loguru used all over the world. | 全世界都在用 Loguru**_
 
 ## Installation
 You can install Loguru Ever from PyPI:  
 ```shell
```

### Comparing `EverLoguru-1.1.0/PKG-INFO` & `EverLoguru-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: EverLoguru
-Version: 1.1.0
+Version: 1.1.1
 Summary: Loguru all over the world. | 全世界都在用 Lo~guru~~
 Home-page: 
 Author: cyan
 Author-email: Cyan <lc_shizuku@outlook.com>
 Project-URL: Homepage, https://github.com/Chinese-Cyq20100313/loguruEverywhere
 Project-URL: Bug Tracker, https://github.com/Chinese-Cyq20100313/loguruEverywhere/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires: loguru
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Loguru Ever
 [![PyPI version](https://img.shields.io/pypi/v/EverLoguru.svg)](https://pypi.org/project/EverLoguru/)
-[![PyPI license](https://img.shields.io/pypi/l/EverLoguru.svg)](https://pypi.org/project/EverLoguru/)
-[![PyPI downloads](https://img.shields.io/pypi/dm/EverLoguru.svg)](https://pypi.org/project/EverLoguru/)
+[![GitHub Latest](https://img.shields.io/github/downloads/Chinese-Cyq20100313/loguruEverywhere/latest/total)](https://github.com/Chinese-Cyq20100313/loguruEverywhere/releases)
+  
 Use and replace logging to loguru everywhere!
 
 _**Loguru used all over the world. | 全世界都在用 Loguru**_
 
 ## Installation
 You can install Loguru Ever from PyPI:  
 ```shell
```

### Comparing `EverLoguru-1.1.0/README.md` & `EverLoguru-1.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Loguru Ever
 [![PyPI version](https://img.shields.io/pypi/v/EverLoguru.svg)](https://pypi.org/project/EverLoguru/)
-[![PyPI license](https://img.shields.io/pypi/l/EverLoguru.svg)](https://pypi.org/project/EverLoguru/)
-[![PyPI downloads](https://img.shields.io/pypi/dm/EverLoguru.svg)](https://pypi.org/project/EverLoguru/)
+[![GitHub Latest](https://img.shields.io/github/downloads/Chinese-Cyq20100313/loguruEverywhere/latest/total)](https://github.com/Chinese-Cyq20100313/loguruEverywhere/releases)
+  
 Use and replace logging to loguru everywhere!
 
 _**Loguru used all over the world. | 全世界都在用 Loguru**_
 
 ## Installation
 You can install Loguru Ever from PyPI:  
 ```shell
```

### Comparing `EverLoguru-1.1.0/ever_loguru/handler.py` & `EverLoguru-1.1.1/ever_loguru/handler.py`

 * *Files identical despite different names*

### Comparing `EverLoguru-1.1.0/ever_loguru/install.py` & `EverLoguru-1.1.1/ever_loguru/install.py`

 * *Files identical despite different names*

### Comparing `EverLoguru-1.1.0/ever_loguru/wrapper.py` & `EverLoguru-1.1.1/ever_loguru/wrapper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from loguru import logger
 from logging import PlaceHolder
 
 
 class LoggingLoguruWrapper(PlaceHolder):
-    def __init__(self, __placeholder: str = None, _depth=0):
+    def __init__(self, name: str = None, _depth=0):
+        self.name = name
         self._depth = _depth
-        pass
 
     def __getattr__(self, item):
         return getattr(logger.opt(depth=self._depth), item)
 
 
 class AsyncLoggingLoguruWrapper(PlaceHolder):
-    def __init__(self, __placeholder: str = None, _depth=2):
+    def __init__(self, name: str = None, _depth=2):
+        self.name = name
         self._depth = _depth
 
     @staticmethod
     def _async_wrapper(func):
         async def __logger_wrapper(*args, **kwargs):
             return func(*args, **kwargs)
```

### Comparing `EverLoguru-1.1.0/pyproject.toml` & `EverLoguru-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EverLoguru"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
     { name = "Cyan", email = "lc_shizuku@outlook.com" }
 ]
 description = "Loguru all over the world. | 全世界都在用 Lo~guru~~"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

