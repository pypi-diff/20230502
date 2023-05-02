# Comparing `tmp/winval-0.6.1.tar.gz` & `tmp/winval-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winval-0.6.1.tar", max compression
+gzip compressed data, was "winval-0.6.2.tar", max compression
```

## Comparing `winval-0.6.1.tar` & `winval-0.6.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    10765 2023-03-01 14:20:53.081846 winval-0.6.1/LICENSE
--rw-r--r--   0        0        0     2873 2023-03-01 14:20:53.081846 winval-0.6.1/README.md
--rw-r--r--   0        0        0      439 2023-03-01 14:20:53.081846 winval-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      572 2023-03-01 14:20:53.081846 winval-0.6.1/winval/__init__.py
--rw-r--r--   0        0        0     3703 2023-03-01 14:20:53.081846 winval-0.6.1/winval/antlr/winval.interp
--rw-r--r--   0        0        0      611 2023-03-01 14:20:53.081846 winval-0.6.1/winval/antlr/winval.tokens
--rw-r--r--   0        0        0     9502 2023-03-01 14:20:53.081846 winval-0.6.1/winval/antlr/winvalLexer.interp
--rw-r--r--   0        0        0     9570 2023-03-01 14:20:53.081846 winval-0.6.1/winval/antlr/winvalLexer.py
--rw-r--r--   0        0        0      611 2023-03-01 14:20:53.081846 winval-0.6.1/winval/antlr/winvalLexer.tokens
--rw-r--r--   0        0        0     4571 2023-03-01 14:20:53.081846 winval-0.6.1/winval/antlr/winvalListener.py
--rw-r--r--   0        0        0    38746 2023-03-01 14:20:53.081846 winval-0.6.1/winval/antlr/winvalParser.py
--rw-r--r--   0        0        0     2876 2023-03-01 14:20:53.081846 winval-0.6.1/winval/antlr/winvalVisitor.py
--rw-r--r--   0        0        0     4606 2023-03-01 14:20:53.081846 winval-0.6.1/winval/cloud_files_validator.py
--rw-r--r--   0        0        0     5454 2023-03-01 14:20:53.081846 winval-0.6.1/winval/constraint_eval.py
--rw-r--r--   0        0        0      849 2023-03-01 14:20:53.081846 winval-0.6.1/winval/constraints_pre_processor.py
--rw-r--r--   0        0        0     1843 2023-03-01 14:20:53.081846 winval-0.6.1/winval/parsed_workflow_inputs.py
--rw-r--r--   0        0        0     1099 2023-03-01 14:20:53.081846 winval-0.6.1/winval/python_extensions.py
--rw-r--r--   0        0        0     1901 2023-03-01 14:20:53.081846 winval-0.6.1/winval/validate_wdl_constraints.py
--rw-r--r--   0        0        0     7496 2023-03-01 14:20:53.081846 winval-0.6.1/winval/wdl_parser.py
--rw-r--r--   0        0        0     1710 2023-03-01 14:20:53.081846 winval-0.6.1/winval/winval.g4
--rw-r--r--   0        0        0     3297 2023-03-01 14:20:53.081846 winval-0.6.1/winval/winval_class.py
--rw-r--r--   0        0        0     4531 2023-03-01 14:20:53.081846 winval-0.6.1/winval/workflow_var.py
--rw-r--r--   0        0        0     3611 1970-01-01 00:00:00.000000 winval-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-05-02 07:47:08.951592 winval-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2873 2023-05-02 07:47:08.951592 winval-0.6.2/README.md
+-rw-r--r--   0        0        0      439 2023-05-02 07:47:08.951592 winval-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      572 2023-05-02 07:47:08.951592 winval-0.6.2/winval/__init__.py
+-rw-r--r--   0        0        0     3703 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winval.interp
+-rw-r--r--   0        0        0      611 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winval.tokens
+-rw-r--r--   0        0        0     9502 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winvalLexer.interp
+-rw-r--r--   0        0        0     9570 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winvalLexer.py
+-rw-r--r--   0        0        0      611 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winvalLexer.tokens
+-rw-r--r--   0        0        0     4571 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winvalListener.py
+-rw-r--r--   0        0        0    38746 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winvalParser.py
+-rw-r--r--   0        0        0     2876 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winvalVisitor.py
+-rw-r--r--   0        0        0     4606 2023-05-02 07:47:08.951592 winval-0.6.2/winval/cloud_files_validator.py
+-rw-r--r--   0        0        0     5574 2023-05-02 07:47:08.951592 winval-0.6.2/winval/constraint_eval.py
+-rw-r--r--   0        0        0      849 2023-05-02 07:47:08.951592 winval-0.6.2/winval/constraints_pre_processor.py
+-rw-r--r--   0        0        0     1843 2023-05-02 07:47:08.951592 winval-0.6.2/winval/parsed_workflow_inputs.py
+-rw-r--r--   0        0        0     1099 2023-05-02 07:47:08.955592 winval-0.6.2/winval/python_extensions.py
+-rw-r--r--   0        0        0     1901 2023-05-02 07:47:08.955592 winval-0.6.2/winval/validate_wdl_constraints.py
+-rw-r--r--   0        0        0     7496 2023-05-02 07:47:08.955592 winval-0.6.2/winval/wdl_parser.py
+-rw-r--r--   0        0        0     1710 2023-05-02 07:47:08.955592 winval-0.6.2/winval/winval.g4
+-rw-r--r--   0        0        0     3297 2023-05-02 07:47:08.955592 winval-0.6.2/winval/winval_class.py
+-rw-r--r--   0        0        0     4531 2023-05-02 07:47:08.955592 winval-0.6.2/winval/workflow_var.py
+-rw-r--r--   0        0        0     3611 1970-01-01 00:00:00.000000 winval-0.6.2/PKG-INFO
```

### Comparing `winval-0.6.1/LICENSE` & `winval-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/README.md` & `winval-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/__init__.py` & `winval-0.6.2/winval/__init__.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/antlr/winval.interp` & `winval-0.6.2/winval/antlr/winval.interp`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/antlr/winval.tokens` & `winval-0.6.2/winval/antlr/winval.tokens`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/antlr/winvalLexer.interp` & `winval-0.6.2/winval/antlr/winvalLexer.interp`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/antlr/winvalLexer.py` & `winval-0.6.2/winval/antlr/winvalLexer.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/antlr/winvalLexer.tokens` & `winval-0.6.2/winval/antlr/winvalLexer.tokens`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/antlr/winvalListener.py` & `winval-0.6.2/winval/antlr/winvalListener.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/antlr/winvalParser.py` & `winval-0.6.2/winval/antlr/winvalParser.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/antlr/winvalVisitor.py` & `winval-0.6.2/winval/antlr/winvalVisitor.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/cloud_files_validator.py` & `winval-0.6.2/winval/cloud_files_validator.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/constraint_eval.py` & `winval-0.6.2/winval/constraint_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,19 +44,21 @@
 
     def visitStringExpr(self, ctx):
         return strip_string(ctx.getText())
 
     def visitEmptySetExpr(self, ctx):
         return set()
 
