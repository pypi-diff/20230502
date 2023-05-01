# Comparing `tmp/py_to_proto-0.1.1-py39-none-any.whl.zip` & `tmp/py_to_proto-0.1.2-py39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 31362 bytes, number of entries: 15
--rw-r--r--  2.0 unx     1174 b- defN 23-Apr-27 02:58 py_to_proto/__init__.py
--rw-r--r--  2.0 unx      251 b- defN 23-Apr-27 02:58 py_to_proto/compat_annotated.py
--rw-r--r--  2.0 unx    26041 b- defN 23-Apr-27 02:58 py_to_proto/converter_base.py
--rw-r--r--  2.0 unx    11392 b- defN 23-Apr-27 02:58 py_to_proto/dataclass_to_proto.py
--rw-r--r--  2.0 unx     9686 b- defN 23-Apr-27 02:58 py_to_proto/descriptor_to_file.py
--rw-r--r--  2.0 unx     4799 b- defN 23-Apr-27 02:58 py_to_proto/descriptor_to_message_class.py
--rw-r--r--  2.0 unx     9092 b- defN 23-Apr-27 02:58 py_to_proto/json_to_service.py
--rw-r--r--  2.0 unx     8288 b- defN 23-Apr-27 02:58 py_to_proto/jtd_to_proto.py
--rw-r--r--  2.0 unx    12660 b- defN 23-Apr-27 02:58 py_to_proto/utils.py
--rw-r--r--  2.0 unx    14885 b- defN 23-Apr-27 02:58 py_to_proto/validation.py
--rw-r--r--  2.0 unx     1088 b- defN 23-Apr-27 02:59 py_to_proto-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6777 b- defN 23-Apr-27 02:59 py_to_proto-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Apr-27 02:59 py_to_proto-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-27 02:59 py_to_proto-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1272 b- defN 23-Apr-27 02:59 py_to_proto-0.1.1.dist-info/RECORD
-15 files, 107510 bytes uncompressed, 29256 bytes compressed:  72.8%
+Zip file size: 31558 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     1174 b- defN 23-May-01 23:14 py_to_proto/__init__.py
+-rw-r--r--  2.0 unx      251 b- defN 23-May-01 23:14 py_to_proto/compat_annotated.py
+-rw-r--r--  2.0 unx    26041 b- defN 23-May-01 23:14 py_to_proto/converter_base.py
+-rw-r--r--  2.0 unx    12097 b- defN 23-May-01 23:14 py_to_proto/dataclass_to_proto.py
+-rw-r--r--  2.0 unx     9686 b- defN 23-May-01 23:14 py_to_proto/descriptor_to_file.py
+-rw-r--r--  2.0 unx     4799 b- defN 23-May-01 23:14 py_to_proto/descriptor_to_message_class.py
+-rw-r--r--  2.0 unx     9092 b- defN 23-May-01 23:14 py_to_proto/json_to_service.py
+-rw-r--r--  2.0 unx     8288 b- defN 23-May-01 23:14 py_to_proto/jtd_to_proto.py
+-rw-r--r--  2.0 unx    12660 b- defN 23-May-01 23:14 py_to_proto/utils.py
+-rw-r--r--  2.0 unx    14885 b- defN 23-May-01 23:14 py_to_proto/validation.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-01 23:16 py_to_proto-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6777 b- defN 23-May-01 23:16 py_to_proto-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-May-01 23:16 py_to_proto-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-01 23:16 py_to_proto-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1272 b- defN 23-May-01 23:16 py_to_proto-0.1.2.dist-info/RECORD
+15 files, 108215 bytes uncompressed, 29452 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: py_to_proto/utils.py
 Comment: 
 
 Filename: py_to_proto/validation.py
 Comment: 
 
-Filename: py_to_proto-0.1.1.dist-info/LICENSE
+Filename: py_to_proto-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: py_to_proto-0.1.1.dist-info/METADATA
+Filename: py_to_proto-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: py_to_proto-0.1.1.dist-info/WHEEL
+Filename: py_to_proto-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: py_to_proto-0.1.1.dist-info/top_level.txt
+Filename: py_to_proto-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: py_to_proto-0.1.1.dist-info/RECORD
+Filename: py_to_proto-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## py_to_proto/dataclass_to_proto.py

