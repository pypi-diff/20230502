# Comparing `tmp/xdynamo-0.2.0.tar.gz` & `tmp/xdynamo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdynamo-0.2.0.tar", max compression
+gzip compressed data, was "xdynamo-0.3.0.tar", max compression
```

## Comparing `xdynamo-0.2.0.tar` & `xdynamo-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      692 2023-05-01 15:58:55.864390 xdynamo-0.2.0/README.md
--rw-r--r--   0        0        0     1683 2023-05-01 15:58:55.868391 xdynamo-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    22378 2023-05-01 15:58:55.868391 xdynamo-0.2.0/xdynamo/__init__.py
--rw-r--r--   0        0        0     5401 2023-05-01 15:58:55.868391 xdynamo-0.2.0/xdynamo/api.py
--rw-r--r--   0        0        0    32980 2023-05-01 15:58:55.868391 xdynamo-0.2.0/xdynamo/client.py
--rw-r--r--   0        0        0    14349 2023-05-01 15:58:55.868391 xdynamo-0.2.0/xdynamo/common_types.py
--rw-r--r--   0        0        0     6464 2023-05-01 15:58:55.868391 xdynamo-0.2.0/xdynamo/db.py
--rw-r--r--   0        0        0       45 2023-05-01 15:58:55.868391 xdynamo-0.2.0/xdynamo/errors.py
--rw-r--r--   0        0        0     1052 2023-05-01 15:58:55.868391 xdynamo-0.2.0/xdynamo/fields.py
--rw-r--r--   0        0        0       25 2023-05-01 15:58:55.868391 xdynamo-0.2.0/xdynamo/meta.json
--rw-r--r--   0        0        0     2049 2023-05-01 15:58:55.868391 xdynamo-0.2.0/xdynamo/model.py
--rw-r--r--   0        0        0     5522 2023-05-01 15:58:55.868391 xdynamo-0.2.0/xdynamo/resources.py
--rw-r--r--   0        0        0     8648 2023-05-01 15:58:55.868391 xdynamo-0.2.0/xdynamo/structure.py
--rw-r--r--   0        0        0      161 2023-05-01 15:58:55.868391 xdynamo-0.2.0/xdynamo/utils.py
--rw-r--r--   0        0        0     1710 1970-01-01 00:00:00.000000 xdynamo-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      692 2023-05-02 21:03:20.566472 xdynamo-0.3.0/README.md
+-rw-r--r--   0        0        0     1683 2023-05-02 21:03:20.570472 xdynamo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    22321 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/__init__.py
+-rw-r--r--   0        0        0     5401 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/api.py
+-rw-r--r--   0        0        0    32959 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/client.py
+-rw-r--r--   0        0        0    14349 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/common_types.py
+-rw-r--r--   0        0        0     6464 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/db.py
+-rw-r--r--   0        0        0       45 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/errors.py
+-rw-r--r--   0        0        0     3501 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/fields.py
+-rw-r--r--   0        0        0       25 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/meta.json
+-rw-r--r--   0        0        0     2085 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/model.py
+-rw-r--r--   0        0        0     5522 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/resources.py
+-rw-r--r--   0        0        0    10193 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/structure.py
+-rw-r--r--   0        0        0      161 2023-05-02 21:03:20.570472 xdynamo-0.3.0/xdynamo/utils.py
+-rw-r--r--   0        0        0     1710 1970-01-01 00:00:00.000000 xdynamo-0.3.0/PKG-INFO
```

### Comparing `xdynamo-0.2.0/README.md` & `xdynamo-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `xdynamo-0.2.0/pyproject.toml` & `xdynamo-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "xdynamo"
-version = "0.2.0"
+version = "0.3.0"
 description = "Use dynamo with xmodel objects."
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xdynamo"}]
 readme = "README.md"
 repository = "https://github.com/xyngular/py-xdynamo"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: The Unlicense (Unlicense)"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = "^1.17.54"
 
-xmodel = "^0.3.1"
+xmodel = "^0.4.0"
 xinject = "^1.4.0"
 xloop = "^1.0.1"
 xsentinels = "^1.2.1"
 xurls = "^0.2.1"
 ciso8601 = "^2.3.0"
 xsettings = "^1.3.0"
 xboto = "^1.0.2"
```

