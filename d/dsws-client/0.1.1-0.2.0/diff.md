# Comparing `tmp/dsws_client-0.1.1.tar.gz` & `tmp/dsws_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsws_client-0.1.1.tar", max compression
+gzip compressed data, was "dsws_client-0.2.0.tar", max compression
```

## Comparing `dsws_client-0.1.1.tar` & `dsws_client-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      753 2023-05-02 12:09:18.233705 dsws_client-0.1.1/README.md
--rw-r--r--   0        0        0      252 2023-05-02 12:09:18.233705 dsws_client-0.1.1/dsws_client/__init__.py
--rw-r--r--   0        0        0    10015 2023-05-02 12:09:18.233705 dsws_client-0.1.1/dsws_client/client.py
--rw-r--r--   0        0        0     1139 2023-05-02 12:09:18.233705 dsws_client-0.1.1/dsws_client/config.py
--rw-r--r--   0        0        0     2542 2023-05-02 12:09:18.233705 dsws_client-0.1.1/dsws_client/converters.py
--rw-r--r--   0        0        0    11641 2023-05-02 12:09:18.233705 dsws_client-0.1.1/dsws_client/ds_request.py
--rw-r--r--   0        0        0     3233 2023-05-02 12:09:18.233705 dsws_client-0.1.1/dsws_client/ds_response.py
--rw-r--r--   0        0        0      510 2023-05-02 12:09:18.233705 dsws_client-0.1.1/dsws_client/exceptions.py
--rw-r--r--   0        0        0     7558 2023-05-02 12:09:18.233705 dsws_client-0.1.1/dsws_client/parse.py
--rw-r--r--   0        0        0        0 2023-05-02 12:09:18.233705 dsws_client-0.1.1/dsws_client/py.typed
--rw-r--r--   0        0        0      436 2023-05-02 12:09:18.233705 dsws_client-0.1.1/dsws_client/utils.py
--rw-r--r--   0        0        0      488 2023-05-02 12:09:18.233705 dsws_client-0.1.1/dsws_client/value_objects/__init__.py
--rw-r--r--   0        0        0     1603 2023-05-02 12:09:18.233705 dsws_client-0.1.1/dsws_client/value_objects/enums.py
--rw-r--r--   0        0        0      266 2023-05-02 12:09:18.233705 dsws_client-0.1.1/dsws_client/value_objects/types.py
--rw-r--r--   0        0        0       77 2023-05-02 12:09:18.233705 dsws_client-0.1.1/dsws_client/version.py
--rw-r--r--   0        0        0     3568 2023-05-02 12:09:18.233705 dsws_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 dsws_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      753 2023-05-02 19:28:09.498046 dsws_client-0.2.0/README.md
+-rw-r--r--   0        0        0      319 2023-05-02 19:28:09.498046 dsws_client-0.2.0/dsws_client/__init__.py
+-rw-r--r--   0        0        0    10015 2023-05-02 19:28:09.498046 dsws_client-0.2.0/dsws_client/client.py
+-rw-r--r--   0        0        0     1139 2023-05-02 19:28:09.498046 dsws_client-0.2.0/dsws_client/config.py
+-rw-r--r--   0        0        0     2542 2023-05-02 19:28:09.498046 dsws_client-0.2.0/dsws_client/converters.py
+-rw-r--r--   0        0        0    11641 2023-05-02 19:28:09.498046 dsws_client-0.2.0/dsws_client/ds_request.py
+-rw-r--r--   0        0        0     3233 2023-05-02 19:28:09.498046 dsws_client-0.2.0/dsws_client/ds_response.py
+-rw-r--r--   0        0        0      510 2023-05-02 19:28:09.498046 dsws_client-0.2.0/dsws_client/exceptions.py
+-rw-r--r--   0        0        0     8009 2023-05-02 19:28:09.498046 dsws_client-0.2.0/dsws_client/parse.py
+-rw-r--r--   0        0        0        0 2023-05-02 19:28:09.498046 dsws_client-0.2.0/dsws_client/py.typed
+-rw-r--r--   0        0        0      436 2023-05-02 19:28:09.498046 dsws_client-0.2.0/dsws_client/utils.py
+-rw-r--r--   0        0        0      488 2023-05-02 19:28:09.498046 dsws_client-0.2.0/dsws_client/value_objects/__init__.py
+-rw-r--r--   0        0        0     1603 2023-05-02 19:28:09.498046 dsws_client-0.2.0/dsws_client/value_objects/enums.py
+-rw-r--r--   0        0        0      266 2023-05-02 19:28:09.498046 dsws_client-0.2.0/dsws_client/value_objects/types.py
+-rw-r--r--   0        0        0       77 2023-05-02 19:28:09.498046 dsws_client-0.2.0/dsws_client/version.py
+-rw-r--r--   0        0        0     3568 2023-05-02 19:28:09.498046 dsws_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 dsws_client-0.2.0/PKG-INFO
```

### Comparing `dsws_client-0.1.1/README.md` & `dsws_client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dsws_client-0.1.1/dsws_client/client.py` & `dsws_client-0.2.0/dsws_client/client.py`

 * *Files identical despite different names*

### Comparing `dsws_client-0.1.1/dsws_client/config.py` & `dsws_client-0.2.0/dsws_client/config.py`

 * *Files identical despite different names*

### Comparing `dsws_client-0.1.1/dsws_client/converters.py` & `dsws_client-0.2.0/dsws_client/converters.py`

 * *Files identical despite different names*

### Comparing `dsws_client-0.1.1/dsws_client/ds_request.py` & `dsws_client-0.2.0/dsws_client/ds_request.py`

 * *Files identical despite different names*

### Comparing `dsws_client-0.1.1/dsws_client/ds_response.py` & `dsws_client-0.2.0/dsws_client/ds_response.py`

 * *Files identical despite different names*

### Comparing `dsws_client-0.1.1/dsws_client/parse.py` & `dsws_client-0.2.0/dsws_client/parse.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,30 @@
 class Meta:
     """Meta object."""
 
     data_type_names: Dict[str, str] = attrs.field(factory=dict)
     symbol_names: Dict[str, str] = attrs.field(factory=dict)
     additional_responses: Dict[str, str] = attrs.field(factory=dict)
     tags: List[str] = attrs.field(factory=list)
