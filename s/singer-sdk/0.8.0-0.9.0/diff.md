# Comparing `tmp/singer-sdk-0.8.0.tar.gz` & `tmp/singer-sdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singer-sdk-0.8.0.tar", max compression
+gzip compressed data, was "singer-sdk-0.9.0.tar", max compression
```

## Comparing `singer-sdk-0.8.0.tar` & `singer-sdk-0.9.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0    11337 2022-08-05 22:39:33.895381 singer-sdk-0.8.0/LICENSE
--rw-r--r--   0        0        0     2230 2022-08-05 22:39:33.895381 singer-sdk-0.8.0/README.md
--rw-r--r--   0        0        0     6201 2022-08-05 22:39:33.903381 singer-sdk-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      733 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/__init__.py
--rw-r--r--   0        0        0    16482 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/authenticators.py
--rw-r--r--   0        0        0       51 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/cli/__init__.py
--rw-r--r--   0        0        0      815 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/cli/common_options.py
--rw-r--r--   0        0        0       42 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/configuration/__init__.py
--rw-r--r--   0        0        0     3247 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/configuration/_dict_config.py
--rw-r--r--   0        0        0     1626 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/exceptions.py
--rw-r--r--   0        0        0       34 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/helpers/__init__.py
--rw-r--r--   0        0        0     4026 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/helpers/_catalog.py
--rw-r--r--   0        0        0      369 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/helpers/_classproperty.py
--rw-r--r--   0        0        0      380 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/helpers/_compat.py
--rw-r--r--   0        0        0    10798 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/helpers/_flattening.py
--rw-r--r--   0        0        0     1064 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/helpers/_secrets.py
--rw-r--r--   0        0        0    21794 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/helpers/_simpleeval.py
--rw-r--r--   0        0        0     9175 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/helpers/_singer.py
--rw-r--r--   0        0        0     9652 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/helpers/_state.py
--rw-r--r--   0        0        0     8418 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/helpers/_typing.py
--rw-r--r--   0        0        0      846 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/helpers/_util.py
--rw-r--r--   0        0        0     6240 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/helpers/capabilities.py
--rw-r--r--   0        0        0      995 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/helpers/jsonpath.py
--rw-r--r--   0        0        0     4010 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/io_base.py
--rw-r--r--   0        0        0    23826 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/mapper.py
--rw-r--r--   0        0        0     4920 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/mapper_base.py
--rw-r--r--   0        0        0    14046 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/plugin_base.py
--rw-r--r--   0        0        0        0 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/py.typed
--rw-r--r--   0        0        0      316 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/sinks/__init__.py
--rw-r--r--   0        0        0     2965 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/sinks/batch.py
--rw-r--r--   0        0        0    13266 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/sinks/core.py
--rw-r--r--   0        0        0     1829 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/sinks/record.py
--rw-r--r--   0        0        0     8989 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/sinks/sql.py
--rw-r--r--   0        0        0      354 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/streams/__init__.py
--rw-r--r--   0        0        0    40758 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/streams/core.py
--rw-r--r--   0        0        0     2599 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/streams/graphql.py
--rw-r--r--   0        0        0    20330 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/streams/rest.py
--rw-r--r--   0        0        0    34913 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/streams/sql.py
--rw-r--r--   0        0        0    19483 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/tap_base.py
--rw-r--r--   0        0        0    19034 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/target_base.py
--rw-r--r--   0        0        0     5828 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/testing.py
--rw-r--r--   0        0        0    16170 2022-08-05 22:39:33.911381 singer-sdk-0.8.0/singer_sdk/typing.py
--rw-r--r--   0        0        0     3717 2022-08-05 22:39:45.759347 singer-sdk-0.8.0/setup.py
--rw-r--r--   0        0        0     4555 2022-08-05 22:39:45.759884 singer-sdk-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11337 2022-08-24 21:47:17.737385 singer-sdk-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2230 2022-08-24 21:47:17.737385 singer-sdk-0.9.0/README.md
+-rw-r--r--   0        0        0     4516 2022-08-24 21:47:17.741385 singer-sdk-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      733 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/__init__.py
+-rw-r--r--   0        0        0    16861 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/authenticators.py
+-rw-r--r--   0        0        0       51 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/cli/__init__.py
+-rw-r--r--   0        0        0      815 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/cli/common_options.py
+-rw-r--r--   0        0        0       42 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/configuration/__init__.py
+-rw-r--r--   0        0        0     3247 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/configuration/_dict_config.py
+-rw-r--r--   0        0        0     1626 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/exceptions.py
+-rw-r--r--   0        0        0       34 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/helpers/__init__.py
+-rw-r--r--   0        0        0     4026 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/helpers/_catalog.py
+-rw-r--r--   0        0        0      369 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/helpers/_classproperty.py
+-rw-r--r--   0        0        0      380 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/helpers/_compat.py
+-rw-r--r--   0        0        0    10798 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/helpers/_flattening.py
+-rw-r--r--   0        0        0     3082 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/helpers/_schema.py
+-rw-r--r--   0        0        0     1064 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/helpers/_secrets.py
+-rw-r--r--   0        0        0    21794 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/helpers/_simpleeval.py
+-rw-r--r--   0        0        0     9201 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/helpers/_singer.py
+-rw-r--r--   0        0        0     9652 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/helpers/_state.py
+-rw-r--r--   0        0        0     8418 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/helpers/_typing.py
+-rw-r--r--   0        0        0      846 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/helpers/_util.py
+-rw-r--r--   0        0        0     6240 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/helpers/capabilities.py
+-rw-r--r--   0        0        0      995 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/helpers/jsonpath.py
+-rw-r--r--   0        0        0     4010 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/io_base.py
+-rw-r--r--   0        0        0    23826 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/mapper.py
+-rw-r--r--   0        0        0     4920 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/mapper_base.py
+-rw-r--r--   0        0        0    14046 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/plugin_base.py
+-rw-r--r--   0        0        0        0 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/py.typed
+-rw-r--r--   0        0        0      316 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/sinks/__init__.py
+-rw-r--r--   0        0        0     2965 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/sinks/batch.py
+-rw-r--r--   0        0        0    13266 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/sinks/core.py
+-rw-r--r--   0        0        0     1829 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/sinks/record.py
+-rw-r--r--   0        0        0     9598 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/sinks/sql.py
+-rw-r--r--   0        0        0      354 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/streams/__init__.py
+-rw-r--r--   0        0        0    42017 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/streams/core.py
+-rw-r--r--   0        0        0     2599 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/streams/graphql.py
+-rw-r--r--   0        0        0    21074 2022-08-24 21:47:17.749385 singer-sdk-0.9.0/singer_sdk/streams/rest.py
+-rw-r--r--   0        0        0    34946 2022-08-24 21:47:17.753385 singer-sdk-0.9.0/singer_sdk/streams/sql.py
+-rw-r--r--   0        0        0    19483 2022-08-24 21:47:17.753385 singer-sdk-0.9.0/singer_sdk/tap_base.py
+-rw-r--r--   0        0        0    19034 2022-08-24 21:47:17.753385 singer-sdk-0.9.0/singer_sdk/target_base.py
+-rw-r--r--   0        0        0     5828 2022-08-24 21:47:17.753385 singer-sdk-0.9.0/singer_sdk/testing.py
+-rw-r--r--   0        0        0    16170 2022-08-24 21:47:17.753385 singer-sdk-0.9.0/singer_sdk/typing.py
+-rw-r--r--   0        0        0     3768 2022-08-24 21:47:35.877102 singer-sdk-0.9.0/setup.py
+-rw-r--r--   0        0        0     4628 2022-08-24 21:47:35.877513 singer-sdk-0.9.0/PKG-INFO
```

### Comparing `singer-sdk-0.8.0/LICENSE` & `singer-sdk-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/README.md` & `singer-sdk-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/__init__.py` & `singer-sdk-0.9.0/singer_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/authenticators.py` & `singer-sdk-0.9.0/singer_sdk/authenticators.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,26 @@
         """Get query parameters.
 
         Returns:
             URL query parameters for authentication.
         """
         return self._auth_params or {}
 
