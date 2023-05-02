# Comparing `tmp/jsonschema_gentypes-2.0.0.tar.gz` & `tmp/jsonschema_gentypes-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_gentypes-2.0.0.tar", max compression
+gzip compressed data, was "jsonschema_gentypes-2.1.0.tar", max compression
```

## Comparing `jsonschema_gentypes-2.0.0.tar` & `jsonschema_gentypes-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1304 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/LICENSE
--rw-r--r--   0        0        0     2428 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/README.md
--rw-r--r--   0        0        0    21740 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/__init__.py
--rw-r--r--   0        0        0    17139 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/api.py
--rw-r--r--   0        0        0    12886 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/api_draft_04.py
--rw-r--r--   0        0        0     1767 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/api_draft_06.py
--rw-r--r--   0        0        0      149 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/api_draft_07.py
--rw-r--r--   0        0        0     2999 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/api_draft_2019_09.py
--rw-r--r--   0        0        0     4296 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/api_draft_2020_12.py
--rw-r--r--   0        0        0     7328 2023-04-15 09:40:34.876489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/cli.py
--rw-r--r--   0        0        0     2538 2023-04-15 09:41:31.924517 jsonschema_gentypes-2.0.0/jsonschema_gentypes/configuration.py
--rw-r--r--   0        0        0     4982 2023-04-15 09:41:34.536516 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_04.py
--rw-r--r--   0        0        0     5251 2023-04-15 09:41:36.888514 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_06.py
--rw-r--r--   0        0        0     5481 2023-04-15 09:41:39.152513 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_07.py
--rw-r--r--   0        0        0     1698 2023-04-15 09:41:41.516512 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09.py
--rw-r--r--   0        0        0     1596 2023-04-15 09:41:48.024510 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py
--rw-r--r--   0        0        0      384 2023-04-15 09:41:54.484511 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_content.py
--rw-r--r--   0        0        0     1260 2023-04-15 09:41:43.672510 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_core.py
--rw-r--r--   0        0        0      296 2023-04-15 09:41:52.360511 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_format.py
--rw-r--r--   0        0        0      973 2023-04-15 09:41:45.848510 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py
--rw-r--r--   0        0        0     3019 2023-04-15 09:41:50.236511 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py
--rw-r--r--   0        0        0     2569 2023-04-15 09:41:57.064512 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12.py
--rw-r--r--   0        0        0     1691 2023-04-15 09:42:03.348514 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py
--rw-r--r--   0        0        0      384 2023-04-15 09:42:07.720515 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12_content.py
--rw-r--r--   0        0        0      859 2023-04-15 09:41:59.116513 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12_core.py
--rw-r--r--   0        0        0      973 2023-04-15 09:42:01.164513 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py
--rw-r--r--   0        0        0     3019 2023-04-15 09:42:05.572515 jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py
--rw-r--r--   0        0        0        0 2023-04-15 09:40:34.880489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/py.typed
--rw-r--r--   0        0        0     4133 2023-04-15 09:40:34.880489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/resolver.py
--rw-r--r--   0        0        0     3067 2023-04-15 09:40:34.880489 jsonschema_gentypes-2.0.0/jsonschema_gentypes/schema.json
--rw-r--r--   0        0        0     2514 2023-04-15 09:43:16.148113 jsonschema_gentypes-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3947 1970-01-01 00:00:00.000000 jsonschema_gentypes-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1304 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3358 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/README.md
+-rw-r--r--   0        0        0    21740 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/__init__.py
+-rw-r--r--   0        0        0    17327 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/api.py
+-rw-r--r--   0        0        0    12990 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_04.py
+-rw-r--r--   0        0        0     2574 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_06.py
+-rw-r--r--   0        0        0      149 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_07.py
+-rw-r--r--   0        0        0     3042 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_2019_09.py
+-rw-r--r--   0        0        0     4339 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_2020_12.py
+-rw-r--r--   0        0        0    15226 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/cli.py
+-rw-r--r--   0        0        0     2538 2023-05-02 14:37:22.874370 jsonschema_gentypes-2.1.0/jsonschema_gentypes/configuration.py
+-rw-r--r--   0        0        0     4982 2023-05-02 14:37:25.806417 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_04.py
+-rw-r--r--   0        0        0     5251 2023-05-02 14:37:28.478461 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_06.py
+-rw-r--r--   0        0        0     5481 2023-05-02 14:37:31.146504 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_07.py
+-rw-r--r--   0        0        0     1698 2023-05-02 14:37:33.790546 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09.py
+-rw-r--r--   0        0        0     1596 2023-05-02 14:37:41.358667 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py
+-rw-r--r--   0        0        0      384 2023-05-02 14:37:48.854789 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_content.py
+-rw-r--r--   0        0        0     1260 2023-05-02 14:37:36.302586 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_core.py
+-rw-r--r--   0        0        0      296 2023-05-02 14:37:46.378749 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_format.py
+-rw-r--r--   0        0        0      973 2023-05-02 14:37:38.822626 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py
+-rw-r--r--   0        0        0     3019 2023-05-02 14:37:43.906709 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py
+-rw-r--r--   0        0        0     2569 2023-05-02 14:37:51.830837 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12.py
+-rw-r--r--   0        0        0     1691 2023-05-02 14:37:59.450962 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py
+-rw-r--r--   0        0        0      384 2023-05-02 14:38:04.543085 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_content.py
+-rw-r--r--   0        0        0      859 2023-05-02 14:37:54.358878 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_core.py
+-rw-r--r--   0        0        0      973 2023-05-02 14:37:56.894920 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py
+-rw-r--r--   0        0        0     3019 2023-05-02 14:38:02.035009 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py
+-rw-r--r--   0        0        0        0 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/py.typed
+-rw-r--r--   0        0        0     5868 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/resolver.py
+-rw-r--r--   0        0        0     3067 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/schema.json
+-rw-r--r--   0        0        0     2514 2023-05-02 14:39:31.276556 jsonschema_gentypes-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4877 1970-01-01 00:00:00.000000 jsonschema_gentypes-2.1.0/PKG-INFO
```

### Comparing `jsonschema_gentypes-2.0.0/LICENSE` & `jsonschema_gentypes-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/README.md` & `jsonschema_gentypes-2.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -87,14 +87,49 @@
 ```yaml
 pre_commit:
   enabled: true
   arguments:
     - --color=never
 ```
 