-
     def visitAccessExpr(self, ctx):
         collection = self.visit(ctx.struct)
         key = self.visit(ctx.key)
-        return collection[key]
+        if type(collection) == dict:
+            return collection[key] if key in collection else None
+        else:
+            return collection[key]
 
     def visitListExpr(self, ctx):
         if len(ctx.elements().INT()) > 0:
             return [int(elm.getText()) for elm in ctx.elements().INT()]
         elif len(ctx.elements().FLOAT()) > 0:
             return [float(elm.getText()) for elm in ctx.elements().FLOAT()]
         elif len(ctx.elements().STRING()) > 0:
```

### Comparing `winval-0.6.1/winval/constraints_pre_processor.py` & `winval-0.6.2/winval/constraints_pre_processor.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/parsed_workflow_inputs.py` & `winval-0.6.2/winval/parsed_workflow_inputs.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/python_extensions.py` & `winval-0.6.2/winval/python_extensions.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/validate_wdl_constraints.py` & `winval-0.6.2/winval/validate_wdl_constraints.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/wdl_parser.py` & `winval-0.6.2/winval/wdl_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                     self.__parse_structs(import_path)
 
     def _parse_structs_iter(self, wdl_lines: list[str]) -> None:
         # For extra safety, in case someone uses this protected function from outside
         wdl_lines = self.get_code_lines(wdl_lines)
         wdl_text = '\n'.join(wdl_lines)
         struct_paragraphs: list[str] = \
-            re.findall(r'struct\s+\w+\s+{\s*\n*[\[\]\w+\s*?\n]*}', wdl_text)
+            re.findall(r'struct\s+\w+\s*{\s*\n*[\[\]\w+\s*?\n]*}', wdl_text)
 
         for struct_paragraph in struct_paragraphs:
             struct_lines = re.split(r'[\n{}]', struct_paragraph)
             tokens = re.split(r'\s+', struct_lines[0])
             struct_name = tokens[1]
             logger.debug(f'\t{struct_name}')
             struct_variables = self.__parse_variables_from_block(struct_lines[1:])
```

### Comparing `winval-0.6.1/winval/winval.g4` & `winval-0.6.2/winval/winval.g4`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/winval_class.py` & `winval-0.6.2/winval/winval_class.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/winval/workflow_var.py` & `winval-0.6.2/winval/workflow_var.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.1/PKG-INFO` & `winval-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winval
-Version: 0.6.1
+Version: 0.6.2
 Summary: WDL workflow inputs validation
 License: Apache-2.0
 Author: doron
 Author-email: doron.shemtov@ultimagen.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

