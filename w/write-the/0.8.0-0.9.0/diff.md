# Comparing `tmp/write_the-0.8.0.tar.gz` & `tmp/write_the-0.9.0.tar.gz`

## Comparing `write_the-0.8.0.tar` & `write_the-0.9.0.tar`

### file list

```diff
@@ -1,66 +1,70 @@
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.8.0/mkdocs.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 write_the-0.8.0/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 write_the-0.8.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 write_the-0.8.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.8.0/docs/CNAME
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 write_the-0.8.0/docs/index.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.8.0/docs/reference/cli.md
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 write_the-0.8.0/docs/reference/commands.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.8.0/docs/reference/cst.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 write_the-0.8.0/docs/reference/llm.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.8.0/docs/reference/utils.md
--rw-r--r--   0        0        0   118788 2020-02-02 00:00:00.000000 write_the-0.8.0/images/docs-help.png
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 write_the-0.8.0/images/logo-black.svg
--rw-r--r--   0        0        0   821015 2020-02-02 00:00:00.000000 write_the-0.8.0/images/logo.png
--rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.8.0/images/mkdocs-help.png
--rw-r--r--   0        0        0  1092197 2020-02-02 00:00:00.000000 write_the-0.8.0/images/multiply-docs-tests.png
--rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.8.0/images/tests-help.png
--rw-r--r--   0        0        0  3588464 2020-02-02 00:00:00.000000 write_the-0.8.0/images/untitled.blend
--rw-r--r--   0        0        0  3580784 2020-02-02 00:00:00.000000 write_the-0.8.0/images/untitled.blend1
--rw-r--r--   0        0        0   464261 2020-02-02 00:00:00.000000 write_the-0.8.0/images/write-the-docs.gif
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.8.0/images/write-the-icon.svg
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 write_the-0.8.0/images/write-the.svg
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_cli_main.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_cst_docstring_adder.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_cst_docstring_remover.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_cst_function_and_class_collector.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_cst_node_extractor.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_cst_node_remover.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_cst_utils.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/test_utils.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/data/calculate.py
--rw-r--r--   0        0        0    98897 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/data/expected.dat
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/data/multiply.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 write_the-0.8.0/tests/data/multiply_docstring.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/__about__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/__main__.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/llm.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cli/__init__.py
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cli/main.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cli/tasks.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/docs/__init__.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/docs/docs.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/docs/prompts.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/docs/utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/mkdocs/__init__.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/mkdocs/mkdocs.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/mkdocs/templates.py
--rwxr-xr-x   0        0        0       35 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/tests/__init__.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/tests/prompts.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/commands/tests/tests.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/__init__.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/docstring_adder.py
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/docstring_remover.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/function_and_class_collector.py
--rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/node_batcher.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/node_extractor.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/node_remover.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 write_the-0.8.0/write_the/cst/utils.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 write_the-0.8.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 write_the-0.8.0/README.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 write_the-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 write_the-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.9.0/mkdocs.yml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 write_the-0.9.0/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 write_the-0.9.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 write_the-0.9.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.9.0/docs/CNAME
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 write_the-0.9.0/docs/index.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.9.0/docs/reference/cli.md
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 write_the-0.9.0/docs/reference/commands.md
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 write_the-0.9.0/docs/reference/cst.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 write_the-0.9.0/docs/reference/llm.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.9.0/docs/reference/utils.md
+-rw-r--r--   0        0        0   121662 2020-02-02 00:00:00.000000 write_the-0.9.0/images/convert-help.png
+-rw-r--r--   0        0        0   118788 2020-02-02 00:00:00.000000 write_the-0.9.0/images/docs-help.png
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 write_the-0.9.0/images/logo-black.svg
+-rw-r--r--   0        0        0   821015 2020-02-02 00:00:00.000000 write_the-0.9.0/images/logo.png
+-rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.9.0/images/mkdocs-help.png
+-rw-r--r--   0        0        0  1092197 2020-02-02 00:00:00.000000 write_the-0.9.0/images/multiply-docs-tests.png
+-rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.9.0/images/tests-help.png
+-rw-r--r--   0        0        0  3588464 2020-02-02 00:00:00.000000 write_the-0.9.0/images/untitled.blend
+-rw-r--r--   0        0        0  3580784 2020-02-02 00:00:00.000000 write_the-0.9.0/images/untitled.blend1
+-rw-r--r--   0        0        0   464261 2020-02-02 00:00:00.000000 write_the-0.9.0/images/write-the-docs.gif
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.9.0/images/write-the-icon.svg
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 write_the-0.9.0/images/write-the.svg
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_cli_main.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_cst_docstring_adder.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_cst_docstring_remover.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_cst_function_and_class_collector.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_cst_node_extractor.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_cst_node_remover.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_cst_utils.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/test_utils.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/data/calculate.py
+-rw-r--r--   0        0        0    98897 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/data/expected.dat
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/data/multiply.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 write_the-0.9.0/tests/data/multiply_docstring.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/__about__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/__main__.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/llm.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cli/__init__.py
+-rw-r--r--   0        0        0    10009 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cli/main.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cli/tasks.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/converters/__init__.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/converters/converters.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/converters/prompts.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/docs/__init__.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/docs/docs.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/docs/prompts.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/docs/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/mkdocs/__init__.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/mkdocs/mkdocs.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/mkdocs/templates.py
+-rwxr-xr-x   0        0        0       35 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/tests/__init__.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/tests/prompts.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/commands/tests/tests.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/__init__.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/docstring_adder.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/docstring_remover.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/function_and_class_collector.py
+-rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/node_batcher.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/node_extractor.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/node_remover.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 write_the-0.9.0/write_the/cst/utils.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 write_the-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 write_the-0.9.0/README.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 write_the-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 write_the-0.9.0/PKG-INFO
```