+## OpenAPI3
+
+We can also generate types for OpenAPI3 schemas (automatically detected).
+
+The result of our example in `tests/openapi3.json` can be used in pyramid with for example:
+
+```python
+import pyramid.request
+from pyramid.view import view_config
+from openaoi3 import *
+
+def open_api(func):
+    def wrapper(request: pyramid.request.Request, **kwargs) -> Any:
+        typed_request = {}
+        try:
+            typed_request{'request_body'} = request.json
+        except Exception as e:
+            pass
+        typed_request{'path'} = request.matchdict
+        typed_request{'query'} = request.params
+
+        return = func(request, request_typed=typed_request, **kwargs)
+
+    return wrapper
+
+
+@view_config(route_name="route_name", renderer="json")
+@open_api
+def view(
+  request: pyramid.request.Request,
+  request_typed: OgcapiCollectionsCollectionidGet,
+) -> OgcapiCollectionsCollectionidGetResponse:
+    return {...}
+```
+
 ## Contributing
 
 Install the pre-commit hooks:
 
 ```bash
 pip install pre-commit
 pre-commit install --allow-missing-config
```

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/__init__.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/api.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,30 @@
 from jsonschema_gentypes.resolver import RefResolver
 
 # Raise issues here.
 ISSUE_URL = "https://github.com/camptcamp/jsonschema-gentypes"
 
 
 class API:
-    """
+    r"""
     Base class for JSON schema types API.
