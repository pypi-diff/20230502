# Comparing `tmp/customdataclass-0.1.1.tar.gz` & `tmp/customdataclass-0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customdataclass-0.1.1.tar", last modified: Thu Apr 27 15:30:51 2023, max compression
+gzip compressed data, was "customdataclass-0.1.1.1.tar", last modified: Mon May  1 19:09:16 2023, max compression
```

## Comparing `customdataclass-0.1.1.tar` & `customdataclass-0.1.1.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-04-27 15:30:51.546733 customdataclass-0.1.1/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1074 2023-04-27 13:55:41.000000 customdataclass-0.1.1/LICENSE.md
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4089 2023-04-27 15:30:51.546733 customdataclass-0.1.1/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3499 2023-04-27 14:45:14.000000 customdataclass-0.1.1/README.md
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      731 2023-04-27 15:30:41.000000 customdataclass-0.1.1/pyproject.toml
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-04-27 15:30:51.546733 customdataclass-0.1.1/setup.cfg
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-04-27 15:30:51.546733 customdataclass-0.1.1/src/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       46 2023-04-27 15:30:35.000000 customdataclass-0.1.1/src/__init__.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-04-27 15:30:51.546733 customdataclass-0.1.1/src/customdataclass.egg-info/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4089 2023-04-27 15:30:51.000000 customdataclass-0.1.1/src/customdataclass.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      550 2023-04-27 15:30:51.000000 customdataclass-0.1.1/src/customdataclass.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-04-27 15:30:51.000000 customdataclass-0.1.1/src/customdataclass.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       53 2023-04-27 15:30:51.000000 customdataclass-0.1.1/src/customdataclass.egg-info/requires.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       25 2023-04-27 15:30:51.000000 customdataclass-0.1.1/src/customdataclass.egg-info/top_level.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    15497 2023-04-27 12:20:16.000000 customdataclass-0.1.1/src/customdataclass.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-04-27 15:30:51.546733 customdataclass-0.1.1/tests/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2219 2023-04-27 14:42:16.000000 customdataclass-0.1.1/tests/test_complex_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3889 2023-04-27 14:42:16.000000 customdataclass-0.1.1/tests/test_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      752 2023-04-27 14:42:16.000000 customdataclass-0.1.1/tests/test_default_value_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1455 2023-04-27 14:42:16.000000 customdataclass-0.1.1/tests/test_incomplete_typing_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1465 2023-04-27 14:42:16.000000 customdataclass-0.1.1/tests/test_mutable_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3861 2023-04-27 14:42:16.000000 customdataclass-0.1.1/tests/test_nested_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2762 2023-04-27 14:42:16.000000 customdataclass-0.1.1/tests/test_partial_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1127 2023-04-27 14:42:16.000000 customdataclass-0.1.1/tests/test_random_dataclass.py
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-01 19:09:16.583337 customdataclass-0.1.1.1/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1074 2023-04-27 13:55:41.000000 customdataclass-0.1.1.1/LICENSE.md
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4572 2023-05-01 19:09:16.583337 customdataclass-0.1.1.1/PKG-INFO
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4009 2023-04-27 15:41:41.000000 customdataclass-0.1.1.1/README.md
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      700 2023-05-01 14:01:22.000000 customdataclass-0.1.1.1/pyproject.toml
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-05-01 19:09:16.583337 customdataclass-0.1.1.1/setup.cfg
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-01 19:09:16.580003 customdataclass-0.1.1.1/src/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       48 2023-04-27 16:09:58.000000 customdataclass-0.1.1.1/src/__init__.py
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-01 19:09:16.580003 customdataclass-0.1.1.1/src/customdataclass.egg-info/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4572 2023-05-01 19:09:16.000000 customdataclass-0.1.1.1/src/customdataclass.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      579 2023-05-01 19:09:16.000000 customdataclass-0.1.1.1/src/customdataclass.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-05-01 19:09:16.000000 customdataclass-0.1.1.1/src/customdataclass.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       37 2023-05-01 19:09:16.000000 customdataclass-0.1.1.1/src/customdataclass.egg-info/requires.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       25 2023-05-01 19:09:16.000000 customdataclass-0.1.1.1/src/customdataclass.egg-info/top_level.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    15703 2023-04-27 16:07:23.000000 customdataclass-0.1.1.1/src/customdataclass.py
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-01 19:09:16.583337 customdataclass-0.1.1.1/tests/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2223 2023-04-27 15:56:13.000000 customdataclass-0.1.1.1/tests/test_complex_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3893 2023-04-27 15:56:25.000000 customdataclass-0.1.1.1/tests/test_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2116 2023-05-01 13:46:55.000000 customdataclass-0.1.1.1/tests/test_dataclass_list.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      756 2023-04-27 15:56:26.000000 customdataclass-0.1.1.1/tests/test_default_value_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1459 2023-04-27 15:56:27.000000 customdataclass-0.1.1.1/tests/test_incomplete_typing_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1469 2023-04-27 15:56:31.000000 customdataclass-0.1.1.1/tests/test_mutable_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     5043 2023-04-27 16:09:06.000000 customdataclass-0.1.1.1/tests/test_nested_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2766 2023-04-27 15:56:38.000000 customdataclass-0.1.1.1/tests/test_partial_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1131 2023-04-27 15:56:43.000000 customdataclass-0.1.1.1/tests/test_random_dataclass.py
```

### Comparing `customdataclass-0.1.1/LICENSE.md` & `customdataclass-0.1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `customdataclass-0.1.1/PKG-INFO` & `customdataclass-0.1.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,15 @@
-Metadata-Version: 2.1
-Name: customdataclass
-Version: 0.1.1
-Summary: A custom dataclass implementation
-Author-email: Lorenzo Rossi <pypi@lorenzoros.si>
-License: MIT
-Project-URL: Homepage, https://github.com/lorossi/customdataclass
-Project-URL: Bug Tracker, https://github.com/lorossi/customdataclass/issues
-Project-URL: documentation, https://lorossi.github.io/customdataclass/
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dependencies
-License-File: LICENSE.md
-
 # Customdataclass
 
+![coverage](https://img.shields.io/badge/dynamic/json?color=informational&label=code%20coverage&query=totals.percent_covered_display&suffix=%25&url=https%3A%2F%2Fraw.githubusercontent.com%2Florossi%2Fcustomdataclass%2Fmain%2Fcoverage.json)
+![issues](https://img.shields.io/github/issues-raw/lorossi/customdataclass)
+![license](https://img.shields.io/pypi/l/customdataclass)
+![python-version](https://img.shields.io/pypi/pyversions/customdataclass)
+![version](https://img.shields.io/pypi/v/customdataclass)
+
 Custom implementation of the `dataclass` module from the standard Python library as a base class for other dataclasses.
 The documentation is available [here](https://lorossi.github.io/customdataclass).
 
 ## Details
 
 A while back I was working on a project *(now lost in a dusty corner of my GitHub profile)* that required me to create a lot of data structures *(variables used only to hold complex data)* and I quickly realised that using dictionaries *(or named dictionaries)* was slowly becoming messy because:
 
@@ -73,17 +63,17 @@
 
 If you're using VScode, you can also use the `Run Tests` command from the `Python Test Explorer for Visual Studio Code` extension.
 
 ### Computing the coverage
 
 To compute the coverage, simply run the following commands from the root folder of the project:
 
--`coverage run -m unittest discover -s ./tests -p "test*.py"`
--`coverage report -m` to see the report in the terminal
--`coverage html` to see format the report in HTML and see it in the browser
+- `coverage run -m unittest discover -s ./tests -p "test*.py"`
+- `coverage report -m` to see the report in the terminal
+- `coverage html` to see format the report in HTML and see it in the browser
 
 ## Documentation
 
 Documentation can be found in the `docs` folder of the repo and on this [page](https://lorossi.github.io/customdataclass).
 
 ### Building the documentation
```