### Comparing `write_the-0.8.0/mkdocs.yml` & `write_the-0.9.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/.github/workflows/publish.yml` & `write_the-0.9.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/.github/workflows/tests.yml` & `write_the-0.9.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/docs/index.md` & `write_the-0.9.0/docs/index.md`

 * *Files 16% similar despite different names*

```diff
@@ -19,34 +19,36 @@
 ## Real-world examples
 
 - [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/master/write_the/docs/write.py#L14)
 - [`write-the mkdocs` to build the documentation site for `write-the` 🤖](https://write-the.wytamma.com/)
 - [`write-the tests` to write tests for `write-the docs` 🤖](https://github.com/Wytamma/write-the/commit/6b6c8a08d7991e07e4972281c471f7842c04dda0)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `autoresearcher` 🤖](https://github.com/eimenhmdt/autoresearcher/pull/17)
 - [`write-the docs` and `write-the mkdocs` to build documenation for `hyperspec` 🤖](https://github.com/smutch/hyperspec/pull/1)
-
+- [`write-the docs` and `write-the mkdocs` to build documenation for `CUPCAKEAGI` 🤖](https://github.com/AkshitIreddy/CUPCAKEAGI/pull/4)
 
 ## Installation
 ```console
 pip install write-the
 ```
 ## Features
 
 Write-the offers the following AI-driven features:
 
 - Write-the Docs: Automatically generate documentation for your codebase, including class and function descriptions, parameter explanations, and examples.
 - Write-the Tests: Create test cases for your code, ensuring thorough test coverage and better code quality.
+- Write-the Convert: Convert code and data from any format into another. 
 - Write-the Refactor: Receive refactoring suggestions, reduce code complexity, optimize performance, and fix bugs (TBD).
 
 ## Requirements
 - Python 3.9 or higher  
 - OpenAI API key
 
 ## Usage
-To use `write-the`, run the following commands:
+
+To use `write-the` you must set an OPENAI_API_KEY environment variable (e.g. `export OPENAI_API_KEY=...`).
 
 ### Docs:
 ```bash
 write-the docs [OPTIONS] [PATH_TO_SOURCE_CODE]
 ```
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/docs-help.png)
@@ -64,19 +66,28 @@
 ```bash
 write-the tests [OPTIONS] [PATH_TO_SOURCE_CODE]
 ```
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/tests-help.png)
 
 
+### Convert:
+```bash
+write-the convert [OPTIONS] IN_FILE [OUT_FILE]
+```
+
+![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/convert-help.png)
+
 For detailed information on available options and parameters, refer to the official (`write-the` generated) [documentation](https://write-the.wytamma.com/).
 
 ## Roadmap
 
-For a detailed project roadmap, including planned features, improvements, and milestones, please see our Project Timeline.
+The main goal for write-the is to develop a generic module system to document, test, and optimise code in any language in a reliable and repatable way.
+
+For a detailed project roadmap, including planned features, improvements, and milestones, please see our Project Timeline (TBD).
 
 ## Contributing
 We welcome contributions from the community. If you would like to contribute to Write-The, please follow these steps:
 
 - Fork the repository and create a new branch for your feature or bugfix.
 - Develop your changes and ensure that your code follows the project's coding standards.
 - Create a pull request with a clear description of your changes and any relevant documentation.
```

