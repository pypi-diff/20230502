# Comparing `tmp/nmodl_preprocessor-1.0.4.tar.gz` & `tmp/nmodl_preprocessor-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmodl_preprocessor-1.0.4.tar", last modified: Thu Apr 20 22:56:42 2023, max compression
+gzip compressed data, was "nmodl_preprocessor-1.0.5.tar", last modified: Mon May  1 22:39:03 2023, max compression
```

## Comparing `nmodl_preprocessor-1.0.4.tar` & `nmodl_preprocessor-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-20 22:56:42.482044 nmodl_preprocessor-1.0.4/
--rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-19 23:44:54.000000 nmodl_preprocessor-1.0.4/.gitignore
--rw-rw-r--   0 dm        (1000) dm        (1000)    37883 2023-04-19 23:02:12.000000 nmodl_preprocessor-1.0.4/DETAILS.pdf
--rw-rw-r--   0 dm        (1000) dm        (1000)     1076 2023-03-28 16:31:04.000000 nmodl_preprocessor-1.0.4/LICENSE.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)     2030 2023-04-20 22:56:42.482044 nmodl_preprocessor-1.0.4/PKG-INFO
--rw-rw-r--   0 dm        (1000) dm        (1000)     1289 2023-04-20 22:05:56.000000 nmodl_preprocessor-1.0.4/README.md
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-20 22:56:42.482044 nmodl_preprocessor-1.0.4/nmodl_preprocessor/
--rw-rw-r--   0 dm        (1000) dm        (1000)    15449 2023-04-20 22:50:31.000000 nmodl_preprocessor-1.0.4/nmodl_preprocessor/__main__.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     3664 2023-04-19 22:43:58.000000 nmodl_preprocessor-1.0.4/nmodl_preprocessor/nmodl_to_python.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     2994 2023-04-19 23:30:29.000000 nmodl_preprocessor-1.0.4/nmodl_preprocessor/rw_patterns.py
--rw-rw-r--   0 dm        (1000) dm        (1000)      480 2023-04-19 21:45:07.000000 nmodl_preprocessor-1.0.4/nmodl_preprocessor/utils.py
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-20 22:56:42.482044 nmodl_preprocessor-1.0.4/nmodl_preprocessor.egg-info/
--rw-rw-r--   0 dm        (1000) dm        (1000)     2030 2023-04-20 22:56:42.000000 nmodl_preprocessor-1.0.4/nmodl_preprocessor.egg-info/PKG-INFO
--rw-rw-r--   0 dm        (1000) dm        (1000)      444 2023-04-20 22:56:42.000000 nmodl_preprocessor-1.0.4/nmodl_preprocessor.egg-info/SOURCES.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)        1 2023-04-20 22:56:42.000000 nmodl_preprocessor-1.0.4/nmodl_preprocessor.egg-info/dependency_links.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)       80 2023-04-20 22:56:42.000000 nmodl_preprocessor-1.0.4/nmodl_preprocessor.egg-info/entry_points.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)        6 2023-04-20 22:56:42.000000 nmodl_preprocessor-1.0.4/nmodl_preprocessor.egg-info/requires.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)       19 2023-04-20 22:56:42.000000 nmodl_preprocessor-1.0.4/nmodl_preprocessor.egg-info/top_level.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)      957 2023-04-20 22:54:54.000000 nmodl_preprocessor-1.0.4/pyproject.toml
--rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-20 22:56:42.482044 nmodl_preprocessor-1.0.4/setup.cfg
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-01 22:39:03.243815 nmodl_preprocessor-1.0.5/
+-rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-19 23:44:54.000000 nmodl_preprocessor-1.0.5/.gitignore
+-rw-rw-r--   0 dm        (1000) dm        (1000)    37883 2023-04-19 23:02:12.000000 nmodl_preprocessor-1.0.5/DETAILS.pdf
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1076 2023-03-28 16:31:04.000000 nmodl_preprocessor-1.0.5/LICENSE.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)     2030 2023-05-01 22:39:03.243815 nmodl_preprocessor-1.0.5/PKG-INFO
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1289 2023-04-20 22:05:56.000000 nmodl_preprocessor-1.0.5/README.md
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-01 22:39:03.243815 nmodl_preprocessor-1.0.5/nmodl_preprocessor/
+-rw-rw-r--   0 dm        (1000) dm        (1000)    20861 2023-05-01 15:35:14.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor/__main__.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1642 2023-04-29 16:57:39.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor/cpp_keywords.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     4533 2023-04-30 22:51:37.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor/nmodl_to_python.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     3700 2023-05-01 00:53:22.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor/rw_patterns.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)      550 2023-05-01 00:53:17.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor/utils.py
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-01 22:39:03.243815 nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/
+-rw-rw-r--   0 dm        (1000) dm        (1000)     2030 2023-05-01 22:39:03.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/PKG-INFO
+-rw-rw-r--   0 dm        (1000) dm        (1000)      479 2023-05-01 22:39:03.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/SOURCES.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)        1 2023-05-01 22:39:03.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/dependency_links.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)       80 2023-05-01 22:39:03.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/entry_points.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)        6 2023-05-01 22:39:03.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/requires.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)       19 2023-05-01 22:39:03.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/top_level.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)      957 2023-05-01 22:38:08.000000 nmodl_preprocessor-1.0.5/pyproject.toml
+-rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-05-01 22:39:03.243815 nmodl_preprocessor-1.0.5/setup.cfg
```

### Comparing `nmodl_preprocessor-1.0.4/DETAILS.pdf` & `nmodl_preprocessor-1.0.5/DETAILS.pdf`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.4/LICENSE.txt` & `nmodl_preprocessor-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.4/PKG-INFO` & `nmodl_preprocessor-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmodl_preprocessor
-Version: 1.0.4
+Version: 1.0.5
 Summary: Optimize NMODL files for the NEURON simulator
 Author-email: David McDougall <dam1784@rit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/ctrl-z-9000-times/nmodl_preprocessor
 Keywords: nmodl,neuron
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
```