+
+    Call tree:
+      get_type()
+        |-> get_type_start()
+        |-> build_type()
+        |     |-> _resolve_ref()
+        |     |-> get_type()
+        |     |-> ref()
+        |     |-> any_of()
+        |     |-> enum()
+        |     |-> default()
+        |     \-> _get_type()
+        |           \-> get_type_handler()
+        \-> get_type_end()
     """
 
     def __init__(
         self,
         resolver: RefResolver,
         additional_properties: configuration.AdditionalProperties = configuration.ADDITIONALPROPERTIES_ONLY_EXPLICIT,
     ) -> None:
@@ -84,14 +98,15 @@
 
     def get_type_start(
         self,
         schema: Union[
             jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
         ],
         proxy: Type,
+        proposed_name: str,
     ) -> None:
         """
         Start getting the type for a schema.
         """
 
     def get_type_end(
         self,
@@ -134,17 +149,17 @@
                 assert self.root is not None
                 self.root.set_type(type_)
             return type_
         assert not isinstance(schema, bool)
 
         proxy = TypeProxy()
 
-        self.get_type_start(schema, proxy)
+        self.get_type_start(schema, proxy, proposed_name)
 
-        the_type = self._get_type_internal(schema, proposed_name)
+        the_type = self.build_type(schema, proposed_name)
         assert the_type is not None
         additional_description = the_type.comments()
         description = get_description(schema_meta_data)
         if description and additional_description:
             description.append("")
         description += additional_description
         if not isinstance(the_type, NamedType) and description:
@@ -178,44 +193,41 @@
         ],
     ) -> Union[jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020]:
         if "$ref" in schema:
             with self.resolver.resolving(schema["$ref"]) as resolved:  # type: ignore
                 schema.update(resolved)
         return schema
 
-    def _get_type_internal(
+    def build_type(
         self,
         schema: Union[
             jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
         ],
         proposed_name: str,
     ) -> Type:
-        """
-        Get a :class:`.Type` for a JSON schema.
-        """
+        """Get a :class:`.Type` for a JSON schema."""
 
         schema_meta_data = cast(
             Union[jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2019_09_meta_data.JSONSchemaItemD2019],
             schema,
         )
         schema_core = cast(
             Union[jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_core.JSONSchemaItemD2020],
             schema,
         )
-        schema_validation = cast(
-            Union[jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_validation.JSONSchemaItemD2020],
-            schema,
-        )
 
         proposed_name = schema_meta_data.get("title", proposed_name)
 
         if "if" in schema:
-            base_schema: Union[
-                jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
-            ] = {}
+            base_schema = cast(
+                Union[
+                    jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
+                ],
+                {},
+            )
             base_schema.update(schema)  # type: ignore
             for key in ("if", "then", "else", "title", "description"):
                 if key in base_schema:
                     del base_schema[key]  # type: ignore
             then_schema = cast(
                 Union[
                     jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
@@ -245,17 +257,20 @@
                         jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020,
                     ],
                     schema.get("if", {}),
                 )
             ).get("properties", {})
             assert if_properties
             then_properties.update(if_properties)  # type: ignore
-            else_schema: Union[
-                jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
-            ] = {}
+            else_schema = cast(
+                Union[
+                    jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
+                ],
+                {},
+            )
             else_schema.update(base_schema)  # type: ignore
             else_schema.update(
                 self._resolve_ref(  # type: ignore
                     cast(
                         Union[
                             jsonschema_draft_04.JSONSchemaD4,
                             jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020,
@@ -272,16 +287,22 @@
                     self.get_type(else_schema, proposed_name + " else"),
                 ],
             )
 
         if "$ref" in schema or "$recursiveRef" in schema or "$dynamicRef" in schema:
             return self.ref(schema_core, proposed_name)
 
-        if "const" in schema:
-            return self.const(schema, proposed_name)
+        schema_meta_data = cast(
+            Union[jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2019_09_meta_data.JSONSchemaItemD2019],
+            schema,
+        )
+        schema_validation = cast(
+            Union[jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_validation.JSONSchemaItemD2020],
+            schema,
+        )
 
         # 6.1.1. type
         # The value of this keyword MUST be either a string or an array. If it
         # is an array, elements of the array MUST be strings and MUST be
         # unique.
         #
         # String values MUST be one of the six primitive types ("null",
@@ -429,15 +450,15 @@
         self,
         schema: Union[jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_core.JSONSchemaItemD2020],
         proposed_name: str,
     ) -> Type:
         """
         Treat the ref keyword.
 
