# Comparing `tmp/appeal-0.5.3.tar.gz` & `tmp/appeal-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appeal-0.5.3.tar", last modified: Mon Feb 27 09:21:03 2023, max compression
+gzip compressed data, was "appeal-0.5.5.tar", last modified: Tue May  2 08:19:16 2023, max compression
```

## Comparing `appeal-0.5.3.tar` & `appeal-0.5.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       19 2022-01-26 11:06:53.000000 appeal-0.5.3/.gitignore
--rw-r--r--   0        0        0     1090 2023-02-27 06:45:35.508319 appeal-0.5.3/LICENSE
--rw-r--r--   0        0        0    64885 2023-02-27 09:18:43.996114 appeal-0.5.3/README.md
--rw-r--r--   0        0        0   170175 2023-02-27 09:20:06.562667 appeal-0.5.3/appeal/__init__.py
--rw-r--r--   0        0        0    23346 2023-02-27 09:13:43.802831 appeal-0.5.3/appeal/argument_grouping.py
--rw-r--r--   0        0        0     4637 2022-01-29 18:22:11.000000 appeal-0.5.3/appeal/cpp.py
--rw-r--r--   0        0        0    19640 2023-02-27 08:51:32.213401 appeal-0.5.3/appeal/text.py
--rw-r--r--   0        0        0      439 2022-01-26 11:06:53.000000 appeal-0.5.3/pyproject.toml
--rw-r--r--   0        0        0    50634 2022-01-26 11:06:53.000000 appeal-0.5.3/resources/images/appeal.logo.png
--rw-r--r--   0        0        0    18772 2022-01-26 11:06:53.000000 appeal-0.5.3/resources/images/give.your.program.appeal.png
--rw-r--r--   0        0        0      125 2022-01-26 11:06:53.000000 appeal-0.5.3/resources/links.txt
--rw-r--r--   0        0        0    64835 2023-02-27 08:50:36.639666 appeal-0.5.3/tests/run_tests.py
--rw-r--r--   0        0        0    65347 1970-01-01 00:00:00.000000 appeal-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0       19 2022-01-26 11:06:53.000000 appeal-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1090 2023-04-27 05:54:38.102243 appeal-0.5.5/LICENSE
+-rw-r--r--   0        0        0    66711 2023-05-02 08:12:32.474761 appeal-0.5.5/README.md
+-rw-r--r--   0        0        0   171316 2023-05-02 08:01:55.426889 appeal-0.5.5/appeal/__init__.py
+-rw-r--r--   0        0        0    23346 2023-04-27 05:54:38.106243 appeal-0.5.5/appeal/argument_grouping.py
+-rw-r--r--   0        0        0     4637 2022-02-12 23:26:33.980913 appeal-0.5.5/appeal/cpp.py
+-rw-r--r--   0        0        0    19692 2023-05-02 08:10:35.559115 appeal-0.5.5/appeal/text.py
+-rw-r--r--   0        0        0      537 2023-05-02 08:18:05.889159 appeal-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0    50634 2022-01-26 11:06:53.000000 appeal-0.5.5/resources/images/appeal.logo.png
+-rw-r--r--   0        0        0    18772 2022-01-26 11:06:53.000000 appeal-0.5.5/resources/images/give.your.program.appeal.png
+-rw-r--r--   0        0        0      125 2022-01-26 11:06:53.000000 appeal-0.5.5/resources/links.txt
+-rw-r--r--   0        0        0    64835 2023-04-27 05:54:38.106243 appeal-0.5.5/tests/run_tests.py
+-rw-r--r--   0        0        0    67205 1970-01-01 00:00:00.000000 appeal-0.5.5/PKG-INFO
```

### Comparing `appeal-0.5.3/LICENSE` & `appeal-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `appeal-0.5.3/README.md` & `appeal-0.5.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,30 +57,34 @@
     app.main()
 ```
 
 
 ## Overview
 
 Appeal is a command-line argument processing library for
-Python, like `argparse`, `optparse`, `getopt`, `click`,
-`docopt`, and `Typer`.  But Appeal takes a refreshing new
-approach.
+Python, like `argparse`, `optparse`, `getopt`,
+`docopt`, `Typer`, and `click`.  But Appeal takes a
+refreshing new approach.
 
 Other libraries have complicated, cumbersome interfaces
 that force you to repeat yourself over and over.
 Appeal leverages Python's rich function call interface,
-which makes defining your command-line interface effortless.
+making it effortless to define your command-line interface.
 You write Python functions, and Appeal translates them into
 command-line options and arguments.
 
 Appeal provides amazing power and flexibility--but it's
 also intuitive, because it mirrors Python itself.
 If you understand how to write Python functions,
 you're already halfway to understanding Appeal!
 
