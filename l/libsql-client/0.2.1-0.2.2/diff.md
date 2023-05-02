# Comparing `tmp/libsql-client-0.2.1.tar.gz` & `tmp/libsql-client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsql-client-0.2.1.tar", max compression
+gzip compressed data, was "libsql-client-0.2.2.tar", max compression
```

## Comparing `libsql-client-0.2.1.tar` & `libsql-client-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-02-27 08:58:08.764134 libsql-client-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     2912 2023-04-27 07:46:00.306317 libsql-client-0.2.1/README.md
--rw-r--r--   0        0        0      268 2023-04-19 10:43:28.755257 libsql-client-0.2.1/libsql_client/__init__.py
--rw-r--r--   0        0        0     3039 2023-04-17 12:00:30.657316 libsql-client-0.2.1/libsql_client/client.py
--rw-r--r--   0        0        0      993 2023-04-17 12:00:30.657316 libsql-client-0.2.1/libsql_client/config.py
--rw-r--r--   0        0        0      801 2023-04-17 12:00:30.657316 libsql-client-0.2.1/libsql_client/create_client.py
--rw-r--r--   0        0        0       85 2023-04-17 12:00:30.657316 libsql-client-0.2.1/libsql_client/hrana/__init__.py
--rw-r--r--   0        0        0     4254 2023-04-28 14:43:03.375368 libsql-client-0.2.1/libsql_client/hrana/client.py
--rw-r--r--   0        0        0    12135 2023-04-28 14:43:03.379368 libsql-client-0.2.1/libsql_client/hrana/conn.py
--rw-r--r--   0        0        0     4816 2023-04-20 09:18:36.654076 libsql-client-0.2.1/libsql_client/hrana/convert.py
--rw-r--r--   0        0        0     1610 2023-04-17 12:00:30.661316 libsql-client-0.2.1/libsql_client/hrana/id_alloc.py
--rw-r--r--   0        0        0     3974 2023-04-17 12:00:30.661316 libsql-client-0.2.1/libsql_client/hrana/proto.py
--rw-r--r--   0        0        0     3441 2023-04-17 12:00:30.661316 libsql-client-0.2.1/libsql_client/http.py
--rw-r--r--   0        0        0     3071 2023-04-28 14:52:18.017515 libsql-client-0.2.1/libsql_client/result.py
--rw-r--r--   0        0        0     4896 2023-04-20 09:19:13.406247 libsql-client-0.2.1/libsql_client/sqlite3.py
--rw-r--r--   0        0        0     6347 2023-04-19 11:59:20.956756 libsql-client-0.2.1/libsql_client/sync.py
--rw-r--r--   0        0        0      960 2023-04-28 15:10:54.208794 libsql-client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3726 1970-01-01 00:00:00.000000 libsql-client-0.2.1/setup.py
--rw-r--r--   0        0        0     3757 1970-01-01 00:00:00.000000 libsql-client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-27 08:58:08.764134 libsql-client-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0     2912 2023-04-27 07:46:00.306317 libsql-client-0.2.2/README.md
+-rw-r--r--   0        0        0      268 2023-04-19 10:43:28.755257 libsql-client-0.2.2/libsql_client/__init__.py
+-rw-r--r--   0        0        0     3039 2023-04-17 12:00:30.657316 libsql-client-0.2.2/libsql_client/client.py
+-rw-r--r--   0        0        0      993 2023-04-17 12:00:30.657316 libsql-client-0.2.2/libsql_client/config.py
+-rw-r--r--   0        0        0      801 2023-04-17 12:00:30.657316 libsql-client-0.2.2/libsql_client/create_client.py
+-rw-r--r--   0        0        0       85 2023-04-17 12:00:30.657316 libsql-client-0.2.2/libsql_client/hrana/__init__.py
+-rw-r--r--   0        0        0     4254 2023-04-28 14:43:03.375368 libsql-client-0.2.2/libsql_client/hrana/client.py
+-rw-r--r--   0        0        0    12135 2023-04-28 14:43:03.379368 libsql-client-0.2.2/libsql_client/hrana/conn.py
+-rw-r--r--   0        0        0     4816 2023-04-20 09:18:36.654076 libsql-client-0.2.2/libsql_client/hrana/convert.py
+-rw-r--r--   0        0        0     1610 2023-04-17 12:00:30.661316 libsql-client-0.2.2/libsql_client/hrana/id_alloc.py
+-rw-r--r--   0        0        0     3974 2023-04-17 12:00:30.661316 libsql-client-0.2.2/libsql_client/hrana/proto.py
+-rw-r--r--   0        0        0     3441 2023-04-17 12:00:30.661316 libsql-client-0.2.2/libsql_client/http.py
+-rw-r--r--   0        0        0     3071 2023-04-28 14:52:18.017515 libsql-client-0.2.2/libsql_client/result.py
+-rw-r--r--   0        0        0     4896 2023-04-20 09:19:13.406247 libsql-client-0.2.2/libsql_client/sqlite3.py
+-rw-r--r--   0        0        0     7175 2023-05-02 07:53:42.957852 libsql-client-0.2.2/libsql_client/sync.py
+-rw-r--r--   0        0        0      960 2023-05-02 08:27:39.682207 libsql-client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3726 1970-01-01 00:00:00.000000 libsql-client-0.2.2/setup.py
+-rw-r--r--   0        0        0     3757 1970-01-01 00:00:00.000000 libsql-client-0.2.2/PKG-INFO
```

### Comparing `libsql-client-0.2.1/LICENSE.md` & `libsql-client-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.1/README.md` & `libsql-client-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.1/libsql_client/client.py` & `libsql-client-0.2.2/libsql_client/client.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.1/libsql_client/config.py` & `libsql-client-0.2.2/libsql_client/config.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.1/libsql_client/create_client.py` & `libsql-client-0.2.2/libsql_client/create_client.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.1/libsql_client/hrana/client.py` & `libsql-client-0.2.2/libsql_client/hrana/client.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.1/libsql_client/hrana/conn.py` & `libsql-client-0.2.2/libsql_client/hrana/conn.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.1/libsql_client/hrana/convert.py` & `libsql-client-0.2.2/libsql_client/hrana/convert.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.1/libsql_client/hrana/id_alloc.py` & `libsql-client-0.2.2/libsql_client/hrana/id_alloc.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.1/libsql_client/hrana/proto.py` & `libsql-client-0.2.2/libsql_client/hrana/proto.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.1/libsql_client/http.py` & `libsql-client-0.2.2/libsql_client/http.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.1/libsql_client/result.py` & `libsql-client-0.2.2/libsql_client/result.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.1/libsql_client/sqlite3.py` & `libsql-client-0.2.2/libsql_client/sqlite3.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.1/libsql_client/sync.py` & `libsql-client-0.2.2/libsql_client/sync.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,16 +36,15 @@
         return self._executor.submit_coro(self._client.batch(stmts))
 
     def transaction(self) -> TransactionSync:
         transaction: Transaction = self._executor.submit_func(self._client.transaction)
         return TransactionSync(self._executor, transaction)
 
     def close(self) -> None:
