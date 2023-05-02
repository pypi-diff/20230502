# Comparing `tmp/shed-2023.4.1.tar.gz` & `tmp/shed-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shed-2023.4.1.tar", last modified: Wed Apr 19 23:32:28 2023, max compression
+gzip compressed data, was "shed-2023.5.1.tar", last modified: Tue May  2 05:28:10 2023, max compression
```

## Comparing `shed-2023.4.1.tar` & `shed-2023.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:32:28.381337 shed-2023.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-19 23:32:17.000000 shed-2023.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-19 23:32:28.381337 shed-2023.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-19 23:32:17.000000 shed-2023.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:32:28.381337 shed-2023.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-19 23:32:17.000000 shed-2023.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:32:28.381337 shed-2023.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:32:28.381337 shed-2023.4.1/src/shed/
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-04-19 23:32:17.000000 shed-2023.4.1/src/shed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-19 23:32:17.000000 shed-2023.4.1/src/shed/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-19 23:32:17.000000 shed-2023.4.1/src/shed/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    27062 2023-04-19 23:32:17.000000 shed-2023.4.1/src/shed/_codemods.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:32:17.000000 shed-2023.4.1/src/shed/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:32:28.381337 shed-2023.4.1/src/shed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-19 23:32:28.000000 shed-2023.4.1/src/shed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-19 23:32:28.000000 shed-2023.4.1/src/shed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:32:28.000000 shed-2023.4.1/src/shed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 23:32:28.000000 shed-2023.4.1/src/shed.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-19 23:32:28.000000 shed-2023.4.1/src/shed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 23:32:28.000000 shed-2023.4.1/src/shed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:32:28.381337 shed-2023.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-19 23:32:17.000000 shed-2023.4.1/tests/test_expected_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-19 23:32:17.000000 shed-2023.4.1/tests/test_shed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-19 23:32:17.000000 shed-2023.4.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:10.376080 shed-2023.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-02 05:27:59.000000 shed-2023.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-02 05:28:10.376080 shed-2023.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-02 05:27:59.000000 shed-2023.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:28:10.376080 shed-2023.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-02 05:27:59.000000 shed-2023.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:10.376080 shed-2023.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:10.376080 shed-2023.5.1/src/shed/
+-rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-05-02 05:27:59.000000 shed-2023.5.1/src/shed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-02 05:27:59.000000 shed-2023.5.1/src/shed/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-02 05:27:59.000000 shed-2023.5.1/src/shed/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30471 2023-05-02 05:27:59.000000 shed-2023.5.1/src/shed/_codemods.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:27:59.000000 shed-2023.5.1/src/shed/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:10.376080 shed-2023.5.1/src/shed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-02 05:28:10.000000 shed-2023.5.1/src/shed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-02 05:28:10.000000 shed-2023.5.1/src/shed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:28:10.000000 shed-2023.5.1/src/shed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-02 05:28:10.000000 shed-2023.5.1/src/shed.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 05:28:10.000000 shed-2023.5.1/src/shed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 05:28:10.000000 shed-2023.5.1/src/shed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:10.376080 shed-2023.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-02 05:27:59.000000 shed-2023.5.1/tests/test_expected_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-02 05:27:59.000000 shed-2023.5.1/tests/test_shed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-02 05:27:59.000000 shed-2023.5.1/tests/test_version.py
```

### Comparing `shed-2023.4.1/LICENSE` & `shed-2023.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shed-2023.4.1/PKG-INFO` & `shed-2023.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shed
-Version: 2023.4.1
+Version: 2023.5.1
 Summary: `shed` canonicalises Python code.
 Home-page: https://github.com/Zac-HD/shed
 Author: Zac Hatfield-Dodds
 Author-email: zac@zhd.dev
 License: AGPL-3.0
 Project-URL: Source, https://github.com/Zac-HD/shed/
 Project-URL: Changelog, https://github.com/Zac-HD/shed/blob/master/CHANGELOG.md
@@ -77,15 +77,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with Shed by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/Zac-HD/shed
-  rev: 2023.4.1
+  rev: 2023.5.1
   hooks:
     - id: shed
       # args: [--refactor, --py39-plus]
       types_or: [python, pyi, markdown, rst]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
