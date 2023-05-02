# Comparing `tmp/shell_whisperer-0.1.1.tar.gz` & `tmp/shell_whisperer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_whisperer-0.1.1.tar", max compression
+gzip compressed data, was "shell_whisperer-0.1.2.tar", max compression
```

## Comparing `shell_whisperer-0.1.1.tar` & `shell_whisperer-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1152 2023-05-02 02:49:06.010665 shell_whisperer-0.1.1/README.md
--rw-r--r--   0        0        0      621 2023-05-02 03:22:37.832844 shell_whisperer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 22:15:29.864014 shell_whisperer-0.1.1/shell_whisperer/__init__.py
--rw-r--r--   0        0        0     1815 2023-05-02 01:57:51.702857 shell_whisperer-0.1.1/shell_whisperer/gpt_whisperer.py
--rw-r--r--   0        0        0     3173 2023-05-02 03:12:02.744104 shell_whisperer-0.1.1/shell_whisperer/main.py
--rw-r--r--   0        0        0      446 2023-05-01 23:52:51.186418 shell_whisperer-0.1.1/shell_whisperer/utils.py
--rw-r--r--   0        0        0     1984 1970-01-01 00:00:00.000000 shell_whisperer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1152 2023-05-02 02:49:06.010665 shell_whisperer-0.1.2/README.md
+-rw-r--r--   0        0        0      617 2023-05-02 03:25:05.262068 shell_whisperer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 22:15:29.864014 shell_whisperer-0.1.2/shell_whisperer/__init__.py
+-rw-r--r--   0        0        0     1815 2023-05-02 01:57:51.702857 shell_whisperer-0.1.2/shell_whisperer/gpt_whisperer.py
+-rw-r--r--   0        0        0     3173 2023-05-02 03:12:02.744104 shell_whisperer-0.1.2/shell_whisperer/main.py
+-rw-r--r--   0        0        0      446 2023-05-01 23:52:51.186418 shell_whisperer-0.1.2/shell_whisperer/utils.py
+-rw-r--r--   0        0        0     1984 1970-01-01 00:00:00.000000 shell_whisperer-0.1.2/PKG-INFO
```

### Comparing `shell_whisperer-0.1.1/README.md` & `shell_whisperer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `shell_whisperer-0.1.1/pyproject.toml` & `shell_whisperer-0.1.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shell-whisperer"
-version = "0.1.1"
+version = "0.1.2"
 description = "Shell Whisperer is a command-line tool that generates CLI (Command Line Interface) commands based on natural language input."
 authors = ["ishan <ishannagpal554@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shell_whisperer"}]
 license = "MIT"
 
 [tool.poetry.dependencies]
@@ -12,12 +12,12 @@
 requests = "^2.29.0"
 openai = "^0.27.5"
 typer = "^0.8.0"
 rich = "^13.3.5"
 pyperclip = "^1.8.2"
 
 [tool.poetry.scripts]
-command-whisperer = "command_whisperer.main:app"
+shell-whisperer = "shell_whisperer.main:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `shell_whisperer-0.1.1/shell_whisperer/gpt_whisperer.py` & `shell_whisperer-0.1.2/shell_whisperer/gpt_whisperer.py`

 * *Files identical despite different names*

### Comparing `shell_whisperer-0.1.1/shell_whisperer/main.py` & `shell_whisperer-0.1.2/shell_whisperer/main.py`

 * *Files identical despite different names*

### Comparing `shell_whisperer-0.1.1/PKG-INFO` & `shell_whisperer-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-whisperer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Shell Whisperer is a command-line tool that generates CLI (Command Line Interface) commands based on natural language input.
 License: MIT
 Author: ishan
 Author-email: ishannagpal554@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

