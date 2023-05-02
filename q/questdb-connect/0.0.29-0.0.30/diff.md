# Comparing `tmp/questdb-connect-0.0.29.tar.gz` & `tmp/questdb-connect-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.29.tar", last modified: Mon May  1 21:01:09 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.30.tar", last modified: Tue May  2 10:43:42 2023, max compression
```

## Comparing `questdb-connect-0.0.29.tar` & `questdb-connect-0.0.30.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 21:01:09.663452 questdb-connect-0.0.29/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.29/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-01 21:01:09.663311 questdb-connect-0.0.29/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.29/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2477 2023-05-01 20:59:25.000000 questdb-connect-0.0.29/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-01 21:01:09.663486 questdb-connect-0.0.29/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 21:01:09.659530 questdb-connect-0.0.29/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 21:01:09.661480 questdb-connect-0.0.29/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1401 2023-05-01 20:59:25.000000 questdb-connect-0.0.29/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11147 2023-05-01 21:00:28.000000 questdb-connect-0.0.29/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5250 2023-04-27 10:02:14.000000 questdb-connect-0.0.29/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10693 2023-05-01 20:15:41.000000 questdb-connect-0.0.29/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-05-01 20:15:41.000000 questdb-connect-0.0.29/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 21:01:09.662384 questdb-connect-0.0.29/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-01 21:01:09.000000 questdb-connect-0.0.29/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      526 2023-05-01 21:01:09.000000 questdb-connect-0.0.29/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-01 21:01:09.000000 questdb-connect-0.0.29/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-01 21:01:09.000000 questdb-connect-0.0.29/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-01 21:01:09.000000 questdb-connect-0.0.29/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-01 21:01:09.000000 questdb-connect-0.0.29/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-01 21:01:09.663008 questdb-connect-0.0.29/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-01 20:18:00.000000 questdb-connect-0.0.29/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.29/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.29/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:43:42.587191 questdb-connect-0.0.30/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.30/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-02 10:43:42.587059 questdb-connect-0.0.30/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.30/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2519 2023-05-02 10:43:24.000000 questdb-connect-0.0.30/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-02 10:43:42.587223 questdb-connect-0.0.30/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:43:42.582392 questdb-connect-0.0.30/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:43:42.584639 questdb-connect-0.0.30/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-02 10:25:08.000000 questdb-connect-0.0.30/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11132 2023-05-02 10:41:38.000000 questdb-connect-0.0.30/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5665 2023-05-02 10:39:22.000000 questdb-connect-0.0.30/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10657 2023-05-02 10:25:13.000000 questdb-connect-0.0.30/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-05-01 20:15:41.000000 questdb-connect-0.0.30/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:43:42.585690 questdb-connect-0.0.30/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-02 10:43:42.000000 questdb-connect-0.0.30/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      555 2023-05-02 10:43:42.000000 questdb-connect-0.0.30/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-02 10:43:42.000000 questdb-connect-0.0.30/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-02 10:43:42.000000 questdb-connect-0.0.30/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-02 10:43:42.000000 questdb-connect-0.0.30/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-02 10:43:42.000000 questdb-connect-0.0.30/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:43:42.586614 questdb-connect-0.0.30/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.30/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1183 2023-05-02 10:41:32.000000 questdb-connect-0.0.30/tests/test_function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.30/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.30/tests/test_types.py
```

### Comparing `questdb-connect-0.0.29/LICENSE` & `questdb-connect-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.29/PKG-INFO` & `questdb-connect-0.0.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.29
+Version: 0.0.30
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.29/README.md` & `questdb-connect-0.0.30/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.29/pyproject.toml` & `questdb-connect-0.0.30/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.29"
+version = "0.0.30"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -76,8 +76,9 @@
 max-branches = 20
 max-args = 10
 
 [tool.ruff.per-file-ignores]
 "tests/test_dialect.py" = ["S101"]
 "tests/test_types.py" = ["S101"]
 "tests/test_superset.py" = ["S101"]