### Comparing `write_the-0.8.0/images/docs-help.png` & `write_the-0.9.0/images/docs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/images/logo-black.svg` & `write_the-0.9.0/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/images/logo.png` & `write_the-0.9.0/images/logo.png`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/images/mkdocs-help.png` & `write_the-0.9.0/images/mkdocs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/images/multiply-docs-tests.png` & `write_the-0.9.0/images/multiply-docs-tests.png`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/images/tests-help.png` & `write_the-0.9.0/images/tests-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/images/untitled.blend` & `write_the-0.9.0/images/untitled.blend`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/images/untitled.blend1` & `write_the-0.9.0/images/untitled.blend1`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/images/write-the-docs.gif` & `write_the-0.9.0/images/write-the-docs.gif`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/images/write-the-icon.svg` & `write_the-0.9.0/images/write-the-icon.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/images/write-the.svg` & `write_the-0.9.0/images/write-the.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/tests/test_cli_main.py` & `write_the-0.9.0/tests/test_cli_main.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/tests/test_cst_docstring_adder.py` & `write_the-0.9.0/tests/test_cst_docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/tests/test_cst_docstring_remover.py` & `write_the-0.9.0/tests/test_cst_docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/tests/test_cst_function_and_class_collector.py` & `write_the-0.9.0/tests/test_cst_function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/tests/test_cst_node_extractor.py` & `write_the-0.9.0/tests/test_cst_node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/tests/test_cst_node_remover.py` & `write_the-0.9.0/tests/test_cst_node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/tests/test_cst_utils.py` & `write_the-0.9.0/tests/test_cst_utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/tests/test_utils.py` & `write_the-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/tests/data/expected.dat` & `write_the-0.9.0/tests/data/expected.dat`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/llm.py` & `write_the-0.9.0/write_the/llm.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/utils.py` & `write_the-0.9.0/write_the/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/cli/tasks.py` & `write_the-0.9.0/write_the/cli/tasks.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/commands/docs/docs.py` & `write_the-0.9.0/write_the/commands/docs/docs.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/commands/docs/prompts.py` & `write_the-0.9.0/write_the/commands/docs/prompts.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/commands/docs/utils.py` & `write_the-0.9.0/write_the/commands/docs/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/commands/mkdocs/mkdocs.py` & `write_the-0.9.0/write_the/commands/mkdocs/mkdocs.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/commands/mkdocs/templates.py` & `write_the-0.9.0/write_the/commands/mkdocs/templates.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/commands/tests/tests.py` & `write_the-0.9.0/write_the/commands/tests/tests.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/cst/docstring_adder.py` & `write_the-0.9.0/write_the/cst/docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/cst/docstring_remover.py` & `write_the-0.9.0/write_the/cst/docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/cst/function_and_class_collector.py` & `write_the-0.9.0/write_the/cst/function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/cst/node_batcher.py` & `write_the-0.9.0/write_the/cst/node_batcher.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/cst/node_extractor.py` & `write_the-0.9.0/write_the/cst/node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/cst/node_remover.py` & `write_the-0.9.0/write_the/cst/node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/write_the/cst/utils.py` & `write_the-0.9.0/write_the/cst/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/LICENSE.txt` & `write_the-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/README.md` & `write_the-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 ```
 ## Features
 
 Write-the offers the following AI-driven features:
 
 - Write-the Docs: Automatically generate documentation for your codebase, including class and function descriptions, parameter explanations, and examples.
 - Write-the Tests: Create test cases for your code, ensuring thorough test coverage and better code quality.