-        See: https://json-schema.org/understanding-json-schema/structuring.html.
+        See: https://json-schema.org/understanding-json-schema/structuring.html#ref.
         """
 
     @abstractmethod
     def any_of(
         self,
         schema: Union[
             jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
@@ -451,28 +472,14 @@
         """
         Treat the anyOf keyword.
 
         See: https://json-schema.org/understanding-json-schema/reference/combining.html#anyof.
         """
 
     @abstractmethod
-    def const(
-        self,
-        schema: Union[
-            jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
-        ],
-        proposed_name: str,
-    ) -> Type:
-        """
-        Treat the const  keyword.
-
-        See: https://json-schema.org/understanding-json-schema/reference/generic.html#constant-values
-        """
-
-    @abstractmethod
     def enum(
         self,
         schema: Union[
             jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_validation.JSONSchemaItemD2020
         ],
         proposed_name: str,
     ) -> Type:
```

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/api_draft_04.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_04.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,26 +27,14 @@
 
 
 class APIv4(API):
     """
     JSON Schema draft 4.
     """
 
-    def const(
-        self,
-        schema: Union[
-            jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
-        ],
-        proposed_name: str,
-    ) -> Type:
-        """
-        Generate a ``Literal`` for a const value.
-        """
-        raise NotImplementedError("const is not supported in draft 4")
-
     def enum(
         self,
         schema: Union[
             jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_validation.JSONSchemaItemD2020
         ],
         proposed_name: str,
     ) -> Type:
@@ -303,19 +291,31 @@
         if ref in self.ref_type:
             return self.ref_type[ref]
 
         resolve = getattr(self.resolver, "resolve", None)
         if resolve is None:
             resolved = self.resolver.lookup(ref)
             schema_casted.update(resolved)  # type: ignore
-            type_ = self.get_type(resolved, self.ref_to_proposed_name(ref))
+            resolved_all = cast(
+                Union[
+                    jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
+                ],
+                resolved,
+            )
+            type_ = self.get_type(resolved_all, self.ref_to_proposed_name(ref))
         else:
             resolved = self.resolver.lookup(ref)
             schema_casted.update(resolved)  # type: ignore
-            type_ = self.get_type(resolved, self.ref_to_proposed_name(ref))
+            resolved_all = cast(
+                Union[
+                    jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
+                ],
+                resolved,
+            )
+            type_ = self.get_type(resolved_all, self.ref_to_proposed_name(ref))
 
         if ref:
             self.ref_type[ref] = type_
         return type_
 
     def string(
         self,
```

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/api_draft_06.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_06.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
     def get_type_start(
         self,
         schema: Union[
             jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
         ],
         proxy: Type,
+        proposed_name: str,
     ) -> None:
         """
         Get the type for a schema.
         """
 
         schema_casted = cast(
             Union[
@@ -38,24 +39,49 @@
             schema,
         )
         property_names = schema_casted.get("propertyNames")
         if isinstance(property_names, dict) and "type" in property_names:
             property_names["__type__"] = property_names["type"]  # type: ignore
             del property_names["type"]  # type: ignore
 
-        super().get_type_start(schema, proxy)
+        super().get_type_start(schema, proxy, proposed_name)
 
-    def const(
+    def build_type(
         self,
         schema: Union[
             jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
         ],
         proposed_name: str,
     ) -> Type:
+        """Build a type for a schema."""
+
+        if "const" in schema:
+            return self.const(
+                cast(
+                    Union[
+                        jsonschema_draft_06.JSONSchemaItemD6,
+                        jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020,
+                    ],
+                    schema,
+                )
+            )
+
+        return super().build_type(schema, proposed_name)
+
+    def const(
+        self,
+        schema: Union[
+            jsonschema_draft_06.JSONSchemaItemD6, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
+        ],
+    ) -> Type:
         """
