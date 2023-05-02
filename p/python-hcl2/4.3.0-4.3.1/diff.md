# Comparing `tmp/python-hcl2-4.3.0.tar.gz` & `tmp/python-hcl2-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-hcl2/python-hcl2/dist/.tmp-nu6ienfq/python-hcl2-4.3.0.tar", last modified: Mon Jan 16 14:11:30 2023, max compression
+gzip compressed data, was "/home/runner/work/python-hcl2/python-hcl2/dist/.tmp-zyb9vd1n/python-hcl2-4.3.1.tar", last modified: Tue May  2 15:14:38 2023, max compression
```

## Comparing `python-hcl2-4.3.0.tar` & `python-hcl2-4.3.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/.codacy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/.github/workflows/pr_check.yml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/.yamllint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/bin/terraform_test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/hcl2/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/hcl2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/hcl2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/hcl2/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/hcl2/hcl2.lark
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/hcl2/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/hcl2/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/hcl2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/python_hcl2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/python_hcl2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/python_hcl2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/python_hcl2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/python_hcl2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 14:11:19.000000 python-hcl2-4.3.0/python_hcl2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/python_hcl2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/python_hcl2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/reports/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/reports/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 14:11:30.000000 python-hcl2-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-01-16 14:11:09.000000 python-hcl2-4.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.codacy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.github/workflows/pr_check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/.yamllint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/bin/terraform_test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/hcl2/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/hcl2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/hcl2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/hcl2/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/hcl2/hcl2.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/hcl2/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/hcl2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/hcl2/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/hcl2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/python_hcl2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/python_hcl2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/python_hcl2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/python_hcl2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/python_hcl2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:14:27.000000 python-hcl2-4.3.1/python_hcl2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/python_hcl2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/python_hcl2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/reports/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:14:38.000000 python-hcl2-4.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-02 15:14:18.000000 python-hcl2-4.3.1/tox.ini
```

### Comparing `python-hcl2-4.3.0/.github/workflows/codeql-analysis.yml` & `python-hcl2-4.3.1/.github/workflows/codeql-analysis.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ---
 name: CodeQL
 
 on:
   push:
-    branches: [master]
+    branches: [main]
   pull_request:
     # The branches below must be a subset of the branches above
-    branches: [master]
+    branches: [main]
   schedule:
     - cron: 0 18 * * 3
 
 jobs:
   analyse:
     name: Analyse
     runs-on: ubuntu-latest
@@ -19,37 +19,32 @@
       - name: Checkout repository
         uses: actions/checkout@v2
         with:
         # We must fetch at least the immediate parents so that if this is
         # a pull request then we can checkout the head.
           fetch-depth: 2
 
-    # If this run was triggered by a pull request event, then checkout
-    # the head of the pull request instead of the merge commit.
-      - run: git checkout HEAD^2
-        if: ${{ github.event_name == 'pull_request' }}
-
     # Initializes the CodeQL tools for scanning.
       - name: Initialize CodeQL
-        uses: github/codeql-action/init@v1
+        uses: github/codeql-action/init@v2
       # Override language selection by uncommenting this and choosing your languages
       # with:
       #   languages: go, javascript, csharp, python, cpp, java
 
     # Autobuild attempts to build any compiled languages  (C/C++, C#, or Java).
     # If this step fails, then you should remove it and run the build manually (see below)
       - name: Autobuild
-        uses: github/codeql-action/autobuild@v1
+        uses: github/codeql-action/autobuild@v2
 
     # ℹ️ Command-line programs to run using the OS shell.
     # 📚 https://git.io/JvXDl
 
     # ✏️ If the Autobuild fails above, remove it and uncomment the following three lines
     #    and modify them (or add more) to build your code if your project
     #    uses a compiled language
 
     #- run: |
     #   make bootstrap
     #   make release
 
       - name: Perform CodeQL Analysis
-        uses: github/codeql-action/analyze@v1
+        uses: github/codeql-action/analyze@v2
```

### Comparing `python-hcl2-4.3.0/.github/workflows/pr_check.yml` & `python-hcl2-4.3.1/.github/workflows/pr_check.yml`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.0/.github/workflows/publish.yml` & `python-hcl2-4.3.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.0/.gitignore` & `python-hcl2-4.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.0/.pre-commit-config.yaml` & `python-hcl2-4.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.0/CHANGELOG.md` & `python-hcl2-4.3.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## \[4.3.1\] - 2023-05-02
+
+### Added
+
+- Support for the braces in the next line. Thanks @rout39574 ([#129](https://github.com/amplify-education/python-hcl2/pull/129))
+- Support for the ternary multi-line expression. Thanks @seksham ([#128](https://github.com/amplify-education/python-hcl2/pull/128))
+
 ## \[4.3.0\] - 2022-01-16
 
 ### Added
 
 - Add tests for multiline comments inside a tuple ([#118](https://github.com/amplify-education/python-hcl2/pull/118))
 - Add `__begin_line__` and `__end_line__` meta parameters ([#120](https://github.com/amplify-education/python-hcl2/pull/120))
 - Add feature to parse comments in function args and list elems ([#119](https://github.com/amplify-education/python-hcl2/pull/119))
```

