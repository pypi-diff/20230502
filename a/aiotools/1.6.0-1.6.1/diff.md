# Comparing `tmp/aiotools-1.6.0.tar.gz` & `tmp/aiotools-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotools-1.6.0.tar", last modified: Tue Mar 14 07:58:21 2023, max compression
+gzip compressed data, was "aiotools-1.6.1.tar", last modified: Tue May  2 14:29:39 2023, max compression
```

## Comparing `aiotools-1.6.0.tar` & `aiotools-1.6.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 07:58:21.395865 aiotools-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-03-14 07:58:06.000000 aiotools-1.6.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-14 07:58:06.000000 aiotools-1.6.0/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-14 07:58:06.000000 aiotools-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-14 07:58:06.000000 aiotools-1.6.0/LICENSE-EXTRA
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-14 07:58:06.000000 aiotools-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-03-14 07:58:21.395865 aiotools-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-03-14 07:58:06.000000 aiotools-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-14 07:58:06.000000 aiotools-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-03-14 07:58:21.399865 aiotools-1.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-03-14 07:58:06.000000 aiotools-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 07:58:21.383864 aiotools-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 07:58:21.391865 aiotools-1.6.0/src/aiotools/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/defer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/fork.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/func.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 07:58:21.395865 aiotools-1.6.0/src/aiotools/taskgroup/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/taskgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/taskgroup/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/taskgroup/base_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/taskgroup/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/taskgroup/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/taskgroup/persistent_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/taskgroup/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/taskgroup/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-03-14 07:58:06.000000 aiotools-1.6.0/src/aiotools/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 07:58:21.391865 aiotools-1.6.0/src/aiotools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19934 2023-03-14 07:58:21.000000 aiotools-1.6.0/src/aiotools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-03-14 07:58:21.000000 aiotools-1.6.0/src/aiotools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 07:58:21.000000 aiotools-1.6.0/src/aiotools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 07:58:21.000000 aiotools-1.6.0/src/aiotools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-14 07:58:21.000000 aiotools-1.6.0/src/aiotools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-14 07:58:21.000000 aiotools-1.6.0/src/aiotools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 07:58:21.395865 aiotools-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-03-14 07:58:06.000000 aiotools-1.6.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-03-14 07:58:06.000000 aiotools-1.6.0/tests/test_defer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-03-14 07:58:06.000000 aiotools-1.6.0/tests/test_fork.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-03-14 07:58:06.000000 aiotools-1.6.0/tests/test_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-14 07:58:06.000000 aiotools-1.6.0/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15158 2023-03-14 07:58:06.000000 aiotools-1.6.0/tests/test_ptaskgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-03-14 07:58:06.000000 aiotools-1.6.0/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-03-14 07:58:06.000000 aiotools-1.6.0/tests/test_taskgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-03-14 07:58:06.000000 aiotools-1.6.0/tests/test_taskgroup_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-03-14 07:58:06.000000 aiotools-1.6.0/tests/test_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:29:39.701790 aiotools-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-05-02 14:29:23.000000 aiotools-1.6.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-02 14:29:23.000000 aiotools-1.6.1/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-02 14:29:23.000000 aiotools-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-02 14:29:23.000000 aiotools-1.6.1/LICENSE-EXTRA
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-02 14:29:23.000000 aiotools-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-05-02 14:29:39.701790 aiotools-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-02 14:29:23.000000 aiotools-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-02 14:29:23.000000 aiotools-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-02 14:29:39.701790 aiotools-1.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-05-02 14:29:23.000000 aiotools-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:29:39.693790 aiotools-1.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:29:39.697790 aiotools-1.6.1/src/aiotools/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/defer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:29:39.701790 aiotools-1.6.1/src/aiotools/taskgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/taskgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/taskgroup/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/taskgroup/base_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/taskgroup/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/taskgroup/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/taskgroup/persistent_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/taskgroup/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/taskgroup/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-02 14:29:23.000000 aiotools-1.6.1/src/aiotools/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:29:39.697790 aiotools-1.6.1/src/aiotools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-05-02 14:29:39.000000 aiotools-1.6.1/src/aiotools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-02 14:29:39.000000 aiotools-1.6.1/src/aiotools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:29:39.000000 aiotools-1.6.1/src/aiotools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:29:39.000000 aiotools-1.6.1/src/aiotools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-02 14:29:39.000000 aiotools-1.6.1/src/aiotools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 14:29:39.000000 aiotools-1.6.1/src/aiotools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:29:39.701790 aiotools-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-05-02 14:29:23.000000 aiotools-1.6.1/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-02 14:29:23.000000 aiotools-1.6.1/tests/test_defer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-02 14:29:23.000000 aiotools-1.6.1/tests/test_fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-02 14:29:23.000000 aiotools-1.6.1/tests/test_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-02 14:29:23.000000 aiotools-1.6.1/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15158 2023-05-02 14:29:23.000000 aiotools-1.6.1/tests/test_ptaskgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-05-02 14:29:23.000000 aiotools-1.6.1/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-02 14:29:23.000000 aiotools-1.6.1/tests/test_taskgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-02 14:29:23.000000 aiotools-1.6.1/tests/test_taskgroup_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-02 14:29:23.000000 aiotools-1.6.1/tests/test_timer.py
```

### Comparing `aiotools-1.6.0/CHANGES.md` & `aiotools-1.6.1/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,21 @@
     We named the news folder "changes".
 
     WARNING: Don't drop the last line!
 -->
 
 <!-- towncrier release notes start -->
 