### Comparing `xdynamo-0.2.0/xdynamo/__init__.py` & `xdynamo-0.3.0/xdynamo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 .. note:: You can see models vary similar to these in action in sine unit-tests
     Look at
     [tests/test_dynamo.py](https://github.com/xyngular/py-xyn-model-dynamo/blob/master/tests/test_dynamo.py)
     in xdynamo source if your interested.
 
 >>> class ModelWithRangeKey(
-...     DynModel["ModelWithRangeKey"],
+...     DynModel,
 ...     # ---> used for end of table name:
 ...     dyn_name="modelWithRangeKey"
 ... ):
 ...     my_hash: str = HashField()
 ...     my_range: str = RangeField()
 ...     name: str
 ...     a_number: int
@@ -92,27 +92,27 @@
 
 Here is a normal non-dynamo model. We will be using this as a way to parse a sub-dict
 automatically into a regular model object.
 We enabled `Field.include_in_repr` in the below example, it will make `sub_name` print out
 in string when object is converted to a string (such as when logging object out).
 
 >>> from xmodel.fields import Field
->>> class ModelAsSubJsonDict(BaseModel['ModelAsSubDict'], has_id_field=False):
+>>> class ModelAsSubJsonDict(BaseModel, has_id_field=False):
 ...
 ...     # It puts 'sub-name' into the object description when converting object
 ...     # to a string
 ...     # (ie: such as when you log out a object of type 'ModelAsSubJsonDict')
 ...     sub_name: str = Field(include_in_repr=True)
 ...     queue: bool
 
 Here is a second `DynModel` for a separate table.  It has a relationship to a
 `ModelWithRangeKey`.
 
 >>> class ModelOnlyHash(
-...     DynModel['VisiblePackage'],
+...     DynModel,
 ...     dyn_name="visibleShipConfirm",
 ...     dyn_service="experimental"
 ... ):
 ...     hash_only: str = HashField()
 ...     name: str
 ...     items: List[Dict[str, str]]
 ...     a_number: int
```

### Comparing `xdynamo-0.2.0/xdynamo/api.py` & `xdynamo-0.3.0/xdynamo/api.py`

 * *Files identical despite different names*

### Comparing `xdynamo-0.2.0/xdynamo/client.py` & `xdynamo-0.3.0/xdynamo/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 from xloop import xloop
 
 if TYPE_CHECKING:
     from xdynamo.model import DynModel
     from xdynamo.api import DynApi
 
 log = getLogger(__name__)
-M = TypeVar('M')
+M = TypeVar('M', bound='DynModel')
 
 
 class DynClient(RemoteClient[M]):
     """
     Skeleton/Placeholder Class for future work, see story and the other classes in
     this file for more details: https://app.clubhouse.io/xyngular/story/13989
     """
 
     # This is only here to give IDE's a more concrete-class to use for type/code completion.
     # The type-hint is not otherwise used. That var is valid/gettable on an instance.
     # See `xmodel.remote.client.RemoteClient.api` for more details.
     api: 'DynApi[M]'
 
-    def delete_obj(self, obj: Union['DynModel[M]', DynKey]):
+    def delete_obj(self, obj: Union['M', DynKey]):
         # raise NotImplementedError()
 
         # table_name = self.api.structure.dyn_name
         # params = {
         #     "TableName": table_name,
         #     # todo: find out if need "S", "N", level...
         #     "Key": DynKey.via_obj(obj).key_as_dict()
@@ -57,15 +57,15 @@
         key = obj if isinstance(obj, DynKey) else DynKey.via_obj(obj)
 
         # To keep things simple, I am using 'put' which replaces entire item,
         # so get all properties of item regardless if they changed or not.
         # todo: Check for primary key and raise a nicer, higher-level exception in that case.
         resource.delete_item(Key=key.key_as_dict())
 
-    def delete_objs(self, objs: Sequence[Union['DynModel[M]', DynKey]]):
+    def delete_objs(self, objs: Sequence[Union['M', DynKey]]):
         """ Uses a batch-writer to put the items.
             WAY more efficient then doing it one at a time.
             If you only give me one item, directly calls `delete_obj` without a batch-writer.
         """
         if not objs:
             return
 
@@ -75,15 +75,15 @@
 
         with _DynBatchResource.grab().current_writer(create_if_none=True):
             for i in objs:
                 self.delete_obj(obj=i)
 
     def send_objs(
             self,
-            objs: Sequence['DynModel[M]'],
+            objs: Sequence['M'],
             *,
             url: URLStr = None,
             send_limit: int = None
     ):
         """
         Used to send any number of objects to Dynamo in as efficient a manner as possible.
 
@@ -409,16 +409,16 @@
                 need. If you provide both dynamo_params and query, the ones in query will overwrite
                 ones in dynamo_params if there is a conflict;
 
                 The `query` param could use either a `KeyConditionExpression` or `FilterExpression`
                 depending on what attributes are in the query dict.
 
         Yields:
-            DynModel[M]: The next object we got from dynamo. This method returns a generator
-                that will eventually go though all the results from dynamo in a memory-efficient
+            M: The next object we got from dynamo. This method returns a generator
+                that will eventually go through all the results from dynamo in a memory-efficient
                 manner.
         """
 
         # todo: support in/lists as values....
         # todo: support `id`.
 
         structure = self.api.structure
```

### Comparing `xdynamo-0.2.0/xdynamo/common_types.py` & `xdynamo-0.3.0/xdynamo/common_types.py`

 * *Files identical despite different names*

### Comparing `xdynamo-0.2.0/xdynamo/db.py` & `xdynamo-0.3.0/xdynamo/db.py`

 * *Files identical despite different names*

### Comparing `xdynamo-0.2.0/xdynamo/model.py` & `xdynamo-0.3.0/xdynamo/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from typing import TypeVar, Optional
 from xmodel.remote import XRemoteError
 from xmodel.remote.model import RemoteModel
 from xdynamo.api import DynApi
 from xdynamo.common_types import DynKey
+from xmodel.base.model import Self
+
 
 M = TypeVar('M')
 
 
-class DynModel(RemoteModel[M], dyn_name=None, dyn_service=None):
+class DynModel(RemoteModel, dyn_name=None, dyn_service=None):
     """
     Used to easily parse/generate JSON from xyn_sdk model's for use in Dynamo.
     So it will take advantage of all the other features of the xyn_sdk models.
     This includes automatically converting dates to/from strings, converting strings
     to numbers, looking up child-objects from other tables automatically, etc.
     It also will modify the results JSON so remove blank values; to easily prevent
     these sorts of errors in dynamo boto3 library.
 
     We pass in None for name/service to indicate we don't have an associated table,
     that we are more of an abstract class.
     """
-    api: DynApi[M]
+    api: DynApi[Self]
     id: str
 
     @property
     def id(self) -> Optional[str]:
         # We could do some intelligent caching, but for now just calculate each time.
         try:
             return DynKey.via_obj(self).id
```

### Comparing `xdynamo-0.2.0/xdynamo/resources.py` & `xdynamo-0.3.0/xdynamo/resources.py`

 * *Files identical despite different names*

### Comparing `xdynamo-0.2.0/xdynamo/structure.py` & `xdynamo-0.3.0/xdynamo/structure.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,17 +19,19 @@
     will eventually be put into this structure for use by the DynClient/DynApi classes.
     """
 
     # Todo: Refer to parent docs, but put more info about how virtual-id's are used for our
     #  dynamo tables.
     virtual_id: bool = True
 
-    dyn_name: str = None
+    dyn_name: str = Default
     """ Table name, minus service/environment name.
         We generally want to use camelCase for this and no dashes/underscores.
+
+        If left as `Default`, will use a "camelCase" version of the model class name.
     """
 
     dyn_service: str = Default
     """ Service to use, by `Default` we use current `xcon.conf.XconSettings.service`.
         If Blank/None we won't include it in the name.
     """
 
@@ -37,19 +39,33 @@
     """ Environment to use, by `Default` we use current `xcon.conf.XconSettings.environment`.
         If Blank/None we won't include it in the name.
     """
 
     dyn_hash_key_name: str = None
     """ Name of hash key [for now both model and table attribute must be same name].
         If left as None, an error will be raised when we try connect to table.
+
+        You can more easily indicate this via `HashField`, ie:
+
+        >>> class MyModel(DynModel):
+        ...     my_hash: str = HashField()
+
+        When you do this, we will fill in `dyn_hash_key_name` for you.
     """
 
     dyn_range_key_name: str = None
     """ Name of range key [for now both model and table attribute must be same name];
         If left as None, we don't have one on the table.
+
+        You can more easily indicate this via `RangeField`, ie:
+
+        >>> class MyModel(DynModel):
+        ...     my_hash: str = RangeField()
+
+        When you do this, we will fill in `dyn_range_key_name` for you.
     """
 
     dyn_id_delimiter = "|"
     """
     Default way to delimit the hash/range keys when used in external systems and with code under
     the `xmodel` library. In general, it's assumed we only have one key that can uniquely
     identify model objects/items in general. For DynamoDB, if it has a range key we can merge
@@ -71,17 +87,23 @@
 
     def has_id_field(self):
         id_field = self.get_field('id')
         return (id_field.dyn_key is DynKeyType.hash) if id_field else False
 
     def configure_for_model_type(
             self,
-            dyn_name: str,
+
+            # These fields are used to name the table
+            # format: `{dyn_service}-{dyn_environment}-{dyn_name}`
+            dyn_name: Optional[str] = Default,
+            dyn_environment: str = Default,
             dyn_service: str = Default,
+
             dyn_id_delimiter: str = Default,
+
             **kwargs
     ):
         """
         See superclass method `xmodel.base.structure.BaseStructure.configure_for_model_type`
         first. It has more information about what calls this method and how to
         customize value via class arguments
         (see `xmodel.base.model.BaseModel.__init_subclass__` for more about the class argument
@@ -96,35 +118,58 @@
         See super-class method `xmodel.base.structure.BaseStructure.configure_for_model_type`
         doc's for additional arguments and details.
 
         Args:
             dyn_name: Name of the table.  We will add dyn_service and current environment to the
                 final name.  See `DynStructure.fully_qualified_table_name` for more details.
 
-            dyn_service: Name of the service.  For now this is required. I was thinking of making
-                this optional and grabbing the current `xcon.conf.XconSettings.service`
-                each time it's needed.  But this would be a bit weird. It would be the equivalent
-                of changing an API endpoint name based on the current service name.
-
-                I consider the table's service + table names part of the 'endpoint' name.
-
-                However....
-                The current `xcon.conf.XconSettings.environment` environmental name makes sense to
-                look up each time when needed. The current APP_ENV is used in the host-name
-                for our normal API's.  And so it makes sense to look up the APP_ENV dynamically
-                each time to get the final table name.
+                This can also be `None` to indicate that it has no direct-table
+                (ie: this is an abstract base class, with commonly shared fields, etc).
+
+            dyn_service: Name of the service to use for that portion of the table name.
+                If not provided, and `xcon` is available, will use `con.conf.XconSettings.service`.
+                Right now `xcon` is a required dependency, but will make it optional in the future.
+
+                In that future version, leaving this as `Default` would make it not format
+                the service name into the table name.
+
+            dyn_environment: Name of the environment to use for that portion of the table name.
+                Right now `xcon` is a required dependency, but will make it optional in the future.
+
+                In that future version, leaving this as `Default` would make it not format
+                the environment name into the table name.
+
+            dyn_id_delimiter: Delimiter to use for the `id` value when table has both a
+                hash and range key (to delimit the values of the two).
+
+                By default, a pipe char `|` is used.
+
             **kwargs: These all come from class-arguments given to the
                 `xdynamo.model.DynModel` at class-definition time that need to be sent to
                 my super-class via
                 `xmodel.base.structure.BaseStructure.configure_for_model_type`. See that
                 for more on what other arguments are supported.
         """
         super().configure_for_model_type(**kwargs)
+
+        # Resolve default `dyn_name` if needed
+        if dyn_name is Default:
+            model_name = self.model_cls.__name__
+            dyn_name = model_name[:1].lower() + model_name[1:] if model_name else ''
+
+        if dyn_name == '':
+            raise XRemoteError(
+                f"The `dyn_name` of dynamo model ({self.model_cls}) was blank/None; "
+                f"model must be `None` or have a non-blank `dyn_name`."
+            )
+
         self.dyn_name = dyn_name
         self.dyn_service = dyn_service
+        self.dyn_environment = dyn_environment
+
         if dyn_id_delimiter:
             self.dyn_id_delimiter = dyn_id_delimiter
 
         type_to_attr_map = {
             DynKeyType.hash: 'dyn_hash_key_name',
             DynKeyType.range: 'dyn_range_key_name',
         }
```

### Comparing `xdynamo-0.2.0/PKG-INFO` & `xdynamo-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdynamo
-Version: 0.2.0
+Version: 0.3.0
 Summary: Use dynamo with xmodel objects.
 Home-page: https://github.com/xyngular/py-xdynamo
 Author: Josh Orr
 Author-email: josh@orr.blue
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: boto3 (>=1.17.54,<2.0.0)
 Requires-Dist: ciso8601 (>=2.3.0,<3.0.0)
 Requires-Dist: xboto (>=1.0.2,<2.0.0)
 Requires-Dist: xinject (>=1.4.0,<2.0.0)
 Requires-Dist: xloop (>=1.0.1,<2.0.0)
-Requires-Dist: xmodel (>=0.3.1,<0.4.0)
+Requires-Dist: xmodel (>=0.4.0,<0.5.0)
 Requires-Dist: xsentinels (>=1.2.1,<2.0.0)
 Requires-Dist: xsettings (>=1.3.0,<2.0.0)
 Requires-Dist: xurls (>=0.2.1,<0.3.0)
 Project-URL: Repository, https://github.com/xyngular/py-xdynamo
 Description-Content-Type: text/markdown
 
 ![PythonSupport](https://img.shields.io/static/v1?label=python&message=%203.8|%203.9|%203.10|%203.11&color=blue?style=flat-square&logo=python)
```