+    def authenticate_request(self, request: requests.Request) -> None:
+        """Authenticate a request.
+
+        Args:
+            request: A `request object`_.
+
+        .. _request object:
+            https://requests.readthedocs.io/en/latest/api/#requests.Request
+        """
+        request.headers.update(self.auth_headers)
+        request.params.update(self.auth_params)
+
 
 class SimpleAuthenticator(APIAuthenticatorBase):
     """DEPRECATED: Please use a more specific authenticator.
 
     This authenticator will merge a key-value pair to the stream
     in either the request headers or query parameters.
     """
```

### Comparing `singer-sdk-0.8.0/singer_sdk/cli/common_options.py` & `singer-sdk-0.9.0/singer_sdk/cli/common_options.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/configuration/_dict_config.py` & `singer-sdk-0.9.0/singer_sdk/configuration/_dict_config.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/exceptions.py` & `singer-sdk-0.9.0/singer_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/helpers/_catalog.py` & `singer-sdk-0.9.0/singer_sdk/helpers/_catalog.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/helpers/_flattening.py` & `singer-sdk-0.9.0/singer_sdk/helpers/_flattening.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/helpers/_secrets.py` & `singer-sdk-0.9.0/singer_sdk/helpers/_secrets.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/helpers/_simpleeval.py` & `singer-sdk-0.9.0/singer_sdk/helpers/_simpleeval.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/helpers/_singer.py` & `singer-sdk-0.9.0/singer_sdk/helpers/_singer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 from dataclasses import dataclass, fields
 from enum import Enum
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union, cast
 
 from singer.catalog import Catalog as BaseCatalog
 from singer.catalog import CatalogEntry as BaseCatalogEntry
