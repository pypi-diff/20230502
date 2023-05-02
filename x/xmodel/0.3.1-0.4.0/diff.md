# Comparing `tmp/xmodel-0.3.1.tar.gz` & `tmp/xmodel-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmodel-0.3.1.tar", max compression
+gzip compressed data, was "xmodel-0.4.0.tar", max compression
```

## Comparing `xmodel-0.3.1.tar` & `xmodel-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1211 2023-04-15 14:12:05.475085 xmodel-0.3.1/LICENSE
--rw-r--r--   0        0        0     1046 2023-04-15 14:12:05.475085 xmodel-0.3.1/README.md
--rw-r--r--   0        0        0     2072 2023-04-15 14:12:05.475085 xmodel-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    20864 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/__init__.py
--rw-r--r--   0        0        0       18 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/_private/__init__.py
--rw-r--r--   0        0        0       33 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/_private/api/__init__.py
--rw-r--r--   0        0        0     7004 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/_private/api/state.py
--rw-r--r--   0        0        0      828 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/_private/api/utils.py
--rw-r--r--   0        0        0      191 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/base/__init__.py
--rw-r--r--   0        0        0    48954 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/base/api.py
--rw-r--r--   0        0        0    35396 2023-04-15 14:12:05.475085 xmodel-0.3.1/xmodel/base/fields.py
--rw-r--r--   0        0        0    29418 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/base/model.py
--rw-r--r--   0        0        0    21759 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/base/structure.py
--rw-r--r--   0        0        0        1 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/common/__init__.py
--rw-r--r--   0        0        0    13348 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/common/children.py
--rw-r--r--   0        0        0     1943 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/common/lazy.py
--rw-r--r--   0        0        0      963 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/common/types.py
--rw-r--r--   0        0        0     1635 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/common/unwrap.py
--rw-r--r--   0        0        0     2555 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/common/utils.py
--rw-r--r--   0        0        0     7716 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/converters.py
--rw-r--r--   0        0        0       89 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/errors.py
--rw-r--r--   0        0        0      804 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/json.py
--rw-r--r--   0        0        0      273 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/__init__.py
--rw-r--r--   0        0        0    30698 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/api.py
--rw-r--r--   0        0        0     7828 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/client.py
--rw-r--r--   0        0        0      301 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/errors.py
--rw-r--r--   0        0        0     2235 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/model.py
--rw-r--r--   0        0        0     3112 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/options.py
--rw-r--r--   0        0        0    12775 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/response_state.py
--rw-r--r--   0        0        0     6709 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/structure.py
--rw-r--r--   0        0        0     7935 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/remote/weak_cache_pool.py
--rw-r--r--   0        0        0      240 2023-04-15 14:12:05.479085 xmodel-0.3.1/xmodel/util.py
--rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 xmodel-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-05-02 19:24:12.630477 xmodel-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1046 2023-05-02 19:24:12.630477 xmodel-0.4.0/README.md
+-rw-r--r--   0        0        0     2072 2023-05-02 19:24:12.630477 xmodel-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    20732 2023-05-02 19:24:12.630477 xmodel-0.4.0/xmodel/__init__.py
+-rw-r--r--   0        0        0       18 2023-05-02 19:24:12.630477 xmodel-0.4.0/xmodel/_private/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-02 19:24:12.630477 xmodel-0.4.0/xmodel/_private/api/__init__.py
+-rw-r--r--   0        0        0     7007 2023-05-02 19:24:12.630477 xmodel-0.4.0/xmodel/_private/api/state.py
+-rw-r--r--   0        0        0      828 2023-05-02 19:24:12.630477 xmodel-0.4.0/xmodel/_private/api/utils.py
+-rw-r--r--   0        0        0      191 2023-05-02 19:24:12.630477 xmodel-0.4.0/xmodel/base/__init__.py
+-rw-r--r--   0        0        0    48893 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/base/api.py
+-rw-r--r--   0        0        0    35396 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/base/fields.py
+-rw-r--r--   0        0        0    31842 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/base/model.py
+-rw-r--r--   0        0        0    21759 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/base/structure.py
+-rw-r--r--   0        0        0        1 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/common/__init__.py
+-rw-r--r--   0        0        0    13348 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/common/children.py
+-rw-r--r--   0        0        0     1943 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/common/lazy.py
+-rw-r--r--   0        0        0      963 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/common/types.py
+-rw-r--r--   0        0        0     1635 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/common/unwrap.py
+-rw-r--r--   0        0        0     2555 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/common/utils.py
+-rw-r--r--   0        0        0     7716 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/converters.py
+-rw-r--r--   0        0        0       89 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/errors.py
+-rw-r--r--   0        0        0      801 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/json.py
+-rw-r--r--   0        0        0      273 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/__init__.py
+-rw-r--r--   0        0        0    30590 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/api.py
+-rw-r--r--   0        0        0     7789 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/client.py
+-rw-r--r--   0        0        0      301 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/errors.py
+-rw-r--r--   0        0        0     2242 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/model.py
+-rw-r--r--   0        0        0     3112 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/options.py
+-rw-r--r--   0        0        0    12775 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/response_state.py
+-rw-r--r--   0        0        0     6709 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/structure.py
+-rw-r--r--   0        0        0     7935 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/weak_cache_pool.py
+-rw-r--r--   0        0        0      240 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/util.py
+-rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 xmodel-0.4.0/PKG-INFO
```

### Comparing `xmodel-0.3.1/LICENSE` & `xmodel-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/README.md` & `xmodel-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/pyproject.toml` & `xmodel-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xmodel"
-version = "0.3.1"
+version = "0.4.0"
 description = "Models for working with JSON, ie: JsonModel"
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xmodel"}]
 readme = "README.md"
 repository = "https://github.com/xyngular/py-xmodel"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `xmodel-0.3.1/xmodel/__init__.py` & `xmodel-0.4.0/xmodel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Provides easy way to map dict to/from Full-Fledged 'JsonModel' object.
 
-Also, an abstract RemoteModel interface used in xmodel-rest and xmodel-dynamo along with
+Also, an abstract RemoteModel interface used in xmodel-rest and xdynamo along with
 some common code.
 
 .. important:: Doc-comments in varius classes have out-of-date/broken refs; will be fixed soon.
 
 
 .. important:: Docs Below Are OUT OF DATE!!!
-    Most of the docs below belong int xmodel-rest and xmodel-dynamo.
+    Most of the docs below belong int xmodel-rest and xdynamo.
     We will revamp them soon, and put more into the README.md as well.
     Currently, I would look at the docs above or README.md for info on how to use
     `JsonModel` class, which is the main-class of this library.
 
 
 # Old Docs Below - Need A Lot Of Updates (ORM is old reference)
 
@@ -71,16 +71,15 @@
 ### Basic Model Example
 [model-fields]: #basic-model-example
 
 >>> from xmodel import Field, BaseModel
 >>> import datetime as dt
 >>>
 >>> class MyModel(
-...    BaseModel['MyModel'],  # <-- Need to put class name as type-var value
-...                           #     (use str to forward ref)
+...    BaseModel,
 ...    base_url="accounts"  # <-- Class argument passed to underlying Structure object.
 ... ):
 ...    my_attribute: str  # <-- Automatically maps to API without extra effort
 ...    created_at: dt.datetime  # <-- Can auto-convert other types for you
 ...
 ...    other_attribute: int = Field(read_only=True)  # <-- Customize options
 ...
@@ -497,8 +496,8 @@
     'BaseStructure',
     'Field',
     'Converter',
     'XModelError',
     'JsonModel'
 ]
 
-__version__ = '0.3.1'
+__version__ = '0.4.0'
```

