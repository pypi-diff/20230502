# Comparing `tmp/pybash-0.2.3.tar.gz` & `tmp/pybash-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybash-0.2.3.tar", max compression
+gzip compressed data, was "pybash-0.2.4.tar", max compression
```

## Comparing `pybash-0.2.3.tar` & `pybash-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1060 2023-01-27 05:02:40.066110 pybash-0.2.3/LICENSE
--rw-r--r--   0        0        0     3486 2023-01-27 05:02:40.066110 pybash-0.2.3/README.md
--rw-r--r--   0        0        0    15869 2023-01-27 05:02:40.066110 pybash-0.2.3/pybash.py
--rw-r--r--   0        0        0      676 2023-01-27 05:02:40.066110 pybash-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4220 1970-01-01 00:00:00.000000 pybash-0.2.3/setup.py
--rw-r--r--   0        0        0     3907 1970-01-01 00:00:00.000000 pybash-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-05-02 05:39:28.860136 pybash-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3794 2023-05-02 05:39:28.860136 pybash-0.2.4/README.md
+-rw-r--r--   0        0        0    15993 2023-05-02 05:39:28.860136 pybash-0.2.4/pybash.py
+-rw-r--r--   0        0        0      676 2023-05-02 05:39:28.860136 pybash-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4215 1970-01-01 00:00:00.000000 pybash-0.2.4/PKG-INFO
```

### Comparing `pybash-0.2.3/LICENSE` & `pybash-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pybash-0.2.3/README.md` & `pybash-0.2.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # PyBash
 
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/jaykv/pybash/python-app.yml?branch=main)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pybash)
+![PyPI](https://img.shields.io/pypi/v/pybash)
+![GitHub](https://img.shields.io/github/license/jaykv/pybash)
+
 Streamline bash-command execution from python with a new syntax. It combines the simplicity of writing bash scripts with the flexibility of python. Under the hood, any line or variable assignment starting with `>` or surrounded by parentheses is transformed to python `subprocess` calls and then injected into `sys.meta_path` as an import hook. All possible thanks to the wonderful [ideas](https://github.com/aroberge/ideas) project!
 
-For security and performance reasons, PyBash will NOT execute as shell, unless explicitly specified with a `$` instead of a single `>` before the command. While running commands as shell can be convenient, it can also spawn security risks and  if you're not too careful. If you're curious about the transformations, look at the [unit tests](test_pybash.py) for some quick examples.
+For security and performance reasons, PyBash will NOT execute as shell, unless explicitly specified with a `$` instead of a single `>` before the command. While running commands as shell can be convenient, it can also spawn security risks if you're not too careful. If you're curious about the transformations, look at the [unit tests](test_pybash.py) for some quick examples.
 
 Note: this is a mainly experimental library. Consider the risks and test before using in prod.
 
 # Installation
 `pip install pybash`
 
 # Setup hook
@@ -82,16 +87,16 @@
 >sort < test.txt | sed 's/SORT/TEST\\n/g'
 ```
 ### 9. Glob patterns with shell
 ```python
 $ls .github/*
 ```
 
-### 10. Static interpolation
-Denoted by {{variable_or_function_call_here}}. For static interpolation, no quotes, spaces or expressions within the {{}} or in the string being injected.
+### 10. Direct interpolation
+Denoted by {{code here}}. Interpolated as direct code replace. The value/output of the variable, function call, or the expression must not include spaces.
 
 ```python
 ## GOOD
 command = "status"
 def get_option(command):
     return "-s" if command == "status" else "-v"
 >git {{command}} {{get_option(command)}}
@@ -107,31 +112,31 @@
 >git status {{" ".join(options)}}
 
 # use dynamic interpolation
 options = {'version': '-v'}
 >git status {{options['version']}}
 ```
 
-### 11. Dynamic interpolation
-Denoted by {{{ any python variable, function call, or expression here }}}. The output of the variable, function call, or the expression must still not include spaces.
+### 11. f-string interpolation
+Denoted by f{ any python variable, function call, or expression here }. Interpolated as f-string. The output of the variable, function call, or the expression must still not include spaces.
 
 ```python
 ## GOOD
 
 # git -h
 options = {'version': '-v', 'help': '-h'}
->git {{{options['h']}}}
+>git f{options['h']}
 
 # kubectl get pods --show-labels -n coffee
 namespace = "coffee"
->kubectl get pods {{{"--" + "-".join(['show', 'labels'])}}} -n {{{namespace}}}
+>kubectl get pods f{"--" + "-".join(['show', 'labels'])} -n f{namespace}
 
 ## BAD
 option = "-s -v"
->git status {{{ option }}}
+>git status f{option}
 ```
 
 #### Also works inside methods!
 ```python
 # PYBASH DEMO #
 def cp_test():
     >cp test.txt test_copy.txt
```

### Comparing `pybash-0.2.3/pybash.py` & `pybash-0.2.4/pybash.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,77 +1,79 @@
 import re
 import shlex
+from typing import Callable, Union
 
 import token_utils
 from ideas import import_hook
 
 
 def source_init():
     """Adds subprocess import"""
-    import_subprocess = "import subprocess"
-    return import_subprocess
+    return "import subprocess"
 
 
 def add_hook(**_kwargs):
     """Creates and automatically adds the import hook in sys.meta_path"""
-    hook = import_hook.create_hook(
-        hook_name=__name__, transform_source=Transformer.transform_source, source_init=source_init
+    return import_hook.create_hook(
+        hook_name=__name__,
+        transform_source=Transformer.transform_source,
+        source_init=source_init,
     )
-    return hook
 
 
 class InvalidInterpolation(Exception):
     pass
 
 
 class Processor:
     command_char = ">"
 
-    def __init__(self, token: str) -> None:
+    def __init__(self, token: token_utils.Token) -> None:
         self.token = token
         self.token_line = token.line
         self.parse()
 
-    def parse(self):
+    def parse(self) -> None:
         self.parsed_line = shlex.split(self.token_line)
         self.command = Commander.get_bash_command(self.parsed_line, command_char=self.command_char)
 
     def transform(self) -> token_utils.Token:
         raise NotImplementedError
 
-    def interpolate(self) -> str:
-        self.token.string = Processor.dynamic_interpolate(self.token_line, self.token.string)
-        self.token.string = Processor.static_interpolate(self.token.string)
+    def interpolate(self) -> None:
+        self.token.string = Processor.fstring_interpolate(self.token_line, self.token.string)
+        self.token.string = Processor.direct_interpolate(self.token.string)
 
     @staticmethod
-    def dynamic_interpolate(token_string: str, parsed_command: str) -> str:
-        """Process {{{ dynamic interpolations }}} and substitute.
-            Dynamic interpolations are denotated by a {{{ }}} with any expression inside.
+    def fstring_interpolate(token_string: str, parsed_command: str) -> str:
+        """Process f{ dynamic interpolations } and substitute.
+            Dynamic interpolations are denotated by a f{ } with any expression inside.
             Substitution in the parsed command string happens relative to the order of the interpolations in the original command string.
 
         Args:
             token_string (str): Original command string
             parsed_command (str): Parsed command string
 
         Returns:
             str: Interpolated parsed command string
         """
-        pattern = r'{{{(.+?)}}}'
+        pattern = r'f{(.+?)}'
         subs = re.findall(pattern, token_string)
 
         if not subs:
             return parsed_command
 
+        command_pattern = f'\"{pattern}\"'
         for sub in subs:
-            parsed_command = re.sub(pattern, '" + ' + sub + ' + "', parsed_command, 1)
+            parsed_command = re.sub(command_pattern, 'f\"\"\"{' + sub + '}\"\"\"', parsed_command, 1)
 
         return parsed_command
 
     @staticmethod
-    def static_interpolate(string: str) -> str:
+    def direct_interpolate(string: str) -> str:
         """Process {{ static interpolations }} and substitute.
             Static interpolations are denotated by a {{ }} with a variable or a function call inside.
             Substitution happens directly on the parsed command string. Therefore, certain characters cannot be interpolated as they get parsed out before substitution.
 
         Args:
             string (str): String to interpolate
 
@@ -108,39 +110,39 @@
             # no pipers
             self.token.string = Commander.build_subprocess_list_cmd("run", self.command) + '\n'
         return self.token
 
 
 class Variablized(Processor):
     # a = >cat test.txt
-    def parse(self):
+    def parse(self) -> None:
         self.parsed_line = shlex.split(self.token.line)
         self.start_index = Commander.get_start_index(self.parsed_line)
         self.command = Commander.get_bash_command(self.parsed_line, start_index=self.start_index)
 
-    def transform(self):
+    def transform(self) -> None:
         pipeline_command = Pipeline(self.command).parse_command(variablized=True)
         if pipeline_command != self.command:
             self.token.string = pipeline_command
             self.token.string += ';' if pipeline_command[-1] != ';' else ''
             self.token.string += ' '.join(self.parsed_line[: self.start_index]) + ' cmd1\n'
         else:
             self.token.string = ' '.join(self.parsed_line[: self.start_index])
             self.token.string += Commander.build_subprocess_list_cmd("check_output", self.command) + '\n'
 
 
 class Wrapped(Processor):
     # print(>cat test.txt)
-    def parse(self):
+    def parse(self) -> None:
         self.parsed_line = shlex.split(self.token.line)
         self.raw_line = [tok for tok in self.token.line.split(' ') if tok]
         self.start_index = Commander.get_start_index(self.parsed_line)
         self.command = Commander.get_bash_command(self.parsed_line, start_index=self.start_index, wrapped=True)
 
-    def transform(self):
+    def transform(self) -> token_utils.Token:
         # shlex strips out single quotes and double quotes-- use raw_line for the code around the wrapped command
         self.token.string = (
             ' '.join(self.raw_line[: self.start_index])
             + self.raw_line[self.start_index][: self.raw_line[self.start_index].index('>')]
         )
         self.token.string += (
             Commander.build_subprocess_list_cmd("check_output", self.command)
@@ -161,28 +163,24 @@
         new_tokens = []
         for line in token_utils.get_lines(source):
             token = token_utils.get_first(line)
             if not token:
                 new_tokens.extend(line)
                 continue
 
-            # matches exact token
-            token_match = [tokenizer for match, tokenizer in Transformer.tokenizers.items() if token == match]
-            if token_match:
+            if token_match := [tokenizer for match, tokenizer in Transformer.tokenizers.items() if token == match]:
                 parser = token_match[0](token)
                 parser.transform()
                 parser.interpolate()
                 new_tokens.append(parser.token)
                 continue
 
-            # matches anywhere in line
-            greedy_match = [
+            if greedy_match := [
                 tokenizer for match, tokenizer in Transformer.greedy_tokenizers.items() if match in token.line
-            ]
-            if greedy_match:
+            ]:
                 parser = greedy_match[0](token)
                 parser.transform()
                 parser.interpolate()
                 new_tokens.append(parser.token)
                 continue
 
             # no match
@@ -193,15 +191,15 @@
 
 class Pipers:
     """Handles the logic of chaining operators"""
 
     OPS = ['|', '>', '>>', '<', '&&']
 
     @classmethod
-    def get_piper(cls, op: str):
+    def get_piper(cls, op: str) -> Callable:
         if op == '|':
             # Pipe output to next command
             return cls.chain_pipe_command
         elif op == '>':
             # Write to out file
             return cls.chain_sredirect_command
         elif op == '>>':
@@ -209,37 +207,39 @@
             return cls.chain_dredirect_command
         elif op == '<':
             # Redirect file as input to command
             return cls.chain_iredirect_command
         elif op == '&&':
             # Run next command only if previous succeeds
             return cls.chain_and_command
-        return None
+
+        raise NotImplementedError
 
     @classmethod
     def chain_iredirect_command(
         cls, command: list, pipeline: list, start_index: int = 0, fmode: str = "r", fvar: str = "fout", **kwargs
-    ):
+    ) -> str:
         first_idx, _ = pipeline.pop(0)
         pre_command = command[start_index:first_idx]
         filename = command[first_idx + 1 : first_idx + 2][0]
 
         fout = f'open("{filename}", "{fmode}")'
 
-        if len(pipeline) == 0:
+        if not pipeline:
             # out to file
             cmd1 = Commander.build_subprocess_list_cmd("run", pre_command, stdin=fvar, **kwargs)
             return f"{fvar} = {fout}; cmd1 = {cmd1}"
 
         cmd1 = Commander.build_subprocess_list_cmd("Popen", pre_command, stdin=fvar, stdout="subprocess.PIPE", **kwargs)
 
         out = f"{fvar} = {fout}; cmd1 = {cmd1};"
-        while len(pipeline) > 0:
+        while pipeline:
             idx, piper = pipeline[0]
             fvar = f"fout{idx}"
+            cmd = ""
             if piper == '>':
                 # >sort < test.txt > test2.txt
                 cmd = cls.write_to_file(
                     command, pipeline, reader='cmd1.stdout.read()', start_index=first_idx + 1, fmode="wb"
                 )
             elif piper == '>>':
                 # >sort < test.txt >> test2.txt
@@ -255,45 +255,44 @@
             first_idx = idx
 
         return out
 
     @classmethod
     def write_to_file(
         cls, command: list, pipeline: list, reader: str, start_index: int = 0, fvar: str = 'fout', fmode: str = 'wb'
-    ):
+    ) -> str:
         first_idx, _ = pipeline.pop(0)
         filename = command[first_idx + 1 : first_idx + 2][0]
-        cmd = f'{fvar} = open("{filename}", "{fmode}"); {fvar}.write({reader});'
-        return cmd
+        return f'{fvar} = open("{filename}", "{fmode}"); {fvar}.write({reader});'
 
     @classmethod
     def chain_and_command(cls, command: list, pipeline: list, **kwargs):
         raise NotImplementedError
 
     @classmethod
-    def chain_pipe_command(cls, command: list, pipeline: list, start_index: int = 0, chained: bool = False, **kwargs):
+    def chain_pipe_command(
+        cls, command: list, pipeline: list, start_index: int = 0, chained: bool = False, **kwargs
+    ) -> str:
         first_idx, _ = pipeline.pop(0)
         pre_command = command[start_index:first_idx]
-
-        if not chained:
-            cmd1 = Commander.build_subprocess_list_cmd('Popen', pre_command, stdout='subprocess.PIPE', **kwargs)
-
-        if len(pipeline) == 0:
+        cmd1 = (
+            ""
+            if chained
+            else Commander.build_subprocess_list_cmd('Popen', pre_command, stdout='subprocess.PIPE', **kwargs)
+        )
+        cmd2 = ""
+        if not pipeline:
             ## No other pipes
             post_command = command[first_idx + 1 :]
 
             cmd2 = Commander.build_subprocess_list_cmd('run', post_command, stdin='cmd1.stdout')
 
-            if not chained:
-                return f"cmd1 = {cmd1}; cmd2 = {cmd2}"
-            else:
-                return f"cmd2 = {cmd2}"
-
-        out = f"cmd1 = {cmd1};" if not chained else ""
-        while len(pipeline) > 0:
+            return f"cmd2 = {cmd2}" if chained else f"cmd1 = {cmd1}; cmd2 = {cmd2}"
+        out = "" if chained else f"cmd1 = {cmd1};"
+        while pipeline:
             idx, piper = pipeline[0]
             cmd = cls.get_piper(piper)(command, pipeline, start_index=first_idx + 1, stdin="cmd1.stdout")
             out += cmd
             first_idx = idx
 
         return out
 
@@ -303,66 +302,66 @@
         command: list,
         pipeline: list,
         start_index: int = 0,
         fvar: str = "fout",
         fmode: str = "wb",
         chained: bool = False,
         **kwargs,
-    ):
+    ) -> str:
         first_idx, _ = pipeline.pop(0)
         pre_command = command[start_index:first_idx]
         filename = command[first_idx + 1 : first_idx + 2][0]
 
         if chained:
             # file-to-file redirection so cat from source file
             pre_command.insert(0, 'cat')
 
         # out to file
         fout = f'open("{filename}", "{fmode}")'
         cmd1 = Commander.build_subprocess_list_cmd("run", pre_command, stdout=fvar, **kwargs)
 
-        if len(pipeline) == 0:
+        if not pipeline:
             return f"{fvar} = {fout}; cmd1 = {cmd1}"
 
         out = f"{fvar} = {fout}; cmd1 = {cmd1};"
-        while len(pipeline) > 0:
+        while pipeline:
             idx, piper = pipeline[0]
             fvar = f"fout{idx}"
             if piper in ['>', '>>']:
                 cmd = cls.get_piper(piper)(command, pipeline, start_index=first_idx + 1, fvar=fvar, chained=True)
             else:
                 cmd = cls.get_piper(piper)(command, pipeline, start_index=first_idx + 1, stdin=fvar)
             out += cmd
             first_idx = idx
 
         return out
 
     @classmethod
     def chain_sredirect_command(
         cls, command: list, pipeline: list, start_index: int = 0, fvar: str = "fout", chained: bool = False, **kwargs
-    ):
+    ) -> str:
         return cls.chain_redirect(command, pipeline, start_index, fmode="wb", fvar=fvar, chained=chained, **kwargs)
 
     @classmethod
     def chain_dredirect_command(
         cls, command: list, pipeline: list, start_index: int = 0, fvar: str = "fout", chained: bool = False, **kwargs
-    ):
+    ) -> str:
         return cls.chain_redirect(command, pipeline, start_index, fmode="ab", fvar=fvar, chained=chained, **kwargs)
 
 
 class Pipeline:
     """Parses and transformers command chainings by generating pipers"""
 
     __slots__ = ['command', 'pipeline']
 
-    def __init__(self, command: list):
+    def __init__(self, command: list[str]):
         self.command = command
         self.pipeline = [(i, arg) for i, arg in enumerate(self.command) if arg in Pipers.OPS]
 
-    def parse_command(self, variablized: bool = False, **kwargs):
+    def parse_command(self, variablized: bool = False, **kwargs) -> Union[list[str], str]:
         if not self.pipeline:
             return self.command
 
         _, first_piper = self.pipeline[0]
         return Pipers.get_piper(first_piper)(self.command, self.pipeline, **kwargs)
 
 
@@ -379,17 +378,22 @@
         Returns:
             int: starting index
         """
         for i, val in enumerate(parsed_line):
             if '>' in val:
                 return i
 
+        return 0
+
     @staticmethod
     def get_bash_command(
-        parsed_line: list, start_index: int = None, wrapped: bool = None, command_char: str = ">"
+        parsed_line: list,
+        start_index: Union[int, None] = None,
+        wrapped: Union[bool, None] = None,
+        command_char: str = ">",
     ) -> list:
         """Parses line to bash command
 
         Args:
             parsed_line (list): line to parse
             start_index (int, optional): index to start parsing command from. Defaults to None.
             wrapped (bool, optional): input is surrounded by parentheses
```

### Comparing `pybash-0.2.3/pyproject.toml` & `pybash-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyBash"
-version = "0.2.3"
+version = "0.2.4"
 description = ">execute bash commands from python easily"
 authors = ["Jay"]
 readme = "README.md"
 packages = [{include = "pybash.py"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pybash-0.2.3/PKG-INFO` & `pybash-0.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: pybash
-Version: 0.2.3
+Version: 0.2.4
 Summary: >execute bash commands from python easily
 Author: Jay
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ideas (>=0.1.5,<0.2.0)
 Description-Content-Type: text/markdown
 
 # PyBash
 
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/jaykv/pybash/python-app.yml?branch=main)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pybash)
+![PyPI](https://img.shields.io/pypi/v/pybash)
+![GitHub](https://img.shields.io/github/license/jaykv/pybash)
+
 Streamline bash-command execution from python with a new syntax. It combines the simplicity of writing bash scripts with the flexibility of python. Under the hood, any line or variable assignment starting with `>` or surrounded by parentheses is transformed to python `subprocess` calls and then injected into `sys.meta_path` as an import hook. All possible thanks to the wonderful [ideas](https://github.com/aroberge/ideas) project!
 
-For security and performance reasons, PyBash will NOT execute as shell, unless explicitly specified with a `$` instead of a single `>` before the command. While running commands as shell can be convenient, it can also spawn security risks and  if you're not too careful. If you're curious about the transformations, look at the [unit tests](test_pybash.py) for some quick examples.
+For security and performance reasons, PyBash will NOT execute as shell, unless explicitly specified with a `$` instead of a single `>` before the command. While running commands as shell can be convenient, it can also spawn security risks if you're not too careful. If you're curious about the transformations, look at the [unit tests](test_pybash.py) for some quick examples.
 
 Note: this is a mainly experimental library. Consider the risks and test before using in prod.
 
 # Installation
 `pip install pybash`
 
 # Setup hook
@@ -95,16 +100,16 @@
 >sort < test.txt | sed 's/SORT/TEST\\n/g'
 ```
 ### 9. Glob patterns with shell
 ```python
 $ls .github/*
 ```
 
-### 10. Static interpolation
-Denoted by {{variable_or_function_call_here}}. For static interpolation, no quotes, spaces or expressions within the {{}} or in the string being injected.
+### 10. Direct interpolation
+Denoted by {{code here}}. Interpolated as direct code replace. The value/output of the variable, function call, or the expression must not include spaces.
 
 ```python
 ## GOOD
 command = "status"
 def get_option(command):
     return "-s" if command == "status" else "-v"
 >git {{command}} {{get_option(command)}}
@@ -120,31 +125,31 @@
 >git status {{" ".join(options)}}
 
 # use dynamic interpolation
 options = {'version': '-v'}
 >git status {{options['version']}}
 ```
 
-### 11. Dynamic interpolation
-Denoted by {{{ any python variable, function call, or expression here }}}. The output of the variable, function call, or the expression must still not include spaces.
+### 11. f-string interpolation
+Denoted by f{ any python variable, function call, or expression here }. Interpolated as f-string. The output of the variable, function call, or the expression must still not include spaces.
 
 ```python
 ## GOOD
 
 # git -h
 options = {'version': '-v', 'help': '-h'}
->git {{{options['h']}}}
+>git f{options['h']}
 
 # kubectl get pods --show-labels -n coffee
 namespace = "coffee"
->kubectl get pods {{{"--" + "-".join(['show', 'labels'])}}} -n {{{namespace}}}
+>kubectl get pods f{"--" + "-".join(['show', 'labels'])} -n f{namespace}
 
 ## BAD
 option = "-s -v"
->git status {{{ option }}}
+>git status f{option}
 ```
 
 #### Also works inside methods!
 ```python
 # PYBASH DEMO #
 def cp_test():
     >cp test.txt test_copy.txt
```