+Appeal has only one dependency,
+[my **big** library.](https://github.com/larryhastings/big)
+
+
 ### A New And Appealing Approach
 
 Appeal isn't like other command-line parsing libraries.
 In fact, you really shouldn't think of Appeal as a
 "command-line parsing library" per se. And, although you
 work with Appeal by passing in functions for Appeal to call,
 you shouldn't think of these functions as "callbacks".
@@ -704,36 +708,39 @@
 how many opargs it should consume from the command-line and how
 to convert them.
 
 
 > **An important note about annotations**
 >
 > If you use static type analysis in your project,
-> your static type analyzer may not appreciate you
-> using normal Python functions as annotations.
-> Depending on the behavior of your static type analyzer,
-> you may need to decorate your Appeal command functions
-> and converters with `@typing.no_type_check()`.  If you
-> only ever use types and classes this shouldn't be
-> necessary.
+> your static type analyzer may not enjoy analyzing Python
+> code using Appeal.  Static type analyzers are designed
+> to understand "type hints", a means of specifying static
+> type information introduced in Python 3.5 with the
+> `typing` module.  But Appeal doesn't use type hints,
+> and there are some ways Appeal uses annotations that
+> static type analyzers may not like.
 >
-> Also, Appeal doesn't understand "type hint"
-> annotations.  It expects annotations to be callables,
-> like functions or classes or types.  It should be
-> possible to add limited support in the future.
+> Fortunately, there are ways to get static type analyzers
+> to work alongside Appeal.
+>
+> First, you can decorate your Appeal command functions
+> and converters with `@typing.no_type_check()`.  This should
+> only be necessary if you use functions as annotations;
+> if you only ever use types and classes, this shouldn't be
+> necessary.
 >
-> Finally, Appeal uses function calls and related
-> snazzy technology in annotations--but many static
-> type checkers expect annotations to conform strictly
-> to only what is used for "type hints".  So it's
-> possible static type checkers may abort processing
-> in a file with advanced Appeal configuration.
-> It may be best to mix "type hints" and Appeal
-> in the same Python script, and to not run your
-> static type checker on scripts with Appeal code.
+> Second, if you're using Python 3.9 or newer, you can use
+> `typing.Annotated` with your annotations.  `typing.Annotated`
+> allows you to specify an ordered list of values, and static
+> type hints only ever use the *first* value.  Appeal also
+> handles `typing.Annotated`, but Appeal only ever uses the
+> *last* value.  This makes it easy--you can have both types
+> of annotations, side by side, and both static type checkers
+> and Appeal are perfectly happy.
 
 
 ## Converter Flexibility
 
 You can use almost any function as an annotation...
 within reason.  Appeal will introspect your annotation,
 determine its input parameters, and call it to convert
@@ -877,15 +884,15 @@
 
 
 Of course, you can also subclass `MultiOption` to make your own
 converter classes with custom behavior. `MultiOption` subclasses
 can override these three methods:
 
 ```Python
-class Option:
+class MultiOption:
 
     def init(self, default):
         ...
 
     def option(self, ...):
         ...
 
@@ -938,17 +945,29 @@
 you to decide how to store them, and how to
 render them into a single value returned
 by your `render()` method.
 
 `MultiOption` is a subclass of a general
 `Option` class.  `Option` behaves identically
 to `MultiOption`, except it only permits
-specifying the option once on the command-line.
-(Which means it will only your `option()`
-method once.)
+specifying the option once on the command-line,
+which means it will only your `option()`
+method once.
+You usually don't need to bother with making subclasses
+of `Option`--it's usually better to just use a class
+directly, like our `class IntAndFloat` example.
+The only feature you get by subclassing `Option` is,
+you get the default value for the parameter passed in
+to your constructor.
+
+(The downside of subclassing `Option` and `MultiOption`
+is that it makes exporting your Appeal API as an automation
+API a little less convenient for the user, because your
+users will have to construct these objects and feed
+values into them by calling the `option` method.)
 
 
 ## Data Validation
 
 What if you want to restrict the data the user provides
 on the command-line?  That's simple, just use a converter!
 Appeal provides a couple sample converters for data validation,
@@ -1939,7 +1958,42 @@
 
 Restrictions on Appeal command functions:
 
 * You may not use `inspect.Parameter.empty` as a default value
   for any keyword-only parameter to a converter or command function.
 * The converter for a *var_positional* (`*args`) parameter
   *must* require at least one positional argument.
+
+
+## Changelog
+
+**0.5.5**
+
+* Add support for `typing.Annotated`, new in Python 3.9.
+* Add dependency to
+  [my **big** library.](https://github.com/larryhastings/big)
+  This gives Appeal a much better implementation of `multisplit`,
+  and I plan to switch to the **big** word wrapper and columnizer
+  functions, which are a... "big" improvement over what's in
+  Appeal right now.
+* Rename `SingleOption` to just `Option`.  (The name
+  `SingleOption` is now deprecated, but I'll leave it
+  as a redundant name for `Option`... for now.)
+
+**0.5.3**
+
+* Fix compatibility back to Python 3.6.
+
+**0.5.2**
+
+* Fix compatibility with Python 3.11.  Python's `inspect.Parameter` object
+  no longer allows a `name` that happens to be a keyword, which was a minor
+  inconvenience (Appeal used to use `lambda` here sometimes).
+
+**0.5.1**
+
+* Fixed regression, issue #5.  If you didn't supply enough required
+  parameters, you'd get a `TypeError` instead of a proper usage error.
+
+**0.5**
+
+* Initial release!
```

### Comparing `appeal-0.5.3/appeal/__init__.py` & `appeal-0.5.5/appeal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 "A powerful & Pythonic command-line parsing library.  Give your program Appeal!"
-__version__ = "0.5.3"
+__version__ = "0.5.5"
 
 
 # please leave this copyright notice in binary distributions.
 license = """
 appeal/__init__.py
 part of the Appeal software package
 Copyright 2021-2023 by Larry Hastings
@@ -31,14 +31,15 @@
 """
 
 want_prints = 1
 want_prints = 0
 
 
 from abc import abstractmethod, ABCMeta
+import big.all as big
 import builtins
 import collections
 import enum
 import functools
 import inspect
 import itertools
 import math
@@ -48,14 +49,26 @@
 import shlex
 import string
 import sys
 import textwrap
 import time
 import types
 
+try:
+    from typing import Annotated
+    AnnotatedType = type(Annotated[int, str])
+    del Annotated
+    def dereference_annotated(annotation):
+        if isinstance(annotation, AnnotatedType):
+            return annotation.__metadata__[-1]
+        return annotation
+except ImportError:
+    def dereference_annotated(annotation):
+        return annotation
+
 from . import argument_grouping
 from . import text
 
 reversed_dict_values = argument_grouping.reversed_dict_values
 
 
 POSITIONAL_ONLY = inspect.Parameter.POSITIONAL_ONLY
@@ -1257,29 +1270,30 @@
             a.load_converter(key)
             a.consume_argument(is_oparg=True)
             a.store_kwargs(parameter.name)
             a.pop_context()
             a.end(name=program_name, id=program.id)
             program.opcodes = a.opcodes
         else:
-            if not is_legal_annotation(parameter.annotation):
+            annotation = dereference_annotated(parameter.annotation)
+            if not is_legal_annotation(annotation):
                 raise AppealConfigurationError(f"{parent_callable.__name__}: parameter {parameter.name!r} annotation is {parameter.annotation}, which you can't use directly, you must call it")
 
             # self.ensure_callables_have_unique_names(callable)
             multioption = issubclass(cls, MultiOption)
 
             cc = CharmCompiler(self.appeal, name=program_name, converter_key=self.program.converter_key)
             a = cc.initial_a
             a.push_context()
 
             a = cc.final_a
             a.pop_context()
 
             store_kwargs = key, parameter.name
-            program = cc.compile(parameter.annotation, parameter.default, is_option=True, multioption=multioption, depth=depth+1, store_kwargs=store_kwargs)
+            program = cc.compile(annotation, parameter.default, is_option=True, multioption=multioption, depth=depth+1, store_kwargs=store_kwargs)
             assert self.program.converter_key != cc.program.converter_key
             self.program.converter_key = cc.program.converter_key
 
         for option in options:
             # option doesn't have to be unique in this argument group,
             # but it must be unique per consumed argument.
             # (you can't define the same option twice without at least one consume_argument between.)
@@ -1304,15 +1318,15 @@
             print(f"[cc] {indent}{callable.__name__} map_options parameter={parameter} key={key} signature={signature}")
         _, kw_parameters, _ = self.appeal.fn_database_lookup(callable)
         mappings = kw_parameters.get(parameter.name, ())
 
         if not mappings:
             p = signature.parameters.get(parameter.name)
             assert p
-            annotation = p.annotation
+            annotation = dereference_annotated(p.annotation)
             default = p.default
             default_options = self.appeal.root.default_options
             assert builtins.callable(default_options)
             default_options(self.appeal, callable, parameter.name, annotation, default)
 
         parameter_index_to_options = collections.defaultdict(list)
         parameters = []
@@ -1344,20 +1358,21 @@
             indent = "  " * depth
             print(f"[cc] {indent}compiling 'parameter={parameter}' depth={depth}, pgi, multioption={multioption} append={append}")
 
         maps_to_positional = set((POSITIONAL_ONLY, POSITIONAL_OR_KEYWORD, VAR_POSITIONAL))
         tracked_by_argument_grouping = set((POSITIONAL_ONLY, POSITIONAL_OR_KEYWORD, VAR_POSITIONAL))
 
         # hard-coded, at least for now
-        if parameter.annotation is not empty:
-            cls = parameter.annotation
+        annotation = dereference_annotated(parameter.annotation)
+        if annotation is not empty:
+            cls = annotation
         elif parameter.default is not empty:
             cls = type(parameter.default)
 
-        callable = parameter.annotation
+        callable = annotation
         cls = self.root.map_to_converter(parameter)
         signature = cls.get_signature(parameter)
         parameters = signature.parameters
         if want_prints:
             print(f"[cc] {indent}cls={cls} signature={signature}")
 
         if depth == 0:
@@ -1438,16 +1453,17 @@
         # of that degenerate converter tree--in this case, the parameter "abc" from
         # the function "foo".
 
         for i, (parameter_name, p) in enumerate(parameters.items()):
             if not p.kind in maps_to_positional:
                 continue
 
-            if not is_legal_annotation(p.annotation):
-                raise AppealConfigurationError(f"{callable.__name__}: parameter {parameter.name!r} annotation is {parameter.annotation}, which you can't use directly, you must call it")
+            annotation = dereference_annotated(p.annotation)
+            if not is_legal_annotation(annotation):
+                raise AppealConfigurationError(f"{callable.__name__}: parameter {p.name!r} annotation is {p.annotation}, which you can't use directly, you must call it")
 
             # FIXME it's lame to do this here,
             # you need to rewrite _compile so it
             # always recurses for positional parameters
             cls = self.root.map_to_converter(p)
 
             if p.kind == VAR_POSITIONAL:
@@ -1462,15 +1478,15 @@
                 usage_callable = callable
                 usage = usage_parameter = parameter_name
 
             usage = positionals.get(parameter_name, usage)
 
             if want_prints:
                 printable_default = "(empty)" if p.default is empty else repr(p.default)
-                print(f"[cc] {indent}{callable.__name__} positional parameter {i}: p={p} p.kind={p.kind!s} annotation={p.annotation.__name__} default={printable_default} cls={cls}")
+                print(f"[cc] {indent}{callable.__name__} positional parameter {i}: p={p} p.kind={p.kind!s} annotation={annotation.__name__} default={printable_default} cls={cls}")
 
             # only create new groups here if it's an optional group
             # (we pre-create the initial, required group)
             pgi_parameter = next(pgi)
             if want_prints:
                 print(f"[cc] {indent}pgi_parameter={pgi_parameter}")
             if pgi_parameter.first_in_group and (not pgi_parameter.in_required_group):
@@ -1699,20 +1715,20 @@
             print("________________")
             print()
         else:
             print_divider = True
         program = programs.popleft()
         width = 2
         padding = " " * width
-        indent2 = indent + f" {padding}|   "
+        indent2 = indent + f"{padding}|   "
         print(program)
         for i, op in enumerate(program):
             suffix = ""
             printable_op = str(op.op).rpartition(".")[2]
-            print(f"{indent}[{i:0{width}}] {printable_op}{suffix}")
+            print(f"{indent}{i:0{width}}| {printable_op}{suffix}")
             # for slot in op.__class__.__slots__:
             for slot in dir(op):
                 if slot.startswith("_") or slot in ("copy", "op"):
                     continue
                 value = getattr(op, slot, None)
                 if slot == "program":
                     print(f"{indent2}program={value}")
@@ -1954,60 +1970,58 @@
     next_options_token = 0
     options_stack = []
     options_bucket = {}
 
     options_bucket = None
     options_token = None
 
+    if want_prints:
+        ip_spacer = '    '
+
     def push_options():
         nonlocal options_bucket
         nonlocal options_token
         nonlocal next_options_token
         options_stack.append(options_bucket)
         options_bucket = {}
         options_token = next_options_token
         next_options_token += 1
         token_to_bucket[options_token] = options_bucket
         bucket_to_token[id(options_bucket)] = options_token
         if want_prints:
-            print(f"##       push_options options_token={options_token}")
-
-    # create our first actual options bucket
-    push_options()
-    # ... but remove the useless None in the stack
-    options_stack.clear()
+            print(f"## {ip_spacer} push_options options_token={options_token}")
 
     def pop_options():
         nonlocal options_bucket
         nonlocal options_token
 
         token = bucket_to_token[id(options_bucket)]
         del bucket_to_token[id(options_bucket)]
         del token_to_bucket[token]
 
         options_bucket = options_stack.pop()
         options_token = bucket_to_token[id(options_bucket)]
 
         if want_prints:
-            print(f"##       pop_options, now at token {options_token}, popped options_bucket={options_bucket}")
+            print(f"## {ip_spacer} pop_options, now at token {options_token}, popped options_bucket={options_bucket}")
 
     def pop_options_to_token(token):
         bucket = token_to_bucket.get(token)
         if bucket is None:
             return
         pop_count = 0
         while options_bucket != bucket:
             pop_count += 1
             pop_options()
         if want_prints:
-            print(f"##     pop_options_to_token token={token} took {pop_count} pops")
+            print(f"## {ip_spacer} pop_options_to_token token={token} took {pop_count} pops")
 
     def pop_options_to_base():
         if want_prints:
-            print(f"##     pop_options_to_base, popping {len(options_stack)} times")
+            print(f"## {ip_spacer} pop_options_to_base, popping {len(options_stack)} times")
         for _ in range(len(options_stack)):
             pop_options()
 
     def find_option(option):
         depth = 0
         bucket = options_bucket
         bucket_iter = reversed(options_stack)
@@ -2061,28 +2075,28 @@
     undo_converters_stack = []
 
     def reset_undo_converters():
         nonlocal converters_are_undoable
         converters_are_undoable = True
         undo_converters_list.clear()
         if want_prints:
-            print(f"##     reset_undo_converters()")
+            print(f"## {ip_spacer} reset_undo_converters()")
 
     def forget_undo_converters():
         nonlocal converters_are_undoable
         undo_converters_list.clear()
         converters_are_undoable = False
         if want_prints:
-            print(f"##     forget_undo_converters()")
+            print(f"## {ip_spacer} forget_undo_converters()")
 
     def add_undoable_converter(parent):
         if converters_are_undoable:
             undo_converters_list.append(parent)
             if want_prints:
-                print(f"##     add_undoable_converter(parent={parent})")
+                print(f"## {ip_spacer} add_undoable_converter(parent={parent})")
 
     def push_undo_converters():
         nonlocal undo_converters_list
         nonlocal converters_are_undoable
         undo_converters_stack.append((undo_converters_list, converters_are_undoable))
         undo_converters_list = []
         converters_are_undoable = True
@@ -2096,28 +2110,39 @@
         print_spacer=True
         for parent in reversed(undo_converters_list):
             o = parent.args_converters.pop()
             if want_prints:
                 if print_spacer:
                     print(f"##")
                     print_spacer = False
-                print(f"##     undo converter")
-                print(f"##         parent={parent}")
-                print(f"##         popped o={o}")
-                print(f"##         arg_converters={parent.args_converters}")
+                print(f"## {ip_spacer} undo converter")
+                print(f"## {ip_spacer}     parent={parent}")
+                print(f"## {ip_spacer}     popped o={o}")
+                print(f"## {ip_spacer}     arg_converters={parent.args_converters}")
         undo_converters_list.clear()
 
-    first_print_string = ""
+    if want_prints:
+        charm_separator_line = f"############################################################"
+        print(charm_separator_line)
+        print("##")
+        print('## charm_parse start')
+        print('##')
+        print('## create initial options bucket')
+
+    # create our first actual options bucket
+    push_options()
+    # ... but remove the useless None in the stack
+    options_stack.clear()
+
     waiting_op = None
     prev_op = None
     while ci or argi:
         if want_prints:
-            print(first_print_string)
-            first_print_string = "##"
-            print(f"############################################################")
+            print('##')
+            print(charm_separator_line)
             print(f"## cmdline {list(argi.values)}")
 
         # first, run ci until we either
         #    * finish the program, or
         #    * must consume a command-line argument
         for op in ci:
             prev_op = waiting_op
@@ -2128,61 +2153,61 @@
                 ip_spacer = " " * len(ip)
                 converter = ci.repr_converter(ci.converter)
                 o = ci.repr_converter(ci.o)
                 _total = ci.total and ci.total.summary()
                 _group = ci.group and ci.group.summary()
                 print(f"##")
                 print(f"## {ip} converter={converter} o={o}")
-                print(f"## {ip_spacer} total={_total}")
-                print(f"## {ip_spacer} group={_group}")
+                print(f"## {ip_spacer} - total={_total}")
+                print(f"## {ip_spacer} - group={_group}")
 
             if op.op == opcode.create_converter:
                 r = None if op.parameter.kind == KEYWORD_ONLY else root
                 cls = appeal.map_to_converter(op.parameter)
                 converter = cls(op.parameter, appeal)
                 ci.converters[op.key] = ci.o = converter
                 if not root:
                     root = converter
                 if want_prints:
-                    print(f"##     create_converter key={op.key} parameter={op.parameter}")
-                    print(f"##         converter={converter}")
+                    print(f"## {ip_spacer} create_converter key={op.key} parameter={op.parameter}")
+                    print(f"## {ip_spacer}   converter={converter}")
                 continue
 
             if op.op == opcode.load_converter:
                 ci.converter = ci.converters.get(op.key, None)
                 converter = ci.repr_converter(ci.converter)
                 if want_prints:
-                    print(f"##     load_converter op.key={op.key} converter={converter!s}")
+                    print(f"## {ip_spacer} load_converter op.key={op.key} converter={converter!s}")
                 continue
 
             if op.op == opcode.load_o:
                 ci.o = ci.converters.get(op.key, None)
                 if want_prints:
                     o = ci.repr_converter(ci.o)
-                    print(f"##     load_o op.key={op.key} o={o!s}")
+                    print(f"## {ip_spacer} load_o op.key={op.key} o={o!s}")
                 continue
 
             if op.op == opcode.load_o_option:
                 ci.option = op.option
                 if want_prints:
-                    print(f"##     load_o_option op.option={op.option} o={o!s}")
+                    print(f"## {ip_spacer} load_o_option op.option={op.option} o={o!s}")
                 continue
 
             if op.op == opcode.map_option:
                 options_bucket[op.option] = op.program
                 if want_prints:
-                    print(f"##     map_option op.option={op.option} op.program={op.program} token {options_token}")
+                    print(f"## {ip_spacer} map_option op.option={op.option} op.program={op.program} token {options_token}")
                 continue
 
             if op.op == opcode.append_args:
                 ci.converter.args_converters.append(ci.o)
                 add_undoable_converter(ci.converter)
                 if want_prints:
                     o = ci.repr_converter(ci.o)
-                    print(f"##     append_args o={o}")
+                    print(f"## {ip_spacer} append_args o={o}")
                 continue
 
             if op.op == opcode.store_kwargs:
                 converter = ci.o
                 if op.name in ci.converter.kwargs_converters:
                     existing = ci.converter.kwargs_converters[op.name]
                     if not ((existing == converter) and isinstance(existing, MultiOption)):
@@ -2190,83 +2215,83 @@
                         raise AppealUsageError(f"{ci.option} specified more than once.")
                     # we're setting the kwarg to the value it's already set to,
                     # and it's a multioption, so this is fine.
                     continue
                 ci.converter.kwargs_converters[op.name] = ci.o
                 if want_prints:
                     o = ci.repr_converter(ci.o)
-                    print(f"##     store_kwargs name={op.name} o={o}")
+                    print(f"## {ip_spacer} store_kwargs name={op.name} o={o}")
                 continue
 
             if op.op == opcode.consume_argument:
                 if want_prints:
-                    print(f"##     consume_argument is_oparg={op.is_oparg}")
+                    print(f"## {ip_spacer} consume_argument is_oparg={op.is_oparg}")
                 if not argi:
                     if want_prints:
-                        print(f"##     no more arguments, aborting program")
+                        print(f"## {ip_spacer}     no more arguments, aborting program")
                     ci.abort()
                 break
 
             if op.op == opcode.push_context:
                 ci.push_context()
                 push_undo_converters()
                 if want_prints:
-                    print(f"##     push_context")
+                    print(f"## {ip_spacer} push_context")
                 continue
 
             if op.op == opcode.pop_context:
                 pop_undo_converters()
                 ci.pop_context()
                 if want_prints:
-                    print(f"##     pop_context")
+                    print(f"## {ip_spacer} pop_context")
                 continue
 
             if op.op == opcode.set_group:
                 ci.group = op.group.copy()
                 reset_undo_converters()
                 if want_prints:
-                    print(f"##     set_group {ci.group.summary()}")
+                    print(f"## {ip_spacer} set_group {ci.group.summary()}")
                 continue
 
             if op.op == opcode.flush_multioption:
                 assert isinstance(ci.o, MultiOption), f"expected instance of MultiOption but ci.o={ci.o}"
                 ci.o.flush()
                 if want_prints:
                     o = ci.repr_converter(ci.o)
-                    print(f"##     flush_multioption o={o}")
+                    print(f"## {ip_spacer} flush_multioption o={o}")
                 continue
 
             if op.op == opcode.jump:
                 if want_prints:
-                    print(f"##     jump op.address={op.address}")
+                    print(f"## {ip_spacer} jump op.address={op.address}")
                 ci.i.jump(op.address)
                 continue
 
             if op.op == opcode.jump_relative:
                 if want_prints:
-                    print(f"##     jump_relative op.delta={op.delta}")
+                    print(f"## {ip_spacer} jump_relative op.delta={op.delta}")
                 ci.i.jump_relative(op.delta)
                 continue
 
             if op.op == opcode.branch_on_o:
                 if want_prints:
-                    print(f"##     branch_on_o o={ci.o} op.address={op.address}")
+                    print(f"## {ip_spacer} branch_on_o o={ci.o} op.address={op.address}")
                 if ci.o:
                     ci.i.jump(op.address)
                 continue
 
             if op.op == opcode.comment:
                 if want_prints:
-                    print(f"##     comment {op.comment!r}")
+                    print(f"## {ip_spacer} comment {op.comment!r}")
                 continue
 
             if op.op == opcode.end:
                 if want_prints:
                     name = str(op.op).partition(".")[2]
-                    print(f"##     {name} id={op.id} name={op.name!r}")
+                    print(f"## {ip_spacer} {name} id={op.id} name={op.name!r}")
                 continue
 
             raise AppealConfigurationError(f"unhandled opcode op={op}")
 
         else:
             # we finished the program
             if want_prints:
@@ -2306,49 +2331,49 @@
         #        is done, and we don't have a consume_argument
         #        to give it to.  so push it back onto argi
         #        and exit.  (hopefully the argument is the
         #        name of a command/subcomand.)
 
         for a in argi:
             if want_prints:
-                print("#]")
+                print("#[]")
 
             is_oparg = op and (op.op == opcode.consume_argument) and op.is_oparg
             # if this is true, we're consuming a top-level command-line argument.
             # if this is false, we're processing an oparg.
             # what's the difference? opargs can't be options.
             is_positional_argument = (
                 appeal.root.force_positional
                 or ((not a.startswith("-")) or (a == "-"))
                 or is_oparg
                 )
 
             if want_prints:
                 # print_op = "consume_argument" if op else None
                 print_op = op
-                print(f"#] process argument {a!r} {list(argi.values)}")
-                print(f"#] op={print_op}")
+                print(f"#[]  process argument {a!r} {list(argi.values)}")
+                print(f"#[]  op={print_op}")
 
             if is_positional_argument:
                 if not op:
                     if want_prints:
-                        print(f"#]     positional argument we can't handle.  exit.")
+                        print(f"#[]  positional argument we can't handle.  exit.")
                     argi.push(a)
                     return ci.converters[0]
 
                 ci.o = a
                 forget_undo_converters()
                 if ci.group:
                     ci.group.count += 1
                 if ci.total:
                     ci.total.count += 1
                 if not is_oparg:
                     pop_options_to_base()
                 if want_prints:
-                    print(f"#]     positional argument.  o={ci.o!r}")
+                    print(f"#[]  positional argument.  o={ci.o!r}")
                 # return to the interpreter
                 break
 
             # it's an option!  or "--".
 
             if not option_space_oparg:
                 raise AppealConfigurationError("oops, option_space_oparg must currently be True")
@@ -2363,25 +2388,25 @@
             # it's set to X if the user specifies an X, otherwise it's None.
             split_value = None
 
             if a.startswith("--"):
                 if a == "--":
                     appeal.root.force_positional = True
                     if want_prints:
-                        print(f"#]     '--', force_positional=True")
+                        print(f"#[]  '--', force_positional=True")
                     continue
 
                 option, equals, _split_value = a.partition("=")
                 if equals:
                     split_value = _split_value
 
                 program, maximum_arguments, token = find_option(option)
                 option_stack_tokens.append(token)
                 if want_prints:
-                    print(f"#]     option {denormalize_option(option)} program={program}")
+                    print(f"#[]  option {denormalize_option(option)} program={program}")
                 queue.append((option, program, maximum_arguments, split_value, True))
             else:
                 options = collections.deque(a[1:])
 
                 while options:
                     option = options.popleft()
                     equals = short_option_equals_oparg and options and (options[0] == '=')
@@ -2390,27 +2415,27 @@
                         split_value = "".join(options)
                         options = ()
                     program, maximum_arguments, token = find_option(option)
                     option_stack_tokens.append(token)
                     # if it takes no arguments, proceed to the next option
                     if not maximum_arguments:
                         if want_prints:
-                            print(f"#]     option {denormalize_option(option)}")
+                            print(f"#[]  option {denormalize_option(option)}")
                         queue.append([denormalize_option(option), program, maximum_arguments, split_value, False])
                         continue
                     # this eats arguments.  if there are more characters waiting,
                     # they must be the split value.
                     if options:
                         assert not split_value
                         split_value = "".join(options)
                         options = ()
                         if not short_option_concatenated_oparg:
                             raise AppealUsageError(f"'-{option}{split_value}' is not allowed, use '-{option} {split_value}'")
                     if want_prints:
-                        print(f"#]     option {denormalize_option(option)}")
+                        print(f"#[]  option {denormalize_option(option)}")
                     queue.append([denormalize_option(option), program, maximum_arguments, split_value, False])
 
                 # mark the last entry in the queue as last
                 queue[-1][-1] = True
 
             assert queue and option_stack_tokens
 
@@ -2427,31 +2452,31 @@
             # and now push on a new bucket.
             push_options()
 
             # process options in reverse here!
             # that's because we push each program on the interpreter.  so, LIFO.
             for error_option, program, maximum_arguments, split_value, is_last in reversed(queue):
                 if want_prints:
-                    print(f"#]     executing option {option} split_value={split_value}")
-                    print(f"#]     call program={program}")
+                    print(f"#[]  executing option {option} split_value={split_value}")
+                    print(f"#[]  call program={program}")
 
                 if not is_last:
                     total = program.total
                     assert maximum_arguments == 0
 
                 if split_value is not None:
                     assert is_last
                     if maximum_arguments != 1:
                         if maximum_arguments == 0:
                             raise AppealUsageError(f"{error_option} doesn't take an argument")
                         if maximum_arguments >= 2:
                             raise AppealUsageError(f"{error_option} given a single argument but it requires multiple arguments, you must separate the arguments with spaces")
                     argi.push(split_value)
                     if want_prints:
-                        print(f"#]     pushing split value {split_value!r} on argi")
+                        print(f"#[]  pushing split value {split_value!r} on argi")
 
                 ci.option = error_option
                 ci.call(program)
             break
 
     undo_converters()
     satisfied = True
@@ -2478,20 +2503,20 @@
         message = f"{program.name} requires {middle} {which}."
 
         raise AppealUsageError(message)
 
     if want_prints:
         print(f"##")
         print(f"## ending parse.")
-        finished_state = "not finished" if ci else "finished"
-        print(f"##   program was {finished_state}.")
+        finished_state = "did not finish" if ci else "finished"
+        print(f"##      program {finished_state}.")
         if argi:
-            print(f"##   remaining cmdline {list(argi.values)}")
+            print(f"##      remaining cmdline: {list(argi.values)}")
         else:
-            print(f"##   cmdline was consumed.")
+            print(f"##      cmdline was completely consumed.")
         print(f"############################################################")
         print()
 
     return ci.converters[0]
 
 
 class SpecialSection:
@@ -2525,15 +2550,15 @@
     in its parameters using command-line arguments.
     It introspects the function passed in, creating
     a tree of sub-Converter objects underneath it.
 
     A Converter
     """
     def __init__(self, parameter, appeal):
-        callable = parameter.annotation
+        callable = dereference_annotated(parameter.annotation)
         default = parameter.default
 
         # self.fn = callable
         self.callable = callable
 
         if not hasattr(self, '__signature__'):
             self.__signature__ = self.get_signature(parameter)
@@ -2553,15 +2578,15 @@
 
         self.reset()
 
     @classmethod
     def get_signature(cls, parameter):
         if hasattr(cls, "__signature__"):
             return cls.__signature__
-        return inspect.signature(parameter.annotation, follow_wrapped=False)
+        return inspect.signature(dereference_annotated(parameter.annotation), follow_wrapped=False)
 
     def reset(self):
         # collections of converters we'll use to compute *args and **kwargs.
         # contains either raw strings or Converter
         # objects which we'll call.  these are the
         # output of parse() and the input of convert().
         self.args_converters = []
@@ -2694,18 +2719,18 @@
 def parse_str(str) -> str: pass
 class SimpleTypeConverterStr(SimpleTypeConverter):
     __signature__ = inspect.signature(parse_str)
     callable = str
 simple_type_signatures[str] = SimpleTypeConverterStr
 
 
-class Option(Converter):
+class BaseOption(Converter):
     pass
 
-class InferredOption(Option):
+class InferredOption(BaseOption):
     def __init__(self, parameter, appeal):
         if not parameter.default:
             raise AppealConfigurationError(f"empty {type(parameter.default)} used as default, so we can't infer types")
         p2 = inspect.Parameter(parameter.name, kind=parameter.kind, annotation=type(parameter.default), default=parameter.default)
         super().__init__(p2, appeal)
 
     @classmethod
@@ -2769,15 +2794,15 @@
         return_annotation = parameters['return']
         del parameters['return']
     else:
         return_annotation = empty
     return inspect.Signature(parameters.values(), return_annotation=return_annotation)
 
 
-class SingleOption(Option):
+class Option(BaseOption):
     def __init__(self, parameter, appeal):
         # the callable passed in is ignored
         p2 = inspect.Parameter(parameter.name, kind=parameter.kind, annotation=self.option, default=parameter.default)
         super().__init__(p2, appeal)
         self.init(parameter.default)
 
     def __repr__(self):
@@ -2834,29 +2859,32 @@
     # called for the last time.  it should return the "value"
     # for the option.
     @abstractmethod
     def render(self):
         pass
 
 
+# the old name, now deprecated
+SingleOption = Option
+
+
 def parse_bool_option() -> bool: pass
-class BooleanOptionConverter(SingleOption):
+class BooleanOptionConverter(Option):
     __signature__ = inspect.signature(parse_bool_option)
 
     def init(self, default):
         self.value = default
 
     def option(self):
         self.value = not self.value
 
     def render(self):
         return self.value
 
-
-class MultiOption(SingleOption):
+class MultiOption(Option):
     def __init__(self, parameter, appeal):
         self.multi_converters = []
         self.multi_args = []
         # the callable passed in is ignored
         p2 = inspect.Parameter(parameter.name, kind=parameter.kind, annotation=self.option, default=parameter.default)
         super().__init__(p2, appeal)
 
@@ -3002,30 +3030,22 @@
     """
     Creates a converter function that splits a string
     based on one or more separator strings.
 
     If you don't supply any separators, splits on
     any whitespace.
 
-    If strip is True, also calls strip() on the
-    strings after splitting.
+    If strip is True, also strips the separators
+    from the beginning and end of the string.
     """
-    if not separators:
-        def split(str):
-            return str.split()
-        return split
-
     if not all((s and isinstance(s, str)) for s in separators):
         raise AppealConfigurationError("split(): every separator must be a non-empty string")
 
     def split(str):
-        values = text.multisplit(str, separators)
-        if strip:
-            values = [s.strip() for s in values]
-        return values
+        return list(big.multisplit(str, separators, strip=strip))
     return split
 
 
 
 @must_be_instance
 def validate(*values, type=None):
     """
@@ -3117,39 +3137,42 @@
         return None
     if (callable == bool) and (parameter.kind == KEYWORD_ONLY):
         return BooleanOptionConverter
     return cls
 
 none_and_empty = ((None, empty))
 def unannotated_to_converter(parameter):
-    if (parameter.annotation in none_and_empty) and (parameter.default in none_and_empty):
+    if (dereference_annotated(parameter.annotation) in none_and_empty) and (parameter.default in none_and_empty):
         return SimpleTypeConverterStr
 
 
 def type_to_converter(parameter):
-    if not isinstance(parameter.annotation, type):
+    annotation = dereference_annotated(parameter.annotation)
+    if not isinstance(annotation, type):
         return None
-    cls = simple_type_to_converter(parameter, parameter.annotation)
+    cls = simple_type_to_converter(parameter, annotation)
     if cls:
         return cls
-    if issubclass(parameter.annotation, SingleOption):
-        return parameter.annotation
+    if issubclass(annotation, SingleOption):
+        return annotation
     return None
 
 def callable_to_converter(parameter):
-    if (parameter.annotation is empty) or (not builtins.callable(parameter.annotation)):
+    annotation = dereference_annotated(parameter.annotation)
+    if (annotation is empty) or (not builtins.callable(annotation)):
         return None
     if parameter.kind == KEYWORD_ONLY:
-        return Option
+        return BaseOption
     return Converter
 
 illegal_inferred_types = {dict, set, tuple, list}
 
 def inferred_type_to_converter(parameter):
-    if (parameter.annotation is not empty) or (parameter.default is empty):
+    annotation = dereference_annotated(parameter.annotation)
+    if (annotation is not empty) or (parameter.default is empty):
         return None
     inferred_type = type(parameter.default)
     # print(f"inferred_type_to_converter(parameter={parameter})")
     cls = simple_type_to_converter(parameter, inferred_type)
     # print(f"  inferred_type={inferred_type} cls={cls}")
     if cls:
         return cls
@@ -3159,15 +3182,16 @@
         return None
     if parameter.kind == KEYWORD_ONLY:
         return InferredOption
     return InferredConverter
 
 sequence_types = {tuple, list}
 def sequence_to_converter(parameter):
-    if (parameter.annotation is not empty) or (parameter.default is empty):
+    annotation = dereference_annotated(parameter.annotation)
+    if (annotation is not empty) or (parameter.default is empty):
         return None
     inferred_type = type(parameter.default)
     if inferred_type not in sequence_types:
         return None
     if parameter.kind == KEYWORD_ONLY:
         return InferredSequenceOption
     return InferredSequenceConverter
@@ -3831,22 +3855,22 @@
         values = []
         values_callable_index = {}
 
         positional_parameter_kinds = set((POSITIONAL_ONLY, POSITIONAL_OR_KEYWORD, VAR_POSITIONAL))
 
         for c in reversed_dict_values(ci.converters.values()):
             parameter = c['parameter']
-            callable = parameter.annotation
+            callable = dereference_annotated(parameter.annotation)
 
             positional_children = set()
             option_children = set()
             cls = self.root.map_to_converter(parameter)
             signature = cls.get_signature(parameter)
             for p in signature.parameters.values():
-                annotation = p.annotation
+                annotation = dereference_annotated(p.annotation)
                 cls2 = self.root.map_to_converter(p)
                 if not issubclass(cls2, SimpleTypeConverter):
                     if p.kind in positional_parameter_kinds:
                         positional_children.add(annotation)
                     elif p.kind == KEYWORD_ONLY:
                         option_children.add(annotation)
             values_callable_index[callable] = len(values)
@@ -4474,17 +4498,15 @@
         return self.usage(usage=True, summary=True, doc=True)
 
     def version(self):
         print(self.support_version)
 
     def help(self, *command):
         """
-        Print help on a thingy.
-
-        Prints lots and lots of help.
+        Print usage documentation on a specific command.
         """
         commands = " ".join(command)
         appeal = self
         for name in command:
             appeal = appeal.commands.get(name)
             if not appeal:
                 raise AppealUsageError(f'"{name}" is not a legal command.')
```

### Comparing `appeal-0.5.3/appeal/argument_grouping.py` & `appeal-0.5.5/appeal/argument_grouping.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.3/appeal/cpp.py` & `appeal-0.5.5/appeal/cpp.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.3/appeal/text.py` & `appeal-0.5.5/appeal/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,41 +439,41 @@
         line = "".join(line).rstrip()
         lines.append(line)
 
     text = "\n".join(lines)
     return text.rstrip()
 
 
-def multisplit(s, separators):
-    """
-    Like str.split(), but separators is an iterable
-    of strings to separate on.  (separators can be a
-    string, in which case multisplit separates on each
-    character.)
-
-    multsplit('ab:cd,ef', ':,') => ["ab", "cd", "ef"]
-    """
-    if not s or not separators:
-        return [s]
-    if len(separators) == 1:
-        return s.split(separators[0])
-    splits = []
-    while s:
-        candidates = []
-        for separator in separators:
-            split, found, trailing = s.partition(separator)
-            if found:
-                candidates.append((len(split), split, trailing))
-        if not candidates:
-            break
-        candidates.sort()
-        _, fragment, s = candidates[0]
-        splits.append(fragment)
-    splits.append(s)
-    return splits
+# def multisplit(s, separators):
+#     """
+#     Like str.split(), but separators is an iterable
+#     of strings to separate on.  (separators can be a
+#     string, in which case multisplit separates on each
+#     character.)
+
+#     multsplit('ab:cd,ef', ':,') => ["ab", "cd", "ef"]
+#     """
+#     if not s or not separators:
+#         return [s]
+#     if len(separators) == 1:
+#         return s.split(separators[0])
+#     splits = []
+#     while s:
+#         candidates = []
+#         for separator in separators:
+#             split, found, trailing = s.partition(separator)
+#             if found:
+#                 candidates.append((len(split), split, trailing))
+#         if not candidates:
+#             break
+#         candidates.sort()
+#         _, fragment, s = candidates[0]
+#         splits.append(fragment)
+#     splits.append(s)
+#     return splits
 
 
 def _test_merge_columns(input, expected, **kwargs):
     global test_number
     test_number += 1
     got = merge_columns(*input, **kwargs)
     if verbose:
```

### Comparing `appeal-0.5.3/resources/images/appeal.logo.png` & `appeal-0.5.5/resources/images/appeal.logo.png`

 * *Files identical despite different names*

### Comparing `appeal-0.5.3/resources/images/give.your.program.appeal.png` & `appeal-0.5.5/resources/images/give.your.program.appeal.png`

 * *Files identical despite different names*

### Comparing `appeal-0.5.3/tests/run_tests.py` & `appeal-0.5.5/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.3/PKG-INFO` & `appeal-0.5.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: appeal
-Version: 0.5.3
+Version: 0.5.5
 Summary: A powerful & Pythonic command-line parsing library.  Give your program Appeal!
-Home-page: https://github.com/larryhastings/appeal/
-Author: Larry Hastings
-Author-email: larry@hastings.org
+Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Dist: big >= 0.7.1
+Project-URL: Source, https://github.com/larryhastings/appeal/
 
 ![## Appeal](/resources/images/appeal.logo.png)
 
 ![## Give your program Appeal!](/resources/images/give.your.program.appeal.png)
 
 ##### Copyright 2021-2023 by Larry Hastings
 
@@ -70,30 +70,34 @@
     app.main()
 ```
 
 
 ## Overview
 
 Appeal is a command-line argument processing library for
-Python, like `argparse`, `optparse`, `getopt`, `click`,
-`docopt`, and `Typer`.  But Appeal takes a refreshing new
-approach.
+Python, like `argparse`, `optparse`, `getopt`,
+`docopt`, `Typer`, and `click`.  But Appeal takes a
+refreshing new approach.
 
 Other libraries have complicated, cumbersome interfaces
 that force you to repeat yourself over and over.
 Appeal leverages Python's rich function call interface,
-which makes defining your command-line interface effortless.
+making it effortless to define your command-line interface.
 You write Python functions, and Appeal translates them into
 command-line options and arguments.
 
 Appeal provides amazing power and flexibility--but it's
 also intuitive, because it mirrors Python itself.
 If you understand how to write Python functions,
 you're already halfway to understanding Appeal!
 
+Appeal has only one dependency,
+[my **big** library.](https://github.com/larryhastings/big)
+
+
 ### A New And Appealing Approach
 
 Appeal isn't like other command-line parsing libraries.
 In fact, you really shouldn't think of Appeal as a
 "command-line parsing library" per se. And, although you
 work with Appeal by passing in functions for Appeal to call,
 you shouldn't think of these functions as "callbacks".
@@ -717,36 +721,39 @@
 how many opargs it should consume from the command-line and how
 to convert them.
 
 
 > **An important note about annotations**
 >
 > If you use static type analysis in your project,
-> your static type analyzer may not appreciate you
-> using normal Python functions as annotations.
-> Depending on the behavior of your static type analyzer,
-> you may need to decorate your Appeal command functions
-> and converters with `@typing.no_type_check()`.  If you
-> only ever use types and classes this shouldn't be
-> necessary.
+> your static type analyzer may not enjoy analyzing Python
+> code using Appeal.  Static type analyzers are designed
+> to understand "type hints", a means of specifying static
+> type information introduced in Python 3.5 with the
+> `typing` module.  But Appeal doesn't use type hints,
+> and there are some ways Appeal uses annotations that
+> static type analyzers may not like.
 >
-> Also, Appeal doesn't understand "type hint"
-> annotations.  It expects annotations to be callables,
-> like functions or classes or types.  It should be
-> possible to add limited support in the future.
+> Fortunately, there are ways to get static type analyzers
+> to work alongside Appeal.
+>
+> First, you can decorate your Appeal command functions
+> and converters with `@typing.no_type_check()`.  This should
+> only be necessary if you use functions as annotations;
+> if you only ever use types and classes, this shouldn't be
+> necessary.
 >
-> Finally, Appeal uses function calls and related
-> snazzy technology in annotations--but many static
-> type checkers expect annotations to conform strictly
-> to only what is used for "type hints".  So it's
-> possible static type checkers may abort processing
-> in a file with advanced Appeal configuration.
-> It may be best to mix "type hints" and Appeal
-> in the same Python script, and to not run your
-> static type checker on scripts with Appeal code.
+> Second, if you're using Python 3.9 or newer, you can use
+> `typing.Annotated` with your annotations.  `typing.Annotated`
+> allows you to specify an ordered list of values, and static
+> type hints only ever use the *first* value.  Appeal also
+> handles `typing.Annotated`, but Appeal only ever uses the
+> *last* value.  This makes it easy--you can have both types
+> of annotations, side by side, and both static type checkers
+> and Appeal are perfectly happy.
 
 
 ## Converter Flexibility
 
 You can use almost any function as an annotation...
 within reason.  Appeal will introspect your annotation,
 determine its input parameters, and call it to convert
@@ -890,15 +897,15 @@
 
 
 Of course, you can also subclass `MultiOption` to make your own
 converter classes with custom behavior. `MultiOption` subclasses
 can override these three methods:
 
 ```Python
-class Option:
+class MultiOption:
 
     def init(self, default):
         ...
 
     def option(self, ...):
         ...
 
@@ -951,17 +958,29 @@
 you to decide how to store them, and how to
 render them into a single value returned
 by your `render()` method.
 
 `MultiOption` is a subclass of a general
 `Option` class.  `Option` behaves identically
 to `MultiOption`, except it only permits
-specifying the option once on the command-line.
-(Which means it will only your `option()`
-method once.)
+specifying the option once on the command-line,
+which means it will only your `option()`
+method once.
+You usually don't need to bother with making subclasses
+of `Option`--it's usually better to just use a class
+directly, like our `class IntAndFloat` example.
+The only feature you get by subclassing `Option` is,
+you get the default value for the parameter passed in
+to your constructor.
+
+(The downside of subclassing `Option` and `MultiOption`
+is that it makes exporting your Appeal API as an automation
+API a little less convenient for the user, because your
+users will have to construct these objects and feed
+values into them by calling the `option` method.)
 
 
 ## Data Validation
 
 What if you want to restrict the data the user provides
 on the command-line?  That's simple, just use a converter!
 Appeal provides a couple sample converters for data validation,
@@ -1953,7 +1972,42 @@
 Restrictions on Appeal command functions:
 
 * You may not use `inspect.Parameter.empty` as a default value
   for any keyword-only parameter to a converter or command function.
 * The converter for a *var_positional* (`*args`) parameter
   *must* require at least one positional argument.
 
+
+## Changelog
+
+**0.5.5**
+
+* Add support for `typing.Annotated`, new in Python 3.9.
+* Add dependency to
+  [my **big** library.](https://github.com/larryhastings/big)
+  This gives Appeal a much better implementation of `multisplit`,
+  and I plan to switch to the **big** word wrapper and columnizer
+  functions, which are a... "big" improvement over what's in
+  Appeal right now.
+* Rename `SingleOption` to just `Option`.  (The name
+  `SingleOption` is now deprecated, but I'll leave it
+  as a redundant name for `Option`... for now.)
+
+**0.5.3**
+
+* Fix compatibility back to Python 3.6.
+
+**0.5.2**
+
+* Fix compatibility with Python 3.11.  Python's `inspect.Parameter` object
+  no longer allows a `name` that happens to be a keyword, which was a minor
+  inconvenience (Appeal used to use `lambda` here sometimes).
+
+**0.5.1**
+
+* Fixed regression, issue #5.  If you didn't supply enough required
+  parameters, you'd get a `TypeError` instead of a proper usage error.
+
+**0.5**
+
+* Initial release!
+
```