-from singer.schema import Schema
+
+from singer_sdk.helpers._schema import SchemaPlus
 
 Breadcrumb = Tuple[str, ...]
 
 logger = logging.getLogger(__name__)
 
 
 class SelectionMask(Dict[Breadcrumb, bool]):
@@ -206,15 +207,15 @@
 
 @dataclass
 class CatalogEntry(BaseCatalogEntry):
     """Singer catalog entry."""
 
     tap_stream_id: str
     metadata: MetadataMapping
-    schema: Schema
+    schema: SchemaPlus
     stream: Optional[str] = None
     key_properties: Optional[List[str]] = None
     replication_key: Optional[str] = None
     is_view: Optional[bool] = None
     database: Optional[str] = None
     table: Optional[str] = None
     row_count: Optional[int] = None
@@ -227,15 +228,15 @@
         return cls(
             tap_stream_id=stream["tap_stream_id"],
             stream=stream.get("stream"),
             replication_key=stream.get("replication_key"),
             key_properties=stream.get("key_properties"),
             database=stream.get("database_name"),
             table=stream.get("table_name"),
-            schema=Schema.from_dict(stream.get("schema", {})),
+            schema=SchemaPlus.from_dict(stream.get("schema", {})),
             is_view=stream.get("is_view"),
             stream_alias=stream.get("stream_alias"),
             metadata=MetadataMapping.from_iterable(stream.get("metadata", [])),
             replication_method=stream.get("replication_method"),
         )
 
     def to_dict(self):
```

### Comparing `singer-sdk-0.8.0/singer_sdk/helpers/_state.py` & `singer-sdk-0.9.0/singer_sdk/helpers/_state.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/helpers/_typing.py` & `singer-sdk-0.9.0/singer_sdk/helpers/_typing.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/helpers/_util.py` & `singer-sdk-0.9.0/singer_sdk/helpers/_util.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/helpers/capabilities.py` & `singer-sdk-0.9.0/singer_sdk/helpers/capabilities.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/helpers/jsonpath.py` & `singer-sdk-0.9.0/singer_sdk/helpers/jsonpath.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/io_base.py` & `singer-sdk-0.9.0/singer_sdk/io_base.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/mapper.py` & `singer-sdk-0.9.0/singer_sdk/mapper.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/mapper_base.py` & `singer-sdk-0.9.0/singer_sdk/mapper_base.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/plugin_base.py` & `singer-sdk-0.9.0/singer_sdk/plugin_base.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/sinks/batch.py` & `singer-sdk-0.9.0/singer_sdk/sinks/batch.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/sinks/core.py` & `singer-sdk-0.9.0/singer_sdk/sinks/core.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/sinks/record.py` & `singer-sdk-0.9.0/singer_sdk/sinks/record.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/sinks/sql.py` & `singer-sdk-0.9.0/singer_sdk/sinks/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Sink classes load data to SQL targets."""
 
+from textwrap import dedent
 from typing import Any, Dict, Iterable, List, Optional, Type
 
 import sqlalchemy
 from pendulum import now
 from sqlalchemy.sql.expression import bindparam
 
 from singer_sdk.plugin_base import PluginBase
@@ -158,14 +159,39 @@
             schema=schema,
             as_temp_table=as_temp_table,
         )
         self.bulk_insert_records(
             full_table_name=full_table_name, schema=schema, records=records
         )
 
+    def generate_insert_statement(
+        self,
+        full_table_name: str,
+        schema: dict,
+    ) -> str:
+        """Generate an insert statement for the given records.
+
+        Args:
+            full_table_name: the target table name.
+            schema: the JSON schema for the new table.
+
+        Returns:
+            An insert statement.
+        """
+        property_names = list(schema["properties"].keys())
+        statement = dedent(
+            f"""\
+            INSERT INTO {full_table_name}
+            ({", ".join(property_names)})
+            VALUES ({", ".join([f":{name}" for name in property_names])})
+            """
+        )
+
+        return statement.rstrip()
+
     def bulk_insert_records(
         self,
         full_table_name: str,
         schema: dict,
         records: Iterable[Dict[str, Any]],
     ) -> Optional[int]:
         """Bulk insert records to an existing destination table.
