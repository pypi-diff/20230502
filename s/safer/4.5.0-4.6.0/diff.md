# Comparing `tmp/safer-4.5.0.tar.gz` & `tmp/safer-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safer-4.5.0.tar", max compression
+gzip compressed data, was "safer-4.6.0.tar", max compression
```

## Comparing `safer-4.5.0.tar` & `safer-4.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2020-03-02 15:29:53.000000 safer-4.5.0/LICENSE
--rw-r--r--   0        0        0     4676 2023-02-23 19:48:11.107393 safer-4.5.0/README.md
--rw-r--r--   0        0        0      604 2023-02-23 19:55:58.525730 safer-4.5.0/pyproject.toml
--rw-r--r--   0        0        0    20809 2023-02-23 18:18:08.002160 safer-4.5.0/safer.py
--rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 safer-4.5.0/setup.py
--rw-r--r--   0        0        0     5266 1970-01-01 00:00:00.000000 safer-4.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-02 09:24:25.348741 safer-4.6.0/LICENSE
+-rw-r--r--   0        0        0     4713 2023-05-02 09:24:25.349032 safer-4.6.0/README.md
+-rw-r--r--   0        0        0      604 2023-05-02 10:28:30.607550 safer-4.6.0/pyproject.toml
+-rw-r--r--   0        0        0    21703 2023-05-02 10:27:41.070388 safer-4.6.0/safer.py
+-rw-r--r--   0        0        0     5330 1970-01-01 00:00:00.000000 safer-4.6.0/setup.py
+-rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 safer-4.6.0/PKG-INFO
```

### Comparing `safer-4.5.0/LICENSE` & `safer-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safer-4.5.0/README.md` & `safer-4.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# 🧿 `safer`: A safer writer 🧿
+
 Avoid partial writes or corruption!
 
 `safer` wraps file streams, sockets, or a callable, and offers a drop-in
 replacement for regular old `open()`.
 
 ## Quick summary
 
@@ -89,16 +91,16 @@
             write_body(s)  # Exception is thrown here
             write_footer(s)
      except Exception:
         write_error(sock)  # Nothing has been written
 
 ### Example: `safer.open()` and json
 
-`safer.open()` is a a drop-in replacement for built-in `open()` except that when
-used as a context, it leaves the original file unchanged on failure.
+`safer.open()` is a a drop-in replacement for built-in `open()` except that
+when used as a context, it leaves the original file unchanged on failure.
 
 It's easy to write broken JSON if something within it doesn't serialize.
 
     with open(filename, 'w') as fp:
         json.dump(data, fp)
         # If an exception is raised, the file is empty or partly written
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `safer-4.5.0/pyproject.toml` & `safer-4.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 target-version = ['py37']
 
 [tool.doks]
 auto = true
 
 [tool.poetry]
 name = "safer"
-version = "4.5.0"
+version = "4.6.0"
 description = "🧿 A safer writer for files and streams 🧿"
 authors = ["Tom Ritchford <tom@swirly.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `safer-4.5.0/safer.py` & `safer-4.6.0/safer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-🧿 safer: a safer writer for files and streams 🧿
+# 🧿 `safer`: A safer writer 🧿
 
 Avoid partial writes or corruption!
 
 `safer` wraps file streams, sockets, or a callable, and offers a drop-in
 replacement for regular old `open()`.
 
 ## Quick summary
@@ -93,16 +93,16 @@
             write_body(s)  # Exception is thrown here
             write_footer(s)
      except Exception:
         write_error(sock)  # Nothing has been written
 
 ### Example: `safer.open()` and json
 
-`safer.open()` is a a drop-in replacement for built-in `open()` except that when
-used as a context, it leaves the original file unchanged on failure.
+`safer.open()` is a a drop-in replacement for built-in `open()` except that
+when used as a context, it leaves the original file unchanged on failure.
 
 It's easy to write broken JSON if something within it doesn't serialize.
 
     with open(filename, 'w') as fp:
         json.dump(data, fp)
         # If an exception is raised, the file is empty or partly written
 
@@ -152,25 +152,30 @@
 import json
 import os
 import shutil
 import sys
 import tempfile
 import traceback
 