```

### Comparing `shed-2023.4.1/README.md` & `shed-2023.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with Shed by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/Zac-HD/shed
-  rev: 2023.4.1
+  rev: 2023.5.1
   hooks:
     - id: shed
       # args: [--refactor, --py39-plus]
       types_or: [python, pyi, markdown, rst]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
```

### Comparing `shed-2023.4.1/setup.py` & `shed-2023.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `shed-2023.4.1/src/shed/__init__.py` & `shed-2023.5.1/src/shed/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import black
 import isort
 import pyupgrade._main
 from black.mode import TargetVersion
 from black.parsing import lib2to3_parse
 from isort.exceptions import FileSkipComment
 
-__version__ = "2023.4.1"
+__version__ = "2023.5.1"
 __all__ = ["shed", "docshed"]
 
 # Conditionally imported in refactor mode to reduce startup latency in the common case
 com2ann: Any = None
 _run_codemods: Any = None
 
 _version_map = {
```

### Comparing `shed-2023.4.1/src/shed/_cli.py` & `shed-2023.5.1/src/shed/_cli.py`

 * *Files identical despite different names*

### Comparing `shed-2023.4.1/src/shed/_codemods.py` & `shed-2023.5.1/src/shed/_codemods.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 nitpicks about typing unions and literals.
 """
 
 import os
 import re
 from ast import literal_eval
 from functools import wraps
-from typing import List, Tuple
+from typing import List, Tuple, Union
 
 import libcst as cst
 import libcst.matchers as m
 from libcst.codemod import VisitorBasedCodemodCommand
 
 
 def leave(matcher):
@@ -59,22 +59,33 @@
 
     # Only the native parser supports Python 3.9 and later, but for now it's
     # only active if you set an environment variable.  Very well then:
     var = os.environ.get("LIBCST_PARSER_TYPE")
     try:
         os.environ["LIBCST_PARSER_TYPE"] = "native"
         mod = cst.parse_module(code)
+    except cst.ParserSyntaxError:
+        try:
+            compile(code, "<string>", "exec")
+        except SyntaxError:
+            # We successfully parsed this code with lib2to3 for Black, but that
+            # sometimes permits invalid syntax which libcst does not.  We'll just
+            # skip refactoring here; see https://github.com/Zac-HD/shed/issues/93
+            return code  # pragma: no branch  # version-dependent bug
+        else:  # pragma: no cover  # This is only in case of libcst bugs
+            # If the `compile()` builtin is happy, we want to crash after all.
+            raise
     finally:
         os.environ.pop("LIBCST_PARSER_TYPE")
-        if var is not None:
+        if var is not None:  # pragma: no cover  # version-dependent bug
             os.environ["LIBCST_PARSER_TYPE"] = var
 
     if imports_hypothesis(code):  # pragma: no cover
         mod = attempt_hypothesis_codemods(context, mod)
-    mod = ShedFixers(context).transform_module(mod)
+    mod = ShedFixers(context, min_version).transform_module(mod)
     return mod.code
 
 
 def oneof_names(*names):
     return m.OneOf(*map(m.Name, names))
 
 
@@ -133,14 +144,18 @@
 
     Also includes code closely modelled on pybetter's fixers, because it's
     considerably faster to run all transforms in a single pass if possible.
     """
 
     DESCRIPTION = "Fix a variety of style, performance, and correctness issues."
 
+    def __init__(self, context, min_version):
+        super().__init__(context)
+        self.min_version = min_version
+
     @m.call_if_inside(m.Raise(exc=m.Name(value="NotImplemented")))
     def leave_Name(self, _, updated_node):  # noqa
         return updated_node.with_changes(value="NotImplementedError")
 
     def leave_Assert(self, _, updated_node):  # noqa
         test_code = cst.Module("").code_for_node(updated_node.test)
         try:
@@ -672,7 +687,70 @@
                     **{side: cls._remove_recursive_helper(side_node)},
                 )
             elif m.matches(side_node, _collapsible_expression()):
                 bool_node = bool_node.with_changes(
                     **{side: side_node.args[0]},
                 )
         return bool_node
