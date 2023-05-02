# Comparing `tmp/expiringsqlitedict-5.0.1.tar.gz` & `tmp/expiringsqlitedict-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expiringsqlitedict-5.0.1.tar", last modified: Mon May  1 15:44:14 2023, max compression
+gzip compressed data, was "expiringsqlitedict-5.0.2.tar", last modified: Tue May  2 21:06:41 2023, max compression
```

## Comparing `expiringsqlitedict-5.0.1.tar` & `expiringsqlitedict-5.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-5.0.1/.gitignore
--rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-5.0.1/.travis.yml
--rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-5.0.1/CHANGELOG.txt
--rw-r--r--   0        0        0    11401 2021-06-14 18:49:24.994306 expiringsqlitedict-5.0.1/LICENSE.apache
--rw-r--r--   0        0        0      193 2021-06-14 18:49:22.590300 expiringsqlitedict-5.0.1/LICENSE.rst
--rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-5.0.1/Makefile
--rw-r--r--   0        0        0     4042 2023-04-29 13:08:40.273027 expiringsqlitedict-5.0.1/README.rst
--rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-5.0.1/bench.py
--rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-5.0.1/docs/Makefile
--rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-5.0.1/docs/conf.py
--rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-5.0.1/docs/expiringsqlitedict.rst
--rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-5.0.1/docs/index.rst
--rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-5.0.1/docs/make.bat
--rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-5.0.1/docs/requirements.txt
--rw-r--r--   0        0        0      972 2023-05-01 15:38:14.470875 expiringsqlitedict-5.0.1/pyproject.toml
--rwxr-xr-x   0        0        0      920 2023-05-01 15:43:23.632313 expiringsqlitedict-5.0.1/run_all_tests.sh
--rwxr-xr-x   0        0        0    10878 2023-05-01 15:38:14.470875 expiringsqlitedict-5.0.1/src/expiringsqlitedict/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-5.0.1/src/expiringsqlitedict/py.typed
--rwxr-xr-x   0        0        0     7186 2023-04-29 13:11:14.086617 expiringsqlitedict-5.0.1/test.py
--rw-r--r--   0        0        0     4900 1970-01-01 00:00:00.000000 expiringsqlitedict-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-5.0.2/.gitignore
+-rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-5.0.2/.travis.yml
+-rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-5.0.2/CHANGELOG.txt
+-rw-r--r--   0        0        0    11401 2021-06-14 18:49:24.994306 expiringsqlitedict-5.0.2/LICENSE.apache
+-rw-r--r--   0        0        0      193 2021-06-14 18:49:22.590300 expiringsqlitedict-5.0.2/LICENSE.rst
+-rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-5.0.2/Makefile
+-rw-r--r--   0        0        0     4042 2023-04-29 13:08:40.273027 expiringsqlitedict-5.0.2/README.rst
+-rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-5.0.2/bench.py
+-rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-5.0.2/docs/Makefile
+-rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-5.0.2/docs/conf.py
+-rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-5.0.2/docs/expiringsqlitedict.rst
+-rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-5.0.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-5.0.2/docs/make.bat
+-rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-5.0.2/docs/requirements.txt
+-rw-r--r--   0        0        0     1030 2023-05-02 21:02:47.090474 expiringsqlitedict-5.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0     1327 2023-05-02 19:49:18.673775 expiringsqlitedict-5.0.2/run_all_tests.sh
+-rwxr-xr-x   0        0        0    11820 2023-05-02 21:01:50.906531 expiringsqlitedict-5.0.2/src/expiringsqlitedict/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-5.0.2/src/expiringsqlitedict/py.typed
+-rwxr-xr-x   0        0        0     9712 2023-05-02 21:06:03.726774 expiringsqlitedict-5.0.2/test.py
+-rw-r--r--   0        0        0     4961 1970-01-01 00:00:00.000000 expiringsqlitedict-5.0.2/PKG-INFO
```

### Comparing `expiringsqlitedict-5.0.1/CHANGELOG.txt` & `expiringsqlitedict-5.0.2/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.1/LICENSE.apache` & `expiringsqlitedict-5.0.2/LICENSE.apache`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.1/README.rst` & `expiringsqlitedict-5.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.1/bench.py` & `expiringsqlitedict-5.0.2/bench.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.1/docs/Makefile` & `expiringsqlitedict-5.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.1/docs/conf.py` & `expiringsqlitedict-5.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.1/docs/index.rst` & `expiringsqlitedict-5.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.1/docs/make.bat` & `expiringsqlitedict-5.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.1/pyproject.toml` & `expiringsqlitedict-5.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'expiringsqlitedict'
 description = 'Persistent compressed expiring dict in Python, backed up by sqlite3 and json'
-version = '5.0.1'
+version = '5.0.2'
 readme = 'README.rst'
 requires-python = '>= 3.6, < 4'
 license = { text = 'Apache 2.0' }
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -23,7 +23,12 @@
 [project.urls]
 repository  = 'https://github.com/absperf/expiringsqlitedict'
 documentation = 'https://expiringsqlitedict.readthedocs.io/'
 
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4", 'wheel']
+
+[project.optional-dependencies]
+test = [
+    'orjson',
+]
```

