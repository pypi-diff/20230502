# Comparing `tmp/databasez-0.2.2.tar.gz` & `tmp/databasez-0.3.0.tar.gz`

## Comparing `databasez-0.2.2.tar` & `databasez-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/__init__.py
--rw-r--r--   0        0        0    21730 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/core.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/importer.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/interfaces.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/py.typed
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/testclient.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/__init__.py
--rw-r--r--   0        0        0    11259 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/aiopg.py
--rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/asyncmy.py
--rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/mssql.py
--rw-r--r--   0        0        0    10997 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/mysql.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/postgres.py
--rw-r--r--   0        0        0     9414 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/sqlite.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/common/__init__.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/common/records.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/compilers/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/compilers/psycopg.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/dialects/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 databasez-0.2.2/databasez/backends/dialects/psycopg.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 databasez-0.2.2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 databasez-0.2.2/LICENSE.md
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 databasez-0.2.2/README.md
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 databasez-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 databasez-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/__init__.py
+-rw-r--r--   0        0        0    21730 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/core.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/importer.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/interfaces.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/py.typed
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/testclient.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/__init__.py
+-rw-r--r--   0        0        0    11179 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/aiopg.py
+-rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/asyncmy.py
+-rw-r--r--   0        0        0    11987 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/mssql.py
+-rw-r--r--   0        0        0    10917 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/mysql.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/postgres.py
+-rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/sqlite.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/common/__init__.py
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/common/records.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/compilers/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/compilers/psycopg.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/dialects/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/dialects/psycopg.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 databasez-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 databasez-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 databasez-0.3.0/README.md
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 databasez-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 databasez-0.3.0/PKG-INFO
```

### Comparing `databasez-0.2.2/databasez/core.py` & `databasez-0.3.0/databasez/core.py`

 * *Files identical despite different names*

### Comparing `databasez-0.2.2/databasez/importer.py` & `databasez-0.3.0/databasez/importer.py`

 * *Files identical despite different names*

### Comparing `databasez-0.2.2/databasez/interfaces.py` & `databasez-0.3.0/databasez/interfaces.py`

 * *Files identical despite different names*

### Comparing `databasez-0.2.2/databasez/testclient.py` & `databasez-0.3.0/databasez/testclient.py`

 * *Files identical despite different names*

### Comparing `databasez-0.2.2/databasez/backends/aiopg.py` & `databasez-0.3.0/databasez/backends/aiopg.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,17 +122,16 @@
         try:
             await cursor.execute(query_str, args)
             rows = await cursor.fetchall()
             metadata = CursorResultMetaData(context, cursor.description)
             rows = [
                 Row(
                     metadata,
-                    metadata._processors,
-                    metadata._keymap,
-                    Row._default_key_style,
+                    metadata._effective_processors,
+                    metadata._key_to_index,
                     row,
                 )
                 for row in rows
             ]
             return [Record(row, result_columns, dialect, column_maps) for row in rows]
         finally:
             cursor.close()
@@ -147,17 +146,16 @@
             await cursor.execute(query_str, args)
             row = await cursor.fetchone()
             if row is None:
                 return None
             metadata = CursorResultMetaData(context, cursor.description)
             row = Row(
                 metadata,
-                metadata._processors,
-                metadata._keymap,
-                Row._default_key_style,
+                metadata._effective_processors,
+                metadata._key_to_index,
                 row,
             )
             return Record(row, result_columns, dialect, column_maps)
         finally:
             cursor.close()
 
     async def execute(self, query: ClauseElement) -> typing.Any:
@@ -188,17 +186,16 @@
         cursor = await self._connection.cursor()
         try:
             await cursor.execute(query_str, args)
             metadata = CursorResultMetaData(context, cursor.description)
             async for row in cursor:
                 record = Row(
                     metadata,
-                    metadata._processors,
-                    metadata._keymap,
-                    Row._default_key_style,
+                    metadata._effective_processors,
+                    metadata._key_to_index,
                     row,
                 )
                 yield Record(record, result_columns, dialect, column_maps)
         finally:
             cursor.close()
 
     def transaction(self) -> TransactionBackend:
```

### Comparing `databasez-0.2.2/databasez/backends/asyncmy.py` & `databasez-0.3.0/databasez/backends/asyncmy.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,17 +112,16 @@
             try:
                 await cursor.execute(query_str, args)
                 rows = await cursor.fetchall()
                 metadata = CursorResultMetaData(context, cursor.description)
                 rows = [
                     Row(
                         metadata,
-                        metadata._processors,
-                        metadata._keymap,
-                        Row._default_key_style,
+                        metadata._effective_processors,
+                        metadata._key_to_index,
                         row,
                     )
                     for row in rows
                 ]
                 return [Record(row, result_columns, dialect, column_maps) for row in rows]
             finally:
                 await cursor.close()
@@ -137,17 +136,16 @@
                 await cursor.execute(query_str, args)
                 row = await cursor.fetchone()
                 if row is None:
                     return None
                 metadata = CursorResultMetaData(context, cursor.description)
                 row = Row(
                     metadata,
-                    metadata._processors,
-                    metadata._keymap,
-                    Row._default_key_style,
+                    metadata._effective_processors,
+                    metadata._key_to_index,
                     row,
                 )
                 return Record(row, result_columns, dialect, column_maps)
             finally:
                 await cursor.close()
 
     async def execute(self, query: ClauseElement) -> typing.Any:
@@ -180,17 +178,16 @@
         async with self._connection.cursor() as cursor:
             try:
                 await cursor.execute(query_str, args)
                 metadata = CursorResultMetaData(context, cursor.description)
                 async for row in cursor:
                     record = Row(
                         metadata,
-                        metadata._processors,
-                        metadata._keymap,
-                        Row._default_key_style,
+                        metadata._effective_processors,
+                        metadata._key_to_index,
                         row,
                     )
                     yield Record(record, result_columns, dialect, column_maps)
             finally:
                 await cursor.close()
 
     def transaction(self) -> TransactionBackend:
```

### Comparing `databasez-0.2.2/databasez/backends/mssql.py` & `databasez-0.3.0/databasez/backends/mssql.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,17 +136,16 @@
         try:
             await cursor.execute(query_str, args)
             rows = await cursor.fetchall()
             metadata = CursorResultMetaData(context, cursor.description)
             rows = [
                 Row(
                     metadata,
-                    metadata._processors,
-                    metadata._keymap,
-                    Row._default_key_style,
+                    metadata._effective_processors,
+                    metadata._key_to_index,
                     row,
                 )
                 for row in rows
             ]
             return [Record(row, result_columns, dialect, column_maps) for row in rows]
         finally:
             await cursor.close()
@@ -161,17 +160,16 @@
             await cursor.execute(query_str, args)
             row = await cursor.fetchone()
             if row is None:
                 return None
             metadata = CursorResultMetaData(context, cursor.description)
             row = Row(
                 metadata,
-                metadata._processors,
-                metadata._keymap,
-                Row._default_key_style,
+                metadata._effective_processors,
+                metadata._key_to_index,
                 row,
             )
             return Record(row, result_columns, dialect, column_maps)
         finally:
             await cursor.close()
 
     async def execute(self, query: ClauseElement) -> typing.Any:
@@ -206,17 +204,16 @@
         cursor = await self._connection.cursor()
         try:
             await cursor.execute(query_str, args)
             metadata = CursorResultMetaData(context, cursor.description)
             async for row in cursor:
                 record = Row(
                     metadata,
-                    metadata._processors,
-                    metadata._keymap,
-                    Row._default_key_style,
+                    metadata._effective_processors,
+                    metadata._key_to_index,
                     row,
                 )
                 yield Record(record, result_columns, dialect, column_maps)
         finally:
             await cursor.close()
 
     def transaction(self) -> TransactionBackend:
```

### Comparing `databasez-0.2.2/databasez/backends/mysql.py` & `databasez-0.3.0/databasez/backends/mysql.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,17 +111,16 @@
         try:
             await cursor.execute(query_str, args)
             rows = await cursor.fetchall()
             metadata = CursorResultMetaData(context, cursor.description)
             rows = [
                 Row(
                     metadata,
-                    metadata._processors,
-                    metadata._keymap,
-                    Row._default_key_style,
+                    metadata._effective_processors,
+                    metadata._key_to_index,
                     row,
                 )
                 for row in rows
             ]
             return [Record(row, result_columns, dialect, column_maps) for row in rows]
         finally:
             await cursor.close()
@@ -136,17 +135,16 @@
             await cursor.execute(query_str, args)
             row = await cursor.fetchone()
             if row is None:
                 return None
             metadata = CursorResultMetaData(context, cursor.description)
             row = Row(
                 metadata,
-                metadata._processors,
-                metadata._keymap,
-                Row._default_key_style,
+                metadata._effective_processors,
+                metadata._key_to_index,
                 row,
             )
             return Record(row, result_columns, dialect, column_maps)
         finally:
             await cursor.close()
 
     async def execute(self, query: ClauseElement) -> typing.Any:
@@ -179,17 +177,16 @@
         cursor = await self._connection.cursor()
         try:
             await cursor.execute(query_str, args)
             metadata = CursorResultMetaData(context, cursor.description)
             async for row in cursor:
                 record = Row(
                     metadata,
-                    metadata._processors,
-                    metadata._keymap,
-                    Row._default_key_style,
+                    metadata._effective_processors,
+                    metadata._key_to_index,
                     row,
                 )
                 yield Record(record, result_columns, dialect, column_maps)
         finally:
             await cursor.close()
 
     def transaction(self) -> TransactionBackend:
```

### Comparing `databasez-0.2.2/databasez/backends/postgres.py` & `databasez-0.3.0/databasez/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `databasez-0.2.2/databasez/backends/sqlite.py` & `databasez-0.3.0/databasez/backends/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,17 +81,16 @@
 
         async with self._connection.execute(query_str, args) as cursor:
             rows = await cursor.fetchall()
             metadata = CursorResultMetaData(context, cursor.description)
             rows = [
                 Row(
                     metadata,
-                    metadata._processors,
-                    metadata._keymap,
-                    Row._default_key_style,
+                    metadata._effective_processors,
+                    metadata._key_to_index,
                     row,
                 )
                 for row in rows
             ]
             return [Record(row, result_columns, dialect, column_maps) for row in rows]
 
     async def fetch_one(self, query: ClauseElement) -> typing.Optional[Record]:
@@ -103,17 +102,16 @@
         async with self._connection.execute(query_str, args) as cursor:
             row = await cursor.fetchone()
             if row is None:
                 return None
             metadata = CursorResultMetaData(context, cursor.description)
             row = Row(
                 metadata,
-                metadata._processors,
-                metadata._keymap,
-                Row._default_key_style,
+                metadata._effective_processors,
+                metadata._key_to_index,
                 row,
             )
             return Record(row, result_columns, dialect, column_maps)
 
     async def execute(self, query: ClauseElement) -> typing.Any:
         assert self._connection is not None, "Connection is not acquired"
         query_str, args, result_columns, context = self._compile(query)
@@ -135,17 +133,16 @@
         dialect = self._dialect
 
         async with self._connection.execute(query_str, args) as cursor:
             metadata = CursorResultMetaData(context, cursor.description)
             async for row in cursor:
                 record = Row(
                     metadata,
-                    metadata._processors,
-                    metadata._keymap,
-                    Row._default_key_style,
+                    metadata._effective_processors,
+                    metadata._key_to_index,
                     row,
                 )
                 yield Record(record, result_columns, dialect, column_maps)
 
     def transaction(self) -> TransactionBackend:
         return SQLiteTransaction(self)
```