+
+    # rewrite nested `with` statement - code source from https://github.com/lensvol/pybetter/blob/master/pybetter/transformers/nested_withs.py
+
+    @leave(m.With())
+    def remove_nested_with(self, _, updated_node):
+        if self.min_version < (3, 9):
+            return updated_node
+
+        candidate_with: cst.With = updated_node
+        compound_items: List[cst.WithItem] = []
+        final_body: cst.BaseSuite = candidate_with.body
+
+        def has_leading_comment(node: Union[cst.SimpleStatementLine, cst.With]) -> bool:
+            return any([line.comment is not None for line in node.leading_lines])
+
+        header = m.AllOf(
+            m.TrailingWhitespace(),
+            m.MatchIfTrue(lambda h: h.comment is not None),
+        )
+        footer = [m.ZeroOrMore(), m.EmptyLine(comment=m.Comment()), m.ZeroOrMore()]
+
+        def has_footer_comment(body):
+            return m.matches(body, m.IndentedBlock(footer=footer))
+
+        while not (
+            # There is no way to meaningfully represent comments inside
+            # multi-line `with` statements due to how Python grammar is
+            # written, so we do not try to transform such `with` statements
+            # lest we lose something important in the comments.
+            has_leading_comment(candidate_with)
+            or m.matches(candidate_with.body, m.IndentedBlock(header=header))
+            # There is no meaningful way `async with` can be merged into
+            # the compound `with` statement.
+            or candidate_with.asynchronous
+        ):
+            compound_items.extend(candidate_with.items)
+            final_body = candidate_with.body
+
+            if not (
+                isinstance(final_body.body[0], cst.With) and len(final_body.body) == 1
+            ):
+                break  # pragma: no cover  # only reachable on some Python versions
+
+            candidate_with = cst.ensure_type(final_body.body[0], cst.With)
+
+        if len(compound_items) <= 1:
+            return updated_node
+
+        final_body = cst.ensure_type(final_body, cst.IndentedBlock)
+        topmost_body = cst.ensure_type(updated_node.body, cst.IndentedBlock)
+
+        if has_footer_comment(topmost_body) and not has_footer_comment(final_body):
+            final_body = final_body.with_changes(
+                footer=(*final_body.footer, *topmost_body.footer)
+            )
+
+        return updated_node.with_changes(
+            body=final_body,
+            items=compound_items,
+            # Black will only format with parens if they're there to start, so:
+            lpar=cst.LeftParen(),
+            rpar=cst.RightParen(),
+        )
```

### Comparing `shed-2023.4.1/src/shed.egg-info/PKG-INFO` & `shed-2023.5.1/src/shed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shed
-Version: 2023.4.1
+Version: 2023.5.1
 Summary: `shed` canonicalises Python code.
 Home-page: https://github.com/Zac-HD/shed
 Author: Zac Hatfield-Dodds
 Author-email: zac@zhd.dev
 License: AGPL-3.0
 Project-URL: Source, https://github.com/Zac-HD/shed/
 Project-URL: Changelog, https://github.com/Zac-HD/shed/blob/master/CHANGELOG.md
@@ -77,15 +77,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with Shed by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/Zac-HD/shed
-  rev: 2023.4.1
+  rev: 2023.5.1
   hooks:
     - id: shed
       # args: [--refactor, --py39-plus]
       types_or: [python, pyi, markdown, rst]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
```

### Comparing `shed-2023.4.1/tests/test_expected_output.py` & `shed-2023.5.1/tests/test_expected_output.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Update and check saved examples of shed formatting."""
 
 import pathlib
+import re
 import warnings
 
 import pytest
 
 import shed
 
 from .test_shed import check
@@ -25,14 +26,18 @@
     run the tests; the expected results will be automatically appended
     to the file.
 
     On test failure, the expected output is automatically updated.
     You can therefore see what changed by examining the `git diff`
     and roll back with `git reset`.
     """
+    stem = filename.stem
+    if re.search(r"_3\d+$", stem) and not stem.endswith(f"_3{min_version[1]}"):
+        pytest.skip(reason="Requires a different min-version spec.")
+
     joiner = "\n\n" + "=" * 80 + "\n\n"
     input_, expected, *_ = map(str.strip, (filename.read_text() + joiner).split(joiner))
     if filename.suffix == ".py" and "invalid" not in filename.stem:
         compile(input_, filename, "exec")  # check for SyntaxError
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", shed.ShedSyntaxWarning)
         result = check(
```

### Comparing `shed-2023.4.1/tests/test_shed.py` & `shed-2023.5.1/tests/test_shed.py`

 * *Files identical despite different names*

### Comparing `shed-2023.4.1/tests/test_version.py` & `shed-2023.5.1/tests/test_version.py`

 * *Files identical despite different names*