### Comparing `xmodel-0.3.1/xmodel/_private/api/state.py` & `xmodel-0.4.0/xmodel/_private/api/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from xmodel.converters import Direction
 from xmodel.errors import XModelError
 from xsentinels.null import Null
 from typing import TYPE_CHECKING, TypeVar, Generic
 from xmodel.base.model import BaseModel
 from xmodel.common.types import JsonDict
 
-M = TypeVar("M")
+M = TypeVar("M", bound=BaseModel)
 
 # noinspection PyUnreachableCode
 if TYPE_CHECKING:
     # We only need this for the type-hint, and nothing else.
     # Use forward-refs 'BaseApi' [with the quotes].
     # Gives code from outside this module hints about some of the types.
     from xmodel import BaseApi
 
 
 class PrivateApiState(Generic[M]):
     """ This class is used as a private repository to store api related state for a BaseModel
         instance.
     """
 
-    def __init__(self, model: BaseModel[M]):
+    def __init__(self, model: BaseModel):
         self.model = model
         self.related_field_id_area = {}
 
     # ------------------------------------------------------
     # --------- These Can Vary BaseModel per-instance! ---------
 
-    model: BaseModel[M]
+    model: M
     """ Instance of model [or None if this state is directly associated with a BaseModel Class
         and not any particular instance.
     """
 
     last_original_update_json: JsonDict = None
     """ The keys are set to the raw-value of the last time that attribute was updated via
         update_from_json. So the value is what was originally passed to update_from_json, per-key.
```

### Comparing `xmodel-0.3.1/xmodel/_private/api/utils.py` & `xmodel-0.4.0/xmodel/_private/api/utils.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/xmodel/base/api.py` & `xmodel-0.4.0/xmodel/base/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 ...     # change/use. Any unspecified ones will each inherit from the
 ...     # super-class as you would expect.
 ...     auth: MyAuth
 ...     client: MyClient
 ...     settings: MySettings
 ...     structure: MyStructure[Field]
 >>>
->>> class MyModel(xmodel.BaseModel['MyModel']):
+>>> class MyModel(xmodel.BaseModel):
 ...     # Same as in MyApi, this will inherit from superclass if not specified.
 ...     api: MyApi
 
 
 The settings is more about making it easy to get the relevant config most-used by that
 particular Api subclass.  The client is what the Api will allocate to do requests.
 
@@ -419,15 +419,15 @@
             **(type(self).default_converters or {}),
         }
 
     # ----------------------------------------------------
     # --------- Things REQUIRING an Associated BaseModel -----
 
     @property
-    def model(self) -> BaseModel[M]:
+    def model(self) -> M:
         """ REQUIRES associated model object [see doc text below].
 
         Gives you back the model associated with this api. If this BaseApi obj is associated
         directly with the BaseModel class type and so there is no associated model, I will
         raise an exception.
 
         Some BaseApi methods are dependant on having an associated model, and when they ask for it
