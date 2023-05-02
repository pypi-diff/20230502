# Comparing `tmp/questdb-connect-0.0.30.tar.gz` & `tmp/questdb-connect-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.30.tar", last modified: Tue May  2 10:43:42 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.31.tar", last modified: Tue May  2 10:55:59 2023, max compression
```

## Comparing `questdb-connect-0.0.30.tar` & `questdb-connect-0.0.31.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:43:42.587191 questdb-connect-0.0.30/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.30/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-02 10:43:42.587059 questdb-connect-0.0.30/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.30/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2519 2023-05-02 10:43:24.000000 questdb-connect-0.0.30/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-02 10:43:42.587223 questdb-connect-0.0.30/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:43:42.582392 questdb-connect-0.0.30/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:43:42.584639 questdb-connect-0.0.30/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-02 10:25:08.000000 questdb-connect-0.0.30/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11132 2023-05-02 10:41:38.000000 questdb-connect-0.0.30/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5665 2023-05-02 10:39:22.000000 questdb-connect-0.0.30/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10657 2023-05-02 10:25:13.000000 questdb-connect-0.0.30/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-05-01 20:15:41.000000 questdb-connect-0.0.30/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:43:42.585690 questdb-connect-0.0.30/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-02 10:43:42.000000 questdb-connect-0.0.30/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      555 2023-05-02 10:43:42.000000 questdb-connect-0.0.30/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-02 10:43:42.000000 questdb-connect-0.0.30/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-02 10:43:42.000000 questdb-connect-0.0.30/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-02 10:43:42.000000 questdb-connect-0.0.30/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-02 10:43:42.000000 questdb-connect-0.0.30/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:43:42.586614 questdb-connect-0.0.30/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.30/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     1183 2023-05-02 10:41:32.000000 questdb-connect-0.0.30/tests/test_function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.30/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.30/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:55:59.621472 questdb-connect-0.0.31/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.31/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-02 10:55:59.621328 questdb-connect-0.0.31/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.31/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2477 2023-05-02 10:54:34.000000 questdb-connect-0.0.31/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-02 10:55:59.621507 questdb-connect-0.0.31/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:55:59.617226 questdb-connect-0.0.31/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:55:59.619505 questdb-connect-0.0.31/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-02 10:25:08.000000 questdb-connect-0.0.31/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11154 2023-05-02 10:55:20.000000 questdb-connect-0.0.31/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.31/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10657 2023-05-02 10:25:13.000000 questdb-connect-0.0.31/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-05-01 20:15:41.000000 questdb-connect-0.0.31/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:55:59.620421 questdb-connect-0.0.31/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-02 10:55:59.000000 questdb-connect-0.0.31/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      526 2023-05-02 10:55:59.000000 questdb-connect-0.0.31/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-02 10:55:59.000000 questdb-connect-0.0.31/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-02 10:55:59.000000 questdb-connect-0.0.31/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-02 10:55:59.000000 questdb-connect-0.0.31/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-02 10:55:59.000000 questdb-connect-0.0.31/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:55:59.621046 questdb-connect-0.0.31/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.31/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.31/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.31/tests/test_types.py
```

### Comparing `questdb-connect-0.0.30/LICENSE` & `questdb-connect-0.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.30/PKG-INFO` & `questdb-connect-0.0.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.30
+Version: 0.0.31
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.30/README.md` & `questdb-connect-0.0.31/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.30/pyproject.toml` & `questdb-connect-0.0.31/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.30"
+version = "0.0.31"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -76,9 +76,8 @@
 max-branches = 20
 max-args = 10
 
 [tool.ruff.per-file-ignores]
 "tests/test_dialect.py" = ["S101"]
 "tests/test_types.py" = ["S101"]
 "tests/test_superset.py" = ["S101"]
-"tests/test_function_names.py" = ["S101"]
 "tests/conftest.py" = ["S608"]
```

### Comparing `questdb-connect-0.0.30/src/questdb_connect/__init__.py` & `questdb-connect-0.0.31/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.30/src/questdb_connect/dialect.py` & `questdb-connect-0.0.31/src/questdb_connect/dialect.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from sqlalchemy.exc import ArgumentError
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import DDLCompiler, GenericTypeCompiler, IdentifierPreparer, SQLCompiler
 from sqlalchemy.sql.visitors import Traversible
 
 from . import remove_public_schema
-from .function_names import is_function_call
 from .types import PartitionBy, QDBTypeMixin, quote_identifier, resolve_type_from_name
 
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
 # ===== SQLAlchemy Dialect ======
 
 def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
@@ -114,15 +113,15 @@
             quote_case_sensitive_collations=quote_case_sensitive_collations,
             omit_schema=omit_schema)
 
     def quote_identifier(self, value):
         return quote_identifier(value)
 
     def _requires_quotes(self, _value):
-        return not is_function_call(_value)
+        return _value and (' ' in _value or '\t' in _value or '~' in _value or ':' in _value or ';' in _value)
 
     def format_schema(self, name):
         """Prepare a quoted schema name."""
         return ""
 
     def format_table(self, table, use_schema=True, name=None):
         """Prepare a quoted table and schema name."""
```

### Comparing `questdb-connect-0.0.30/src/questdb_connect/function_names.py` & `questdb-connect-0.0.31/src/questdb_connect/function_names.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,16 +38,14 @@
 #                     break;
 #                 }
 #             });
 #         }
 #     });
 # }
 #
-from sqlalchemy.exc import ArgumentError
-
 FUNCTION_NAMES = [
     'VARCHAR',
     'abs',
     'acos',
     'all_tables',
     'and',
     'asin',
@@ -230,22 +228,7 @@
     'typeOf',
     'upper',
     'version',
     'wal_tables',
     'week_of_year',
     'year',
 ]
-
-_func_name_set = set(FUNCTION_NAMES)
-
-
-def is_function_call(token):
-    if token:
-        open_p = token.index('(') if '(' in token else None
-        close_p = token.index(')') if ')' in token else None
-        if open_p and close_p:
-            fun_name = token[:open_p]
-        elif not open_p and not close_p:
-            fun_name = token
-        else:
-            raise ArgumentError(f'bad syntax: {token}')
-        return fun_name.lower() in _func_name_set
```

### Comparing `questdb-connect-0.0.30/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.31/src/questdb_connect/superset_engine.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.30/src/questdb_connect/types.py` & `questdb-connect-0.0.31/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.30/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.31/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.30
+Version: 0.0.31
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.30/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.31/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,10 +9,9 @@
 src/questdb_connect.egg-info/PKG-INFO
 src/questdb_connect.egg-info/SOURCES.txt
 src/questdb_connect.egg-info/dependency_links.txt
 src/questdb_connect.egg-info/entry_points.txt
 src/questdb_connect.egg-info/requires.txt
 src/questdb_connect.egg-info/top_level.txt
 tests/test_dialect.py
-tests/test_function_names.py
 tests/test_superset.py
 tests/test_types.py
```

### Comparing `questdb-connect-0.0.30/tests/test_dialect.py` & `questdb-connect-0.0.31/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.30/tests/test_superset.py` & `questdb-connect-0.0.31/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.30/tests/test_types.py` & `questdb-connect-0.0.31/tests/test_types.py`

 * *Files identical despite different names*

