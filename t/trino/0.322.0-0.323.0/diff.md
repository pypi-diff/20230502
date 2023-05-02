# Comparing `tmp/trino-0.322.0.tar.gz` & `tmp/trino-0.323.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trino-0.322.0.tar", last modified: Fri Mar  3 11:40:44 2023, max compression
+gzip compressed data, was "trino-0.323.0.tar", last modified: Tue May  2 09:18:30 2023, max compression
```

## Comparing `trino-0.322.0.tar` & `trino-0.323.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 11:40:44.769924 trino-0.322.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-03 11:40:32.000000 trino-0.322.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-03 11:40:44.769924 trino-0.322.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14918 2023-03-03 11:40:32.000000 trino-0.322.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-03 11:40:44.769924 trino-0.322.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3342 2023-03-03 11:40:32.000000 trino-0.322.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 11:40:44.769924 trino-0.322.0/trino/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-03 11:40:34.000000 trino-0.322.0/trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-03-03 11:40:32.000000 trino-0.322.0/trino/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    45165 2023-03-03 11:40:32.000000 trino-0.322.0/trino/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-03 11:40:32.000000 trino-0.322.0/trino/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    22136 2023-03-03 11:40:32.000000 trino-0.322.0/trino/dbapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-03-03 11:40:32.000000 trino-0.322.0/trino/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-03 11:40:32.000000 trino-0.322.0/trino/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 11:40:44.769924 trino-0.322.0/trino/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-03 11:40:32.000000 trino-0.322.0/trino/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-03-03 11:40:32.000000 trino-0.322.0/trino/sqlalchemy/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-03-03 11:40:32.000000 trino-0.322.0/trino/sqlalchemy/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)    15610 2023-03-03 11:40:32.000000 trino-0.322.0/trino/sqlalchemy/dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-03 11:40:32.000000 trino-0.322.0/trino/sqlalchemy/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-03-03 11:40:32.000000 trino-0.322.0/trino/sqlalchemy/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-03-03 11:40:32.000000 trino-0.322.0/trino/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 11:40:44.769924 trino-0.322.0/trino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-03 11:40:44.000000 trino-0.322.0/trino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-03 11:40:44.000000 trino-0.322.0/trino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 11:40:44.000000 trino-0.322.0/trino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-03 11:40:44.000000 trino-0.322.0/trino.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-03 11:40:44.000000 trino-0.322.0/trino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-03 11:40:44.000000 trino-0.322.0/trino.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:18:30.679182 trino-0.323.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 09:18:16.000000 trino-0.323.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-02 09:18:30.679182 trino-0.323.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-05-02 09:18:16.000000 trino-0.323.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-02 09:18:30.679182 trino-0.323.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3342 2023-05-02 09:18:16.000000 trino-0.323.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:18:30.675182 trino-0.323.0/trino/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-02 09:18:19.000000 trino-0.323.0/trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-05-02 09:18:16.000000 trino-0.323.0/trino/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47042 2023-05-02 09:18:16.000000 trino-0.323.0/trino/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-02 09:18:16.000000 trino-0.323.0/trino/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22662 2023-05-02 09:18:16.000000 trino-0.323.0/trino/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-02 09:18:16.000000 trino-0.323.0/trino/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-02 09:18:16.000000 trino-0.323.0/trino/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:18:30.679182 trino-0.323.0/trino/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-02 09:18:16.000000 trino-0.323.0/trino/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-02 09:18:16.000000 trino-0.323.0/trino/sqlalchemy/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-05-02 09:18:16.000000 trino-0.323.0/trino/sqlalchemy/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15610 2023-05-02 09:18:16.000000 trino-0.323.0/trino/sqlalchemy/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-02 09:18:16.000000 trino-0.323.0/trino/sqlalchemy/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-02 09:18:16.000000 trino-0.323.0/trino/sqlalchemy/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-02 09:18:16.000000 trino-0.323.0/trino/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:18:30.675182 trino-0.323.0/trino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-02 09:18:30.000000 trino-0.323.0/trino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-02 09:18:30.000000 trino-0.323.0/trino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:18:30.000000 trino-0.323.0/trino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 09:18:30.000000 trino-0.323.0/trino.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-02 09:18:30.000000 trino-0.323.0/trino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 09:18:30.000000 trino-0.323.0/trino.egg-info/top_level.txt
```

### Comparing `trino-0.322.0/LICENSE` & `trino-0.323.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trino-0.322.0/PKG-INFO` & `trino-0.323.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trino
-Version: 0.322.0
+Version: 0.323.0
 Summary: Client for the Trino distributed SQL Engine
 Home-page: https://github.com/trinodb/trino-python-client
 Author: Trino Team
 Author-email: python-client@trino.io
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trino-0.322.0/README.md` & `trino-0.323.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -357,14 +357,26 @@
     host='localhost',
     port=443,
     user='the-user',
     roles={"catalog1": "roleA", "catalog2": "roleB"},
 )
 ```
 
+You could also pass `system` role without explicitly specifing "system" catalog:
+
+```python
+import trino
+conn = trino.dbapi.connect(
+    host='localhost',
+    port=443,
+    user='the-user',
+    roles="role1" # equivalent to {"system": "role1"}
+)
+```
+
 ## Timezone
 
 The time zone for the session can be explicitly set using the IANA time zone
 name. When not set the time zone defaults to the client side local timezone.
 
 ```python
 import trino