+# There's an edge case in #23 I can't yet fix, so I fail
+# deliberately
+BUG_MESSAGE = 'Sorry, safer.writer fails if temp_file (#23)'
+
 __all__ = 'writer', 'open', 'closer', 'dump', 'printer'
 
 
 def writer(
     stream: Union[Callable, None, IO, Path, str] = None,
     is_binary: Optional[bool] = None,
     close_on_exit: bool = False,
     temp_file: bool = False,
     chunk_size: int = 0x100000,
     delete_failures: bool = True,
     dry_run: Union[bool, Callable] = False,
+    enabled: bool = True,
 ) -> Union[Callable, IO]:
     """
     Write safely to file streams, sockets and callables.
 
     `safer.writer` yields an in-memory stream that you can write
     to, but which is only written to the original stream if the
     context finishes without raising an exception.
@@ -208,27 +213,41 @@
       delete_failures: If false, any temporary files created are not deleted
         if there is an exception.
 
       dry_run: If `dry_run` is truthy, the stream or file is left unchanged.
 
         If `dry_run` is also callable, the results of the stream are passed to
         `dry_run()` rather than being written to the stream.
+
+      enabled: If `enabled` is falsey, the stream is returned unchanged
     """
     if isinstance(stream, (str, Path)):
         mode = 'wb' if is_binary else 'w'
         return open(
-            stream, mode, delete_failures=delete_failures, dry_run=dry_run
+            stream, mode,
+            delete_failures=delete_failures, dry_run=dry_run, enabled=enabled
         )
 
     stream = stream or sys.stdout
+    if not enabled:
+        return stream
 
     if callable(dry_run):
         write, dry_run = dry_run, True
+
     elif dry_run:
         write = len
+
+    elif close_on_exit and hasattr(stream, 'write'):
+        if temp_file and BUG_MESSAGE:
+            raise NotImplementedError(BUG_MESSAGE)
+
+        def write(v):
+            with stream:
+                stream.write(v)
     else:
         write = getattr(stream, 'write', None)
 
     send = getattr(stream, 'send', None)
     mode = getattr(stream, 'mode', None)
 
     if dry_run:
@@ -290,14 +309,15 @@
     newline: Optional[str] = None,
     closefd: bool = True,
     opener: Optional[Callable] = None,
     make_parents: bool = False,
     delete_failures: bool = True,
     temp_file: bool = False,
     dry_run: bool = False,
