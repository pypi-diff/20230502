# Comparing `tmp/cleez-0.1.8.tar.gz` & `tmp/cleez-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleez-0.1.8.tar", max compression
+gzip compressed data, was "cleez-0.1.9.tar", max compression
```

## Comparing `cleez-0.1.8.tar` & `cleez-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      583 2023-04-17 08:35:32.159563 cleez-0.1.8/LICENSE
--rw-r--r--   0        0        0      896 2023-04-17 09:52:54.513608 cleez-0.1.8/README.rst
--rw-r--r--   0        0        0     3368 2023-04-25 11:52:09.699984 cleez-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      340 2023-04-17 16:19:10.886202 cleez-0.1.8/src/cleez/__init__.py
--rw-r--r--   0        0        0      553 2023-04-23 08:31:27.115897 cleez-0.1.8/src/cleez/actions.py
--rw-r--r--   0        0        0      522 2023-04-25 05:23:03.518828 cleez-0.1.8/src/cleez/argument.py
--rw-r--r--   0        0        0     5762 2023-04-25 11:51:13.414394 cleez-0.1.8/src/cleez/cleez.py
--rw-r--r--   0        0        0      371 2023-04-16 21:08:33.001276 cleez-0.1.8/src/cleez/colors.py
--rw-r--r--   0        0        0     1765 2023-04-25 08:52:21.338963 cleez-0.1.8/src/cleez/command.py
--rw-r--r--   0        0        0      268 2023-04-17 18:11:58.414950 cleez-0.1.8/src/cleez/exceptions.py
--rw-r--r--   0        0        0     2707 2023-04-24 08:22:54.099009 cleez-0.1.8/src/cleez/help.py
--rw-r--r--   0        0        0    11613 2023-04-25 08:19:46.737002 cleez-0.1.8/src/cleez/testing.py
--rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 cleez-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-04-17 08:35:32.159563 cleez-0.1.9/LICENSE
+-rw-r--r--   0        0        0      896 2023-04-17 09:52:54.513608 cleez-0.1.9/README.rst
+-rw-r--r--   0        0        0     3368 2023-04-25 13:29:37.236574 cleez-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      340 2023-04-17 16:19:10.886202 cleez-0.1.9/src/cleez/__init__.py
+-rw-r--r--   0        0        0      553 2023-04-23 08:31:27.115897 cleez-0.1.9/src/cleez/actions.py
+-rw-r--r--   0        0        0      522 2023-04-25 05:23:03.518828 cleez-0.1.9/src/cleez/argument.py
+-rw-r--r--   0        0        0     5571 2023-04-25 13:29:00.070644 cleez-0.1.9/src/cleez/cleez.py
+-rw-r--r--   0        0        0      371 2023-04-16 21:08:33.001276 cleez-0.1.9/src/cleez/colors.py
+-rw-r--r--   0        0        0     1871 2023-04-25 13:29:07.960908 cleez-0.1.9/src/cleez/command.py
+-rw-r--r--   0        0        0      268 2023-04-17 18:11:58.414950 cleez-0.1.9/src/cleez/exceptions.py
+-rw-r--r--   0        0        0     2707 2023-04-24 08:22:54.099009 cleez-0.1.9/src/cleez/help.py
+-rw-r--r--   0        0        0      292 2023-04-25 13:28:42.877289 cleez-0.1.9/src/cleez/parser.py
+-rw-r--r--   0        0        0    11613 2023-04-25 08:19:46.737002 cleez-0.1.9/src/cleez/testing.py
+-rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 cleez-0.1.9/PKG-INFO
```

### Comparing `cleez-0.1.8/LICENSE` & `cleez-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cleez-0.1.8/README.rst` & `cleez-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `cleez-0.1.8/pyproject.toml` & `cleez-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "cleez"
-version = "0.1.8"
+version = "0.1.9"
 homepage = "https://github.com/abilian/cleez"
 description = "Simple class-based CLI framework."
 authors = ["Abilian SAS <sf@abilian.com>"]
 readme = "README.rst"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
```

### Comparing `cleez-0.1.8/src/cleez/actions.py` & `cleez-0.1.9/src/cleez/actions.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.8/src/cleez/argument.py` & `cleez-0.1.9/src/cleez/argument.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.8/src/cleez/cleez.py` & `cleez-0.1.9/src/cleez/cleez.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from .colors import red
 from .command import Command, Option
 from .exceptions import ParserBuildError
 from .help import HelpMaker
 
 __all__ = ["CLI"]
 
+from .parser import PatchedArgumentParser
+
 DEBUG = os.environ.get("DEBUG_CLEEZ", False)
 
 
 @dataclass(frozen=True)
 class CLI:
     name: str = "cleez"
     version: str = "0.1.0"
@@ -38,15 +40,15 @@
     #
     # Public API
     #
     def run(self, argv=None):
         if not argv:
             argv = sys.argv
 
-        parser = self.make_parser()
+        parser = self.make_parser
 
         try:
             args = parser.parse_args(argv[1:])
         except argparse.ArgumentError as e:
             print(red(f"Argument parsing error: {e}\n"))
             print("Usage:\n")
             self.help_maker.print_help(self)
@@ -102,17 +104,18 @@
     #
     def get_command(self, name: str) -> Command:
         for command in self.commands:
             if command.name == name:
                 return command
         raise KeyError(f"Command {name} not found")
 
+    @property
     def make_parser(self):
-        parser = MyArgParser()
-        subparsers = parser.add_subparsers(parser_class=MyArgParser)
+        parser = PatchedArgumentParser()
+        subparsers = parser.add_subparsers(parser_class=PatchedArgumentParser)
 
         for option in self.options:
             option.add_to_parser(parser)
 
         def sorter(cmd):
             return cmd.main_command_name(), len(cmd)
 
@@ -173,17 +176,7 @@
         self.help_maker.print_help(self)
 
     def get_version(self):
         return self.version
 
     def get_command_name(self):
         return self.name
-
-
-class MyArgParser(argparse.ArgumentParser):
-    """Subclass of argparse.ArgumentParser that doesn't exit on error.
-
-    See: https://github.com/python/cpython/issues/103498
-    """
-
-    def error(self, message):
-        raise argparse.ArgumentError(None, message)
```

### Comparing `cleez-0.1.8/src/cleez/command.py` & `cleez-0.1.9/src/cleez/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import typing
 from abc import ABC, abstractmethod
 
 from .argument import Argument, Option
+from .parser import PatchedArgumentParser
 
 if typing.TYPE_CHECKING:
     from cleez import CLI
 
 
 __all__ = ["Command", "Argument", "Option"]
 
@@ -44,15 +45,17 @@
         for argument in self.arguments:
             argument.add_to_parser(subparser)
 
         for option in self.options:
             option.add_to_parser(subparser)
 
         if self.has_subcommands():
-            self.subparsers = subparser.add_subparsers()
+            self.subparsers = subparser.add_subparsers(
+                parser_class=PatchedArgumentParser
+            )
 
     def add_subcommand(self, command: Command):
         self._subcommands.append(command)
 
     def has_subcommands(self) -> bool:
         return bool(self._subcommands)
```

### Comparing `cleez-0.1.8/src/cleez/help.py` & `cleez-0.1.9/src/cleez/help.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.8/src/cleez/testing.py` & `cleez-0.1.9/src/cleez/testing.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.8/PKG-INFO` & `cleez-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleez
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple class-based CLI framework.
 Home-page: https://github.com/abilian/cleez
 Author: Abilian SAS
 Author-email: sf@abilian.com
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

