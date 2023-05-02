# Comparing `tmp/questdb-connect-0.0.31.tar.gz` & `tmp/questdb-connect-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.31.tar", last modified: Tue May  2 10:55:59 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.32.tar", last modified: Tue May  2 11:07:34 2023, max compression
```

## Comparing `questdb-connect-0.0.31.tar` & `questdb-connect-0.0.32.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:55:59.621472 questdb-connect-0.0.31/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.31/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-02 10:55:59.621328 questdb-connect-0.0.31/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.31/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2477 2023-05-02 10:54:34.000000 questdb-connect-0.0.31/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-02 10:55:59.621507 questdb-connect-0.0.31/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:55:59.617226 questdb-connect-0.0.31/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:55:59.619505 questdb-connect-0.0.31/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-02 10:25:08.000000 questdb-connect-0.0.31/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11154 2023-05-02 10:55:20.000000 questdb-connect-0.0.31/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.31/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10657 2023-05-02 10:25:13.000000 questdb-connect-0.0.31/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-05-01 20:15:41.000000 questdb-connect-0.0.31/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:55:59.620421 questdb-connect-0.0.31/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-02 10:55:59.000000 questdb-connect-0.0.31/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      526 2023-05-02 10:55:59.000000 questdb-connect-0.0.31/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-02 10:55:59.000000 questdb-connect-0.0.31/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-02 10:55:59.000000 questdb-connect-0.0.31/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-02 10:55:59.000000 questdb-connect-0.0.31/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-02 10:55:59.000000 questdb-connect-0.0.31/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 10:55:59.621046 questdb-connect-0.0.31/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.31/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.31/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.31/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 11:07:34.149157 questdb-connect-0.0.32/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.32/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-02 11:07:34.149028 questdb-connect-0.0.32/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.32/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2477 2023-05-02 11:07:16.000000 questdb-connect-0.0.32/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-02 11:07:34.149190 questdb-connect-0.0.32/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 11:07:34.145313 questdb-connect-0.0.32/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 11:07:34.147256 questdb-connect-0.0.32/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-02 10:25:08.000000 questdb-connect-0.0.32/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11412 2023-05-02 11:06:40.000000 questdb-connect-0.0.32/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.32/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10657 2023-05-02 10:25:13.000000 questdb-connect-0.0.32/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-05-01 20:15:41.000000 questdb-connect-0.0.32/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 11:07:34.148108 questdb-connect-0.0.32/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-05-02 11:07:34.000000 questdb-connect-0.0.32/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      526 2023-05-02 11:07:34.000000 questdb-connect-0.0.32/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-02 11:07:34.000000 questdb-connect-0.0.32/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-02 11:07:34.000000 questdb-connect-0.0.32/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-02 11:07:34.000000 questdb-connect-0.0.32/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-05-02 11:07:34.000000 questdb-connect-0.0.32/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-02 11:07:34.148751 questdb-connect-0.0.32/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.32/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.32/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.32/tests/test_types.py
```

### Comparing `questdb-connect-0.0.31/LICENSE` & `questdb-connect-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.31/PKG-INFO` & `questdb-connect-0.0.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.31
+Version: 0.0.32
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.31/README.md` & `questdb-connect-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.31/pyproject.toml` & `questdb-connect-0.0.32/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.31"
+version = "0.0.32"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.31/src/questdb_connect/__init__.py` & `questdb-connect-0.0.32/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.31/src/questdb_connect/dialect.py` & `questdb-connect-0.0.32/src/questdb_connect/dialect.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,28 @@
 
 # ===== QUESTDB DIALECT TYPES =====
 
 def _none(_ignore):
     return None
 
 
+_special_chars = {
+    '(', ')', '[', '[]', '{', '}', "'", '"', ':', ';', '.',
+    '!', '%', '&', '*', '$', '@', '~', '^', '-', '?', '/', '\\',
+    ' ', '\t', '\r', '\n'
+}
+
+
+def _has_special_char(_value):
+    for candidate in _value:
+        if candidate in _special_chars:
+            return True
+    return False
+
+
 class QDBIdentifierPreparer(IdentifierPreparer, abc.ABC):
     schema_for_object = staticmethod(_none)
 
     def __init__(
             self,
             dialect,
             initial_quote='"',
@@ -113,15 +127,15 @@
             quote_case_sensitive_collations=quote_case_sensitive_collations,
             omit_schema=omit_schema)
 
     def quote_identifier(self, value):
         return quote_identifier(value)
 
     def _requires_quotes(self, _value):
-        return _value and (' ' in _value or '\t' in _value or '~' in _value or ':' in _value or ';' in _value)
+        return _value and _has_special_char(_value)
 
     def format_schema(self, name):
         """Prepare a quoted schema name."""
         return ""
 
     def format_table(self, table, use_schema=True, name=None):
         """Prepare a quoted table and schema name."""
```

### Comparing `questdb-connect-0.0.31/src/questdb_connect/function_names.py` & `questdb-connect-0.0.32/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.31/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.32/src/questdb_connect/superset_engine.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.31/src/questdb_connect/types.py` & `questdb-connect-0.0.32/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.31/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.32/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.31
+Version: 0.0.32
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.31/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.32/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.31/tests/test_dialect.py` & `questdb-connect-0.0.32/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.31/tests/test_superset.py` & `questdb-connect-0.0.32/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.31/tests/test_types.py` & `questdb-connect-0.0.32/tests/test_types.py`

 * *Files identical despite different names*