```

### Comparing `trino-0.322.0/setup.py` & `trino-0.323.0/setup.py`

 * *Files identical despite different names*

### Comparing `trino-0.322.0/trino/__init__.py` & `trino-0.323.0/trino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from . import auth, client, constants, dbapi, exceptions, logging
 
 __all__ = ['auth', 'dbapi', 'client', 'constants', 'exceptions', 'logging']
 
-__version__ = "0.322.0"
+__version__ = "0.323.0"
```

### Comparing `trino-0.322.0/trino/auth.py` & `trino-0.323.0/trino/auth.py`

 * *Files identical despite different names*

### Comparing `trino-0.322.0/trino/client.py` & `trino-0.323.0/trino/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 import copy
 import functools
 import os
 import random
 import re
 import threading
 import urllib.parse
+import uuid
 import warnings
 from dataclasses import dataclass
 from datetime import date, datetime, time, timedelta, timezone, tzinfo
 from decimal import Decimal
 from time import sleep
 from typing import Any, Dict, Generic, List, Optional, Tuple, TypeVar, Union
 
@@ -131,15 +132,15 @@
         schema: str = None,
         source: str = None,
         properties: Dict[str, str] = None,
         headers: Dict[str, str] = None,
         transaction_id: str = None,
         extra_credential: List[Tuple[str, str]] = None,
         client_tags: List[str] = None,
-        roles: Dict[str, str] = None,
+        roles: Union[Dict[str, str], str] = None,
         timezone: str = None,
     ):
         self._user = user
         self._catalog = catalog
         self._schema = schema
         self._source = source
         self._properties = properties.copy() if properties is not None else {}
@@ -235,14 +236,16 @@
 
     @property
     def timezone(self):
         with self._object_lock:
             return self._timezone
 
     def _format_roles(self, roles):