### Comparing `customdataclass-0.1.1/pyproject.toml` & `customdataclass-0.1.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "customdataclass"
-version = "0.1.1"
+version = "0.1.1.1"
 authors = [{ name = "Lorenzo Rossi", email = "pypi@lorenzoros.si" }]
 description = "A custom dataclass implementation"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
 license = { text = "MIT" }
-
-[project.optional-dependencies]
 dependencies = ["PyYAML>=6.0", "toml>=0.10.2", "json>=5.4.0"]
 
 [project.urls]
 "Homepage" = "https://github.com/lorossi/customdataclass"
 "Bug Tracker" = "https://github.com/lorossi/customdataclass/issues"
 documentation = "https://lorossi.github.io/customdataclass/"
```

### Comparing `customdataclass-0.1.1/src/customdataclass.egg-info/PKG-INFO` & `customdataclass-0.1.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: customdataclass
-Version: 0.1.1
+Version: 0.1.1.1
 Summary: A custom dataclass implementation
 Author-email: Lorenzo Rossi <pypi@lorenzoros.si>
 License: MIT
 Project-URL: Homepage, https://github.com/lorossi/customdataclass
 Project-URL: Bug Tracker, https://github.com/lorossi/customdataclass/issues
 Project-URL: documentation, https://lorossi.github.io/customdataclass/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dependencies
 License-File: LICENSE.md
 
 # Customdataclass
 