### Comparing `databasez-0.2.2/databasez/backends/common/records.py` & `databasez-0.3.0/databasez/backends/common/records.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,14 +91,23 @@
 
 class Row(SQLRow):
     def __getitem__(self, key: typing.Any) -> typing.Any:
         """
         An instance of a Row in SQLAlchemy allows the access
         to the Row._fields as tuple and the Row._mapping for
         the values.
+
+        return RowMapping(
+            self._parent,
+            None,
+            self._keymap,
+            RowMapping._default_key_style,
+            self._data,
+            return RowMapping(self._parent, None, self._key_to_index, self._data)
+        )
         """
         if isinstance(key, int):
             field = self._fields[key]
             return self._mapping[field]
         return self._mapping[key]
 
     def keys(self):
```

### Comparing `databasez-0.2.2/databasez/backends/dialects/psycopg.py` & `databasez-0.3.0/databasez/backends/dialects/psycopg.py`

 * *Files identical despite different names*

### Comparing `databasez-0.2.2/LICENSE.md` & `databasez-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `databasez-0.2.2/README.md` & `databasez-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `databasez-0.2.2/pyproject.toml` & `databasez-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -33,31 +33,31 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
-dependencies = ["nest_asyncio>=1.5.6,<2.0.0", "sqlalchemy>=2.0.9,<2.1"]
+dependencies = ["nest_asyncio>=1.5.6,<2.0.0", "sqlalchemy>=2.0.12,<2.1"]
 keywords = [
     "mysql",
     "postgres",
     "sqlalchemy",
     "sqlite",
     "asyncio",
     "esmerald",
     "saffier",
 ]
 
 [project.urls]
-Homepage = "https://github.com/dymmond/databasez"
-Documentation = "https://databasez.dymmond.com/"
-Changelog = "https://databasez.dymmond.com/release-notes/"
+Homepage = "https://github.com/tarsil/databasez"
+Documentation = "https://databasez.tarsild/"
+Changelog = "https://databasez.tarsild.io/release-notes/"
 Funding = "https://github.com/sponsors/tarsil"
-Source = "https://github.com/dymmond/databasez"
+Source = "https://github.com/tarsil/databasez"
 
 [project.optional-dependencies]
 test = [
     "autoflake>=2.1.1,<3.0.0",
     "black>=23.3.0,<24.0.0",
     "esmerald>=1.1.0",
     "isort>=5.12.0,<6.0.0",
```

### Comparing `databasez-0.2.2/PKG-INFO` & `databasez-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: databasez
-Version: 0.2.2
+Version: 0.3.0
 Summary: Async database support for Python.
-Project-URL: Homepage, https://github.com/dymmond/databasez
-Project-URL: Documentation, https://databasez.dymmond.com/
-Project-URL: Changelog, https://databasez.dymmond.com/release-notes/
+Project-URL: Homepage, https://github.com/tarsil/databasez
+Project-URL: Documentation, https://databasez.tarsild/
+Project-URL: Changelog, https://databasez.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
-Project-URL: Source, https://github.com/dymmond/databasez
+Project-URL: Source, https://github.com/tarsil/databasez
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.md
 Keywords: asyncio,esmerald,mysql,postgres,saffier,sqlalchemy,sqlite
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AnyIO
@@ -33,15 +33,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: nest-asyncio<2.0.0,>=1.5.6
-Requires-Dist: sqlalchemy<2.1,>=2.0.9
+Requires-Dist: sqlalchemy<2.1,>=2.0.12
 Provides-Extra: aiomysql
 Requires-Dist: aiomysql; extra == 'aiomysql'
 Provides-Extra: aioodbc
 Requires-Dist: aioodbc; extra == 'aioodbc'
 Provides-Extra: aiopg
 Requires-Dist: aiopg; extra == 'aiopg'
 Provides-Extra: aiosqlite
```