+- Write-the Convert: Convert code and data from any format into another. 
 - Write-the Refactor: Receive refactoring suggestions, reduce code complexity, optimize performance, and fix bugs (TBD).
 
 ## Requirements
 - Python 3.9 or higher  
 - OpenAI API key
 
 ## Usage
@@ -62,14 +63,21 @@
 ```bash
 write-the tests [OPTIONS] [PATH_TO_SOURCE_CODE]
 ```
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/tests-help.png)
 
 
+### Convert:
+```bash
+write-the convert [OPTIONS] IN_FILE [OUT_FILE]
+```
+
+![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/convert-help.png)
+
 For detailed information on available options and parameters, refer to the official (`write-the` generated) [documentation](https://write-the.wytamma.com/).
 
 ## Roadmap
 
 The main goal for write-the is to develop a generic module system to document, test, and optimise code in any language in a reliable and repatable way.
 
 For a detailed project roadmap, including planned features, improvements, and milestones, please see our Project Timeline (TBD).
```

### Comparing `write_the-0.8.0/pyproject.toml` & `write_the-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `write_the-0.8.0/PKG-INFO` & `write_the-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: write-the
-Version: 0.8.0
+Version: 0.9.0
 Summary: AI-powered Code Generation and Refactoring Tool
 Project-URL: Documentation, https://github.com/wytamma/write-the#readme
 Project-URL: Issues, https://github.com/wytamma/write-the/issues
 Project-URL: Source, https://github.com/wytamma/write-the
 Author-email: wytamma <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -57,14 +57,15 @@
 ```
 ## Features
 
 Write-the offers the following AI-driven features:
 
 - Write-the Docs: Automatically generate documentation for your codebase, including class and function descriptions, parameter explanations, and examples.
 - Write-the Tests: Create test cases for your code, ensuring thorough test coverage and better code quality.
+- Write-the Convert: Convert code and data from any format into another. 
 - Write-the Refactor: Receive refactoring suggestions, reduce code complexity, optimize performance, and fix bugs (TBD).
 
 ## Requirements
 - Python 3.9 or higher  
 - OpenAI API key
 
 ## Usage
@@ -91,14 +92,21 @@
 ```bash
 write-the tests [OPTIONS] [PATH_TO_SOURCE_CODE]
 ```
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/tests-help.png)
 
 
+### Convert:
+```bash
+write-the convert [OPTIONS] IN_FILE [OUT_FILE]
+```
+
+![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/convert-help.png)
+
 For detailed information on available options and parameters, refer to the official (`write-the` generated) [documentation](https://write-the.wytamma.com/).
 
 ## Roadmap
 
 The main goal for write-the is to develop a generic module system to document, test, and optimise code in any language in a reliable and repatable way.
 
 For a detailed project roadmap, including planned features, improvements, and milestones, please see our Project Timeline (TBD).
```