+        Treat the const  keyword.
+
+        See: https://json-schema.org/understanding-json-schema/reference/generic.html#constant-values
+
         Generate a ``Literal`` for a const value.
         """
 
         schema_casted = cast(
             Union[
                 jsonschema_draft_06.JSONSchemaItemD6, jsonschema_draft_2020_12_validation.JSONSchemaItemD2020
             ],
```

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/api_draft_2019_09.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_2019_09.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,27 +46,28 @@
 
     def get_type_start(
         self,
         schema: Union[
             jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
         ],
         proxy: Type,
+        proposed_name: str,
     ) -> None:
         """
         Get the type for a schema.
         """
 
         schema_core = cast(jsonschema_draft_2019_09_core.JSONSchemaItemD2019, schema)
 
         self.is_recursive_anchor_path.append(schema_core.get("$recursiveAnchor", False))
         if self.is_recursive_anchor_path[-1]:
             del schema_core["$recursiveAnchor"]
             self.recursive_anchor_path.append(proxy)
 
-        super().get_type_start(schema, proxy)
+        super().get_type_start(schema, proxy, proposed_name)
 
     def get_type_end(
         self,
         schema: Union[
             jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
         ],
         proxy: Type,
```

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/api_draft_2020_12.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_2020_12.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,26 +29,27 @@
 
     def get_type_start(
         self,
         schema: Union[
             jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
         ],
         proxy: Type,
+        proposed_name: str,
     ) -> None:
         """
         Get the type for a schema.
         """
 
         schema_core = cast(jsonschema_draft_2020_12_core.JSONSchemaItemD2020, schema)
 
         if "$dynamicAnchor" in schema_core:
             self.dynamic_anchor[schema_core["$dynamicAnchor"]] = proxy
             del schema_core["$dynamicAnchor"]
 
-        super().get_type_start(schema, proxy)
+        super().get_type_start(schema, proxy, proposed_name)
 
     def ref(
         self,
         schema: Union[jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_core.JSONSchemaItemD2020],
         proposed_name: str,
     ) -> Type:
         """
```

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/configuration.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/configuration.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_04.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_04.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_06.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_06.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_07.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_07.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_core.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_core.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12_core.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_core.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/jsonschema_gentypes/schema.json` & `jsonschema_gentypes-2.1.0/jsonschema_gentypes/schema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.0.0/pyproject.toml` & `jsonschema_gentypes-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 ignore_missing_imports = true
 strict = true
 
 [tool.poetry]
 name = "jsonschema-gentypes"
-version = "2.0.0"
+version = "2.1.0"
 description = "Tool to generate Python types based on TypedDict from a JSON Schema"
 readme = "README.md"
 authors = ["Camptocamp <info@camptocamp.com>"]
 repository = "https://github.com/camptocamp/jsonschema-gentypes"
 license = "BSD-2-Clause"
 keywords = ["jsonschema", "types"]
 packages = [{ include = "jsonschema_gentypes" }]
```

### Comparing `jsonschema_gentypes-2.0.0/PKG-INFO` & `jsonschema_gentypes-2.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-gentypes
-Version: 2.0.0
+Version: 2.1.0
 Summary: Tool to generate Python types based on TypedDict from a JSON Schema
 Home-page: https://github.com/camptocamp/jsonschema-gentypes
 License: BSD-2-Clause
 Keywords: jsonschema,types
 Author: Camptocamp
 Author-email: info@camptocamp.com
 Requires-Python: >=3.8,<4
@@ -127,14 +127,49 @@
 ```yaml
 pre_commit:
   enabled: true
   arguments:
     - --color=never
 ```
 
+## OpenAPI3
+
+We can also generate types for OpenAPI3 schemas (automatically detected).
+
+The result of our example in `tests/openapi3.json` can be used in pyramid with for example:
+
+```python
+import pyramid.request
+from pyramid.view import view_config
+from openaoi3 import *
+
+def open_api(func):
+    def wrapper(request: pyramid.request.Request, **kwargs) -> Any:
+        typed_request = {}
+        try:
+            typed_request{'request_body'} = request.json
+        except Exception as e:
+            pass
+        typed_request{'path'} = request.matchdict
+        typed_request{'query'} = request.params
+
+        return = func(request, request_typed=typed_request, **kwargs)
+
+    return wrapper
+
+
+@view_config(route_name="route_name", renderer="json")
+@open_api
+def view(
+  request: pyramid.request.Request,
+  request_typed: OgcapiCollectionsCollectionidGet,
+) -> OgcapiCollectionsCollectionidGetResponse:
+    return {...}
+```
+
 ## Contributing
 
 Install the pre-commit hooks:
 
 ```bash
 pip install pre-commit
 pre-commit install --allow-missing-config
```