+"tests/test_function_names.py" = ["S101"]
 "tests/conftest.py" = ["S608"]
```

### Comparing `questdb-connect-0.0.29/src/questdb_connect/__init__.py` & `questdb-connect-0.0.30/src/questdb_connect/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,34 +16,53 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
+import re
+
 import psycopg2
 
 # ===== DBAPI =====
 
 # https://peps.python.org/pep-0249/
 
 apilevel = '2.0'
 threadsafety = 2
 paramstyle = 'pyformat'
+public_schema_filter = re.compile(r"(')?(public(?(1)\1|)\.)", re.IGNORECASE | re.MULTILINE)
+
+
+def remove_public_schema(query):
+    if query and isinstance(query, str) and 'public' in query:
+        return re.sub(public_schema_filter, '', query)
+    return query
 
 
 class Error(Exception):
     pass
 
 
+class Cursor(psycopg2.extensions.cursor):
+    def execute(self, query, vars=None):
+        return super().execute(remove_public_schema(query), vars)
+
+
+def cursor_factory(*args, **kwargs):
+    return Cursor(*args, **kwargs)
+
+
 def connect(**kwargs):
     host = kwargs.get('host') or '127.0.0.1'
     port = kwargs.get('port') or 8812
     user = kwargs.get('username') or 'admin'
     password = kwargs.get('password') or 'quest'
     database = kwargs.get('database') or 'main'
     return psycopg2.connect(
+        cursor_factory=cursor_factory,
         host=host,
         port=port,
         user=user,
         password=password,
         database=database)
```

### Comparing `questdb-connect-0.0.29/src/questdb_connect/dialect.py` & `questdb-connect-0.0.30/src/questdb_connect/dialect.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,26 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import abc
-import re
 
 import sqlalchemy as sqla
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.reflection import Inspector
 from sqlalchemy.exc import ArgumentError
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import DDLCompiler, GenericTypeCompiler, IdentifierPreparer, SQLCompiler
 from sqlalchemy.sql.visitors import Traversible
 
+from . import remove_public_schema
+from .function_names import is_function_call
 from .types import PartitionBy, QDBTypeMixin, quote_identifier, resolve_type_from_name
 
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
 # ===== SQLAlchemy Dialect ======
 
 def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
@@ -113,15 +114,15 @@
             quote_case_sensitive_collations=quote_case_sensitive_collations,
             omit_schema=omit_schema)
 
     def quote_identifier(self, value):
         return quote_identifier(value)
 
     def _requires_quotes(self, _value):
-        return True
+        return not is_function_call(_value)
 
     def format_schema(self, name):
         """Prepare a quoted schema name."""
         return ""
 
     def format_table(self, table, use_schema=True, name=None):
         """Prepare a quoted table and schema name."""
@@ -143,24 +144,20 @@
 
     def get_column_specification(self, column: sqla.Column, **_):
         if not isinstance(column.type, QDBTypeMixin):
             raise ArgumentError('Column type is not a valid QuestDB type')
         return column.type.column_spec(column.name)
 
 
-_public_schema_filter = re.compile(r"(')?(public(?(1)\1|)\.)", re.IGNORECASE | re.MULTILINE)
-
-
 class QDBSQLCompiler(SQLCompiler, abc.ABC):
-
     def _is_safe_for_fast_insert_values_helper(self):
         return True
 
     def visit_textclause(self, textclause, add_to_result_map=None, **kw):