+    enabled: bool = True,
 ) -> IO:
     """
     Args:
       make_parents: If true, create the parent directory of the file if needed
 
       delete_failures: If false, any temporary files created are not deleted
         if there is an exception.
@@ -308,14 +328,17 @@
           If `temp_file` is a string, use it as the name of the temporary
           file, otherwise select one in the same directory as the target
           file, or in the system tempfile for streams that aren't files.
 
       dry_run:
          If dry_run is True, the file is not written to at all
 
+      enabled:
+         If `enabled` is falsey, the file is opened as normal
+
     The remaining arguments are the same as for built-in `open()`.
 
     `safer.open() is a drop-in replacement for built-in`open()`. It returns a
     stream which only overwrites the original file when close() is called, and
     only if there was no failure.
 
     It works as follows:
@@ -358,21 +381,25 @@
     parent = os.path.dirname(os.path.abspath(name))
     if not os.path.exists(parent):
         if not make_parents:
             raise IOError('Directory does not exist')
         os.makedirs(parent)
 
     def simple_open():
+        print('simple_open', name, mode)
         return __builtins__['open'](name, mode, buffering, **kwargs)
 
     def simple_write(value):
+        print('simple_write', name, value)
         with simple_open() as fp:
             fp.write(value)
+        print('simple_write done')
+        print(__builtins__['open'](name).read())
 
-    if is_read:
+    if is_read or not enabled:
         return simple_open()
 
     if not temp_file:
         if '+' in mode:
             raise ValueError('+ mode requires a temp_file argument')
 
         if callable(dry_run):
@@ -632,15 +659,16 @@
         super().close(parent_close)
 
         if self.close_on_exit:
             closer = getattr(self.write, 'close', None)
             if closer:
                 closer(self.fp.safer_failed)
 
-    def _write(self, v):
+    def _write_on_success(self, v):
+        print('_StreamCloser._write_on_success', v, self.write)
         while True:
             written = self.write(v)
             v = (written is not None) and v[written:]
             if not v:
                 break
 
 
@@ -652,15 +680,15 @@
         assert fp == self.fp
 
     def close(self, parent_close=None):
         self.value = self.fp.getvalue()
         super().close(parent_close)
 
     def _success(self):
-        self._write(self.value)
+        self._write_on_success(self.value)
 
 
 class _FileStreamCloser(_StreamCloser, _FileCloser):
     def __init__(
         self,
         write,
         close_on_exit,
@@ -681,11 +709,11 @@
     def _success(self):
         mode = 'rb' if self.is_binary else 'r'
         with open(self.temp_file, mode) as fp:
             while True:
                 data = fp.read(self.chunk_size)
                 if not data:
                     break
-                self._write(data)
+                self._write_on_success(data)
 
     def _failure(self):
         _FileCloser._failure(self)
```

### Comparing `safer-4.5.0/setup.py` & `safer-4.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['safer']
 setup_kwargs = {
     'name': 'safer',
-    'version': '4.5.0',
+    'version': '4.6.0',
     'description': '🧿 A safer writer for files and streams 🧿',
-    'long_description': "Avoid partial writes or corruption!\n\n`safer` wraps file streams, sockets, or a callable, and offers a drop-in\nreplacement for regular old `open()`.\n\n## Quick summary\n\n### A tiny example\n\n    import safer\n\n    with safer.open(filename, 'w') as fp:\n        fp.write('one')\n        print('two', file=fp)\n        raise ValueError\n        # filename was not written.\n\n\n### How to use\n\nUse [pip](https://pypi.org/project/pip) to install `safer` from the command\nline: `pip install safer`.\n\nTested on Python 3.4 - 3.11.  An old Python 2.7 version\nis [here](https://github.com/rec/safer/tree/v2.0.5).\n\nSee the Medium article [here](https://medium.com/@TomSwirly/%EF%B8%8F-safer-a-safer-file-writer-%EF%B8%8F-5fe267dbe3f5)\n\n### The details\n\n`safer` helps prevent programmer error from corrupting files, socket\nconnections, or generalized streams by writing a whole file or nothing.\n\nIt does not prevent concurrent modification of files from other threads or\nprocesses: if you need atomic file writing, see\nhttps://pypi.org/project/atomicwrites/\n\nIt also has a useful `dry_run` setting to let you test your code without\nactually overwriting the target file.\n\n* `safer.writer()` wraps an existing writer, socket or stream and writes a\n  whole response or nothing\n\n* `safer.open()` is a drop-in replacement for built-in `open` that\n  writes a whole file or nothing\n\n* `safer.closer()` returns a stream like from `safer.write()` that also\n  closes the underlying stream or callable when it closes.\n\n* `safer.dump()` is like a safer `json.dump()` which can be used for any\n  serialization protocol, including Yaml and Toml, and also allows you to\n  write to file streams or any other callable.\n\n* `safer.printer()` is `safer.open()` except that it yields a\n  a function that prints to the stream.\n\nBy default, `safer` buffers the written data in memory in a `io.StringIO`\nor `io.BytesIO`.\n\nFor very large files, `safer.open()` has a `temp_file` argument which\nwrites the data to a temporary file on disk, which is moved over using\n`os.rename` if the operation completes successfully.  This functionality\ndoes not work on Windows.  (In fact, it's unclear if any of this works on\nWindows, but that certainly won't.  Windows developer solicted!)\n\n\n### Example: `safer.writer()`\n\n`safer.writer()` wraps an existing stream - a writer, socket, or callback -\nin a temporary stream which is only copied to the target stream at close(), and\nonly if no exception was raised.\n\nSuppose `sock = socket.socket(*args)`.\n\nThe old, dangerous way goes like this.\n\n    try:\n        write_header(sock)\n        write_body(sock)   # Exception is thrown here\n        write_footer(sock)\n     except Exception:\n        write_error(sock)  # Oops, the header was already written\n\nWith `safer` you write all or nothing:\n\n    try:\n        with safer.writer(sock) as s:\n            write_header(s)\n            write_body(s)  # Exception is thrown here\n            write_footer(s)\n     except Exception:\n        write_error(sock)  # Nothing has been written\n\n### Example: `safer.open()` and json\n\n`safer.open()` is a a drop-in replacement for built-in `open()` except that when\nused as a context, it leaves the original file unchanged on failure.\n\nIt's easy to write broken JSON if something within it doesn't serialize.\n\n    with open(filename, 'w') as fp:\n        json.dump(data, fp)\n        # If an exception is raised, the file is empty or partly written\n\n`safer` prevents this:\n\n    with safer.open(filename, 'w') as fp:\n        json.dump(data, fp)\n        # If an exception is raised, the file is unchanged.\n\n`safer.open(filename)` returns a file stream `fp` like `open(filename)`\nwould, except that `fp` writes to memory stream or a temporary file in the\nsame directory.\n\nIf `fp` is used as a context manager and an exception is raised, then the\nproperty `fp.safer_failed` on the stream is automatically set to `True`.\n\nAnd when `fp.close()` is called, the cached data is stored in `filename` -\n*unless* `fp.safer_failed` is true.\n\n### Example: `safer.printer()`\n\n`safer.printer()` is similar to `safer.open()` except it yields a function\nthat prints to the open file - it's very convenient for printing text.\n\nLike `safer.open()`, if an exception is raised within its context manager,\nthe original file is left unchanged.\n\nBefore.\n\n    with open(file, 'w') as fp:\n        for item in items:\n            print(item, file=fp)\n        # Prints lines until the first exception\n\nWith `safer`\n\n    with safer.printer(file) as print:\n        for item in items:\n            print(item)\n        # Either the whole file is written, or nothing\n\n\n### [API Documentation](https://rec.github.io/safer#safer--api-documentation)\n",
+    'long_description': "# 🧿 `safer`: A safer writer 🧿\n\nAvoid partial writes or corruption!\n\n`safer` wraps file streams, sockets, or a callable, and offers a drop-in\nreplacement for regular old `open()`.\n\n## Quick summary\n\n### A tiny example\n\n    import safer\n\n    with safer.open(filename, 'w') as fp:\n        fp.write('one')\n        print('two', file=fp)\n        raise ValueError\n        # filename was not written.\n\n\n### How to use\n\nUse [pip](https://pypi.org/project/pip) to install `safer` from the command\nline: `pip install safer`.\n\nTested on Python 3.4 - 3.11.  An old Python 2.7 version\nis [here](https://github.com/rec/safer/tree/v2.0.5).\n\nSee the Medium article [here](https://medium.com/@TomSwirly/%EF%B8%8F-safer-a-safer-file-writer-%EF%B8%8F-5fe267dbe3f5)\n\n### The details\n\n`safer` helps prevent programmer error from corrupting files, socket\nconnections, or generalized streams by writing a whole file or nothing.\n\nIt does not prevent concurrent modification of files from other threads or\nprocesses: if you need atomic file writing, see\nhttps://pypi.org/project/atomicwrites/\n\nIt also has a useful `dry_run` setting to let you test your code without\nactually overwriting the target file.\n\n* `safer.writer()` wraps an existing writer, socket or stream and writes a\n  whole response or nothing\n\n* `safer.open()` is a drop-in replacement for built-in `open` that\n  writes a whole file or nothing\n\n* `safer.closer()` returns a stream like from `safer.write()` that also\n  closes the underlying stream or callable when it closes.\n\n* `safer.dump()` is like a safer `json.dump()` which can be used for any\n  serialization protocol, including Yaml and Toml, and also allows you to\n  write to file streams or any other callable.\n\n* `safer.printer()` is `safer.open()` except that it yields a\n  a function that prints to the stream.\n\nBy default, `safer` buffers the written data in memory in a `io.StringIO`\nor `io.BytesIO`.\n\nFor very large files, `safer.open()` has a `temp_file` argument which\nwrites the data to a temporary file on disk, which is moved over using\n`os.rename` if the operation completes successfully.  This functionality\ndoes not work on Windows.  (In fact, it's unclear if any of this works on\nWindows, but that certainly won't.  Windows developer solicted!)\n\n\n### Example: `safer.writer()`\n\n`safer.writer()` wraps an existing stream - a writer, socket, or callback -\nin a temporary stream which is only copied to the target stream at close(), and\nonly if no exception was raised.\n\nSuppose `sock = socket.socket(*args)`.\n\nThe old, dangerous way goes like this.\n\n    try:\n        write_header(sock)\n        write_body(sock)   # Exception is thrown here\n        write_footer(sock)\n     except Exception:\n        write_error(sock)  # Oops, the header was already written\n\nWith `safer` you write all or nothing:\n\n    try:\n        with safer.writer(sock) as s:\n            write_header(s)\n            write_body(s)  # Exception is thrown here\n            write_footer(s)\n     except Exception:\n        write_error(sock)  # Nothing has been written\n\n### Example: `safer.open()` and json\n\n`safer.open()` is a a drop-in replacement for built-in `open()` except that\nwhen used as a context, it leaves the original file unchanged on failure.\n\nIt's easy to write broken JSON if something within it doesn't serialize.\n\n    with open(filename, 'w') as fp:\n        json.dump(data, fp)\n        # If an exception is raised, the file is empty or partly written\n\n`safer` prevents this:\n\n    with safer.open(filename, 'w') as fp:\n        json.dump(data, fp)\n        # If an exception is raised, the file is unchanged.\n\n`safer.open(filename)` returns a file stream `fp` like `open(filename)`\nwould, except that `fp` writes to memory stream or a temporary file in the\nsame directory.\n\nIf `fp` is used as a context manager and an exception is raised, then the\nproperty `fp.safer_failed` on the stream is automatically set to `True`.\n\nAnd when `fp.close()` is called, the cached data is stored in `filename` -\n*unless* `fp.safer_failed` is true.\n\n### Example: `safer.printer()`\n\n`safer.printer()` is similar to `safer.open()` except it yields a function\nthat prints to the open file - it's very convenient for printing text.\n\nLike `safer.open()`, if an exception is raised within its context manager,\nthe original file is left unchanged.\n\nBefore.\n\n    with open(file, 'w') as fp:\n        for item in items:\n            print(item, file=fp)\n        # Prints lines until the first exception\n\nWith `safer`\n\n    with safer.printer(file) as print:\n        for item in items:\n            print(item)\n        # Either the whole file is written, or nothing\n\n\n### [API Documentation](https://rec.github.io/safer#safer--api-documentation)\n",
     'author': 'Tom Ritchford',
     'author_email': 'tom@swirly.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'py_modules': modules,
     'python_requires': '>=3.7,<4.0',
```

### Comparing `safer-4.5.0/PKG-INFO` & `safer-4.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: safer
-Version: 4.5.0
+Version: 4.6.0
 Summary: 🧿 A safer writer for files and streams 🧿
 License: MIT
 Author: Tom Ritchford
 Author-email: tom@swirly.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
+# 🧿 `safer`: A safer writer 🧿
+
 Avoid partial writes or corruption!
 
 `safer` wraps file streams, sockets, or a callable, and offers a drop-in
 replacement for regular old `open()`.
 
 ## Quick summary
 
@@ -106,16 +108,16 @@
             write_body(s)  # Exception is thrown here
             write_footer(s)
      except Exception:
         write_error(sock)  # Nothing has been written
 
 ### Example: `safer.open()` and json
 
-`safer.open()` is a a drop-in replacement for built-in `open()` except that when
-used as a context, it leaves the original file unchanged on failure.
+`safer.open()` is a a drop-in replacement for built-in `open()` except that
+when used as a context, it leaves the original file unchanged on failure.
 
 It's easy to write broken JSON if something within it doesn't serialize.
 
     with open(filename, 'w') as fp:
         json.dump(data, fp)
         # If an exception is raised, the file is empty or partly written
```