+    currencies: Dict[str, Dict[str, Optional[str]]] = attrs.field(
+        factory=lambda: collections.defaultdict(dict)
+    )
+
+    def merge(self, other: "Meta") -> "Meta":
+        """Merge this meta object with another one."""
+        return Meta(
+            data_type_names={**self.data_type_names, **other.data_type_names},
+            symbol_names={**self.symbol_names, **other.symbol_names},
+            additional_responses={
+                **self.additional_responses,
+                **other.additional_responses,
+            },
+            tags=[*self.tags, *other.tags],
+            currencies={**self.currencies, **other.currencies},
+        )
 
 
 @attrs.define()
 class ParsedResponse:
     """Parsed response object."""
 
     records: List[Dict[str, Any]] = attrs.field(factory=list)
@@ -47,57 +63,55 @@
     responses: List[DSDataResponse],
     *,
     process_strings: bool = True,
 ) -> ParsedResponse:
     """Parse a list of DSDataResponse objects into a list of records."""
     parsed_response = ParsedResponse()
     for response in responses:
-        _parsed_response = parse(response, process_strings=process_strings)
+        _parsed_response = parse_response(response, process_strings=process_strings)
         parsed_response.records.extend(_parsed_response.records)
         parsed_response.errors.extend(_parsed_response.errors)
-        parsed_response.meta.data_type_names.update(
-            _parsed_response.meta.data_type_names
-        )
-        parsed_response.meta.symbol_names.update(_parsed_response.meta.symbol_names)
-        parsed_response.meta.additional_responses.update(
-            _parsed_response.meta.additional_responses
-        )
-        parsed_response.meta.tags.extend(_parsed_response.meta.tags)
+        parsed_response.meta = parsed_response.meta.merge(_parsed_response.meta)
     return parsed_response
 
 
-def parse(response: DSDataResponse, *, process_strings: bool = True) -> ParsedResponse:
+def parse_response(
+    response: DSDataResponse,
+    *,
+    process_strings: bool = True,
+) -> ParsedResponse:
     """Parse a DSDataResponse object into a list of records."""
     if response.dates is None:
         raise InvalidResponseError(
             "Response does not contain dates. Probably the request was invalid."
         )
     meta = parse_meta(response)
     records = collections.defaultdict(dict)
     errors = []
     for data_type_value in response.data_type_values:
         field = data_type_value.data_type
         for symbol_value in data_type_value.symbol_values:
-            update_record_dict(
+            meta.currencies[symbol_value.symbol][field] = symbol_value.currency
+            process_symbol_value(
                 records,
                 errors,
                 field,
                 response.dates,
                 symbol_value,
                 process_strings=process_strings,
             )
     record_list = []
     for (symbol, date), record in records.items():
         record["symbol"] = symbol
         record["date"] = date
         record_list.append(record)
-    return ParsedResponse(record_list, errors, meta=meta)
+    return ParsedResponse(record_list, errors, meta)
 
 
-def update_record_dict(
+def process_symbol_value(
     records: RecordDict,
     errors: List[Error],
     field: str,
     dates: List[dt.datetime],
     symbol_value: DSSymbolResponseValue,
     *,
     process_strings: bool,
@@ -122,15 +136,15 @@
             records[(symbol_value.symbol, date)][field] = xvalue
     else:
         if len(dates) > 1:
             raise InvalidResponseError("More than one date found for single value.")
         records[(symbol_value.symbol, dates[0])][field] = value
 
 
-def parse_meta(response: DSDataResponse) -> Dict[str, Any]:
+def parse_meta(response: DSDataResponse) -> Meta:
     """Parse meta information from a response."""
     meta = Meta()
     if response.data_type_names:
         meta.data_type_names = {
             kv_pair.key: kv_pair.value for kv_pair in response.data_type_names
         }
     if response.symbol_names:
```

### Comparing `dsws_client-0.1.1/dsws_client/value_objects/enums.py` & `dsws_client-0.2.0/dsws_client/value_objects/enums.py`

 * *Files identical despite different names*

### Comparing `dsws_client-0.1.1/pyproject.toml` & `dsws_client-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "dsws-client"
-version = "0.1.1"
+version = "0.2.0"
 description = "Python client for the Datastream Web Service API (DSWS)"
 authors = ["ljnsn <info@ljnsn.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "dsws_client"}]
 
 [tool.commitizen]
 name = "cz_gitmoji"
-version = "0.1.1"
+version = "0.2.0"
 version_files = ["pyproject.toml:^version"]
 tag_format = "v$version"
 bump_message = "🔖 bump(release): v$current_version → v$new_version"
 update_changelog_on_bump = true
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dsws_client-0.1.1/PKG-INFO` & `dsws_client-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsws-client
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python client for the Datastream Web Service API (DSWS)
 License: MIT
 Author: ljnsn
 Author-email: info@ljnsn.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