-        textclause.text = re.sub(_public_schema_filter, '', textclause.text)
+        textclause.text = remove_public_schema(textclause.text)
         return super().visit_textclause(textclause, add_to_result_map, **kw)
 
 
 class QDBInspector(Inspector, abc.ABC):
     def reflecttable(
             self,
             table,
```

### Comparing `questdb-connect-0.0.29/src/questdb_connect/function_names.py` & `questdb-connect-0.0.30/src/questdb_connect/function_names.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 #                     break;
 #                 }
 #             });
 #         }
 #     });
 # }
 #
+from sqlalchemy.exc import ArgumentError
+
 FUNCTION_NAMES = [
     'VARCHAR',
     'abs',
     'acos',
     'all_tables',
     'and',
     'asin',
@@ -229,10 +231,21 @@
     'upper',
     'version',
     'wal_tables',
     'week_of_year',
     'year',
 ]
 
-if __name__ == '__main__':
-    for s in sorted(FUNCTION_NAMES):
-        print(f"'{s}',")
+_func_name_set = set(FUNCTION_NAMES)
+
+
+def is_function_call(token):
+    if token:
+        open_p = token.index('(') if '(' in token else None
+        close_p = token.index(')') if ')' in token else None
+        if open_p and close_p:
+            fun_name = token[:open_p]
+        elif not open_p and not close_p:
+            fun_name = token
+        else:
+            raise ArgumentError(f'bad syntax: {token}')
+        return fun_name.lower() in _func_name_set
```

### Comparing `questdb-connect-0.0.29/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.30/src/questdb_connect/superset_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,22 @@
 from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
 import questdb_connect.dialect as qdbcd
 
-from . import types
+from . import remove_public_schema, types
 from .function_names import FUNCTION_NAMES
 
 # https://superset.apache.org/docs/databases/installing-database-drivers
 # Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
 # https://preset.io/blog/building-database-connector/
 
 
-_MATCH_PUBLIC_SCHEMA = r"(')?(public(?(1)\1)\.)"
-
-
 class QDBEngineSpec(BaseEngineSpec, BasicParametersMixin):
     engine = 'questdb'
     engine_name = 'QuestDB Connect'
     default_driver = "psycopg2"
     encryption_parameters = {"sslmode": "prefer"}
     sqlalchemy_uri_placeholder = "questdb://user:password@host:port/dbname[?key=value&key=value...]"
     time_groupby_inline = True
@@ -119,15 +116,16 @@
     def get_text_clause(cls, clause):
         """SQLAlchemy wrapper to ensure text clauses are escaped properly
         :param clause: string clause with potentially unescaped characters
         :return: text clause with escaped characters
         """
         if cls.allows_escaped_colons:
             clause = clause.replace(":", "\\:")
-        return text(re.sub(_MATCH_PUBLIC_SCHEMA, "", clause, flags=re.IGNORECASE | re.MULTILINE))
+            remove_public_schema(clause)
+        return text(remove_public_schema(clause))
 
     @classmethod
     def epoch_to_dttm(cls) -> str:
         """SQL expression that converts epoch (seconds) to datetime that can be used in a
         query. The reference column should be denoted as `{col}` in the return
         expression, e.g. "FROM_UNIXTIME({col})"
         :return: SQL Expression
```

### Comparing `questdb-connect-0.0.29/src/questdb_connect/types.py` & `questdb-connect-0.0.30/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.29/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.30/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.29
+Version: 0.0.30
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.29/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.30/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,9 +9,10 @@
 src/questdb_connect.egg-info/PKG-INFO
 src/questdb_connect.egg-info/SOURCES.txt
 src/questdb_connect.egg-info/dependency_links.txt
 src/questdb_connect.egg-info/entry_points.txt
 src/questdb_connect.egg-info/requires.txt
 src/questdb_connect.egg-info/top_level.txt
 tests/test_dialect.py
+tests/test_function_names.py
 tests/test_superset.py
 tests/test_types.py
```

### Comparing `questdb-connect-0.0.29/tests/test_dialect.py` & `questdb-connect-0.0.30/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.29/tests/test_superset.py` & `questdb-connect-0.0.30/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.29/tests/test_types.py` & `questdb-connect-0.0.30/tests/test_types.py`

 * *Files identical despite different names*