+1.6.1 (2023-05-02)
+------------------
+
+### Fixes
+* PersistentTaskGroup no longer stores the history of unhandled exceptions and raises them as an exception group to prevent memory leaks ([#54](https://github.com/achimnol/aiotools/issues/54))
+
+
 1.6.0 (2023-03-14)
 ------------------
 
 ### Features
 * Add `as_completed_safe()` which enhances `asyncio.as_completed()` using `PersistentTaskGroup` ([#52](https://github.com/achimnol/aiotools/issues/52))
```

### Comparing `aiotools-1.6.0/LICENSE` & `aiotools-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/PKG-INFO` & `aiotools-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotools
-Version: 1.6.0
+Version: 1.6.1
 Summary: Idiomatic asyncio utilities
 Home-page: https://github.com/achimnol/aiotools
 Author: Joongi Kim
 Author-email: me@daybreaker.info
 License: MIT
 Project-URL: Documentation, https://aiotools.readthedocs.io
 Project-URL: Tracker, https://github.com/achimnol/aiotools/issues
@@ -273,14 +273,21 @@
     We named the news folder "changes".
 
     WARNING: Don't drop the last line!
 -->
 
 <!-- towncrier release notes start -->
 
+1.6.1 (2023-05-02)
+------------------
+
+### Fixes
+* PersistentTaskGroup no longer stores the history of unhandled exceptions and raises them as an exception group to prevent memory leaks ([#54](https://github.com/achimnol/aiotools/issues/54))
+
+
 1.6.0 (2023-03-14)
 ------------------
 
 ### Features
 * Add `as_completed_safe()` which enhances `asyncio.as_completed()` using `PersistentTaskGroup` ([#52](https://github.com/achimnol/aiotools/issues/52))
```

### Comparing `aiotools-1.6.0/README.md` & `aiotools-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/pyproject.toml` & `aiotools-1.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/setup.cfg` & `aiotools-1.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/src/aiotools/__init__.py` & `aiotools-1.6.1/src/aiotools/__init__.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/src/aiotools/context.py` & `aiotools-1.6.1/src/aiotools/context.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/src/aiotools/defer.py` & `aiotools-1.6.1/src/aiotools/defer.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/src/aiotools/fork.py` & `aiotools-1.6.1/src/aiotools/fork.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/src/aiotools/func.py` & `aiotools-1.6.1/src/aiotools/func.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import collections
 import functools
+from typing import Optional
 
 from .compat import get_running_loop
 
 __all__ = (
     'apartial',
     'lru_cache',
 )
@@ -22,15 +23,15 @@
         return await coro(*args, *cargs, **kwargs, **ckwargs)
 
     return wrapped
 
 
 def lru_cache(maxsize: int = 128,
               typed: bool = False,
-              expire_after: float = None):
+              expire_after: Optional[float] = None):
     """
     A simple LRU cache just like :func:`functools.lru_cache`, but it works for
     coroutines.  This is not as heavily optimized as :func:`functools.lru_cache`
     which uses an internal C implementation, as it targets async operations
     that take a long time.
 
     It follows the same API that the standard functools provides.  The wrapped
```

### Comparing `aiotools-1.6.0/src/aiotools/iter.py` & `aiotools-1.6.1/src/aiotools/iter.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/src/aiotools/server.py` & `aiotools-1.6.1/src/aiotools/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
     extra_procs: Iterable[Callable] = tuple(),
     stop_signals: Iterable[signal.Signals] = (
         signal.SIGINT,
         signal.SIGTERM
     ),
     num_workers: int = 1,
     args: Iterable[Any] = tuple(),
-    wait_timeout: float = None,
+    wait_timeout: Optional[float] = None,
 ) -> None:
     """
     Starts a multi-process server where each process has their own individual
     asyncio event loop.  Their lifecycles are automantically managed -- if the
     main program receives one of the signals specified in ``stop_signals`` it
     will initiate the shutdown routines on each worker that stops the event
     loop gracefully.
```

### Comparing `aiotools-1.6.0/src/aiotools/taskgroup/__init__.py` & `aiotools-1.6.1/src/aiotools/taskgroup/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import asyncio
 
 from .types import MultiError, TaskGroupError
 
 if hasattr(asyncio, 'TaskGroup'):
-    from . import base
     from . import persistent
     from .base import *        # noqa
     from .persistent import *  # noqa
     __all__ = [
-        'MultiError',
-        'TaskGroupError',
-        *base.__all__,
+        "MultiError",
+        "TaskGroup",
+        "TaskGroupError",
+        "current_taskgroup",
         *persistent.__all__,
     ]
 else:
-    from . import base_compat
     from . import persistent_compat
     from .base_compat import *        # type: ignore  # noqa
     from .persistent_compat import *  # type: ignore  # noqa
-    __all__ = [  # type: ignore
-        'MultiError',
-        'TaskGroupError',
-        *base_compat.__all__,
+    from .base_compat import has_contextvars
+    __all__ = [  # type: ignore  # noqa
+        "MultiError",
+        "TaskGroup",
+        "TaskGroupError",
         *persistent_compat.__all__,
     ]
+    if has_contextvars:
+        __all__.append("current_taskgroup")
+
 
 from .utils import as_completed_safe  # noqa
 
 __all__.append("as_completed_safe")
```

### Comparing `aiotools-1.6.0/src/aiotools/taskgroup/base.py` & `aiotools-1.6.1/src/aiotools/taskgroup/base.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/src/aiotools/taskgroup/base_compat.py` & `aiotools-1.6.1/src/aiotools/taskgroup/base_compat.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/src/aiotools/taskgroup/common.py` & `aiotools-1.6.1/src/aiotools/taskgroup/common.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/src/aiotools/taskgroup/persistent.py` & `aiotools-1.6.1/src/aiotools/taskgroup/persistent.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from contextvars import ContextVar, Token
 from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Callable,
     Coroutine,
-    List,
     Optional,
     Sequence,
     Type,
     Union,
 )
 import weakref
 
@@ -38,33 +37,31 @@
     traceback.print_exc()
 
 
 class PersistentTaskGroup:
 
     _base_error: Optional[BaseException]
     _exc_handler: AsyncExceptionHandler
-    _errors: Optional[List[BaseException]]
     _tasks: "weakref.WeakSet[asyncio.Task]"
     _on_completed_fut: Optional[asyncio.Future]
     _current_taskgroup_token: Optional[Token["PersistentTaskGroup"]]
 
     @classmethod
     def all_ptaskgroups(cls) -> Sequence['PersistentTaskGroup']:
         return list(_all_ptaskgroups)
 
     def __init__(
         self,
         *,
-        name: str = None,
-        exception_handler: AsyncExceptionHandler = None,
+        name: Optional[str] = None,
+        exception_handler: Optional[AsyncExceptionHandler] = None,
     ) -> None:
         self._entered = False
         self._exiting = False
         self._aborting = False
-        self._errors = []
         self._base_error = None
         self._name = name or f"{next(_ptaskgroup_idx)}"
         self._parent_cancel_requested = False
         self._unfinished_tasks = 0
         self._on_completed_fut = None
         self._parent_task = compat.current_task()
         self._tasks = weakref.WeakSet()
@@ -81,28 +78,28 @@
     def get_name(self) -> str:
         return self._name
 
     def create_task(
         self,
         coro: Coroutine[Any, Any, Any],
         *,
-        name: str = None,
+        name: Optional[str] = None,
     ) -> Awaitable[Any]:
         if not self._entered:
             # When used as object attribute, auto-enter.
             self._entered = True
         if self._exiting and self._unfinished_tasks == 0:
             raise RuntimeError(f"{self!r} has already finished")
         return self._create_task_with_name(coro, name=name, cb=self._on_task_done)
 
     def _create_task_with_name(
         self,
         coro: Coroutine[Any, Any, Any],
         *,
-        name: str = None,
+        name: Optional[str] = None,
         cb: Callable[[asyncio.Task], Any],
     ) -> Awaitable[Any]:
         loop = compat.get_running_loop()
         result_future = loop.create_future()
         child_task = loop.create_task(
             self._task_wrapper(coro, weakref.ref(result_future)),
             name=name,
@@ -188,30 +185,28 @@
         finally:
             del fut
 
     def _on_task_done(self, task: asyncio.Task) -> None:
         self._unfinished_tasks -= 1
         assert self._unfinished_tasks >= 0
         assert self._parent_task is not None
-        assert self._errors is not None
 
         if self._on_completed_fut is not None and not self._unfinished_tasks:
             if not self._on_completed_fut.done():
                 self._on_completed_fut.set_result(True)
 
         if task.cancelled():
             _log.debug("%r in %r has been cancelled.", task, self)
             return
 
         exc = task.exception()
         if exc is None:
             return
 
         # Now the exception is BaseException.
-        self._errors.append(exc)
         if self._base_error is None:
             self._base_error = exc
 
         self._trigger_shutdown()
         if not self._parent_task.cancelling():
             self._parent_cancel_requested = True
 
@@ -223,16 +218,16 @@
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> Optional[bool]:
+        assert self._parent_task is not None
         self._exiting = True
-        assert self._errors is not None
         propagate_cancellation_error: Optional[
             Union[Type[BaseException], BaseException]
         ] = None
 
         if (exc_val is not None and
                 self._is_base_error(exc_val) and
                 self._base_error is None):
@@ -259,42 +254,23 @@
             propagate_cancellation_error = prop_ex
         if self._current_taskgroup_token:
             current_ptaskgroup.reset(self._current_taskgroup_token)
             self._current_taskgroup_token = None
         if propagate_cancellation_error is not None:
             raise propagate_cancellation_error
 
-        if exc_val is not None and exc_type is not asyncio.CancelledError:
-            # If there are any unhandled errors, let's add them to
-            # the bubbled up exception group.
-            # Normally, they should have been swallowed and logged
-            # by the fallback exception handler.
-            self._errors.append(exc_val)
-
-        if self._errors:
-            # Bubble up errors
-            errors = self._errors
-            self._errors = None
-            me = BaseExceptionGroup(
-                'unhandled errors in a PersistentTaskGroup',
-                errors,
-            )
-            raise me from None
-
         return None
 
     def __repr__(self) -> str:
         info = ['']
         if self._name:
             info.append(f'name={self._name}')
         if self._tasks:
             info.append(f'tasks={len(self._tasks)}')
         if self._unfinished_tasks:
             info.append(f'unfinished={self._unfinished_tasks}')
-        if self._errors:
-            info.append(f'errors={len(self._errors)}')
         if self._aborting:
             info.append('cancelling')
         elif self._entered:
             info.append('entered')
         info_str = ' '.join(info)
         return f'<PersistentTaskGroup({info_str})>'
```

### Comparing `aiotools-1.6.0/src/aiotools/taskgroup/persistent_compat.py` & `aiotools-1.6.1/src/aiotools/taskgroup/persistent_compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,23 @@
     has_contextvars = False
 from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Callable,
     Coroutine,
-    List,
     Optional,
     Sequence,
     Type,
 )
 import weakref
 
 from .. import compat
 from .common import create_task_with_name, patch_task
-from .types import AsyncExceptionHandler, TaskGroupError
+from .types import AsyncExceptionHandler
 
 __all__ = [
     'PersistentTaskGroup',
 ]
 
 if has_contextvars:
     current_ptaskgroup: ContextVar['PersistentTaskGroup'] = \
@@ -43,33 +42,31 @@
     traceback.print_exc()
 
 
 class PersistentTaskGroup:
 
     _base_error: Optional[BaseException]
     _exc_handler: AsyncExceptionHandler
-    _errors: Optional[List[BaseException]]
     _tasks: "weakref.WeakSet[asyncio.Task]"
     _on_completed_fut: Optional[asyncio.Future]
     _current_taskgroup_token: Optional["Token[PersistentTaskGroup]"]
 
     @classmethod
     def all_ptaskgroups(cls) -> Sequence['PersistentTaskGroup']:
         return list(_all_ptaskgroups)
 
     def __init__(
         self,
         *,
-        name: str = None,
-        exception_handler: AsyncExceptionHandler = None,
+        name: Optional[str] = None,
+        exception_handler: Optional[AsyncExceptionHandler] = None,
     ) -> None:
         self._entered = False
         self._exiting = False
         self._aborting = False
-        self._errors = []
         self._base_error = None
         self._name = name or f"{next(_ptaskgroup_idx)}"
         self._parent_cancel_requested = False
         self._unfinished_tasks = 0
         self._on_completed_fut = None
         self._parent_task = compat.current_task()
         self._tasks = weakref.WeakSet()
@@ -86,28 +83,28 @@
     def get_name(self) -> str:
         return self._name
 
     def create_task(
         self,
         coro: Coroutine[Any, Any, Any],
         *,
-        name: str = None,
+        name: Optional[str] = None,
     ) -> Awaitable[Any]:
         if not self._entered:
             # When used as object attribute, auto-enter.
             self._entered = True
         if self._exiting and self._unfinished_tasks == 0:
             raise RuntimeError(f"{self!r} has already finished")
         return self._create_task_with_name(coro, name=name, cb=self._on_task_done)
 
     def _create_task_with_name(
         self,
         coro: Coroutine[Any, Any, Any],
         *,
-        name: str = None,
+        name: Optional[str] = None,
         cb: Callable[[asyncio.Task], Any],
     ) -> Awaitable[Any]:
         loop = compat.get_running_loop()
         result_future = loop.create_future()
         child_task = create_task_with_name(
             self._task_wrapper(coro, weakref.ref(result_future)),
             name=name,
@@ -193,30 +190,28 @@
         finally:
             del fut
 
     def _on_task_done(self, task: asyncio.Task) -> None:
         self._unfinished_tasks -= 1
         assert self._unfinished_tasks >= 0
         assert self._parent_task is not None
-        assert self._errors is not None
 
         if self._on_completed_fut is not None and not self._unfinished_tasks:
             if not self._on_completed_fut.done():
                 self._on_completed_fut.set_result(True)
 
         if task.cancelled():
             _log.debug("%r in %r has been cancelled.", task, self)
             return
 
         exc = task.exception()
         if exc is None:
             return
 
         # Now the exception is BaseException.
-        self._errors.append(exc)
         if self._base_error is None:
             self._base_error = exc
 
         self._trigger_shutdown()
         if not self._parent_task.__cancel_requested__:  # type: ignore
             self._parent_cancel_requested = True
 
@@ -231,15 +226,14 @@
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> Optional[bool]:
         self._exiting = True
-        assert self._errors is not None
         propagate_cancelation = False
 
         if (exc_val is not None and
                 self._is_base_error(exc_val) and
                 self._base_error is None):
             self._base_error = exc_val
 
@@ -272,42 +266,23 @@
 
         if propagate_cancelation:
             # The wrapping task was cancelled; since we're done with
             # closing all child tasks, just propagate the cancellation
             # request now.
             raise asyncio.CancelledError()
 
-        if exc_val is not None and exc_type is not asyncio.CancelledError:
-            # If there are any unhandled errors, let's add them to
-            # the bubbled up exception group.
-            # Normally, they should have been swallowed and logged
-            # by the fallback exception handler.
-            self._errors.append(exc_val)
-
-        if self._errors:
-            # Bubble up errors
-            errors = self._errors
-            self._errors = None
-            me = TaskGroupError(
-                'unhandled errors in a PersistentTaskGroup',
-                errors,
-            )
-            raise me from None
-
         return None
 
     def __repr__(self) -> str:
         info = ['']
         if self._name:
             info.append(f'name={self._name}')
         if self._tasks:
             info.append(f'tasks={len(self._tasks)}')
         if self._unfinished_tasks:
             info.append(f'unfinished={self._unfinished_tasks}')
-        if self._errors:
-            info.append(f'errors={len(self._errors)}')
         if self._aborting:
             info.append('cancelling')
         elif self._entered:
             info.append('entered')
         info_str = ' '.join(info)
         return f'<PersistentTaskGroup({info_str})>'
```

### Comparing `aiotools-1.6.0/src/aiotools/taskgroup/types.py` & `aiotools-1.6.1/src/aiotools/taskgroup/types.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         exc_tb: TracebackType,
     ) -> None:
         ...
 
 
 if not hasattr(builtins, 'ExceptionGroup'):
 
-    class MultiError(Exception):
+    class MultiError(Exception):  # type: ignore[no-redef]
 
         def __init__(self, msg, errors=()):
             if errors:
                 types = set(type(e).__name__ for e in errors)
                 msg = f'{msg}; {len(errors)} sub errors: ({", ".join(types)})'
                 for er in errors:
                     msg += f'\n + {type(er).__name__}: {er}'
@@ -43,26 +43,26 @@
 
         def get_error_types(self):
             return {type(e) for e in self.__errors__}
 
         def __reduce__(self):
             return (type(self), (self.args,), {'__errors__': self.__errors__})
 
-    class TaskGroupError(MultiError):
+    class TaskGroupError(MultiError):  # type: ignore[no-redef]
         """
         An alias to :exc:`MultiError`.
         """
         pass
 
 else:
 
-    class MultiError(ExceptionGroup):
+    class MultiError(ExceptionGroup):  # type: ignore[no-redef]
 
         def __init__(self, msg, errors=()):
             super().__init__(msg, errors)
             self.__errors__ = errors
 
         def get_error_types(self):
             return {type(e) for e in self.exceptions}
 
-    class TaskGroupError(MultiError):
+    class TaskGroupError(MultiError):  # type: ignore[no-redef]
         pass
```

### Comparing `aiotools-1.6.0/src/aiotools/taskgroup/utils.py` & `aiotools-1.6.1/src/aiotools/taskgroup/utils.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/src/aiotools/timer.py` & `aiotools-1.6.1/src/aiotools/timer.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/src/aiotools.egg-info/PKG-INFO` & `aiotools-1.6.1/src/aiotools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotools
-Version: 1.6.0
+Version: 1.6.1
 Summary: Idiomatic asyncio utilities
 Home-page: https://github.com/achimnol/aiotools
 Author: Joongi Kim
 Author-email: me@daybreaker.info
 License: MIT
 Project-URL: Documentation, https://aiotools.readthedocs.io
 Project-URL: Tracker, https://github.com/achimnol/aiotools/issues
@@ -273,14 +273,21 @@
     We named the news folder "changes".
 
     WARNING: Don't drop the last line!
 -->
 
 <!-- towncrier release notes start -->
 
+1.6.1 (2023-05-02)
+------------------
+
+### Fixes
+* PersistentTaskGroup no longer stores the history of unhandled exceptions and raises them as an exception group to prevent memory leaks ([#54](https://github.com/achimnol/aiotools/issues/54))
+
+
 1.6.0 (2023-03-14)
 ------------------
 
 ### Features
 * Add `as_completed_safe()` which enhances `asyncio.as_completed()` using `PersistentTaskGroup` ([#52](https://github.com/achimnol/aiotools/issues/52))
```

### Comparing `aiotools-1.6.0/src/aiotools.egg-info/SOURCES.txt` & `aiotools-1.6.1/src/aiotools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/tests/test_context.py` & `aiotools-1.6.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/tests/test_defer.py` & `aiotools-1.6.1/tests/test_defer.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/tests/test_fork.py` & `aiotools-1.6.1/tests/test_fork.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/tests/test_func.py` & `aiotools-1.6.1/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/tests/test_iter.py` & `aiotools-1.6.1/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/tests/test_ptaskgroup.py` & `aiotools-1.6.1/tests/test_ptaskgroup.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/tests/test_server.py` & `aiotools-1.6.1/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/tests/test_taskgroup.py` & `aiotools-1.6.1/tests/test_taskgroup.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/tests/test_taskgroup_utils.py` & `aiotools-1.6.1/tests/test_taskgroup_utils.py`

 * *Files identical despite different names*

### Comparing `aiotools-1.6.0/tests/test_timer.py` & `aiotools-1.6.1/tests/test_timer.py`

 * *Files identical despite different names*

