# Comparing `tmp/rxml-0.2.0.tar.gz` & `tmp/rxml-0.4.0.tar.gz`

## Comparing `rxml-0.2.0.tar` & `rxml-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      157 1970-01-01 00:00:00.000000 rxml-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123     2708 2023-04-26 21:05:22.000000 rxml-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-04-26 21:05:22.000000 rxml-0.2.0/.gitignore
--rw-r--r--   0     1001      123     1071 2023-04-26 21:05:22.000000 rxml-0.2.0/LICENSE
--rw-r--r--   0     1001      123     1082 2023-04-26 21:05:22.000000 rxml-0.2.0/README.md
--rw-r--r--   0     1001      123      423 2023-04-26 21:05:22.000000 rxml-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123      340 2023-04-26 21:05:22.000000 rxml-0.2.0/rxml.pyi
--rw-r--r--   0     1001      123     3933 2023-04-26 21:05:22.000000 rxml-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123     8076 2023-04-26 21:05:22.000000 rxml-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     1477 1970-01-01 00:00:00.000000 rxml-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      157 1970-01-01 00:00:00.000000 rxml-0.4.0/Cargo.toml
+-rw-r--r--   0     1001      123     2708 2023-05-01 23:39:02.000000 rxml-0.4.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-05-01 23:39:02.000000 rxml-0.4.0/.gitignore
+-rw-r--r--   0     1001      123     1071 2023-05-01 23:39:02.000000 rxml-0.4.0/LICENSE
+-rw-r--r--   0     1001      123     1366 2023-05-01 23:39:02.000000 rxml-0.4.0/README.md
+-rw-r--r--   0     1001      123      423 2023-05-01 23:39:02.000000 rxml-0.4.0/pyproject.toml
+-rw-r--r--   0     1001      123      717 2023-05-01 23:39:02.000000 rxml-0.4.0/rxml.pyi
+-rw-r--r--   0     1001      123     6173 2023-05-01 23:39:02.000000 rxml-0.4.0/src/lib.rs
+-rw-r--r--   0     1001      123     8076 2023-05-01 23:39:02.000000 rxml-0.4.0/Cargo.lock
+-rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 rxml-0.4.0/PKG-INFO
```

### Comparing `rxml-0.2.0/.github/workflows/CI.yml` & `rxml-0.4.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rxml-0.2.0/.gitignore` & `rxml-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rxml-0.2.0/LICENSE` & `rxml-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rxml-0.2.0/README.md` & `rxml-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: rxml
+Version: 0.4.0
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+License-File: LICENSE
+Summary: A XML parser for Python written in Rust
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+
 # rxml
 
 ## What is rxml?
 
 `rxml` is a simple python library to read xml files up to 2 times faster than python's `xml(ElementTree)` library.
 
 ## Installation
@@ -45,18 +56,32 @@
 After that we can simply iter through the children with:
 
 ```python
 for node in root_file.children:
     # do something whith the node here
 ```
 
+You can also write it to a file or string(refer to the `.pyi` file for the args).
+
+```python
+from rxml import Node, write_file
+
+example_node = Node(
+    name="hello_world", 
+    attrs={"example_attr": "example"},
+    text="Hello World!"
+)
+write_file(example_node, "test_ex.xml")
+```
+
 ## Node attributes
 
 This is how the `Node` looks like:
 
 ```python
 class Node:
     name: str
     attrs: dict[str, str]
     children: list[Node]
     text: str
 ```
+
```

### Comparing `rxml-0.2.0/Cargo.lock` & `rxml-0.4.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rxml"
-version = "0.2.0"
+version = "0.4.0"
 dependencies = [
  "pyo3",
  "quick-xml",
 ]
 
 [[package]]
 name = "scopeguard"
```