### Comparing `expiringsqlitedict-5.0.1/src/expiringsqlitedict/__init__.py` & `expiringsqlitedict-5.0.2/src/expiringsqlitedict/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,25 +10,36 @@
 #  * http://code.activestate.com/recipes/576638-draft-for-an-sqlite3-based-dbm/
 #  * http://code.activestate.com/recipes/526618/
 
 
 import json
 import sqlite3
 from collections.abc import MutableMapping
-from contextlib import closing
+from contextlib import ExitStack, closing, contextmanager
 from datetime import timedelta
-from typing import Any, Iterator, Optional, Tuple, Type
+from types import TracebackType
+from typing import Any, Generator, Iterator, Optional, Tuple, Type
 from weakref import finalize
 
-def _close(db):
-    '''Optimize and close the database.
-    '''
-    with closing(db) as d, closing(d.cursor()) as cursor:
-        cursor.execute('PRAGMA analysis_limit=8192')
-        cursor.execute('PRAGMA optimize')
+@contextmanager
+def _transaction(
+    connection: sqlite3.Connection,
+    begin: str,
+) -> Generator[None, None, None]:
+    with closing(connection.cursor()) as cursor:
+        cursor.execute(begin)
+    try:
+        yield
+    except:
+        with closing(connection.cursor()) as cursor:
+            cursor.execute('ROLLBACK')
+        raise
+    else:
+        with closing(connection.cursor()) as cursor:
+            cursor.execute('COMMIT')
 
 class SqliteDict:
     """
     Set up the sqlite dictionary manager.
 
     This needs to be used as a context manager.  It will not operate at all
     otherwise. args and kwargs are directly passed to sqlite3.connect.  Use
@@ -38,14 +49,15 @@
     be re-opened after it has closed.
     """
 
     __slots__ = (
         '_args',
         '_kwargs',
         '_connection',
+        '_exit_stack',
         '_serializer',
         '_lifespan',
         '_begin',
         '_table',
         '__weakref__'
     )
 
@@ -75,45 +87,55 @@
         return self._lifespan
 
     @lifespan.setter
     def lifespan(self, value: timedelta) -> None:
         self._lifespan = value
 
     def __enter__(self) -> 'Connection':