```diff
@@ -136,15 +136,15 @@
         return True
 
     ## Types ##
 
     def get_concrete_type(self, entry: Any) -> Any:
         """If this is a concrete type, get the type map key for it"""
         # Unwrap any Annotations
-        entry_type = self._resolve_annotated_type(entry)
+        entry_type = self._resolve_wrapped_type(entry)
 
         # If it's a known type, just return it
         if entry_type in self.type_mapping or isinstance(
             entry_type, (_descriptor.Descriptor, _descriptor.EnumDescriptor)
         ):
             return entry_type
 
@@ -242,22 +242,21 @@
 
     def get_oneof_fields(
         self, field_def: dataclasses.Field
     ) -> Optional[Iterable[Tuple[str, Any]]]:
         """If the given field is a Union, return an iterable of the sub-field
         definitions for its
         """
-        field_type = field_def.type
+        field_type = self._resolve_wrapped_type(field_def.type)
         oneof_fields = []
         if get_origin(field_type) is Union:
-            union_args = get_args(field_type)
-            for arg in union_args:
+            for arg in get_args(field_type):
                 oneof_field_name = self._get_unique_annotation(arg, OneofField)
                 if oneof_field_name is None:
-                    res_type = self._resolve_annotated_type(arg)
+                    res_type = self._resolve_wrapped_type(arg)
                     oneof_field_name = (
                         f"{field_def.name}{str(res_type.__name__)}".lower()
                     )
                     log.debug3("Using default oneof field name: %s", oneof_field_name)
                 oneof_fields.append((oneof_field_name, arg))
         return oneof_fields
 
@@ -265,34 +264,50 @@
         """For an identified oneof field def, get the name"""
         return field_def.name
 
     def get_field_type(self, field_def: dataclasses.Field) -> Any:
         """Get the type of the field. The definition of type here will be
         specific to the converter (e.g. string for JTD, py type for dataclass)
         """
-        field_type = self._resolve_annotated_type(field_def.type)
+        field_type = self._resolve_wrapped_type(field_def.type)
         if get_origin(field_type) is list:
             args = get_args(field_type)
             if len(args) == 1:
                 return args[0]
         return field_type
 
     def is_repeated_field(self, field_def: dataclasses.Field) -> bool:
         """Determine if the given field def is repeated"""
-        return get_origin(self._resolve_annotated_type(field_def.type)) is list
+        return get_origin(self._resolve_wrapped_type(field_def.type)) is list
 
     ## Implementation Details ##################################################
 
-    @staticmethod
-    def _resolve_annotated_type(field_type: type) -> type:
-        """Unwrap the type inside an Annotated, or just return the type if not
-        annotated
-        """
-        if get_origin(field_type) is Annotated:
-            return get_args(field_type)[0]
+    @classmethod
+    def _resolve_wrapped_type(cls, field_type: type) -> type:
+        """Unwrap the type inside an Annotated or Optional, or just return the
+        type if not wrapped
+        """
+        origin = get_origin(field_type)
+        args = get_args(field_type)
+
+        # Unwrap Annotated and recurse in case it's an Annotated[Optional]
+        if origin is Annotated:
+            return cls._resolve_wrapped_type(args[0])
+
+        # Unwrap Optional and recurse in case it's an Optional[Annotated]
+        if origin is Union and type(None) in args:
+            non_none_args = [arg for arg in args if arg is not type(None)]
+            assert non_none_args, f"Cannot have a union with only one NoneType arg"
+            if len(non_none_args) > 1:
+                res_type = Union.__getitem__(tuple(non_none_args))
+            else:
+                res_type = non_none_args[0]
+            return cls._resolve_wrapped_type(res_type)
+
+        # If not Annotated or Optional, return as is
         return field_type
 
     @staticmethod
     def _get_annotations(field_type: type, annotation_type: type) -> List:
         """Get all annotations of the given annotation type from the given field
         type if it's annotated
         """
```