@@ -470,15 +470,15 @@
         return model
 
     def get_child_without_lazy_lookup(
             self,
             child_field_name,
             *,
             false_if_not_set=False,
-    ) -> Union[BaseModel[M], None, bool, NullType]:
+    ) -> Union[M, None, bool, NullType]:
         """ REQUIRES associated model object [see self.model].
 
         If the child is current set to Null, or an object, returns that value.
         Will NOT lazily lookup child, even if its possible to do so.
 
         :param child_field_name: The field name of the child object.
         :param false_if_not_set:
@@ -629,15 +629,15 @@
                 #   or should we embed full object anyway?
 
                 child_obj_id = api_state.get_related_field_id(f)
 
                 # Method below should deal with None vs Null.
                 set_value_into_json_dict(child_obj_id, f"{f}_id")
             else:
-                obj: 'BaseModel[M]' = getattr(model, f)
+                obj: 'M' = getattr(model, f)
 
                 # Related-object has no 'id', so get it's json dict and set that into the output.
                 v = obj
                 if obj is not Null and obj is not None:
                     # todo: a Field option to override this and always provide all
                     #   values (if object always needs to be fully embedded).
                     v = obj.api.json(only_include_changes=only_include_changes)
@@ -795,15 +795,15 @@
             If True: Will include the fields value in an update.
             If False: Won't include the fields value in an update.
         """
         # Convert old value to set if new value is set and old value is list (from original JSON).
         # If I was really cool :)... I would find out the inner type in case of int/str
         # and to a conversion to compare Apples to Apples.....
         # But trying to minimize changes so I don't conflict as much with soon to be
-        # xmodel-dynamo feature.
+        # xdynamo feature.
         if type(new_value) is set and type(old_value) is list:
             old_value = set(old_value)
 
         return new_value != old_value
 
     def _get_old_json_value(self, *, field: str, as_type: Type = None) -> Optional[Any]:
         """ Returns the old field-values; Will return `Default` if there is no original value.  """
@@ -964,15 +964,15 @@
                     "Type-hints for xmodel models in this format: `attr: List[SomeType]` "
                     "are not currently supported. We want to support it someday. For now you "
                     "must use lower-cased non-generic `list`. At some point the idea is to "
                     "allow one to do `List[ChildModel]` and then we know it's a list of "
                     "other BaseModel objects and automatically handle that in some way."
                 )
 
