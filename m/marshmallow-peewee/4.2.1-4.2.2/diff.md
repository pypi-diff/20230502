# Comparing `tmp/marshmallow_peewee-4.2.1.tar.gz` & `tmp/marshmallow_peewee-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marshmallow_peewee-4.2.1.tar", max compression
+gzip compressed data, was "marshmallow_peewee-4.2.2.tar", max compression
```

## Comparing `marshmallow_peewee-4.2.1.tar` & `marshmallow_peewee-4.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4452 2023-03-22 05:43:09.459889 marshmallow_peewee-4.2.1/README.md
--rw-r--r--   0        0        0      302 2023-03-22 05:43:09.459889 marshmallow_peewee-4.2.1/marshmallow_peewee/__init__.py
--rw-r--r--   0        0        0      255 2023-03-22 05:43:09.459889 marshmallow_peewee-4.2.1/marshmallow_peewee/config.py
--rw-r--r--   0        0        0     5708 2023-03-22 05:43:09.459889 marshmallow_peewee-4.2.1/marshmallow_peewee/convert.py
--rw-r--r--   0        0        0     2693 2023-03-22 05:43:09.459889 marshmallow_peewee-4.2.1/marshmallow_peewee/fields.py
--rw-r--r--   0        0        0        0 2023-03-22 05:43:09.459889 marshmallow_peewee-4.2.1/marshmallow_peewee/py.typed
--rw-r--r--   0        0        0     4499 2023-03-22 05:43:09.459889 marshmallow_peewee-4.2.1/marshmallow_peewee/schema.py
--rw-r--r--   0        0        0      264 2023-03-22 05:43:09.459889 marshmallow_peewee-4.2.1/marshmallow_peewee/types.py
--rw-r--r--   0        0        0     1355 2023-03-22 05:43:09.459889 marshmallow_peewee-4.2.1/pyproject.toml
--rw-r--r--   0        0        0     5693 1970-01-01 00:00:00.000000 marshmallow_peewee-4.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4452 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/README.md
+-rw-r--r--   0        0        0      302 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/marshmallow_peewee/__init__.py
+-rw-r--r--   0        0        0      255 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/marshmallow_peewee/config.py
+-rw-r--r--   0        0        0     5708 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/marshmallow_peewee/convert.py
+-rw-r--r--   0        0        0     2786 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/marshmallow_peewee/fields.py
+-rw-r--r--   0        0        0        0 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/marshmallow_peewee/py.typed
+-rw-r--r--   0        0        0     4499 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/marshmallow_peewee/schema.py
+-rw-r--r--   0        0        0      264 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/marshmallow_peewee/types.py
+-rw-r--r--   0        0        0     1355 2023-05-02 08:53:16.212144 marshmallow_peewee-4.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5693 1970-01-01 00:00:00.000000 marshmallow_peewee-4.2.2/PKG-INFO
```

### Comparing `marshmallow_peewee-4.2.1/README.md` & `marshmallow_peewee-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `marshmallow_peewee-4.2.1/marshmallow_peewee/convert.py` & `marshmallow_peewee-4.2.2/marshmallow_peewee/convert.py`

 * *Files identical despite different names*

### Comparing `marshmallow_peewee-4.2.1/marshmallow_peewee/fields.py` & `marshmallow_peewee-4.2.2/marshmallow_peewee/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,17 +47,18 @@
 class ForeignKey(fields.Raw):
     string_keys = False
 
     def _bind_to_schema(self, field_name, schema):
         self.string_keys = schema.opts.string_keys
         super()._bind_to_schema(field_name, schema)
 
-    def get_value(self, obj: pw.Model, *_, **__) -> Any:
+    def get_value(self, obj: pw.Model, attr, **_) -> Any:  # type: ignore[override]
         """Return the value for a given key from an object."""
-        value = obj.__data__.get(self.attribute)
+        check_key = attr if self.attribute is None else self.attribute
+        value = obj.__data__.get(check_key)
         if value is not None and self.string_keys:
             return str(value)
         return value
 
 
 class FKNested(fields.Nested):
     """Get an related instance from cache."""
```

### Comparing `marshmallow_peewee-4.2.1/marshmallow_peewee/schema.py` & `marshmallow_peewee-4.2.2/marshmallow_peewee/schema.py`

 * *Files identical despite different names*

### Comparing `marshmallow_peewee-4.2.1/pyproject.toml` & `marshmallow_peewee-4.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marshmallow-peewee"
-version = "4.2.1"
+version = "4.2.2"
 description = "Peewee ORM integration with the Marshmallow (de)serialization library"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klen/marshmallow-peewee"
 repository = "https://github.com/klen/marshmallow-peewee"
 keywords = ["marshmallow", "peewee", "orm", "serialization", "deserialization"]
```

### Comparing `marshmallow_peewee-4.2.1/PKG-INFO` & `marshmallow_peewee-4.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshmallow-peewee
-Version: 4.2.1
+Version: 4.2.2
 Summary: Peewee ORM integration with the Marshmallow (de)serialization library
 Home-page: https://github.com/klen/marshmallow-peewee
 License: MIT
 Keywords: marshmallow,peewee,orm,serialization,deserialization
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