-        self._executor.submit_coro(self._client.close())
-        self._executor.close()
+        self._executor.close_with_coro(self._client.close)
 
     @property
     def closed(self) -> bool:
         return self._executor.is_closed()
 
     def __enter__(self) -> ClientSync:
         return self
@@ -67,19 +66,19 @@
     def rollback(self) -> None:
         return self._executor.submit_coro(self._transaction.rollback())
 
     def commit(self) -> None:
         return self._executor.submit_coro(self._transaction.commit())
 
     def close(self) -> None:
-        self._executor.submit_func(self._transaction.close)
+        self._executor.submit_func_unless_closed(self._transaction.close, lambda: None)
 
     @property
     def closed(self) -> bool:
-        return self._executor.submit_func(lambda: self._transaction.closed)
+        return self._executor.submit_func_unless_closed(lambda: self._transaction.closed, lambda: True)
 
     def __enter__(self) -> TransactionSync:
         return self
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         self.close()
 
@@ -125,15 +124,15 @@
             except Exception as e:
                 item.future.set_exception(e)
 
         with self._lock:
             self._closed = True
             for item in self._queue:
                 if item is not None:
-                    item.future.set_exception(LibsqlError("Client was closed", "CLIENT_CLOSED"))
+                    item.future.set_exception(LibsqlError("Client is closed", "CLIENT_CLOSED"))
             self._queue.clear()
 
     async def _dequeue_item(self) -> Optional[_QueueItem]:
         while True:
             with self._lock:
                 if len(self._queue) > 0:
                     return self._queue.popleft()
@@ -148,31 +147,50 @@
         if waker is not None:
             waker_: asyncio.Future[None] = waker
             def resolve_waker() -> None:
                 waker_.set_result(None)
             self._loop.call_soon_threadsafe(resolve_waker)
 
     def submit_coro(self, coro: Coroutine[Any, Any, T]) -> T:
-        fut: concurrent.futures.Future = concurrent.futures.Future()
         with self._lock:
             if self._closed:
                 raise LibsqlError("Client is closed", "CLIENT_CLOSED")
+            fut: concurrent.futures.Future = concurrent.futures.Future()
             self._enqueue_item_with_lock(_QueueItem(coro, fut))
         return fut.result()
 
     def submit_func(self, func: Callable[[], T]) -> T:
         async def coro() -> T:
             return func()
         return self.submit_coro(coro())
 
-    def close(self) -> None:
+    def submit_func_unless_closed(self, on_open: Callable[[], T], on_closed: Callable[[], T]) -> T:
+        async def on_open_coro() -> T:
+            return on_open()
+        with self._lock:
+            if self._closed:
+                return on_closed()
+            fut: concurrent.futures.Future = concurrent.futures.Future()
+            self._enqueue_item_with_lock(_QueueItem(on_open_coro(), fut))
+        return fut.result()
+
+    def close_with_coro(self, coro_func: Callable[[], Coroutine[Any, Any, None]]) -> None:
         with self._lock:
-            if not self._closed:
-                self._enqueue_item_with_lock(None)
+            if self._closed:
+                return
+            fut: concurrent.futures.Future = concurrent.futures.Future()
+            self._enqueue_item_with_lock(_QueueItem(coro_func(), fut))
+            self._enqueue_item_with_lock(None)
         self._thread.join()
+        fut.result()
+
+    def close(self) -> None:
+        async def noop() -> None:
+            return None
+        self.close_with_coro(noop)
 
     def is_closed(self) -> bool:
         with self._lock:
             return self._closed
 
 # this is copied from CPython's Lib/asyncio/runners.py
 def _cancel_all_tasks(loop: asyncio.AbstractEventLoop) -> None:
```

### Comparing `libsql-client-0.2.1/pyproject.toml` & `libsql-client-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libsql-client"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     "Jan Špaček <honza@chiselstrike.com>",
     "ChiselStrike",
 ]
 description = "Python SDK for libSQL"
 homepage = "https://github.com/libsql/libsql-client-py"
 repository = "https://github.com/libsql/libsql-client-py"
```

### Comparing `libsql-client-0.2.1/setup.py` & `libsql-client-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.0,<4.0', 'typing-extensions>=4.5,<5.0']
 
 setup_kwargs = {
     'name': 'libsql-client',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Python SDK for libSQL',
     'long_description': '# Python SDK for libSQL\n\n**[API reference][reference] | [Github][github] | [PyPI][pypi]**\n\n[reference]: https://libsql.org/libsql-client-py/reference.html\n[github]: https://github.com/libsql/libsql-client-py\n[pypi]: https://pypi.org/project/libsql-client/\n\nThis is the source repository of the Python SDK for libSQL. You can either connect to a local SQLite database or to a remote libSQL server ([sqld][sqld]).\n\n[sqld]: https://github.com/libsql/sqld\n\n## Installation\n\n```\npip install libsql-client\n```\n\n## Getting Started\n\nConnecting to a local SQLite database:\n\n```python\nimport asyncio\nimport libsql_client\n\nasync def main():\n    url = "file:local.db"\n    async with libsql_client.create_client(url) as client:\n        result_set = await client.execute("SELECT * from users")\n        print(len(result_set.rows), "rows")\n        for row in result_set.rows:\n            print(row)\n\nasyncio.run(main())\n```\n\nTo connect to a remote libSQL server ([sqld][sqld]), just change the URL:\n\n```python\nurl = "ws://localhost:8080"\n```\n\n## Supported URLs\n\nThe client can connect to the database using different methods depending on the scheme (protocol) of the passed URL:\n\n* `file:` connects to a local SQLite database (using the builtin `sqlite3` package)\n  * `file:/absolute/path` or `file:///absolute/path` is an absolute path on local filesystem\n  * `file:relative/path` is a relative path on local filesystem\n  * (`file://path` is not a valid URL)\n* `ws:` or `wss:` connect to sqld using WebSockets (the Hrana protocol).\n* `http:` or `https:` connect to sqld using HTTP. The `transaction()` API is not available in this case.\n* `libsql:` is equivalent to `wss:`.\n\n## Synchronous API\n\nThis package also provides a synchronous version of the client, which can be created by calling `create_client_sync()`. It supports the same methods as the default `asyncio` client, except that they block the calling thread:\n\n```python\nimport libsql_client\n\nurl = "file:local.db"\nwith libsql_client.create_client_sync(url) as client:\n    result_set = client.execute("SELECT * from users")\n    print(len(result_set.rows), "rows")\n    for row in result_set.rows:\n        print(row)\n```\n\nThe synchronous client is just a thin wrapper around the asynchronous client, but it runs the event loop in a background thread.\n\n## Contributing to this package\n\nFirst, please install Python and [Poetry][poetry]. To install all dependencies for local development to a\nvirtual environment, run:\n\n[poetry]: https://python-poetry.org/\n\n```\npoetry install --with dev\n```\n\nTo run the tests, use:\n\n```\npoetry run pytest\n```\n\nTo check types with MyPy, use:\n\n```\npoetry run mypy\n```\n\n## License\n\nThis project is licensed under the MIT license.\n\n### Contribution\n\nUnless you explicitly state otherwise, any contribution intentionally submitted for inclusion in `libsql-client` by you, shall be licensed as MIT, without any additional terms or conditions.\n',
     'author': 'Jan Špaček',
     'author_email': 'honza@chiselstrike.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/libsql/libsql-client-py',
```

### Comparing `libsql-client-0.2.1/PKG-INFO` & `libsql-client-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsql-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python SDK for libSQL
 Home-page: https://github.com/libsql/libsql-client-py
 License: MIT
 Author: Jan Špaček
 Author-email: honza@chiselstrike.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