-                # child_type: 'Type[BaseModel[M]]'
+                # child_type: 'Type[M]'
                 # child_type = typing_inspect.get_args(obj_type)
                 # # __args__ returns a tuple of all arguments passed into List[] so we need to
                 # # pull the class out of the tuple
                 # if child_type:
                 #     child_type = child_type[0]
                 #
                 # child_api: BaseApi
```

### Comparing `xmodel-0.3.1/xmodel/base/fields.py` & `xmodel-0.4.0/xmodel/base/fields.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/xmodel/base/model.py` & `xmodel-0.4.0/xmodel/base/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import sys
+import typing
+
 from xmodel.common.lazy import LazyClassAttr  # noqa - orm private module
 from logging import getLogger
 from typing import get_type_hints, TYPE_CHECKING, TypeVar, Generic, Type, Optional, Any, Mapping, \
     Callable
 from abc import ABC
 import inspect
 import typing_inspect
@@ -18,14 +21,15 @@
 if TYPE_CHECKING:
     # Allows IDE to get type reference without a circular import issue.
     from xmodel import BaseApi, ApiOptions
 
     # Just for type-completion of abstract interface,
     # for when we look up a remote sub-model.
     from xmodel.remote import RemoteModel
+    # from typing import Self
 
 log = getLogger(__name__)
 
 M = TypeVar('M')
 
 basic_type_hints_map = {
     int: lambda x: int(x),
@@ -36,15 +40,43 @@
 
 __pdoc__ = {
     # We want to pdoc3 to document this method [starts with `_`, so hidden by default].
     'BaseModel.__init_subclass__': True,
 }
 
 
-class BaseModel(Generic[M], ABC):
+try:
+    # If we are using Python 3.11, can use this new `Self` type that means current class/subclass
+    # that is being used.
+    # (it does appear that PyCharm >=2022.3 knows what `Self` is even if you use python < 3.11)
+    # This is the only way I know to have a class-property/attribute that type-hints as the
+    # subclass.
+    from typing import Self
+
+    # Attempt to use `dataclass_transform` on the `BaseModel` below.
+    #
+    # It happens to be that `Self` and `dataclass_transform` are both available in Python 3.11,
+    # so the import-above is a good enough 'check' to prevent this from executing on Python < 3.11.
+    model_auto_init = typing.dataclass_transform
+except ImportError:
+    # In regard to `Self`:
+    #   In this case, we will set `Self` to `BaseModel` after the `BaseModel` class is defined.
+    #   We need to have something defined for `Self` for Python < 3.11, since BaseModel and
+    #   its subclasses have their type-hints resolved at runtime
+    #   (also, `Self` is imported into modules that subclass `BaseModel` and redefine type-hint
+    #    for `BaseModel.api`).
+
+    # This here to support Python < 3.11 (ie: a decorator that does nothing).
+    globals()['model_auto_init'] = lambda: lambda x: x
+
+
+# Keeping the 'Generic[M]' part below temporarily for backwards compatibility;
+# it's not needed anymore otherwise.
+@model_auto_init()  # noqa - This will be defined.
+class BaseModel(ABC):
     """
     Used as the abstract base-class for classes/object that communicate with our REST API.
 
     This is one of the main classes, and it's highly recommend you read the
     [SDK Library Overview](./#orm-library-overview) first, if you have not already.
     That document has many basic examples of using this class along with other related classes.
 
@@ -102,29 +134,34 @@
         by changing the type-hint on a subclass.
 
     """
 
     # -------------------------------------
     # --------- Public Properties ---------
 
-    api: "BaseApi[M]" = None
+    api: "BaseApi[Self]" = None
     """ Used to access the api class, which is used to retrieve/send objects to/from api.
 
         You can specify this as a type-hint in subclasses to change the class we use for this
         automatically, like so::
             from xmodel import BaseModel, BaseApi
+            from xmodel.base.model import Self
             from typing import TypeVar
 
             M = TypeVar("M")
 
             class MyCoolApi(BaseApi[M]):
                 pass
 
-            class MyCoolModel(BaseModel["MyCoolModel"]):
-                api: MyCoolApi[M]  # If this model will have subclasses, you want to use a type-var
+            class MyCoolModel(BaseModel):
+                # The `Self` here is imported from xmodel
+                # (to maintain backwards compatability with Python < 3.11)
+                # It allows us to communicate our subclass-type to the `api` object,
+                # allowing IDE to type-complete/hint better.
+                api: MyCoolApi[Self] 
 
         The generic ``T`` type-var in this case refers to whatever model class that your using.
         In the example just above, ``T`` would be referring to ``MyCoolModel`` if you did this
         somewhere to get the BaseModel's api: ``MyCoolModel.api``.
     """
 
     # --------------------------------------------
@@ -157,15 +194,15 @@
         If you want to add support for additional BaseModel class arguments,
         you can do it by modifying the base-implementation
         `xmodel.base.structure.BaseStructure`.
         Or if you want it only for a specific sub-set of Models, you can make a custom
         `xmodel.base.structure.BaseStructure` subclass. You can configure your BaseModel to use
         this BaseStructure subclass via a type-hint on `xmodel.base.api.BaseApi.structure`.
 
-        See `xmodel_dynamo.dynamo.DynStructure.configure_for_model_type` for a complete example of a
+        See `xdynamo.dynamo.DynStructure.configure_for_model_type` for a complete example of a
         custom BaseStructure subclass that adds extra class arguments that are specific to Dynamo.
 
         Args:
             lazy_loader: This is a callable where the first argument is `cls/self`.
                 This is an optional param. If provided, we will call when we need to lazy-load
                 but before we do our normal lazy-loading ourselves here.
 
@@ -607,14 +644,29 @@
         """ For BaseModel, by default our identity is based on object instance ID, not any values
             in our attributes.  Makes things simpler when trying to find object/self in a Set;
             which is useful when traversing relationships.
         """
         return id(self)
 
 
+if 'Self' not in globals():
+    # I need to have this set to something because `BaseModel` and it's subclasses get their
+    # typehints resolved at run-time (to implement the needed dynamic behavior).
+    #
+    # This is the best we can do for a `Self` class-property when using python version < 3.11
+    # without resorting to self-referential Generics (which are annoying, since you need to
+    # define them at every model-leaf endpoint);
+    #
+    # Newer PyCharm >=2022.3 will see the above Self typing import and still work even if local project
+    # is using an older version of Python!.
+    #
+    # Using `globals` here to hide this typing-info from PyCharm (and other IDEs).
+    globals()['Self'] = BaseModel
+
+
 def _get_default_value_from_field(model: BaseModel, field: Field = None) -> Any:
     if not field or field.default is None:
         return None
 
     default = field.default
 
     if default is Null:
```

### Comparing `xmodel-0.3.1/xmodel/base/structure.py` & `xmodel-0.4.0/xmodel/base/structure.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/xmodel/common/children.py` & `xmodel-0.4.0/xmodel/common/children.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/xmodel/common/lazy.py` & `xmodel-0.4.0/xmodel/common/lazy.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/xmodel/common/types.py` & `xmodel-0.4.0/xmodel/common/types.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/xmodel/common/unwrap.py` & `xmodel-0.4.0/xmodel/common/unwrap.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/xmodel/common/utils.py` & `xmodel-0.4.0/xmodel/common/utils.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/xmodel/converters.py` & `xmodel-0.4.0/xmodel/converters.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/xmodel/json.py` & `xmodel-0.4.0/xmodel/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 from typing import TypeVar
 from .base import BaseModel
 
 
 M = TypeVar('M')
 
 
-class JsonModel(BaseModel[M]):
+class JsonModel(BaseModel):
     pass
```

### Comparing `xmodel-0.3.1/xmodel/remote/api.py` & `xmodel-0.4.0/xmodel/remote/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     # See xmodel.base.api.BaseApi's for its various special type-hinted attributes
     # for more details, it has more detailed comments/documentation on it.
     client: RemoteClient[M]
     structure: RemoteStructure[Field]
 
     # This type-hint is only for IDE, `RemoteApi` does not use it
     # (self.model_type value is passed in when RemoteApi is allocated, in __init__ method).
-    model: RemoteModel[M]
+    model: M
 
     @property
     def _client(self):
         """ Returns an appropriate concrete `xmodel.remote.client.RemoteClient` subclass.
             We figure out the proper client object to use based on the type-hint for "client"
             property on the sub-class.
 
@@ -60,16 +60,15 @@
                 >>>     client: MyClient[M]  # <-- Type hint on 'client' property.
 
             This is enough for `xmodel.base.BaseModel` subclasses that have this set as their
             api type-hint:
 
                 >>> from xmodel.remote.model import RemoteModel
                 >>>
-                >>> # The ["MyModel"] part allows IDE to do better code-completion.
-                >>> class MyModel(RemoteModel["MyModel"]):
+                >>> class MyModel(RemoteModel):
                 >>>     api: MyApi
 
             When you get MyModel's api like below, it will return a MyApi instance,
             MyApi will in turn return a MyClient:
 
                 >>> print(MyModel.api)
                 MyApi(...)
```

### Comparing `xmodel-0.3.1/xmodel/remote/client.py` & `xmodel-0.4.0/xmodel/remote/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,22 +164,22 @@
             See `RemoteClient.cache_weak_get` for more details.
         """
         _ClientCacheDependency.grab().obj_cache.pop(key, None)
 
     # ------------------------------------------------
     # --------- Send Requests to API Methods ---------
 
-    def delete_obj(self, obj: RemoteModel[M]):
+    def delete_obj(self, obj: M):
         raise NotImplementedError(f"Implement `delete_obj()` on ({type(self)}).")
 
-    def delete_objs(self, objs: Sequence[RemoteModel[M]]):
+    def delete_objs(self, objs: Sequence[M]):
         raise NotImplementedError(f"Implement `delete_objs()` on ({type(self)}).")
 
     def send_objs(
-            self, objs: Sequence[RemoteModel[M]], *, url: URLStr = None, send_limit: int = None
+            self, objs: Sequence[M], *, url: URLStr = None, send_limit: int = None
     ):
         raise NotImplementedError(f"Implement `send_objs()` on ({type(self)}).")
 
     # ---------------------------------------
     # --------- GET via API Methods ---------
 
     def get(
```

### Comparing `xmodel-0.3.1/xmodel/remote/model.py` & `xmodel-0.4.0/xmodel/remote/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import TypeVar, Generic, TYPE_CHECKING
 
-from xmodel.base.model import BaseModel
+from xmodel.base.model import BaseModel, Self
 from xsentinels.default import Default
 
+
 if TYPE_CHECKING:
     from xmodel.remote.api import RemoteApi
 
 # Can't forward-ref the bound type here (ie: 'RemoteModel'), so put BaseModel in at least...
 M = TypeVar("M", bound=BaseModel)
 
 
@@ -25,16 +26,16 @@
     See `xmodel.base.model.BaseModel.__init_subclass__` for more details.
     """
     if 'BaseApi' not in globals():
         from xmodel.remote.api import RemoteApi
         globals()['RemoteApi'] = RemoteApi
 
 
-class RemoteModel(BaseModel[M], lazy_loader=_lazy_load_types):
-    api: 'RemoteApi[M]' = None
+class RemoteModel(BaseModel, lazy_loader=_lazy_load_types):
+    api: 'RemoteApi[Self]' = None
 
     # todo: I think we will want to make the type on the `id` field a TypeVar of some sort,
     #       sometimes we will want to use a `str` for it's type [etc].
     id: int = None
     """ Primary identifier for object, used with API endpoint. """
 
     def __init__(self, *args, id=Default, **initial_values):
```

### Comparing `xmodel-0.3.1/xmodel/remote/options.py` & `xmodel-0.4.0/xmodel/remote/options.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/xmodel/remote/response_state.py` & `xmodel-0.4.0/xmodel/remote/response_state.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/xmodel/remote/structure.py` & `xmodel-0.4.0/xmodel/remote/structure.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/xmodel/remote/weak_cache_pool.py` & `xmodel-0.4.0/xmodel/remote/weak_cache_pool.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.3.1/PKG-INFO` & `xmodel-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmodel
-Version: 0.3.1
+Version: 0.4.0
 Summary: Models for working with JSON, ie: JsonModel
 Home-page: https://github.com/xyngular/py-xmodel
 Author: Josh Orr
 Author-email: josh@orr.blue
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Programming Language :: Python :: 3
```