@@ -179,23 +205,21 @@
             schema: the JSON schema for the new table, to be used when inferring column
                 names.
             records: the input records.
 
         Returns:
             True if table exists, False if not, None if unsure or undetectable.
         """
-        property_names = list(schema["properties"].keys())
-        insert_sql = sqlalchemy.text(
-            f"INSERT INTO {full_table_name} "
-            f"({', '.join([n for n in property_names])})"
-            f" VALUES "
-            f"({', '.join([':' + n for n in property_names])})"
+        insert_sql = self.generate_insert_statement(
+            full_table_name,
+            schema,
         )
+        self.logger.info("Inserting with SQL: %s", insert_sql)
         self.connector.connection.execute(
-            insert_sql,
+            sqlalchemy.text(insert_sql),
             records,
         )
         if isinstance(records, list):
             return len(records)  # If list, we can quickly return record count.
 
         return None  # Unknown record count.
```

### Comparing `singer-sdk-0.8.0/singer_sdk/streams/core.py` & `singer-sdk-0.9.0/singer_sdk/streams/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
     Union,
     cast,
 )
 
 import pendulum
 import requests
 import singer
-from singer import RecordMessage, SchemaMessage, StateMessage
-from singer.schema import Schema
+from singer import RecordMessage, Schema, SchemaMessage, StateMessage
 
 from singer_sdk.exceptions import InvalidStreamSortException, MaxRecordsLimitException
 from singer_sdk.helpers._catalog import pop_deselected_record_properties
 from singer_sdk.helpers._compat import final
 from singer_sdk.helpers._flattening import get_flattening_options
+from singer_sdk.helpers._schema import SchemaPlus
 from singer_sdk.helpers._singer import (
     Catalog,
     CatalogEntry,
     MetadataMapping,
     SelectionMask,
 )
 from singer_sdk.helpers._state import (
@@ -300,14 +300,37 @@
         """
         if not value:
             return
 
         state = self.get_context_state(context)
         write_replication_key_signpost(state, value)
 
+    def compare_start_date(self, value: str, start_date_value: str) -> str:
+        """Compare a bookmark value to a start date and return the most recent value.
+
+        If the replication key is a datetime-formatted string, this method will parse
+        the value and compare it to the start date. Otherwise, the bookmark value is
+        returned.
+
+        If the tap uses a non-datetime replication key (e.g. an UNIX timestamp), the
+        developer is encouraged to override this method to provide custom logic for
+        comparing the bookmark value to the start date.
+
+        Args:
+            value: The replication key value.
+            start_date_value: The start date value from the config.
+
+        Returns:
+            The most recent value between the bookmark and start date.
+        """
+        if self.is_timestamp_replication_key:
+            return max(value, start_date_value, key=pendulum.parse)
+        else:
+            return value
+
     def _write_starting_replication_value(self, context: Optional[dict]) -> None:
         """Write the starting replication value, if available.
 
         Args:
             context: Stream partition or context dictionary.
         """
         value = None
