# Comparing `tmp/pydictable-1.0.1.tar.gz` & `tmp/pydictable-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydictable-1.0.1.tar", last modified: Mon Feb 27 06:03:59 2023, max compression
+gzip compressed data, was "pydictable-1.0.2.tar", last modified: Tue May  2 10:06:55 2023, max compression
```

## Comparing `pydictable-1.0.1.tar` & `pydictable-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:03:59.298004 pydictable-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-27 06:03:47.000000 pydictable-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-27 06:03:59.298004 pydictable-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-02-27 06:03:47.000000 pydictable-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:03:59.294005 pydictable-1.0.1/pydictable/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-27 06:03:47.000000 pydictable-1.0.1/pydictable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-02-27 06:03:47.000000 pydictable-1.0.1/pydictable/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-02-27 06:03:47.000000 pydictable-1.0.1/pydictable/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    26084 2023-02-27 06:03:47.000000 pydictable-1.0.1/pydictable/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-27 06:03:47.000000 pydictable-1.0.1/pydictable/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-02-27 06:03:47.000000 pydictable-1.0.1/pydictable/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 06:03:59.298004 pydictable-1.0.1/pydictable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-27 06:03:59.000000 pydictable-1.0.1/pydictable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-02-27 06:03:59.000000 pydictable-1.0.1/pydictable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 06:03:59.000000 pydictable-1.0.1/pydictable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-27 06:03:59.000000 pydictable-1.0.1/pydictable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 06:03:59.298004 pydictable-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-27 06:03:47.000000 pydictable-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:06:55.421827 pydictable-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-02 10:06:42.000000 pydictable-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-02 10:06:55.421827 pydictable-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-02 10:06:42.000000 pydictable-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:06:55.421827 pydictable-1.0.2/pydictable/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-02 10:06:42.000000 pydictable-1.0.2/pydictable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-02 10:06:42.000000 pydictable-1.0.2/pydictable/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-05-02 10:06:42.000000 pydictable-1.0.2/pydictable/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26708 2023-05-02 10:06:42.000000 pydictable-1.0.2/pydictable/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-02 10:06:42.000000 pydictable-1.0.2/pydictable/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-02 10:06:42.000000 pydictable-1.0.2/pydictable/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:06:55.421827 pydictable-1.0.2/pydictable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-02 10:06:55.000000 pydictable-1.0.2/pydictable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-02 10:06:55.000000 pydictable-1.0.2/pydictable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:06:55.000000 pydictable-1.0.2/pydictable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 10:06:55.000000 pydictable-1.0.2/pydictable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 10:06:55.421827 pydictable-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-02 10:06:42.000000 pydictable-1.0.2/setup.py
```

### Comparing `pydictable-1.0.1/LICENSE` & `pydictable-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydictable-1.0.1/README.md` & `pydictable-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pydictable-1.0.1/pydictable/core.py` & `pydictable-1.0.2/pydictable/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,15 +109,18 @@
 
     def __clear_default_field_values(self):
         for attr, field in self.__class__.__get_fields().items():
             self.__setattr__(attr, None)
 
     def __apply_dict(self, d: dict):
         for attr, field in self.__class__.__get_fields().items():
-            self.__setattr__(attr, field.from_dict(d.get(self.__get_field_key(attr), field.default)))
+            value = d.get(self.__get_field_key(attr), field.default)
+            if not field.required and value is None:
+                continue
+            self.__setattr__(attr, field.from_dict(value))
 
     def __validate_dict(self, raw_values: dict):
         for attr, field in self.__get_fields().items():
             value = raw_values.get(self.__get_field_key(attr), field.default)
             if value is None and not field.required:
                 continue
             try:
@@ -141,15 +144,19 @@
             except AssertionError:
                 raise DataValidationError(attr,
                                           'Post check failed. Invalid value "{}" for field "{}"'.format(value, attr))
 
     def to_dict(self) -> dict:
         d = {}
         for attr, field in self.__class__.__get_fields().items():
-            d[self.__get_field_key(attr)] = field.to_dict(self.__getattribute__(attr))
+            raw_value = self.__getattribute__(attr)
+            if not field.required and raw_value is None:
+                d[self.__get_field_key(attr)] = None
+                continue
+            d[self.__get_field_key(attr)] = field.to_dict(raw_value)
         return d
 
     @classmethod
     def get_input_spec(cls) -> dict:
         d = {}
         for attr, field in cls.__get_fields().items():
             d[cls.__get_field_key(attr)] = field.spec()
```

### Comparing `pydictable-1.0.1/pydictable/field.py` & `pydictable-1.0.2/pydictable/field.py`

 * *Files identical despite different names*

### Comparing `pydictable-1.0.1/pydictable/test_core.py` & `pydictable-1.0.2/pydictable/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -741,7 +741,22 @@
                     'satyam': {'age': 'hi'},
                     'pramod': {'age': 30}
                 }
             })
             raise AssertionError('Should not have passed!')
         except DataValidationError as e:
             self.assertEqual(e.path, 'people.satyam.age')
+
+    def test_nested_optional_list(self):
+        class RefSchema(DictAble):
+            referenceName: str = StrField(required=False)
+
+        class Address(DictAble):
+            location: str
+            references: List[RefSchema] = ListField(ObjectField(RefSchema, required=False), required=False)
+
+        class Profile(DictAble):
+            address: Address = ObjectField(Address)
+
+        profile = Profile(dict={'address': {'location': 'Bengaluru'}})
+        self.assertEqual(profile.address.references, None)
+        self.assertEqual(profile.to_dict(), {'address': {'references': None, 'location': 'Bengaluru'}})
```

### Comparing `pydictable-1.0.1/pydictable/test_field.py` & `pydictable-1.0.2/pydictable/test_field.py`

 * *Files identical despite different names*

### Comparing `pydictable-1.0.1/pydictable/type.py` & `pydictable-1.0.2/pydictable/type.py`

 * *Files identical despite different names*

### Comparing `pydictable-1.0.1/setup.py` & `pydictable-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='pydictable',
-    version='1.0.1',
+    version='1.0.2',
     author='Pramod Kumar',
     author_email='pramodkumar.damam73@gmail.com',
     description='Make your classes from/to dict',
     url='https://github.com/pskd73/pydictable.git',
     packages=['pydictable'],
     include_package_data=True,
     long_description='A tool to create data modals from dict and convert it to dict. '
```

