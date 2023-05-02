# Comparing `tmp/fake_coro-0.1.0.tar.gz` & `tmp/fake_coro-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fake_coro-0.1.0.tar", max compression
+gzip compressed data, was "fake_coro-0.1.1.tar", max compression
```

## Comparing `fake_coro-0.1.0.tar` & `fake_coro-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2023-04-30 12:32:15.993362 fake_coro-0.1.0/LICENSE
--rw-r--r--   0        0        0     1709 2023-05-02 09:25:31.329985 fake_coro-0.1.0/PyPI.md
--rw-r--r--   0        0        0      641 2023-05-02 09:25:53.884454 fake_coro-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10951 2023-05-02 09:21:02.461922 fake_coro-0.1.0/src/fake_coro/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 11:22:18.465186 fake_coro-0.1.0/src/fake_coro/py.typed
--rw-r--r--   0        0        0     2285 1970-01-01 00:00:00.000000 fake_coro-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-30 12:32:15.993362 fake_coro-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1802 2023-05-02 09:42:06.953635 fake_coro-0.1.1/PyPI.md
+-rw-r--r--   0        0        0      692 2023-05-02 10:59:40.928084 fake_coro-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11070 2023-05-02 10:52:17.581920 fake_coro-0.1.1/src/fake_coro/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:22:18.465186 fake_coro-0.1.1/src/fake_coro/py.typed
+-rw-r--r--   0        0        0     2486 1970-01-01 00:00:00.000000 fake_coro-0.1.1/PKG-INFO
```

### Comparing `fake_coro-0.1.0/LICENSE` & `fake_coro-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fake_coro-0.1.0/PyPI.md` & `fake_coro-0.1.1/PyPI.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![workflow status](https://img.shields.io/github/actions/workflow/status/NKID00/fake-coro/test.yaml) ![codecov](https://codecov.io/gh/NKID00/fake-coro/branch/master/graph/badge.svg?token=JENJTW0BLG)
+[![workflow status](https://img.shields.io/github/actions/workflow/status/NKID00/fake-coro/test.yaml)](https://github.com/NKID00/fake-coro/actions) [![codecov](https://codecov.io/gh/NKID00/fake-coro/branch/master/graph/badge.svg?token=JENJTW0BLG)](https://app.codecov.io/gh/NKID00/fake-coro)
 
 This module provides fake coroutines that are not coroutines but act like coroutines.
 
 ```
 >>> from fake_coro import fake_coro, yield_
 >>> @fake_coro
 ... def fib(limit):
```

### Comparing `fake_coro-0.1.0/pyproject.toml` & `fake_coro-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "fake-coro"
-version = "0.1.0"
+version = "0.1.1"
 description = "Coroutines emulated with threads."
 authors = ["NKID00 <this@nkid00.name>"]
 readme = "PyPI.md"
 license = "MIT"
+repository = "https://github.com/NKID00/fake-coro"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 pylint = {version = "^2.17.3", python = "^3.7.2"}
```

### Comparing `fake_coro-0.1.0/src/fake_coro/__init__.py` & `fake_coro-0.1.1/src/fake_coro/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,16 @@
             if isinstance(result, _CoOpRaise):
                 raise result.value
             raise RuntimeError(  # pragma: no cover
                 'unexpected result from fake coroutine')
 
     def close(self) -> None:
         '''raise GeneratorExit inside fake coroutine.'''
+        if self._status == _CoStatus.RUNNING:
+            raise ValueError('fake coroutine already executing')
         if self._status in [_CoStatus.CREATED,
                             _CoStatus.SUSPENDED]:
             try:
                 self.throw(GeneratorExit())
             except (StopIteration, GeneratorExit):
                 pass
 
@@ -232,24 +234,24 @@
         if isinstance(exc, BaseException):
             if value is not None:
                 raise TypeError(
                     'instance exception may not have a separate value')
             value = exc.with_traceback(tb)
         elif isinstance(exc, type):
             if not issubclass(exc, BaseException):
-                raise TypeError('exceptions must be classes or instances '
-                                'deriving from BaseException, not type')
+                raise TypeError('exceptions must be classes or instances'
+                                ' deriving from BaseException, not type')
             if value is None:
                 value = exc()
             else:
                 value = exc(value)
         else:
             raise TypeError(
                 f'exceptions must be classes or instances deriving from'
-                f'BaseException, not {type(value)}')
+                f' BaseException, not {type(exc).__name__}')
         with self._lock:
             self._status = _CoStatus.RUNNING
             self._queue_next_throw.put(_CoOpThrow(value))
             result = self._queue_yield_raise.get()
             if isinstance(result, _CoOpYield):
                 return result.value
             if isinstance(result, _CoOpRaise):
```

### Comparing `fake_coro-0.1.0/PKG-INFO` & `fake_coro-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: fake-coro
-Version: 0.1.0
+Version: 0.1.1
 Summary: Coroutines emulated with threads.
+Home-page: https://github.com/NKID00/fake-coro
 License: MIT
 Author: NKID00
 Author-email: this@nkid00.name
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/NKID00/fake-coro
 Description-Content-Type: text/markdown
 
-![workflow status](https://img.shields.io/github/actions/workflow/status/NKID00/fake-coro/test.yaml) ![codecov](https://codecov.io/gh/NKID00/fake-coro/branch/master/graph/badge.svg?token=JENJTW0BLG)
+[![workflow status](https://img.shields.io/github/actions/workflow/status/NKID00/fake-coro/test.yaml)](https://github.com/NKID00/fake-coro/actions) [![codecov](https://codecov.io/gh/NKID00/fake-coro/branch/master/graph/badge.svg?token=JENJTW0BLG)](https://app.codecov.io/gh/NKID00/fake-coro)
 
 This module provides fake coroutines that are not coroutines but act like coroutines.
 
 ```
 >>> from fake_coro import fake_coro, yield_
 >>> @fake_coro
 ... def fib(limit):
```