+        if isinstance(roles, str):
+            roles = {"system": roles}
         formatted_roles = {}
         for catalog, role in roles.items():
             is_legacy_role_pattern = ROLE_PATTERN.match(role) is not None
             if role in ("NONE", "ALL") or is_legacy_role_pattern:
                 if is_legacy_role_pattern:
                     warnings.warn(f"A role '{role}' is provided using a legacy format. "
                                   "Please remove the ROLE{} wrapping. Support for the legacy format might be "
@@ -1124,22 +1127,56 @@
 
     def map(self, values: List[Any]) -> Optional[List[Any]]:
         if values is None:
             return None
         return [self.mapper.map(value) for value in values]
 
 
+class NamedRowTuple(tuple):
+    """Custom tuple class as namedtuple doesn't support missing or duplicate names"""
+    def __new__(cls, values, names: List[str], types: List[str]):
+        return super().__new__(cls, values)
+
+    def __init__(self, values, names: List[str], types: List[str]):
+        self._names = names
+        # With names and types users can retrieve the name and Trino data type of a row
+        self.__annotations__ = dict()
+        self.__annotations__["names"] = names
+        self.__annotations__["types"] = types
+        elements: List[Any] = []
+        for name, value in zip(names, values):
+            if names.count(name) == 1:
+                setattr(self, name, value)
+                elements.append(f"{name}: {repr(value)}")
+            else:
+                elements.append(repr(value))
+        self._repr = "(" + ", ".join(elements) + ")"
+
+    def __getattr__(self, name):
+        if self._names.count(name):
+            raise ValueError("Ambiguous row field reference: " + name)
+
+    def __repr__(self):
+        return self._repr
+
+
 class RowValueMapper(ValueMapper[Tuple[Optional[Any], ...]]):
-    def __init__(self, mappers: List[ValueMapper[Any]]):
+    def __init__(self, mappers: List[ValueMapper[Any]], names: List[str], types: List[str]):
         self.mappers = mappers
+        self.names = names
+        self.types = types
 
     def map(self, values: List[Any]) -> Optional[Tuple[Optional[Any], ...]]:
         if values is None:
             return None
-        return tuple(self.mappers[index].map(value) for index, value in enumerate(values))
+        return NamedRowTuple(
+            list(self.mappers[index].map(value) for index, value in enumerate(values)),
+            self.names,
+            self.types
+        )
 
 
 class MapValueMapper(ValueMapper[Dict[Any, Optional[Any]]]):
     def __init__(self, key_mapper: ValueMapper[Any], value_mapper: ValueMapper[Any]):
         self.key_mapper = key_mapper
         self.value_mapper = value_mapper
 
@@ -1147,14 +1184,21 @@
         if values is None:
             return None
         return {
             self.key_mapper.map(key): self.value_mapper.map(value) for key, value in values.items()
         }
 
 
+class UuidValueMapper(ValueMapper[uuid.UUID]):
+    def map(self, value: Any) -> Optional[uuid.UUID]:
+        if value is None:
+            return None
+        return uuid.UUID(value)
+
+
 class NoOpRowMapper:
     """
     No-op RowMapper which does not perform any transformation
     Used when legacy_primitive_types is False.
     """
 
     def map(self, rows):
@@ -1179,16 +1223,22 @@
     def _create_value_mapper(self, column) -> ValueMapper:
         col_type = column['rawType']
 
         if col_type == 'array':
             value_mapper = self._create_value_mapper(column['arguments'][0]['value'])
             return ArrayValueMapper(value_mapper)
         elif col_type == 'row':
-            mappers = [self._create_value_mapper(arg['value']['typeSignature']) for arg in column['arguments']]
-            return RowValueMapper(mappers)
+            mappers = []
+            names = []
+            types = []
+            for arg in column['arguments']:
+                mappers.append(self._create_value_mapper(arg['value']['typeSignature']))
+                names.append(arg['value']['fieldName']['name'] if "fieldName" in arg['value'] else None)
+                types.append(arg['value']['typeSignature']['rawType'])
+            return RowValueMapper(mappers, names, types)
         elif col_type == 'map':
             key_mapper = self._create_value_mapper(column['arguments'][0]['value'])
             value_mapper = self._create_value_mapper(column['arguments'][1]['value'])
             return MapValueMapper(key_mapper, value_mapper)
         elif col_type.startswith('decimal'):
             return DecimalValueMapper()
         elif col_type.startswith('double') or col_type.startswith('real'):
@@ -1201,14 +1251,16 @@
             return TimeWithTimeZoneValueMapper(self._get_precision(column))
         elif col_type.startswith('time'):
             return TimeValueMapper(self._get_precision(column))
         elif col_type == 'date':
             return DateValueMapper()
         elif col_type == 'varbinary':
             return BinaryValueMapper()
+        elif col_type == 'uuid':
+            return UuidValueMapper()
         else:
             return NoOpValueMapper()
 
     def _get_precision(self, column: Dict[str, Any]):
         args = column['arguments']
         if len(args) == 0:
             return 3
```

### Comparing `trino-0.322.0/trino/constants.py` & `trino-0.323.0/trino/constants.py`

 * *Files identical despite different names*

### Comparing `trino-0.322.0/trino/dbapi.py` & `trino-0.323.0/trino/dbapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 import datetime
 import math
 import uuid
 from decimal import Decimal
 from typing import Any, Dict, List, NamedTuple, Optional  # NOQA for mypy types
 from urllib.parse import urlparse
 
+import pytz
+
 import trino.client
 import trino.exceptions
 import trino.logging
 from trino import constants
 from trino.constants import LENGTH_TYPES, PRECISION_TYPES, SCALE_TYPES
 from trino.exceptions import (
     DatabaseError,
@@ -429,14 +431,23 @@
             return "TIMESTAMP '%s %s'" % (datetime_str, param.tzinfo.tzname(param))
 
         # We can't calculate the offset for a time without a point in time
         if isinstance(param, datetime.time) and param.tzinfo is None:
             time_str = param.strftime("%H:%M:%S.%f")
             return "TIME '%s'" % time_str
 
+        if isinstance(param, datetime.time) and param.tzinfo is not None:
+            time_str = param.strftime("%H:%M:%S.%f")
+            # named timezones
+            if hasattr(param.tzinfo, 'zone'):
+                utc_offset = datetime.datetime.now(pytz.timezone(param.tzinfo.zone)).strftime('%z')
+                return "TIME '%s %s:%s'" % (time_str, utc_offset[:3], utc_offset[3:])
+            # offset-based timezones
+            return "TIME '%s %s'" % (time_str, param.strftime('%Z')[3:])
+
         if isinstance(param, datetime.date):
             date_str = param.strftime("%Y-%m-%d")
             return "DATE '%s'" % date_str
 
         if isinstance(param, list):
             return "ARRAY[%s]" % ','.join(map(self._format_prepared_param, param))
 
@@ -451,15 +462,15 @@
                 self._format_prepared_param(values)
             )
 
         if isinstance(param, uuid.UUID):
             return "UUID '%s'" % param
 
         if isinstance(param, Decimal):
-            return "DECIMAL '%s'" % param
+            return "DECIMAL '%s'" % format(param, "f")
 
         if isinstance(param, (bytes, bytearray)):
             return "X'%s'" % binascii.hexlify(param).decode("utf-8")
 
         raise trino.exceptions.NotSupportedError("Query parameter of type '%s' is not supported." % type(param))
 
     def _deallocate_prepared_statement(self, statement_name: str) -> None:
```

### Comparing `trino-0.322.0/trino/exceptions.py` & `trino-0.323.0/trino/exceptions.py`

 * *Files identical despite different names*

### Comparing `trino-0.322.0/trino/logging.py` & `trino-0.323.0/trino/logging.py`

 * *Files identical despite different names*

### Comparing `trino-0.322.0/trino/sqlalchemy/__init__.py` & `trino-0.323.0/trino/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `trino-0.322.0/trino/sqlalchemy/compiler.py` & `trino-0.323.0/trino/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `trino-0.322.0/trino/sqlalchemy/datatype.py` & `trino-0.323.0/trino/sqlalchemy/datatype.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import json
 import re
 from typing import Any, Dict, Iterator, List, Optional, Tuple, Type, Union
 
+import sqlalchemy
 from sqlalchemy import util
 from sqlalchemy.sql import sqltypes
 from sqlalchemy.sql.type_api import TypeDecorator, TypeEngine
 from sqlalchemy.types import String
 
 SQLType = Union[TypeEngine, Type[TypeEngine]]
 
@@ -125,14 +126,17 @@
     # 'uuid': UUID,
     # 'hyperloglog': HYPERLOGLOG,
     # 'p4hyperloglog': P4HYPERLOGLOG,
     # 'qdigest': QDIGEST,
     # 'tdigest': TDIGEST,
 }
 