@@ -316,16 +339,21 @@
         if self.replication_key:
             replication_key_value = state.get("replication_key_value")
             if replication_key_value and self.replication_key == state.get(
                 "replication_key"
             ):
                 value = replication_key_value
 
-            elif "start_date" in self.config:
-                value = self.config["start_date"]
+            # Use start_date if it is more recent than the replication_key state
+            start_date_value: Optional[str] = self.config.get("start_date")
+            if start_date_value:
+                if not value:
+                    value = start_date_value
+                else:
+                    value = self.compare_start_date(value, start_date_value)
 
         write_starting_replication_value(state, value)
 
     def get_replication_key_signpost(
         self, context: Optional[dict]
     ) -> Optional[Union[datetime.datetime, Any]]:
         """Get the replication signpost.
@@ -498,15 +526,15 @@
 
         Returns:
             TODO
         """
         return CatalogEntry(
             tap_stream_id=self.tap_stream_id,
             stream=self.name,
-            schema=Schema.from_dict(self.schema),
+            schema=SchemaPlus.from_dict(self.schema),
             metadata=self.metadata,
             key_properties=self.primary_keys or [],
             replication_key=self.replication_key,
             replication_method=self.replication_method,
             is_view=None,
             database=None,
             table=None,
```

### Comparing `singer-sdk-0.8.0/singer_sdk/streams/graphql.py` & `singer-sdk-0.9.0/singer_sdk/streams/graphql.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/streams/rest.py` & `singer-sdk-0.9.0/singer_sdk/streams/rest.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     def requests_session(self) -> requests.Session:
         """Get requests session.
 
         Returns:
             The `requests.Session`_ object for HTTP requests.
 
         .. _requests.Session:
-            https://docs.python-requests.org/en/latest/api/#request-sessions
+            https://requests.readthedocs.io/en/latest/api/#request-sessions
         """
         if not self._requests_session:
             self._requests_session = requests.Session()
         return self._requests_session
 
     def validate_response(self, response: requests.Response) -> None:
         """Validate HTTP response.
@@ -155,15 +155,15 @@
             response: A `requests.Response`_ object.
 
         Raises:
             FatalAPIError: If the request is not retriable.
             RetriableAPIError: If the request is retriable.
 
         .. _requests.Response:
-            https://docs.python-requests.org/en/latest/api/#requests.Response
+            https://requests.readthedocs.io/en/latest/api/#requests.Response
         """
         if (
             response.status_code in self.extra_retry_statuses
             or 500 <= response.status_code < 600
         ):
             msg = self.response_error_message(response)
             raise RetriableAPIError(msg, response)
@@ -209,14 +209,15 @@
             A decorated method.
         """
         decorator: Callable = backoff.on_exception(
             self.backoff_wait_generator,
             (
                 RetriableAPIError,
                 requests.exceptions.ReadTimeout,
+                requests.exceptions.ConnectionError,
             ),
             max_tries=self.backoff_max_tries,
             on_backoff=self.backoff_handler,
         )(func)
         return decorator
 
     def _request(
@@ -259,18 +260,47 @@
                 next page of data.
 
         Returns:
             Dictionary of URL query parameters to use in the request.
         """
         return {}
 
+    def build_prepared_request(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> requests.PreparedRequest:
+        """Build a generic but authenticated request.
+
+        Uses the authenticator instance to mutate the request with authentication.
+
+        Args:
+            *args: Arguments to pass to `requests.Request`_.
+            **kwargs: Keyword arguments to pass to `requests.Request`_.
+
+        Returns:
+            A `requests.PreparedRequest`_ object.
+
+        .. _requests.PreparedRequest:
+            https://requests.readthedocs.io/en/latest/api/#requests.PreparedRequest
+        .. _requests.Request:
+            https://requests.readthedocs.io/en/latest/api/#requests.Request
+        """
+        request = requests.Request(*args, **kwargs)
+
+        if self.authenticator:
+            authenticator = self.authenticator
+            authenticator.authenticate_request(request)
+
+        return self.requests_session.prepare_request(request)
+
     def prepare_request(
         self, context: dict | None, next_page_token: _TToken | None
     ) -> requests.PreparedRequest:
-        """Prepare a request object.
+        """Prepare a request object for this stream.
 
         If partitioning is supported, the `context` object will contain the partition
         definitions. Pagination information can be parsed from `next_page_token` if
         `next_page_token` is not None.
 
         Args:
             context: Stream partition or context dictionary.
@@ -283,29 +313,21 @@
         """
         http_method = self.rest_method
         url: str = self.get_url(context)
         params: dict = self.get_url_params(context, next_page_token)
         request_data = self.prepare_request_payload(context, next_page_token)
         headers = self.http_headers
 
-        authenticator = self.authenticator
-        if authenticator:
-            headers.update(authenticator.auth_headers or {})
-            params.update(authenticator.auth_params or {})
-
-        request = self.requests_session.prepare_request(
-            requests.Request(
-                method=http_method,
-                url=url,
-                params=params,
-                headers=headers,
-                json=request_data,
-            ),
+        return self.build_prepared_request(
+            method=http_method,
+            url=url,
+            params=params,
+            headers=headers,
+            json=request_data,
         )
-        return request
 
     def request_records(self, context: dict | None) -> Iterable[dict]:
         """Request records from REST endpoint(s), returning response records.
 
         If pagination is detected, pages will be recursed automatically.
 
         Args:
@@ -430,15 +452,15 @@
             response: A raw `requests.Response`_ object.
             previous_token: Previous pagination reference.
 
         Returns:
             Reference value to retrieve next page.
 
         .. _requests.Response:
-            https://docs.python-requests.org/en/latest/api/#requests.Response
+            https://requests.readthedocs.io/en/latest/api/#requests.Response
         """
         if self.next_page_token_jsonpath:
             all_matches = extract_jsonpath(
                 self.next_page_token_jsonpath, response.json()
             )
             first_match = next(iter(all_matches), None)
             next_page_token = first_match
@@ -499,15 +521,15 @@
         Args:
             response: A raw `requests.Response`_ object.
 
         Yields:
             One item for every item found in the response.
 
         .. _requests.Response:
-            https://docs.python-requests.org/en/latest/api/#requests.Response
+            https://requests.readthedocs.io/en/latest/api/#requests.Response
         """
         yield from extract_jsonpath(self.records_jsonpath, input=response.json())
 
     # Abstract methods:
 
     @property
     def authenticator(self) -> APIAuthenticatorBase | None:
```

### Comparing `singer-sdk-0.8.0/singer_sdk/streams/sql.py` & `singer-sdk-0.9.0/singer_sdk/streams/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import abc
 import logging
 from datetime import datetime
 from functools import lru_cache
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Type, Union, cast
 
-import singer
 import sqlalchemy
 from sqlalchemy.engine import Engine
 from sqlalchemy.engine.reflection import Inspector
 
 from singer_sdk import typing as th
 from singer_sdk.exceptions import ConfigValidationError
+from singer_sdk.helpers._schema import SchemaPlus
 from singer_sdk.helpers._singer import CatalogEntry, MetadataMapping
 from singer_sdk.plugin_base import PluginBase as TapBaseClass
 from singer_sdk.streams.core import Stream
 
 
 class SQLConnector:
     """Base class for SQLAlchemy-based connectors.
@@ -397,15 +397,15 @@
 
         # Create the catalog entry object
         catalog_entry = CatalogEntry(
             tap_stream_id=unique_stream_id,
             stream=unique_stream_id,
             table=table_name,
             key_properties=key_properties,
-            schema=singer.Schema.from_dict(schema),
+            schema=SchemaPlus.from_dict(schema),
             is_view=is_view,
             replication_method=replication_method,
             metadata=MetadataMapping.get_standard_metadata(
                 schema_name=schema_name,
                 schema=schema,
                 replication_method=replication_method,
                 key_properties=key_properties,
```

### Comparing `singer-sdk-0.8.0/singer_sdk/tap_base.py` & `singer-sdk-0.9.0/singer_sdk/tap_base.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/target_base.py` & `singer-sdk-0.9.0/singer_sdk/target_base.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/testing.py` & `singer-sdk-0.9.0/singer_sdk/testing.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/singer_sdk/typing.py` & `singer-sdk-0.9.0/singer_sdk/typing.py`

 * *Files identical despite different names*

### Comparing `singer-sdk-0.8.0/setup.py` & `singer-sdk-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,19 +29,20 @@
  'typing-extensions>=4.2.0,<5.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata'],
  'docs': ['sphinx>=4.5,<6.0',
           'sphinx-rtd-theme>=0.5.2,<1.1.0',
           'sphinx-copybutton>=0.3.1,<0.6.0',
-          'myst-parser>=0.17.2,<0.19.0']}
+          'myst-parser>=0.17.2,<0.19.0',
+          'sphinx-autobuild>=2021.3.14,<2022.0.0']}
 
 setup_kwargs = {
     'name': 'singer-sdk',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'A framework for building Singer taps',
     'long_description': '# Meltano SDK for Taps and Targets\n\n[![Python Versions](https://img.shields.io/pypi/pyversions/singer-sdk)](https://pypi.org/project/singer-sdk)\n[![Downloads](https://img.shields.io/pypi/dw/singer-sdk?color=blue)](https://pypi.org/project/singer-sdk)\n[![PyPI Version](https://img.shields.io/pypi/v/singer-sdk?color=blue)](https://pypi.org/project/singer-sdk)\n[![Documentation Status](https://readthedocs.org/projects/meltano-sdk/badge/?version=latest)](https://sdk.meltano.com/en/latest/?badge=latest)\n[![codecov](https://codecov.io/gh/meltano/sdk/branch/main/graph/badge.svg?token=kS1zkemAgo)](https://codecov.io/gh/meltano/sdk)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/meltano/sdk/main.svg)](https://results.pre-commit.ci/latest/github/meltano/sdk/main)\n\nThe Tap and Target SDKs are the fastest way to build custom data extractors and loaders!\nTaps and targets built on the SDK are automatically compliant with the\n[Singer Spec](https://hub.meltano.com/singer/spec), the\nde-facto open source standard for extract and load pipelines.\n\n## Future-proof extractors and loaders, with less code\n\nOn average, developers tell us that they write about 70% less code by using the SDK, which\nmakes learning the SDK a great investment. Furthermore, as new features and capabilities\nare added to the SDK, your taps and targets can always take advantage of the latest\ncapabilities and bug fixes, simply by updating your SDK dependency to the latest version.\n\n## Documentation\n\n- See our [online documentation](https://sdk.meltano.com) for instructions on how\nto get started with the SDK.\n\n## Contributing back to the SDK\n\n- For more information on how to contribute, see our [Contributors Guide](https://sdk.meltano.com/en/latest/CONTRIBUTING.html).\n\n## Making a new release of the SDK\n\n1. Trigger a version bump [using the GitHub web UI](https://github.com/edgarrmondragon/sdk/actions/workflows/version_bump.yml) or the cli:\n\n   ```console\n   $ gh workflow run\n   ```\n\n   The `increment: auto` option will figure out the most appropriate bump based on commit history.\n\n1. Follow the checklist in the PR description.\n\n1. Publish a new release [using the GitHub web UI](https://github.com/meltano/sdk/releases/new).\n',
     'author': 'Meltano Team and Contributors',
     'author_email': None,
     'maintainer': 'Meltano Team and Contributors',
     'maintainer_email': None,
     'url': 'https://sdk.meltano.com/en/latest/',
```

### Comparing `singer-sdk-0.8.0/PKG-INFO` & `singer-sdk-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singer-sdk
-Version: 0.8.0
+Version: 0.9.0
 Summary: A framework for building Singer taps
 Home-page: https://sdk.meltano.com/en/latest/
 License: Apache 2.0
 Keywords: Meltano,Meltano SDK,ELT
 Author: Meltano Team and Contributors
 Maintainer: Meltano Team and Contributors
 Requires-Python: >=3.7.1,<3.11
@@ -32,14 +32,15 @@
 Requires-Dist: memoization (>=0.3.2,<0.5.0)
 Requires-Dist: myst-parser (>=0.17.2,<0.19.0); extra == "docs"
 Requires-Dist: pendulum (>=2.1.0,<3.0.0)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: sphinx (>=4.5,<6.0); extra == "docs"
+Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0); extra == "docs"
 Requires-Dist: sphinx-copybutton (>=0.3.1,<0.6.0); extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=0.5.2,<1.1.0); extra == "docs"
 Requires-Dist: sqlalchemy (>=1.4,<2.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
 Project-URL: Changelog, https://github.com/meltano/sdk/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://sdk.meltano.com/en/latest/
 Project-URL: Issue Tracker, https://github.com/meltano/sdk/issues
```

