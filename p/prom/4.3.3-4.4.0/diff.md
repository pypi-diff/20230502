# Comparing `tmp/prom-4.3.3.tar.gz` & `tmp/prom-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prom-4.3.3.tar", last modified: Wed Apr  5 20:28:17 2023, max compression
+gzip compressed data, was "prom-4.4.0.tar", last modified: Mon May  1 23:18:23 2023, max compression
```

## Comparing `prom-4.3.3.tar` & `prom-4.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-04-05 20:28:17.313457 prom-4.3.3/
--rw-r--r--   0 jaymon     (501) staff       (20)     1080 2023-03-13 01:48:38.000000 prom-4.3.3/LICENSE.txt
--rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-04-05 20:28:17.313354 prom-4.3.3/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)     5228 2023-03-13 01:48:38.000000 prom-4.3.3/README.md
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-04-05 20:28:17.310818 prom-4.3.3/prom/
--rw-r--r--   0 jaymon     (501) staff       (20)     1456 2023-04-05 20:25:31.000000 prom-4.3.3/prom/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)      188 2023-03-13 01:48:38.000000 prom-4.3.3/prom/compat.py
--rw-r--r--   0 jaymon     (501) staff       (20)    48122 2023-04-01 01:28:22.000000 prom-4.3.3/prom/config.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2359 2023-04-01 01:28:22.000000 prom-4.3.3/prom/exception.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-04-05 20:28:17.311836 prom-4.3.3/prom/extras/
--rw-r--r--   0 jaymon     (501) staff       (20)        0 2023-03-13 01:48:38.000000 prom-4.3.3/prom/extras/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)     1262 2023-03-13 01:48:38.000000 prom-4.3.3/prom/extras/config.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2447 2023-04-01 01:28:22.000000 prom-4.3.3/prom/extras/model.py
--rw-r--r--   0 jaymon     (501) staff       (20)    22837 2023-04-01 06:47:31.000000 prom-4.3.3/prom/extras/testdata.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-04-05 20:28:17.312715 prom-4.3.3/prom/interface/
--rw-r--r--   0 jaymon     (501) staff       (20)     3032 2023-03-13 01:48:38.000000 prom-4.3.3/prom/interface/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)    27763 2023-04-01 01:28:22.000000 prom-4.3.3/prom/interface/base.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-04-05 20:28:17.313200 prom-4.3.3/prom/interface/postgres/
--rw-r--r--   0 jaymon     (501) staff       (20)    20378 2023-04-05 20:25:20.000000 prom-4.3.3/prom/interface/postgres/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3109 2023-04-01 01:28:22.000000 prom-4.3.3/prom/interface/postgres/gevent.py
--rw-r--r--   0 jaymon     (501) staff       (20)    34457 2023-04-01 01:28:22.000000 prom-4.3.3/prom/interface/sql.py
--rw-r--r--   0 jaymon     (501) staff       (20)    17746 2023-04-01 01:28:22.000000 prom-4.3.3/prom/interface/sqlite.py
--rw-r--r--   0 jaymon     (501) staff       (20)    23906 2023-04-01 01:28:22.000000 prom-4.3.3/prom/model.py
--rw-r--r--   0 jaymon     (501) staff       (20)    34778 2023-04-01 01:28:22.000000 prom-4.3.3/prom/query.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4610 2023-03-13 01:48:38.000000 prom-4.3.3/prom/utils.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-04-05 20:28:17.311397 prom-4.3.3/prom.egg-info/
--rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-04-05 20:28:17.000000 prom-4.3.3/prom.egg-info/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      534 2023-04-05 20:28:17.000000 prom-4.3.3/prom.egg-info/SOURCES.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-04-05 20:28:17.000000 prom-4.3.3/prom.egg-info/dependency_links.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       57 2023-04-05 20:28:17.000000 prom-4.3.3/prom.egg-info/requires.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        5 2023-04-05 20:28:17.000000 prom-4.3.3/prom.egg-info/top_level.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-04-05 20:28:17.313488 prom-4.3.3/setup.cfg
--rw-r--r--   0 jaymon     (501) staff       (20)     2201 2023-03-13 01:48:38.000000 prom-4.3.3/setup.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-05-01 23:18:23.856031 prom-4.4.0/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1080 2017-08-21 19:50:23.000000 prom-4.4.0/LICENSE.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-05-01 23:18:23.855899 prom-4.4.0/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)     5228 2021-05-05 22:06:50.000000 prom-4.4.0/README.md
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-05-01 23:18:23.853579 prom-4.4.0/prom/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1456 2023-05-01 23:16:54.000000 prom-4.4.0/prom/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)      188 2021-05-05 21:14:27.000000 prom-4.4.0/prom/compat.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    48726 2023-05-01 22:59:39.000000 prom-4.4.0/prom/config.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2359 2023-03-27 21:02:23.000000 prom-4.4.0/prom/exception.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-05-01 23:18:23.854758 prom-4.4.0/prom/extras/
+-rw-r--r--   0 jaymon     (501) staff       (20)        0 2023-03-27 21:25:20.000000 prom-4.4.0/prom/extras/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     1262 2023-03-11 10:50:37.000000 prom-4.4.0/prom/extras/config.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2447 2023-03-23 00:59:43.000000 prom-4.4.0/prom/extras/model.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    22837 2023-03-27 23:14:39.000000 prom-4.4.0/prom/extras/testdata.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-05-01 23:18:23.855332 prom-4.4.0/prom/interface/
+-rw-r--r--   0 jaymon     (501) staff       (20)     3032 2023-03-27 23:40:25.000000 prom-4.4.0/prom/interface/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    27763 2023-03-27 23:38:55.000000 prom-4.4.0/prom/interface/base.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-05-01 23:18:23.855595 prom-4.4.0/prom/interface/postgres/
+-rw-r--r--   0 jaymon     (501) staff       (20)    20308 2023-05-01 23:16:39.000000 prom-4.4.0/prom/interface/postgres/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3109 2023-03-23 00:11:15.000000 prom-4.4.0/prom/interface/postgres/gevent.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    34441 2023-05-01 23:10:59.000000 prom-4.4.0/prom/interface/sql.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    17737 2023-05-01 22:51:11.000000 prom-4.4.0/prom/interface/sqlite.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    23906 2023-03-23 22:20:04.000000 prom-4.4.0/prom/model.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    34778 2023-03-26 19:34:46.000000 prom-4.4.0/prom/query.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     4610 2020-12-07 23:23:45.000000 prom-4.4.0/prom/utils.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-05-01 23:18:23.854254 prom-4.4.0/prom.egg-info/
+-rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-05-01 23:18:23.000000 prom-4.4.0/prom.egg-info/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      534 2023-05-01 23:18:23.000000 prom-4.4.0/prom.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-05-01 23:18:23.000000 prom-4.4.0/prom.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       57 2023-05-01 23:18:23.000000 prom-4.4.0/prom.egg-info/requires.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        5 2023-05-01 23:18:23.000000 prom-4.4.0/prom.egg-info/top_level.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-05-01 23:18:23.856073 prom-4.4.0/setup.cfg
+-rw-r--r--   0 jaymon     (501) staff       (20)     2201 2021-10-12 23:47:11.000000 prom-4.4.0/setup.py
```

### Comparing `prom-4.3.3/LICENSE.txt` & `prom-4.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prom-4.3.3/PKG-INFO` & `prom-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prom
-Version: 4.3.3
+Version: 4.4.0
 Summary: A sensible orm for PostgreSQL or SQLite
 Home-page: http://github.com/jaymon/prom
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `prom-4.3.3/README.md` & `prom-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `prom-4.3.3/prom/__init__.py` & `prom-4.4.0/prom/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     UniqueError,
     CloseError,
 )
 
 from . import utils
 
 