## Comparing `py_to_proto-0.1.1.dist-info/LICENSE` & `py_to_proto-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `py_to_proto-0.1.1.dist-info/METADATA` & `py_to_proto-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-to-proto
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool to dynamically create protobuf message classes from python data schemas
 Home-page: https://github.com/IBM/py-to-proto
 Author: Gabe Goodhart
 Author-email: gabe.l.hart@gmail.com
 License: MIT
 Keywords: json,json typedef,jtd,protobuf,proto,dataclass
 Platform: UNKNOWN
```

## Comparing `py_to_proto-0.1.1.dist-info/RECORD` & `py_to_proto-0.1.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 py_to_proto/__init__.py,sha256=0xvSrTlGuMSPzey0U_v2i1ehBcFVzQRk3Z2qbFZiXO4,1174
 py_to_proto/compat_annotated.py,sha256=-JMeTz4v2hSkrRKVfQVqOlI1Az6IVqXoIC3ma2Fu2XI,251
 py_to_proto/converter_base.py,sha256=M_fO8qin-dklE19hPs9gyDTnjmjYvrRlwHdBOgzGLEw,26041
-py_to_proto/dataclass_to_proto.py,sha256=6kDdeubBSsg9_rdrIHkPDK5Zi3bAu89jBDVM-zljegM,11392
+py_to_proto/dataclass_to_proto.py,sha256=e2sjalvr03_aaclbpXHiby5PFSuS_EOaZs_Gvb_hJxk,12097
 py_to_proto/descriptor_to_file.py,sha256=aVOJGMulF_xppS1n3MdjB8hStRXdnSH7Fkmhui6Xd2Q,9686
 py_to_proto/descriptor_to_message_class.py,sha256=GLk9Uh3j66ADzb_HIy_fswm6WSOp23wgvEPJlBSnuv8,4799
 py_to_proto/json_to_service.py,sha256=yI3pyM99rWBbx63jhmSHi6M-_55ERPBmKtSg8tegQes,9092
 py_to_proto/jtd_to_proto.py,sha256=dmRj35Z5rfFgfeP2QRTaJ2sF1tZrYBD7KsyNY5yrCQ0,8288
 py_to_proto/utils.py,sha256=SU9A7S3yFN5EgRFu2gibVbebsng_2uF2wF4zPjedGMk,12660
 py_to_proto/validation.py,sha256=ssTE17roJwMYwTkRSuDUKL_JGAf1C3Ua0bcAsSPEtLE,14885
-py_to_proto-0.1.1.dist-info/LICENSE,sha256=t-ZkY-vak1QWjzid8VIzMds6wT0xEafbk406cLmdj_Q,1088
-py_to_proto-0.1.1.dist-info/METADATA,sha256=oG7WO_LFKFI2OqDdC_k2iZCNZNVqZY8RYnHD6NgZhls,6777
-py_to_proto-0.1.1.dist-info/WHEEL,sha256=ijjRDmPkGsL9eKpOeSzmTjLbiyw0Dy8TY4QGa2Zy9J8,93
-py_to_proto-0.1.1.dist-info/top_level.txt,sha256=AScY99r2vRxOMZGEg6sfYg7B5BlIyy9sXKc6CrlBR5s,12
-py_to_proto-0.1.1.dist-info/RECORD,,
+py_to_proto-0.1.2.dist-info/LICENSE,sha256=t-ZkY-vak1QWjzid8VIzMds6wT0xEafbk406cLmdj_Q,1088
+py_to_proto-0.1.2.dist-info/METADATA,sha256=ePYaUZkVRqGCxznMVhSbejgdfMDG5Rx7nyFJtFVKQj0,6777
+py_to_proto-0.1.2.dist-info/WHEEL,sha256=ijjRDmPkGsL9eKpOeSzmTjLbiyw0Dy8TY4QGa2Zy9J8,93
+py_to_proto-0.1.2.dist-info/top_level.txt,sha256=AScY99r2vRxOMZGEg6sfYg7B5BlIyy9sXKc6CrlBR5s,12
+py_to_proto-0.1.2.dist-info/RECORD,,
```