+![coverage](https://img.shields.io/badge/dynamic/json?color=informational&label=code%20coverage&query=totals.percent_covered_display&suffix=%25&url=https%3A%2F%2Fraw.githubusercontent.com%2Florossi%2Fcustomdataclass%2Fmain%2Fcoverage.json)
+![issues](https://img.shields.io/github/issues-raw/lorossi/customdataclass)
+![license](https://img.shields.io/pypi/l/customdataclass)
+![python-version](https://img.shields.io/pypi/pyversions/customdataclass)
+![version](https://img.shields.io/pypi/v/customdataclass)
+
 Custom implementation of the `dataclass` module from the standard Python library as a base class for other dataclasses.
 The documentation is available [here](https://lorossi.github.io/customdataclass).
 
 ## Details
 
 A while back I was working on a project *(now lost in a dusty corner of my GitHub profile)* that required me to create a lot of data structures *(variables used only to hold complex data)* and I quickly realised that using dictionaries *(or named dictionaries)* was slowly becoming messy because:
 
@@ -73,17 +78,17 @@
 
 If you're using VScode, you can also use the `Run Tests` command from the `Python Test Explorer for Visual Studio Code` extension.
 
 ### Computing the coverage
 
 To compute the coverage, simply run the following commands from the root folder of the project:
 
--`coverage run -m unittest discover -s ./tests -p "test*.py"`
--`coverage report -m` to see the report in the terminal
--`coverage html` to see format the report in HTML and see it in the browser
+- `coverage run -m unittest discover -s ./tests -p "test*.py"`
+- `coverage report -m` to see the report in the terminal
+- `coverage html` to see format the report in HTML and see it in the browser
 
 ## Documentation
 
 Documentation can be found in the `docs` folder of the repo and on this [page](https://lorossi.github.io/customdataclass).
 
 ### Building the documentation
```

### Comparing `customdataclass-0.1.1/src/customdataclass.egg-info/SOURCES.txt` & `customdataclass-0.1.1.1/src/customdataclass.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,13 +6,14 @@
 src/customdataclass.egg-info/PKG-INFO
 src/customdataclass.egg-info/SOURCES.txt
 src/customdataclass.egg-info/dependency_links.txt
 src/customdataclass.egg-info/requires.txt
 src/customdataclass.egg-info/top_level.txt
 tests/test_complex_dataclass.py
 tests/test_dataclass.py
+tests/test_dataclass_list.py
 tests/test_default_value_dataclass.py
 tests/test_incomplete_typing_dataclass.py
 tests/test_mutable_dataclass.py
 tests/test_nested_dataclass.py
 tests/test_partial_dataclass.py
 tests/test_random_dataclass.py
```

### Comparing `customdataclass-0.1.1/src/customdataclass.py` & `customdataclass-0.1.1.1/src/customdataclass.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,15 +152,22 @@
 
         Returns:
             bool: True if the type is correct, False otherwise.
         """
         if valid_type in (Any, None):
             return True
 
-        return isinstance(value, valid_type)
+        try:
+            valid = isinstance(value, valid_type)
+        except TypeError:
+            valid = all(issubclass(v.__class__, valid_type.__args__[0]) for v in value)
+        except Exception:
+            valid = False
+
+        return valid
 
     def _checkDeserializedIterator(self, value: list[Any], valid_type: type) -> bool:
         """Check if the value is a valid iterator.
 
         Args:
             value (list[Any]): value to check
             valid_type (type): type of the value
```

### Comparing `customdataclass-0.1.1/tests/test_complex_dataclass.py` & `customdataclass-0.1.1.1/tests/test_complex_dataclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from customdataclass import Dataclass
+from src.customdataclass import Dataclass
 
 
 class ComplexDataclass(Dataclass):
     """Test class."""
 
     list_var: list
     tuple_var: tuple
```

### Comparing `customdataclass-0.1.1/tests/test_dataclass.py` & `customdataclass-0.1.1.1/tests/test_dataclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from customdataclass import Dataclass
+from src.customdataclass import Dataclass
 
 
 class SampleClass(Dataclass):
     """Test class."""
 
     int_var: int
     float_var: float
```

### Comparing `customdataclass-0.1.1/tests/test_default_value_dataclass.py` & `customdataclass-0.1.1.1/tests/test_default_value_dataclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from customdataclass import Dataclass
+from src.customdataclass import Dataclass
 
 
 class DefaultValue(Dataclass):
     int_val: int = 4
     float_val: float = 4.0
```

### Comparing `customdataclass-0.1.1/tests/test_incomplete_typing_dataclass.py` & `customdataclass-0.1.1.1/tests/test_incomplete_typing_dataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from customdataclass import Dataclass
+from src.customdataclass import Dataclass
 
 
 class IncompleteDataclass(Dataclass):
     """Test class."""
 
     int_var: int
     float_var: float
```

### Comparing `customdataclass-0.1.1/tests/test_mutable_dataclass.py` & `customdataclass-0.1.1.1/tests/test_mutable_dataclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from customdataclass import Dataclass
+from src.customdataclass import Dataclass
 
 
 class MutableDataclass(Dataclass, frozen=False):
     """Test class."""
 
     int_var: int
     float_var: float
```

### Comparing `customdataclass-0.1.1/tests/test_nested_dataclass.py` & `customdataclass-0.1.1.1/tests/test_nested_dataclass.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from customdataclass import Dataclass
+from src.customdataclass import Dataclass
 
 
 class SubDataclass1(Dataclass):
     """Test class."""
 
     int_var: int
     float_var: float
@@ -130,7 +130,60 @@
         self.assertEqual(d, d3)
 
         d4 = DataclassLevel4.from_toml(d.to_toml)
         self.assertEqual(d, d4)
 
         d5 = DataclassLevel4.from_yaml(d.to_yaml)
         self.assertEqual(d, d5)
+
+
+class Person(Dataclass):
+    """Test class."""
+
+    name: str
+    age: int
+
+
+class Room(Dataclass):
+    """Test class."""
+
+    name: str
+    occupants: list[Person]
+
+
+class Inner(Dataclass):
+    """Test class."""
+
+    names: list[str]
+    value: int
+
+
+class Outer(Dataclass):
+    """Test class."""
+
+    inner: Inner
+
+
+class TestNestedDataclassList(unittest.TestCase):
+    def testCreation(self):
+        p1 = Person(name="Alice", age=1)
+        p2 = Person(name="Bob", age=2)
+        r = Room(name="Room", occupants=[p1, p2])
+        self.assertEqual(r.name, "Room")
+        self.assertEqual(r.occupants[0].name, "Alice")
+        self.assertEqual(r.occupants[0].age, 1)
+        self.assertEqual(r.occupants[1].name, "Bob")
+        self.assertEqual(r.occupants[1].age, 2)
+
+    def testSerializeDeserialize(self):
+        o1 = Outer(inner=Inner(names=["Alice", "Bob"], value=1))
+        o2 = Outer.from_dict(o1.to_dict)
+        self.assertEqual(o1, o2)
+
+        o3 = Outer.from_json(o1.to_json)
+        self.assertEqual(o1, o3)
+
+        o4 = Outer.from_toml(o1.to_toml)
+        self.assertEqual(o1, o4)
+
+        o5 = Outer.from_yaml(o1.to_yaml)
+        self.assertEqual(o1, o5)
```

### Comparing `customdataclass-0.1.1/tests/test_partial_dataclass.py` & `customdataclass-0.1.1.1/tests/test_partial_dataclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from customdataclass import Dataclass
+from src.customdataclass import Dataclass
 
 
 class PartialDataclass(Dataclass, partial=True):
     """Test class."""
 
     int_var: int
     float_var: float
```

### Comparing `customdataclass-0.1.1/tests/test_random_dataclass.py` & `customdataclass-0.1.1.1/tests/test_random_dataclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 import unittest
 
-from customdataclass import Dataclass
+from src.customdataclass import Dataclass
 
 
 class RandomClass(Dataclass):
     """Test class."""
 
     int_var: int
     float_var: float
```