-__version__ = '4.3.3'
+__version__ = '4.4.0'
 
 
 def transaction(connection_name="", **kwargs):
     """Create a transaction 
 
     Sometimes you just need to batch a whole bunch of operation across a whole bunch
     of different models, this allows you to create a transaction outside of any
```

### Comparing `prom-4.3.3/prom/config.py` & `prom-4.4.0/prom/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -700,39 +700,43 @@
         """
         create a field
 
         :param field_type: type, the python type of the field, so for a string
             you would pass str, integer: int, boolean: bool, float: float
         :param field_required: boolean, true if this field has to be there to insert
         :param field_options: dict, everything else in key: val notation. Current options:
-            - size: int -- the size you want the string to be, or the int to be
-            - min_size: int -- the minimum size
-            - max_size: int -- if you want a varchar, set this
-            - unique: bool -- True to set a unique index on this field, this is just for convenience and is
+            * size: int -- the size you want the string to be, or the int to be
+            * min_size: int -- the minimum size
+            * max_size: int -- if you want a varchar, set this
+            * unique: bool -- True to set a unique index on this field, this is just for convenience and is
                 equal to self.set_index(field_name, [field_name], unique=True). this is a convenience option
                 to set a unique index on the field without having to add a separate index statement
-            - ignore_case: bool -- True to ignore case if this field is used in indexes
-            - default: mixed -- defaults to None, can be anything the db can support
-            - jsonable_name: str, the name of the field when Orm.jsonable() is called
-            - jsonable_field: bool, if False then this field won't be part of
+            * ignore_case: bool -- True to ignore case if this field is used in indexes
+            * default: mixed -- defaults to None, can be anything the db can support
+            * jsonable_name: str, the name of the field when Orm.jsonable() is called
+            * jsonable_field: bool, if False then this field won't be part of
                 Orm.jsonable() output