### Comparing `python-hcl2-4.3.0/LICENSE` & `python-hcl2-4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.0/PKG-INFO` & `python-hcl2-4.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hcl2
-Version: 4.3.0
+Version: 4.3.1
 Summary: A parser for HCL2
 Author-email: Amplify Education <github@amplify.com>
 License: MIT
 Project-URL: Homepage, https://github.com/amplify-education/python-hcl2
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
```

### Comparing `python-hcl2-4.3.0/README.md` & `python-hcl2-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.0/bin/terraform_test` & `python-hcl2-4.3.1/bin/terraform_test`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.0/hcl2/__main__.py` & `python-hcl2-4.3.1/hcl2/__main__.py`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.0/hcl2/api.py` & `python-hcl2-4.3.1/hcl2/api.py`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.0/hcl2/hcl2.lark` & `python-hcl2-4.3.1/hcl2/hcl2.lark`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 start : body
 body : (new_line_or_comment? (attribute | block))* new_line_or_comment?
 attribute : identifier "=" expression
-block : identifier (identifier | STRING_LIT)* "{" body "}"
+block : identifier (identifier | STRING_LIT)* new_line_or_comment? "{" body "}"
 new_line_and_or_comma: new_line_or_comment | "," | "," new_line_or_comment
 new_line_or_comment: ( /\n/ | /#.*\n/ | /\/\/.*\n/ )+
 
 identifier : /[a-zA-Z_][a-zA-Z0-9_-]*/
 
 ?expression : expr_term | operation | conditional
 
-conditional : expression "?" new_line_or_comment? expression new_line_or_comment? ":" new_line_or_comment? expression
+conditional : expression "?" new_line_or_comment? expression new_line_or_comment? ":" new_line_or_comment? expression new_line_or_comment?
 
 ?operation : unary_op | binary_op
 !unary_op : ("-" | "!") expr_term
-binary_op : expression binary_term
+binary_op : expression binary_term new_line_or_comment?
 !binary_operator : "==" | "!=" | "<" | ">" | "<=" | ">=" | "-" | "*" | "/" | "%" | "&&" | "||" | "+"
 binary_term : binary_operator new_line_or_comment? expression
 
 expr_term : "(" new_line_or_comment? expression new_line_or_comment? ")"
             | float_lit
             | int_lit
             | STRING_LIT
```

### Comparing `python-hcl2-4.3.0/hcl2/transformer.py` & `python-hcl2-4.3.1/hcl2/transformer.py`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.0/pylintrc` & `python-hcl2-4.3.1/pylintrc`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.0/pyproject.toml` & `python-hcl2-4.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-hcl2-4.3.0/python_hcl2.egg-info/PKG-INFO` & `python-hcl2-4.3.1/python_hcl2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hcl2
-Version: 4.3.0
+Version: 4.3.1
 Summary: A parser for HCL2
 Author-email: Amplify Education <github@amplify.com>
 License: MIT
 Project-URL: Homepage, https://github.com/amplify-education/python-hcl2
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
```

### Comparing `python-hcl2-4.3.0/python_hcl2.egg-info/SOURCES.txt` & `python-hcl2-4.3.1/python_hcl2.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 .github/workflows/publish.yml
 bin/terraform_test
 hcl2/__init__.py
 hcl2/__main__.py
 hcl2/api.py
 hcl2/hcl2.lark
 hcl2/parser.py
+hcl2/py.typed
 hcl2/transformer.py
 hcl2/version.py
 python_hcl2.egg-info/PKG-INFO
 python_hcl2.egg-info/SOURCES.txt
 python_hcl2.egg-info/dependency_links.txt
 python_hcl2.egg-info/entry_points.txt
 python_hcl2.egg-info/not-zip-safe
```

### Comparing `python-hcl2-4.3.0/tox.ini` & `python-hcl2-4.3.1/tox.ini`

 * *Files identical despite different names*