+if hasattr(sqlalchemy, "Uuid"):
+    _type_map["uuid"] = sqlalchemy.Uuid
+
 
 def unquote(string: str, quote: str = '"', escape: str = "\\") -> str:
     """
     If string starts and ends with a quote, unquote it
     """
     if string.startswith(quote) and string.endswith(quote):
         string = string[1:-1]
```

### Comparing `trino-0.322.0/trino/sqlalchemy/dialect.py` & `trino-0.323.0/trino/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `trino-0.322.0/trino/sqlalchemy/error.py` & `trino-0.323.0/trino/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `trino-0.322.0/trino/sqlalchemy/util.py` & `trino-0.323.0/trino/sqlalchemy/util.py`

 * *Files identical despite different names*

### Comparing `trino-0.322.0/trino/transaction.py` & `trino-0.323.0/trino/transaction.py`

 * *Files identical despite different names*

### Comparing `trino-0.322.0/trino.egg-info/PKG-INFO` & `trino-0.323.0/trino.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trino
-Version: 0.322.0
+Version: 0.323.0
 Summary: Client for the Trino distributed SQL Engine
 Home-page: https://github.com/trinodb/trino-python-client
 Author: Trino Team
 Author-email: python-client@trino.io
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trino-0.322.0/trino.egg-info/SOURCES.txt` & `trino-0.323.0/trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