-            - jsonable: str|callable|bool,
+            * jsonable: str|callable|bool,
                 - str, will be set to jsonable_name
                 - callable, will be used as self.jsonable
                 - bool, will set jsonable_field to False
-            - empty: bool, (default is True), set to False if the value cannot be
+            * empty: bool, (default is True), set to False if the value cannot be
                 empty when being sent to the db (empty is None, "", 0, False)
+            * pk: bool, True to make this field the primary key
+            * auto: bool, True to tag this field as an auto-generated field. Used
+                with an int to set it to an auto-increment, use it with UUID to
+                have uuids auto generated
+            * autopk: bool, shortcut for setting pk=True, auto=True
         :param **field_options_kwargs: dict, will be combined with field_options
         """
         field_options = utils.make_dict(field_options, field_options_kwargs)
 
         d = self.get_size(field_options)
         field_options.update(d)
 
-        #self.orm_class = field_options.pop("orm_class", None)
         name = field_options.pop("name", "")
         orm_class = field_options.pop("orm_class", None)
 
         choices = field_options.pop("choices", set())
         if choices or not self.choices:
             self.choices = choices
 
@@ -742,14 +746,17 @@
 
             elif isinstance(jsonable, bool):
                 field_options.setdefault("jsonable_field", jsonable)
 
             else:
                 field_options["jsonable"] = jsonable
 
+        if autopk := field_options.pop("autopk", False):
+            field_options["pk"] = autopk
+            field_options["auto"] = autopk
 
         for k in list(field_options.keys()):
             if hasattr(self, k):
                 setattr(self, k, field_options.pop(k))
 
         self.options = field_options
         self.required = field_required or self.is_pk()
@@ -757,14 +764,20 @@
         self.set_type(field_type)
 
         # this class is being created manually so mimic what the python parser
         # would do
         if name and orm_class:
             self.__set_name__(orm_class, name)
 
+        elif orm_class:
+            self.orm_class = orm_class
+
+        elif name:
+            self.__set_name__(orm_class, name)
+
     def __set_name__(self, orm_class, name):
         """This is called right after __init__
 
         https://docs.python.org/3/howto/descriptor.html#customized-names
 
         This is only called when an instance is created while a class is being
         parsed/created, so if you just created an instance of Field you would
