# Comparing `tmp/appeal-0.5.5.tar.gz` & `tmp/appeal-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appeal-0.5.5.tar", last modified: Tue May  2 08:19:16 2023, max compression
+gzip compressed data, was "appeal-0.5.6.tar", last modified: Tue May  2 09:10:26 2023, max compression
```

## Comparing `appeal-0.5.5.tar` & `appeal-0.5.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       19 2022-01-26 11:06:53.000000 appeal-0.5.5/.gitignore
--rw-r--r--   0        0        0     1090 2023-04-27 05:54:38.102243 appeal-0.5.5/LICENSE
--rw-r--r--   0        0        0    66711 2023-05-02 08:12:32.474761 appeal-0.5.5/README.md
--rw-r--r--   0        0        0   171316 2023-05-02 08:01:55.426889 appeal-0.5.5/appeal/__init__.py
--rw-r--r--   0        0        0    23346 2023-04-27 05:54:38.106243 appeal-0.5.5/appeal/argument_grouping.py
--rw-r--r--   0        0        0     4637 2022-02-12 23:26:33.980913 appeal-0.5.5/appeal/cpp.py
--rw-r--r--   0        0        0    19692 2023-05-02 08:10:35.559115 appeal-0.5.5/appeal/text.py
--rw-r--r--   0        0        0      537 2023-05-02 08:18:05.889159 appeal-0.5.5/pyproject.toml
--rw-r--r--   0        0        0    50634 2022-01-26 11:06:53.000000 appeal-0.5.5/resources/images/appeal.logo.png
--rw-r--r--   0        0        0    18772 2022-01-26 11:06:53.000000 appeal-0.5.5/resources/images/give.your.program.appeal.png
--rw-r--r--   0        0        0      125 2022-01-26 11:06:53.000000 appeal-0.5.5/resources/links.txt
--rw-r--r--   0        0        0    64835 2023-04-27 05:54:38.106243 appeal-0.5.5/tests/run_tests.py
--rw-r--r--   0        0        0    67205 1970-01-01 00:00:00.000000 appeal-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0       19 2022-01-26 11:06:53.000000 appeal-0.5.6/.gitignore
+-rw-r--r--   0        0        0     1090 2023-04-27 05:54:38.102243 appeal-0.5.6/LICENSE
+-rw-r--r--   0        0        0    66802 2023-05-02 09:09:34.290513 appeal-0.5.6/README.md
+-rw-r--r--   0        0        0   171409 2023-05-02 09:08:54.290186 appeal-0.5.6/appeal/__init__.py
+-rw-r--r--   0        0        0    23346 2023-04-27 05:54:38.106243 appeal-0.5.6/appeal/argument_grouping.py
+-rw-r--r--   0        0        0     4637 2022-02-12 23:26:33.980913 appeal-0.5.6/appeal/cpp.py
+-rw-r--r--   0        0        0    19692 2023-05-02 08:57:46.416604 appeal-0.5.6/appeal/text.py
+-rw-r--r--   0        0        0      537 2023-05-02 08:57:46.416604 appeal-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0    50634 2022-01-26 11:06:53.000000 appeal-0.5.6/resources/images/appeal.logo.png
+-rw-r--r--   0        0        0    18772 2022-01-26 11:06:53.000000 appeal-0.5.6/resources/images/give.your.program.appeal.png
+-rw-r--r--   0        0        0      125 2022-01-26 11:06:53.000000 appeal-0.5.6/resources/links.txt
+-rw-r--r--   0        0        0    64835 2023-04-27 05:54:38.106243 appeal-0.5.6/tests/run_tests.py
+-rw-r--r--   0        0        0    67296 1970-01-01 00:00:00.000000 appeal-0.5.6/PKG-INFO
```

### Comparing `appeal-0.5.5/LICENSE` & `appeal-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `appeal-0.5.5/README.md` & `appeal-0.5.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1962,14 +1962,19 @@
   for any keyword-only parameter to a converter or command function.
 * The converter for a *var_positional* (`*args`) parameter
   *must* require at least one positional argument.
 
 
 ## Changelog
 
+**0.5.6**
+
+* Fix formatting for usage when you have a
+  global command *and* subcommands.
+
 **0.5.5**
 
 * Add support for `typing.Annotated`, new in Python 3.9.
 * Add dependency to
   [my **big** library.](https://github.com/larryhastings/big)
   This gives Appeal a much better implementation of `multisplit`,
   and I plan to switch to the **big** word wrapper and columnizer
```

### Comparing `appeal-0.5.5/appeal/__init__.py` & `appeal-0.5.6/appeal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 "A powerful & Pythonic command-line parsing library.  Give your program Appeal!"
-__version__ = "0.5.5"
+__version__ = "0.5.6"
 
 
 # please leave this copyright notice in binary distributions.
 license = """
 appeal/__init__.py
 part of the Appeal software package
 Copyright 2021-2023 by Larry Hastings
@@ -3765,14 +3765,16 @@
         callable = self._global
         fn_name = callable.__name__
 
         formatter = self.root.format_positional_parameter
         usage_str, arguments_values, options_values = charm_usage(self._global_program, formatter=formatter)
 
         if commands:
+            if usage_str and (not usage_str[-1].isspace()):
+                usage_str += ' '
             usage_str += formatter("command")
 
         # {"{command_name}" : "help string"}
         # summary text parsed from docstring on using that command
         commands_definitions = {}
 
         if commands:
```

### Comparing `appeal-0.5.5/appeal/argument_grouping.py` & `appeal-0.5.6/appeal/argument_grouping.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.5/appeal/cpp.py` & `appeal-0.5.6/appeal/cpp.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.5/appeal/text.py` & `appeal-0.5.6/appeal/text.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.5/pyproject.toml` & `appeal-0.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `appeal-0.5.5/resources/images/appeal.logo.png` & `appeal-0.5.6/resources/images/appeal.logo.png`

 * *Files identical despite different names*

### Comparing `appeal-0.5.5/resources/images/give.your.program.appeal.png` & `appeal-0.5.6/resources/images/give.your.program.appeal.png`

 * *Files identical despite different names*

### Comparing `appeal-0.5.5/tests/run_tests.py` & `appeal-0.5.6/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.5/PKG-INFO` & `appeal-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appeal
-Version: 0.5.5
+Version: 0.5.6
 Summary: A powerful & Pythonic command-line parsing library.  Give your program Appeal!
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -1975,14 +1975,19 @@
   for any keyword-only parameter to a converter or command function.
 * The converter for a *var_positional* (`*args`) parameter
   *must* require at least one positional argument.
 
 
 ## Changelog
 
+**0.5.6**
+
+* Fix formatting for usage when you have a
+  global command *and* subcommands.
+
 **0.5.5**
 
 * Add support for `typing.Annotated`, new in Python 3.9.
 * Add dependency to
   [my **big** library.](https://github.com/larryhastings/big)
   This gives Appeal a much better implementation of `multisplit`,
   and I plan to switch to the **big** word wrapper and columnizer
```

