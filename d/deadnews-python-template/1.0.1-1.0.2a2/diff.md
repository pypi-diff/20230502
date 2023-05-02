# Comparing `tmp/deadnews_python_template-1.0.1.tar.gz` & `tmp/deadnews_python_template-1.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadnews_python_template-1.0.1.tar", max compression
+gzip compressed data, was "deadnews_python_template-1.0.2a2.tar", max compression
```

## Comparing `deadnews_python_template-1.0.1.tar` & `deadnews_python_template-1.0.2a2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1065 2022-11-30 18:16:52.071097 deadnews_python_template-1.0.1/LICENSE
--rw-r--r--   0        0        0      845 2022-11-30 18:16:52.071097 deadnews_python_template-1.0.1/README.md
--rw-r--r--   0        0        0     2549 2022-11-30 18:16:52.071097 deadnews_python_template-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      196 2022-11-30 18:16:52.071097 deadnews_python_template-1.0.1/src/deadnews_python_template/__init__.py
--rw-r--r--   0        0        0     1518 1970-01-01 00:00:00.000000 deadnews_python_template-1.0.1/setup.py
--rw-r--r--   0        0        0     1550 1970-01-01 00:00:00.000000 deadnews_python_template-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-02 02:45:50.545911 deadnews_python_template-1.0.2a2/LICENSE
+-rw-r--r--   0        0        0      845 2023-05-02 02:45:50.545911 deadnews_python_template-1.0.2a2/README.md
+-rw-r--r--   0        0        0     2517 2023-05-02 02:46:16.142064 deadnews_python_template-1.0.2a2/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-05-02 02:45:50.549911 deadnews_python_template-1.0.2a2/src/deadnews_python_template/__init__.py
+-rw-r--r--   0        0        0     1557 1970-01-01 00:00:00.000000 deadnews_python_template-1.0.2a2/PKG-INFO
```

### Comparing `deadnews_python_template-1.0.1/LICENSE` & `deadnews_python_template-1.0.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `deadnews_python_template-1.0.1/README.md` & `deadnews_python_template-1.0.2a2/README.md`

 * *Files identical despite different names*

### Comparing `deadnews_python_template-1.0.1/pyproject.toml` & `deadnews_python_template-1.0.2a2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,104 +1,109 @@
 [tool.poetry]
 name = "deadnews-python-template"
-version = "1.0.1"
+version = "1.0.2-alpha.2"
 description = "Python Project Template"
-authors = ["DeadNews <uhjnnn@gmail.com>"]
+authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/deadnews-python-template"
 repository = "https://github.com/DeadNews/deadnews-python-template"
 keywords = ["python", "template", "layout"]
 classifiers = ["Operating System :: OS Independent"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
-[tool.poetry.group.dev.dependencies]
-pre-commit = "^2.20.0"
-
 [tool.poetry.group.ci.dependencies]
-bandit = "^1.7.4"
-black = "^22.10.0"
-flake8 = "^6.0.0"
-flake8-bugbear = "^22.10.27"
-flake8-builtins = "^2.0.1"
-flake8-comprehensions = "^3.10.1"
-flake8-implicit-str-concat = "^0.3.0"
-flake8-pie = "^0.16.0"
-flake8-pyproject = "^1.2.1"
-flake8-pytest-style = "^1.6.0"
-flake8-requirements = "^1.7.5"
-flake8-simplify = "^0.19.3"
-flake8-unused-arguments = "^0.0.12"
-flake8-use-pathlib = "^0.3.0"
-isort = "^5.10.1"
-mypy = "^0.991"
-pep8-naming = "^0.13.2"
-poethepoet = "^0.16.5"
-safety = "^2.3.3"
+black = "^23.3.0"
+isort = "^5.12.0"
+mypy = "^1.2.0"
+poethepoet = "^0.19.0"
+ruff = "^0.0.263"
+safety = "^2.3.5"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.2.0"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 
+[tool.poetry.group.build.dependencies]
+poetry-dynamic-versioning = "^0.21.4"
+
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
+
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.black]
 line-length = 99
 
 [tool.isort]
 line_length = 99
 profile = "black"
 
-[tool.flake8]
-max-line-length = 99
-max-complexity = 18
-show-source = true
-ignore = [
-  "E501",   # Line too long.
-  "PIE786", # Use precise exception handlers.
-  "PIE803", # Use lazy % formatting in logging functions.
-  "W503",   # Line break occurred before a binary operator.
-]
-per-file-ignores = [
-  "tests/*: I900", # Package is not listed as a requirement.
-]
-
 [tool.mypy]
 disallow_untyped_defs = true
 follow_imports = "silent"
 ignore_missing_imports = true
 show_column_numbers = true
 show_error_codes = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 allow_untyped_defs = true
 
-[tool.bandit]
-exclude_dirs = ["tests"]
-skips = [
-  "B404", # Importing subprocess.
-  "B603", # Calling subprocess.Popen without shell=True.
-]
-
 [tool.pytest.ini_options]
 addopts = "--verbose --cov=./src"
 testpaths = ["tests"]
 markers = ["docker", "slow"]
 
 [tool.coverage.report]
 exclude_lines = ["if __name__ == .__main__.:"]
 
 [tool.poe.tasks]
 isort = "isort . --check-only --diff"
 black = "black . --check --diff"
 mypy = "mypy ."
-flake8 = "flake8 ."
-bandit = "bandit -r . -c pyproject.toml"
+ruff = "ruff check ."
 safety = "safety check -r pyproject.toml -o bare"
-ci.sequence = ["isort", "black", "mypy", "flake8", "bandit", "safety"]
-pc = "pre-commit run -a"
+ci.sequence = ["isort", "black", "mypy", "ruff"]  # safety
+
+[tool.ruff]
+line-length = 99
+select = [
+  "A",   # flake8-builtins
+  "ARG", # flake8-unused-arguments
+  "B",   # flake8-bugbear
+  "C4",  # flake8-comprehensions
+  "C90", # mccabe
+  "E",   # pycodestyle
+  "F",   # pyflakes
+  # "I",   # isort
+  "ISC", # flake8-implicit-str-concat
+  "N",   # pep8-naming
+  "PIE", # flake8-pie
+  "PT",  # flake8-pytest-style
+  "PTH", # flake8-use-pathlib
+  "RUF", # ruff-specific rules
+  "S",   # flake8-bandit
+  "SIM", # flake8-simplify
+  "T10", # flake8-debugger
+  "UP",  # pyupgrade
+]
+ignore = [
+  "E501", # Line too long
+  "S603", # Calling subprocess.Popen with shell=False
+]
+
+[tool.ruff.mccabe]
+max-complexity = 10
+
+[tool.ruff.flake8-comprehensions]
+allow-dict-calls-with-keyword-arguments = false
+
+[tool.ruff.per-file-ignores]
+"tests/*" = ["S"]
```

### Comparing `deadnews_python_template-1.0.1/PKG-INFO` & `deadnews_python_template-1.0.2a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deadnews-python-template
-Version: 1.0.1
+Version: 1.0.2a2
 Summary: Python Project Template
 Home-page: https://github.com/DeadNews/deadnews-python-template
 License: MIT
 Keywords: python,template,layout
 Author: DeadNews
-Author-email: uhjnnn@gmail.com
+Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