@@ -1342,14 +1355,15 @@
 
 
 class AutoIncrement(Field):
     """an auto-incrementing Serial field, by default this will be set as primary key"""
     def __init__(self, **kwargs):
         kwargs.setdefault("pk", True)
         kwargs.setdefault("auto", True)
+        kwargs.setdefault("max_size", 9223372036854775807)
         super().__init__(
             field_type=int,
             field_required=True,
             **kwargs
         )
```

### Comparing `prom-4.3.3/prom/exception.py` & `prom-4.4.0/prom/exception.py`

 * *Files identical despite different names*

### Comparing `prom-4.3.3/prom/extras/config.py` & `prom-4.4.0/prom/extras/config.py`

 * *Files identical despite different names*

### Comparing `prom-4.3.3/prom/extras/model.py` & `prom-4.4.0/prom/extras/model.py`

 * *Files identical despite different names*

### Comparing `prom-4.3.3/prom/extras/testdata.py` & `prom-4.4.0/prom/extras/testdata.py`

 * *Files identical despite different names*

### Comparing `prom-4.3.3/prom/interface/__init__.py` & `prom-4.4.0/prom/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `prom-4.3.3/prom/interface/base.py` & `prom-4.4.0/prom/interface/base.py`

 * *Files identical despite different names*

### Comparing `prom-4.3.3/prom/interface/postgres/__init__.py` & `prom-4.4.0/prom/interface/postgres/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,41 +408,39 @@
 
         for k, v in field_kwargs.items():
             fstrs.append([k_opts[k].format(self.render_field_name_sql(field_name)), self.PLACEHOLDER, v])
 
         return fstrs
 
     def render_datatype_int_sql(self, field_name, field, **kwargs):
-        if field.is_pk():
-            field_type = 'BIGSERIAL PRIMARY KEY' # INT8
+        if field.is_ref():
+            field_type = 'BIGINT' # INT8
 
         else:
-            if field.is_ref():
-                field_type = 'BIGINT' # INT8
-
-            else:
-                # https://www.postgresql.org/docs/current/datatype-numeric.html
-                size_info = field.size_info()
-                size = size_info["size"]
-
-                if size == 0:
-                    field_type = 'INTEGER' # INT4
+            # https://www.postgresql.org/docs/current/datatype-numeric.html
+            size_info = field.size_info()
+            size = size_info["size"]
 
-                elif size < 32767:
-                    field_type = 'SMALLINT' # INT2
+            if size == 0:
+                field_type = 'INTEGER' # INT4
 
-                elif size < 2147483647:
-                    field_type = 'INTEGER' # INT4
+            elif size <= 32767:
+                field_type = 'SMALLINT' # INT2
 
-                elif size < 9223372036854775807:
-                    field_type = 'BIGINT' # INT8
+            elif size <= 2147483647:
+                # INT4
+                field_type = 'SERIAL' if field.is_auto() else 'INTEGER'
+
+            elif size <= 9223372036854775807:
+                # INT8
+                field_type = 'BIGSERIAL' if field.is_auto() else 'BIGINT'
 
-                else:
-                    precision = size_info["precision"]
-                    field_type = f'NUMERIC({precision}, 0)'
+            else:
+                precision = size_info["precision"]
+                field_type = f'NUMERIC({precision}, 0)'
 
         return field_type
 
     def render_datatype_str_sql(self, field_name, field, **kwargs):
         if field.interface_options.get('ignore_case', False):
             kwargs.setdefault("datatype", "CITEXT")
 