-        self._connection = sqlite3.connect(
-            *self._args,
-            isolation_level=None,
-            **self._kwargs,
-        )
-        with closing(self._connection.cursor()) as cursor:
-            cursor.execute('PRAGMA journal_mode=WAL')
-            cursor.execute('PRAGMA synchronous=NORMAL')
-            cursor.execute(self._begin)
-
-        return Connection(
-            self._connection,
-            serializer=self._serializer,
-            lifespan=self._lifespan,
-            table=self._table,
-        )
+        with ExitStack() as exit_stack:
+            self._connection = exit_stack.enter_context(closing(sqlite3.connect(
+                *self._args,
+                isolation_level=None,
+                **self._kwargs,
+            )))
+
+            with closing(self._connection.cursor()) as cursor:
+                cursor.execute('PRAGMA journal_mode=WAL')
+                cursor.execute('PRAGMA synchronous=NORMAL')
+
+            def optimize() -> None:
+                with closing(self._connection.cursor()) as cursor:
+                    cursor.execute('PRAGMA analysis_limit=8192')
+                    cursor.execute('PRAGMA optimize')
+
+            exit_stack.callback(optimize)
+
+            exit_stack.enter_context(_transaction(self._connection, self._begin))
+
+            connection = Connection(
+                self._connection,
+                serializer=self._serializer,
+                lifespan=self._lifespan,
+                table=self._table,
+            )
+            self._exit_stack = exit_stack.pop_all()
+            return connection
+
+        assert False, 'UNREACHABLE'
 
     def __exit__(
         self,
         type: Optional[Type[BaseException]],
         value: Optional[BaseException],
-        traceback: Optional[BaseException],
-    ) -> None:
-        with closing(self._connection) as db, closing(db.cursor()) as cursor:
-            if (type and value and traceback) is None:
-                cursor.execute('COMMIT')
-            else:
-                cursor.execute('ROLLBACK')
-
-            cursor.execute('PRAGMA analysis_limit=8192')
-            cursor.execute('PRAGMA optimize')
+        traceback: Optional[TracebackType],
+    ) -> bool:
+        try:
+            return self._exit_stack.__exit__(type, value, traceback)
+        finally:
+            del self._connection, self._exit_stack
 
 def SimpleSqliteDict(
     *args,
     serializer: Any = json,
     lifespan: timedelta = timedelta(weeks=1),
     isolation_level: Optional[str] = None,
     table: str = 'expiringsqlitedict',
@@ -134,15 +156,22 @@
     connection = Connection(
         db,
         serializer=serializer,
         lifespan=lifespan,
         table=table,
     )
 
-    finalize(connection, _close, db)
+    def _close():
+        '''Optimize and close the database.
+        '''
+        with closing(db) as d, closing(d.cursor()) as cursor:
+            cursor.execute('PRAGMA analysis_limit=8192')
+            cursor.execute('PRAGMA optimize')
+
+    finalize(connection, _close)
 
     return connection
 
 _trailers = []
 if sqlite3.sqlite_version_info >= (3, 8, 2):
     _trailers.append('WITHOUT ROWID')
 
@@ -314,18 +343,18 @@
                 (key, self._lifespan, self._serializer.dumps(value)),
                 )
 
     def __delitem__(self, key: str) -> None:
         '''Delete an item from the table.
         '''
 
-        if key not in self:
-            raise KeyError(key)
         with closing(self._connection.cursor()) as cursor:
             cursor.execute(f'DELETE FROM "{self._safe_table}" WHERE key=?', (key,))
+            if cursor.rowcount != 1:
+                raise KeyError(key)
 
     def clear(self) -> None:
         '''Delete all items from the table.
         '''
 
         with closing(self._connection.cursor()) as cursor:
             cursor.execute(f'DELETE FROM "{self._safe_table}"')
```

### Comparing `expiringsqlitedict-5.0.1/PKG-INFO` & `expiringsqlitedict-5.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: expiringsqlitedict
-Version: 5.0.1
+Version: 5.0.2
 Summary: Persistent compressed expiring dict in Python, backed up by sqlite3 and json
 Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Requires-Python: >= 3.6, < 4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: orjson ; extra == "test"
 Project-URL: documentation, https://expiringsqlitedict.readthedocs.io/
 Project-URL: repository, https://github.com/absperf/expiringsqlitedict
+Provides-Extra: test
 
 expiringsqlitedict -- expiring file-backed ``dict``
 ===================================================
 
 .. _Downloads: https://pypi.python.org/pypi/expiringsqlitedict
 .. _License: https://pypi.python.org/pypi/expiringsqlitedict
```

