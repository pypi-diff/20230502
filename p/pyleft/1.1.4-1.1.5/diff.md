# Comparing `tmp/pyleft-1.1.4.tar.gz` & `tmp/pyleft-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyleft-1.1.4.tar", max compression
+gzip compressed data, was "pyleft-1.1.5.tar", max compression
```

## Comparing `pyleft-1.1.4.tar` & `pyleft-1.1.5.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1069 2022-12-29 01:38:52.954684 pyleft-1.1.4/LICENSE
--rw-r--r--   0        0        0     3386 2022-12-29 01:38:52.954684 pyleft-1.1.4/README.md
--rw-r--r--   0        0        0        0 2022-12-29 01:38:52.954684 pyleft-1.1.4/pyleft/__init__.py
--rw-r--r--   0        0        0       37 2022-12-29 01:38:52.954684 pyleft-1.1.4/pyleft/__main__.py
--rw-r--r--   0        0        0     8898 2022-12-29 01:38:52.958684 pyleft-1.1.4/pyleft/api.py
--rw-r--r--   0        0        0     1246 2022-12-29 01:38:52.958684 pyleft-1.1.4/pyleft/console.py
--rw-r--r--   0        0        0     1307 2022-12-29 01:38:52.958684 pyleft-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     4280 1970-01-01 00:00:00.000000 pyleft-1.1.4/setup.py
--rw-r--r--   0        0        0     4406 1970-01-01 00:00:00.000000 pyleft-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-01 22:17:15.683375 pyleft-1.1.5/LICENSE
+-rw-r--r--   0        0        0     3528 2023-05-01 22:17:15.683375 pyleft-1.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 22:17:15.683375 pyleft-1.1.5/pyleft/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-01 22:17:15.683375 pyleft-1.1.5/pyleft/__main__.py
+-rw-r--r--   0        0        0     8980 2023-05-01 22:17:15.683375 pyleft-1.1.5/pyleft/api.py
+-rw-r--r--   0        0        0     1246 2023-05-01 22:17:15.683375 pyleft-1.1.5/pyleft/console.py
+-rw-r--r--   0        0        0     1327 2023-05-01 22:17:15.683375 pyleft-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4574 1970-01-01 00:00:00.000000 pyleft-1.1.5/PKG-INFO
```

### Comparing `pyleft-1.1.4/LICENSE` & `pyleft-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyleft-1.1.4/README.md` & `pyleft-1.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # PyLeft
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![GitHub license](https://img.shields.io/github/license/NathanVaughn/pyleft)](https://github.com/NathanVaughn/pyleft/blob/main/LICENSE)
 [![PyPi versions](https://img.shields.io/pypi/pyversions/pyleft)](https://pypi.org/project/pyleft)
 [![PyPi downloads](https://img.shields.io/pypi/dm/pyleft)](https://pypi.org/project/pyleft)
 
 Python type annotation existence checker
 
 ---
 
 `pyleft` is a complement to Microsoft's [pyright](https://github.com/microsoft/pyright)
 tool. While `pyright` does an excellent job at type checking your Python code,
 it doesn't check to make sure type hints exist. If you forget to add type hints
 to a function, `pyright` will usually see no problems with it. This tool checks
-to make sure all of your code _has_ type hints, while leaving it to `pyright` to make
-sure they are actually correct.
+to make sure all of your code _has_ type hints, while leaving it to
+`pyright` to make sure they are actually correct.
 
 ## Installation
 
 PyLeft requires Python 3.7+.
 
 `pip install pyleft`
 
@@ -45,26 +46,29 @@
 - tests\files\fail_4.py
         Argument 'one' of function 'wheels:4' has no type annotation
 ```
 
 ## Options
 
 - `files`: List of filenames and/or directories to recursively check.
-- `--exclude`: (optional) List of patterns to exclude, in `.gitignore` format. Takes predecence over `files`.
-- `--no-gitignore`: (optional) Don't use the exclusions from the .gitignore from the current working directory.
+- `--exclude`: (optional) List of patterns to exclude, in `.gitignore` format.
+  Takes precedence over `files`.
+- `--no-gitignore`: (optional) Don't use the exclusions from the .gitignore from
+  the current working directory.
 - `--quiet`: (optional) Don't print any output to STDOUT.
 - `--verbose`: (optional) Print debugging information to STDERR.
 
 ## Configuration
 
 Configuration is done through the `pyproject.toml` file.
 
 ```toml
 [tool.pyleft]
-# "files" in the configuration file are added to the option given on the command line
+# "files" in the configuration file are added to the option given on the
+# command line
 # This can either be a list, or a space separated string
 files = ["extra/directory/"]
 # This can either be a list, or a space separated string
 exclude = ["*_pb2.py"]
 no-gitignore = true
 ```
```

### Comparing `pyleft-1.1.4/pyleft/api.py` & `pyleft-1.1.5/pyleft/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import ast
 import os
 import sys
 from pathlib import Path
 from typing import List, Optional, Tuple, Union
 
 import pathspec
-import tomli
+
+try:
+    import tomllib as toml
+except ImportError:
+    import tomli as toml  # pyright: ignore
 
 type_comments = sys.version_info >= (3, 8)
 
 
 def debug_print(verbose: bool, message: str) -> None:
     if verbose:
         print(message, file=sys.stderr)
@@ -141,15 +145,15 @@
     # try to load config from pyproject.toml file
     pyproject = os.path.join(os.getcwd(), "pyproject.toml")
     if not os.path.isfile(pyproject):
         return [], [], False
 
     debug_print(verbose, f"Loading {pyproject}")
     with open(pyproject, "rb") as fp:
-        pyproject_config = tomli.load(fp)
+        pyproject_config = toml.load(fp)
 
     if "tool" not in pyproject_config or "pyleft" not in pyproject_config["tool"]:
         return [], [], False
 
     debug_print(verbose, "Loading tool.pyleft settings")
     config = pyproject_config["tool"]["pyleft"]
 
@@ -206,15 +210,14 @@
 
 def main(
     filenames: List[str],
     exclusions: Optional[List[str]] = None,
     no_gitignore: bool = False,
     verbose: bool = False,
 ) -> List[str]:
-
     cwd = Path(os.getcwd())
 
     # prevent using mutable type
     if exclusions is None:
         exclusions = []
 
     # load config
```

### Comparing `pyleft-1.1.4/pyleft/console.py` & `pyleft-1.1.5/pyleft/console.py`

 * *Files identical despite different names*

### Comparing `pyleft-1.1.4/pyproject.toml` & `pyleft-1.1.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "pyleft"
-    version = "1.1.4"
+    version = "1.1.5"
     description = "Python type annotation existence checker"
     license = "MIT"
     readme = "README.md"
     homepage = "https://github.com/NathanVaughn/pyleft"
     repository = "https://github.com/NathanVaughn/pyleft.git"
     authors = ["Nathan Vaughn <nvaughn51@gmail.com>"]
     classifiers = [
@@ -16,31 +16,32 @@
 [tool.poetry.urls]
     Issues = "https://github.com/NathanVaughn/pyleft/issues"
 
 [tool.poetry.dependencies]
     python = ">=3.7,<4.0"
 
     # match Black's dependencies
-    # https://github.com/psf/black/blob/6064a435453cdba47c43d71f3d0ea1aa19a29206/setup.py#L99
-    tomli    = ">=1.1.0"
+    # https://github.com/psf/black/blob/e712e48e06420d9240ce95c81acfcf6f11d14c83/pyproject.toml#L69-L71
+    tomli    = { version = ">=1.1.0", python = "<3.11" }
     pathspec = ">=0.9.0"
 
-[tool.poetry.dev-dependencies]
-    pytest           = "^7.2.0"
-    black            = "^22.12"
-    isort            = "^5.11.4"
-    autoflake        = "^1.7"
-    flake8           = "<5"
-    pyproject-flake8 = "^4.0.1"
+[tool.poetry.group.dev.dependencies]
+    pytest     = "^7.2.0"
+    pre-commit = "^2.21.0"
+
+[tool.pyright]
+    typeCheckingMode = "basic"
+    venvPath         = "."
+    venv             = ".venv"
 
-[tool.poetry.scripts]
-    pyleft = "pyleft.console:run"
+[tool.pyleft]
+    exclude = ["tests/**"]
 
-[tool.isort]
-    profile = "black"
+[tool.ruff]
+    ignore = ["E501"]
 
-[tool.flake8]
-    ignore = "E501,W503"
+[tool.poetry.scripts]
+    pyleft = "pyleft.console:run"
 
 [build-system]
     requires      = ["poetry-core>=1.0.0"]
     build-backend = "poetry.core.masonry.api"
```

### Comparing `pyleft-1.1.4/setup.py` & `pyleft-1.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,124 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyleft
+Version: 1.1.5
+Summary: Python type annotation existence checker
+Home-page: https://github.com/NathanVaughn/pyleft
+License: MIT
+Author: Nathan Vaughn
+Author-email: nvaughn51@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
+Requires-Dist: pathspec (>=0.9.0)
+Requires-Dist: tomli (>=1.1.0) ; python_version < "3.11"
+Project-URL: Issues, https://github.com/NathanVaughn/pyleft/issues
+Project-URL: Repository, https://github.com/NathanVaughn/pyleft.git
+Description-Content-Type: text/markdown
+
+# PyLeft
+
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![GitHub license](https://img.shields.io/github/license/NathanVaughn/pyleft)](https://github.com/NathanVaughn/pyleft/blob/main/LICENSE)
+[![PyPi versions](https://img.shields.io/pypi/pyversions/pyleft)](https://pypi.org/project/pyleft)
+[![PyPi downloads](https://img.shields.io/pypi/dm/pyleft)](https://pypi.org/project/pyleft)
+
+Python type annotation existence checker
+
+---
+
+`pyleft` is a complement to Microsoft's [pyright](https://github.com/microsoft/pyright)
+tool. While `pyright` does an excellent job at type checking your Python code,
+it doesn't check to make sure type hints exist. If you forget to add type hints
+to a function, `pyright` will usually see no problems with it. This tool checks
+to make sure all of your code _has_ type hints, while leaving it to
+`pyright` to make sure they are actually correct.
+
+## Installation
+
+PyLeft requires Python 3.7+.
+
+`pip install pyleft`
+
+## Usage
+
+PyLeft is a Python module that can be run via `python -m`. Just provide the directories
+or files to recursively check.
+
+`python -m pyleft .`
+
+The module will exit with an exit code of 0 if all type hints are present, or 1
+if there are any issues.
+
+### Example
+
+```bash
+> pyleft .
+- tests\files\fail_1.py
+        Argument 'two' of function 'add:1' has no type annotation
+- tests\files\fail_2.py
+        Function 'add:1' has no return type annotation
+- tests\files\fail_3.py
+        Function 'drive:2' has no return type annotation
+- tests\files\fail_4.py
+        Argument 'one' of function 'wheels:4' has no type annotation
+```
+
+## Options
+
+- `files`: List of filenames and/or directories to recursively check.
+- `--exclude`: (optional) List of patterns to exclude, in `.gitignore` format.
+  Takes precedence over `files`.
+- `--no-gitignore`: (optional) Don't use the exclusions from the .gitignore from
+  the current working directory.
+- `--quiet`: (optional) Don't print any output to STDOUT.
+- `--verbose`: (optional) Print debugging information to STDERR.
+
+## Configuration
+
+Configuration is done through the `pyproject.toml` file.
+
+```toml
+[tool.pyleft]
+# "files" in the configuration file are added to the option given on the
+# command line
+# This can either be a list, or a space separated string
+files = ["extra/directory/"]
+# This can either be a list, or a space separated string
+exclude = ["*_pb2.py"]
+no-gitignore = true
+```
+
+The `quiet` and `verbose` options can only be specified from the command line.
+
+## Design Decisions
+
+Only files with a `.py` extension are checked. Currently, `.pyi` files are not checked.
+
+The `__init__` and `__new__` methods of a class are not required to
+have return type hints. `pyright` automatically assumes this to be `None`.
+
+The first (`self`) argument of any class method is not required to have a type hint.
+
+The first (`cls`) argument of any class `@property` or `@classmethod` or `__new__`
+method is not required to have a type hint.
+
+Any variable argument list (`*arg`) or keyword argument dict (`**kwarg`)
+is not required to have a type hint.
+
+Types of types, such as `List` or `Tuple` are not required. For example,
+a type hint of just `list` is allowed, although you should normally be as specific
+as possible with a better type hint like `List[int]`.
 
-packages = \
-['pyleft']
+## Disclaimer
 
-package_data = \
-{'': ['*']}
+This project is not affiliated in any way with Microsoft.
 
-install_requires = \
-['pathspec>=0.9.0', 'tomli>=1.1.0']
-
-entry_points = \
-{'console_scripts': ['pyleft = pyleft.console:run']}
-
-setup_kwargs = {
-    'name': 'pyleft',
-    'version': '1.1.4',
-    'description': 'Python type annotation existence checker',
-    'long_description': '# PyLeft\n\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![GitHub license](https://img.shields.io/github/license/NathanVaughn/pyleft)](https://github.com/NathanVaughn/pyleft/blob/main/LICENSE)\n[![PyPi versions](https://img.shields.io/pypi/pyversions/pyleft)](https://pypi.org/project/pyleft)\n[![PyPi downloads](https://img.shields.io/pypi/dm/pyleft)](https://pypi.org/project/pyleft)\n\nPython type annotation existence checker\n\n---\n\n`pyleft` is a complement to Microsoft\'s [pyright](https://github.com/microsoft/pyright)\ntool. While `pyright` does an excellent job at type checking your Python code,\nit doesn\'t check to make sure type hints exist. If you forget to add type hints\nto a function, `pyright` will usually see no problems with it. This tool checks\nto make sure all of your code _has_ type hints, while leaving it to `pyright` to make\nsure they are actually correct.\n\n## Installation\n\nPyLeft requires Python 3.7+.\n\n`pip install pyleft`\n\n## Usage\n\nPyLeft is a Python module that can be run via `python -m`. Just provide the directories\nor files to recursively check.\n\n`python -m pyleft .`\n\nThe module will exit with an exit code of 0 if all type hints are present, or 1\nif there are any issues.\n\n### Example\n\n```bash\n> pyleft .\n- tests\\files\\fail_1.py\n        Argument \'two\' of function \'add:1\' has no type annotation\n- tests\\files\\fail_2.py\n        Function \'add:1\' has no return type annotation\n- tests\\files\\fail_3.py\n        Function \'drive:2\' has no return type annotation\n- tests\\files\\fail_4.py\n        Argument \'one\' of function \'wheels:4\' has no type annotation\n```\n\n## Options\n\n- `files`: List of filenames and/or directories to recursively check.\n- `--exclude`: (optional) List of patterns to exclude, in `.gitignore` format. Takes predecence over `files`.\n- `--no-gitignore`: (optional) Don\'t use the exclusions from the .gitignore from the current working directory.\n- `--quiet`: (optional) Don\'t print any output to STDOUT.\n- `--verbose`: (optional) Print debugging information to STDERR.\n\n## Configuration\n\nConfiguration is done through the `pyproject.toml` file.\n\n```toml\n[tool.pyleft]\n# "files" in the configuration file are added to the option given on the command line\n# This can either be a list, or a space separated string\nfiles = ["extra/directory/"]\n# This can either be a list, or a space separated string\nexclude = ["*_pb2.py"]\nno-gitignore = true\n```\n\nThe `quiet` and `verbose` options can only be specified from the command line.\n\n## Design Decisions\n\nOnly files with a `.py` extension are checked. Currently, `.pyi` files are not checked.\n\nThe `__init__` and `__new__` methods of a class are not required to\nhave return type hints. `pyright` automatically assumes this to be `None`.\n\nThe first (`self`) argument of any class method is not required to have a type hint.\n\nThe first (`cls`) argument of any class `@property` or `@classmethod` or `__new__`\nmethod is not required to have a type hint.\n\nAny variable argument list (`*arg`) or keyword argument dict (`**kwarg`)\nis not required to have a type hint.\n\nTypes of types, such as `List` or `Tuple` are not required. For example,\na type hint of just `list` is allowed, although you should normally be as specific\nas possible with a better type hint like `List[int]`.\n\n## Disclaimer\n\nThis project is not affiliated in any way with Microsoft.\n',
-    'author': 'Nathan Vaughn',
-    'author_email': 'nvaughn51@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/NathanVaughn/pyleft',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