@@ -500,16 +498,17 @@
         """
         return 'BYTEA'
 
     def render_datatype_uuid_sql(self, field_name, field, **kwargs):
         # https://www.postgresql.org/docs/current/datatype-uuid.html
         # https://www.postgresql.org/docs/current/functions-uuid.html
         field_type = 'UUID'
-        if field.is_pk():
-            field_type += ' DEFAULT gen_random_uuid() PRIMARY KEY'
+        if field.is_auto():
+            field_type += ' DEFAULT gen_random_uuid()'
+
         return field_type
 
     def create_error(self, e, **kwargs):
         """
         https://www.psycopg.org/docs/module.html#exceptions
         """
         kwargs.setdefault("error_module", psycopg2)
```

### Comparing `prom-4.3.3/prom/interface/postgres/gevent.py` & `prom-4.4.0/prom/interface/postgres/gevent.py`

 * *Files identical despite different names*

### Comparing `prom-4.3.3/prom/interface/sql.py` & `prom-4.4.0/prom/interface/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -861,15 +861,18 @@
             raise ValueError('Unknown python type: {} for field: {}'.format(
                 interface_type.__name__,
                 field_name,
             ))
 
         field_type += ' ' + self.render_datatype_required_sql(field_name, field)
 
-        if not field.is_pk():
+        if field.is_pk():
+            field_type += ' PRIMARY KEY'
+
+        else:
             if field.is_ref():
                 field_type += ' ' + self.render_datatype_ref_sql(field_name, field)
 
         return '{} {}'.format(self.render_field_name_sql(field_name), field_type)
 
     def render_datatype_bool_sql(self, field_name, field, **kwargs):
         return 'BOOL'
@@ -891,17 +894,14 @@
                 field_type += f" CHECK(length({field_name}) >= {size_info['original']['min_size']}"
                 field_type += " AND "
                 field_type += f"length({field_name}) <= {size_info['original']['max_size']})"
 
             else:
                 field_type += f" CHECK(length({field_name}) <= {size_info['size']})"
 
-        if field.is_pk():
-            field_type += ' PRIMARY KEY'
-
         return field_type
 
     def render_datatype_date_sql(self, field_name, field):
         return 'DATE'
 
     def render_datatype_float_sql(self, field_name, field, **kwargs):
         return 'REAL'
```

### Comparing `prom-4.3.3/prom/interface/sqlite.py` & `prom-4.4.0/prom/interface/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,24 +493,24 @@
             query_args.append(v)
 
         query_sort_str.append('  END')
         query_sort_str = "\n".join(query_sort_str)
         return query_sort_str, query_args
 
     def render_datatype_int_sql(self, field_name, field, **kwargs):
-        if field.is_pk():
-            field_type = 'INTEGER PRIMARY KEY'
+        if field.is_auto():
+            field_type = 'INTEGER'
 
         else:
             # we could break these up into tiny, small, and big but it
             # doesn't really matter so we're not bothering
             # https://www.sqlite.org/datatype3.html
             size = field.size_info()["size"]
 
-            if size < 9223372036854775807:
+            if size <= 9223372036854775807:
                 field_type = 'INTEGER'
 
             else:
                 field_type = NumericType.FIELD_TYPE
 
         return field_type
```

### Comparing `prom-4.3.3/prom/model.py` & `prom-4.4.0/prom/model.py`

 * *Files identical despite different names*

### Comparing `prom-4.3.3/prom/query.py` & `prom-4.4.0/prom/query.py`

 * *Files identical despite different names*

### Comparing `prom-4.3.3/prom/utils.py` & `prom-4.4.0/prom/utils.py`

 * *Files identical despite different names*

### Comparing `prom-4.3.3/prom.egg-info/PKG-INFO` & `prom-4.4.0/prom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prom
-Version: 4.3.3
+Version: 4.4.0
 Summary: A sensible orm for PostgreSQL or SQLite
 Home-page: http://github.com/jaymon/prom
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `prom-4.3.3/prom.egg-info/SOURCES.txt` & `prom-4.4.0/prom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prom-4.3.3/setup.py` & `prom-4.4.0/setup.py`

 * *Files identical despite different names*