### Comparing `nmodl_preprocessor-1.0.4/README.md` & `nmodl_preprocessor-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.4/nmodl_preprocessor/nmodl_to_python.py` & `nmodl_preprocessor-1.0.5/nmodl_preprocessor/nmodl_to_python.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 """
 Adapted from the tutorial:
 https://bluebrain.github.io/nmodl/html/notebooks/nmodl-python-tutorial.html#Easy-code-generation-using-AST-visitors
 """
+import math
 import textwrap
 import nmodl.dsl
 
-# This list of NMODL's built-in functions was copied from the documentation at:
-# https://github.com/neuronsimulator/nrn/blob/master/docs/guide/nmodls_built_in_functions.rst
-builtin_functions = (
-    "abs",
-)
-builtin_math_functions = (
-    "acos",
-    "asin",
-    "atan",
-    "atan2",
-    "ceil",
-    "cos",
-    "cosh",
-    "exp",
-    "fabs",
-    "floor",
-    "fmod",
-    "log",
-    "log10",
-    "pow",
-    "sin",
-    "sinh",
-    "sqrt",
-    "tan",
-    "tanh",
-)
+nmodl_builtins = {
+    # This list of NMODL's built-in functions was copied from the documentation at:
+    # https://github.com/neuronsimulator/nrn/blob/master/docs/guide/nmodls_built_in_functions.rst
+    "abs":      math.fabs,
+    "acos":     math.acos,
+    "asin":     math.asin,
+    "atan":     math.atan,
+    "atan2":    math.atan2,
+    "ceil":     math.ceil,
+    "cos":      math.cos,
+    "cosh":     math.cosh,
+    "exp":      math.exp,
+    "fabs":     math.fabs,
+    "floor":    math.floor,
+    "fmod":     math.fmod,
+    "log":      math.log,
+    "log10":    math.log10,
+    "pow":      math.pow,
+    "sin":      math.sin,
+    "sinh":     math.sinh,
+    "sqrt":     math.sqrt,
+    "tan":      math.tan,
+    "tanh":     math.tanh,
+    # These constants were copied from the documentation at:
+    # https://nrn.readthedocs.io/en/8.2.2/hoc/programming/math/constants.html
+    "PI":       3.14159265358979323846,
+    "E":        2.71828182845904523536,
+    "GAMMA":    0.57721566490153286060,  # Euler
+    "DEG":      57.29577951308232087680, # deg/radian
+    "PHI":      1.61803398874989484820,  # golden ratio
+    "FARADAY":  96520,   # coulombs/mole
+    "R":        8.31441, # molar gas constant, joules/mole/deg-K
+}
 
 class VerbatimError(ValueError): pass
 
 class ComplexityError(ValueError): pass
 
 
 class PyGenerator(nmodl.dsl.visitor.AstVisitor):
@@ -72,15 +80,18 @@
         if op == "^":
             op = '**'
         node.lhs.accept(self)
         self.pycode += f" {op} "
         node.rhs.accept(self)
 
     def visit_var_name(self, node):
-        self.pycode += node.name.get_node_name()
+        if node.name.is_indexed_name():
+            self.visit_indexed_name(node.name)
+        else:
+            self.pycode += node.name.get_node_name()
 
     def visit_integer(self, node):
         self.pycode += nmodl.to_nmodl(node)
 
     def visit_double(self, node):
         self.pycode += nmodl.to_nmodl(node)
 
@@ -99,18 +110,16 @@
             elif_node.statement_block.accept(self)
         if else_node := node.elses:
             self.pycode += "else:\n"
             else_node.statement_block.accept(self)
 
     def visit_function_call(self, node):
         name = node.name.get_node_name()
-        if name in builtin_functions:
+        if name in nmodl_builtins:
             pass
-        elif name in builtin_math_functions:
-            name = f"math.{name}"
         elif name == "net_send":
             raise ComplexityError()
         else:
             # All functions and procedures should have been inlined already.
             # The exceptions mostly involve TABLE statements.
             # I could attempt to evaluate these calls, but that would be very
             # complicated, especially because python does not support ASSIGNED
@@ -123,7 +132,10 @@
             self.pycode += ", "
         self.pycode += ")"
 
     def visit_while_statement(self, node):
         # Can not guarantee correct results BC the condition might reference unknown values.
         raise ComplexityError()
 
+    def visit_indexed_name(self, node):
+        raise ComplexityError()
+
```

### Comparing `nmodl_preprocessor-1.0.4/nmodl_preprocessor/rw_patterns.py` & `nmodl_preprocessor-1.0.5/nmodl_preprocessor/rw_patterns.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,21 +17,36 @@
         for block_name, var_names in self.writes.items():
             self.all_writes.update(var_names)
 
     def visit_statement_block(self, node):
         # Look for top level code blocks.
         if self.current_block is None:
             self.current_block = get_block_name(node.parent)
-            self.reads[self.current_block]  = set()
+            parameters = set(STR(x.get_node_name()) for x in getattr(node.parent, 'parameters', []))
+            self.reads[self.current_block]  = parameters
             self.writes[self.current_block] = set()
             node.visit_children(self)
             self.current_block = None
         else:
             node.visit_children(self)
 
+    def visit_reaction_statement(self, node):
+        self.visit_diff_eq_expression(node)
+
+    def visit_diff_eq_expression(self, node):
+        # The solver may move kinetic equations into different code blocks.
+        current_block = self.current_block
+        self.current_block = object()
+        self.reads[self.current_block]  = set()
+        self.writes[self.current_block] = set()
+        node.visit_children(self)
+        self.reads[current_block]  |= self.reads.pop(self.current_block)
+        self.writes[current_block] |= self.writes.pop(self.current_block)
+        self.current_block = current_block
+
     def visit_binary_expression(self, node):
         if node.op.eval() == '=':
             # Recursively mark all variables on right hand side as being read from.
             node.rhs.accept(self)
             # Mark the left hand side variable of this assignment as being written to.
             name = STR(node.lhs.name.get_node_name())
             self.writes[self.current_block].add(name)
@@ -59,13 +74,14 @@
             inner.writes[self.current_block] = set(self.writes[self.current_block])
             inner.visit_statement_block(x)
         # Apply the results of the child visitors simultaneously.
         for inner in visitors:
             self.reads[self.current_block].update(inner.reads[self.current_block])
             self.writes[self.current_block].update(inner.writes[self.current_block])
 
+    # TODO: For example see model 52034
+    # def visit_from_statement(self, node):
+    #     1/0
+
     def visit_neuron_block(self, node):
         pass # Does not contain any source code.
 
-    def visit_function_block(self, node):
-        pass # Functions are pure and can't access assigned variables.
-
```

### Comparing `nmodl_preprocessor-1.0.4/nmodl_preprocessor.egg-info/PKG-INFO` & `nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmodl-preprocessor
-Version: 1.0.4
+Version: 1.0.5
 Summary: Optimize NMODL files for the NEURON simulator
 Author-email: David McDougall <dam1784@rit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/ctrl-z-9000-times/nmodl_preprocessor
 Keywords: nmodl,neuron
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
```

### Comparing `nmodl_preprocessor-1.0.4/pyproject.toml` & `nmodl_preprocessor-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["nmodl_preprocessor"]
 
 [project]
 name = "nmodl_preprocessor"
-version = "1.0.4"
+version = "1.0.5"
 description = "Optimize NMODL files for the NEURON simulator"
 readme = "README.md"
 license = {text = "MIT"}
 authors = [
     {name = "David McDougall", email = "dam1784@rit.edu"},
 ]
 urls = {Homepage = "https://github.com/ctrl-z-9000-times/nmodl_preprocessor"}
```

