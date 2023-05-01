# Comparing `tmp/poetry_source_env-1.0.1.tar.gz` & `tmp/poetry_source_env-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_source_env-1.0.1.tar", max compression
+gzip compressed data, was "poetry_source_env-1.1.0.tar", max compression
```

## Comparing `poetry_source_env-1.0.1.tar` & `poetry_source_env-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1099 2023-04-29 22:28:03.933338 poetry_source_env-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     2540 2023-04-29 22:28:03.933338 poetry_source_env-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-29 22:28:03.937338 poetry_source_env-1.0.1/poetry_source_env/__init__.py
--rw-r--r--   0        0        0     1175 2023-04-29 22:28:03.937338 poetry_source_env-1.0.1/poetry_source_env/plugin.py
--rw-r--r--   0        0        0      695 2023-04-29 22:28:03.937338 poetry_source_env-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 poetry_source_env-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-01 22:54:07.793303 poetry_source_env-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     4042 2023-05-01 22:54:07.793303 poetry_source_env-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 22:54:07.793303 poetry_source_env-1.1.0/poetry_source_env/__init__.py
+-rw-r--r--   0        0        0     2634 2023-05-01 22:54:07.793303 poetry_source_env-1.1.0/poetry_source_env/plugin.py
+-rw-r--r--   0        0        0      737 2023-05-01 22:54:07.793303 poetry_source_env-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4873 1970-01-01 00:00:00.000000 poetry_source_env-1.1.0/PKG-INFO
```

### Comparing `poetry_source_env-1.0.1/LICENSE.md` & `poetry_source_env-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `poetry_source_env-1.0.1/pyproject.toml` & `poetry_source_env-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [tool.poetry]
 name = "poetry-source-env"
-version = "1.0.1"
+version = "1.1.0"
 description = "Load Poetry package sources from environment variables"
 authors = ["celsius narhwal <hello@celsiusnarhwal.dev>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/celsiusnarhwal/poetry-source-env"
 repository = "https://github.com/celsiusnarhwal/poetry-source-env"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 poetry = "^1.2"
+pydantic = "^1.10.7"
+dict-deep = "^4.1.2"
 
 [tool.black]
 target-version = ["py38"]
 line-length = 88
 
 [tool.isort]
 profile = "black"
```

### Comparing `poetry_source_env-1.0.1/PKG-INFO` & `poetry_source_env-1.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,20 @@
-Metadata-Version: 2.1
-Name: poetry-source-env
-Version: 1.0.1
-Summary: Load Poetry package sources from environment variables
-Home-page: https://github.com/celsiusnarhwal/poetry-source-env
-License: MIT
-Author: celsius narhwal
-Author-email: hello@celsiusnarhwal.dev
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: poetry (>=1.2,<2.0)
-Project-URL: Repository, https://github.com/celsiusnarhwal/poetry-source-env
-Description-Content-Type: text/markdown
-
 # poetry-source-env
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/poetry-source-env?logo=python&logoColor=white&style=for-the-badge)](https://pypi.org/project/poetry-source-env)
 [![PyPI](https://img.shields.io/pypi/v/poetry-source-env?logo=pypi&color=green&logoColor=white&style=for-the-badge)](https://pypi.org/project/poetry-source-env)
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/celsiusnarhwal/poetry-source-env?logo=github&color=orange&logoColor=white&style=for-the-badge)](https://github.com/celsiusnarhwal/poetry-source-env/releases)
 [![PyPI - License](https://img.shields.io/pypi/l/poetry-source-env?color=03cb98&style=for-the-badge)](https://github.com/celsiusnarhwal/poetry-source-env/blob/main/LICENSE.md)
 [![Code style: Black](https://aegis.celsiusnarhwal.dev/badge/black?style=for-the-badge)](https://github.com/psf/black)
 
-poetry-source-env is a Poetry plugin that allows for [package sources](https://python-poetry.org/docs/repositories/#package-sources)
-to be defined in environment variables. This lets you define private package sources for your project without exposing
-their URLs in `pyproject.toml`.
+poetry-source-env is a Poetry plugin that lets you define private package sources for your project without exposing
+their URLs in `pyproject.toml`. It can load package source definitions from environment variables and expand environment
+variables in the `tool.poetry.source` section of `pyproject.toml`.
 
-This plugin is intended as a workaround for python-poetry/poetry#5958 and will be deprecated if its functionality
+This plugin is intended as a workaround for python-poetry/poetry#5958 and will be deprecated if comparable functionality
 is ever implemented in Poetry itself.
 
 ## Installation
 
 ```bash
 poetry self add poetry-source-env
 ```
@@ -56,18 +37,45 @@
 
 ```bash
 export POETRY_REPOSITORIES_MY_EPIC_SOURCE_URL=https://pkg.celsiusnarhwal.dev
 export POETRY_REPOSITORIES_MY_EPIC_SOURCE_DEFAULT=false
 export POETRY_REPOSITORIES_MY_EPIC_SOURCE_SECONDARY=false
 ```
 
+If you prefer to keep the source defined in `pyproject.toml`, you can opt to conceal parts of its definition behind
+environment variables:
+
+```bash
+export INDEX_URL="https://pkg.celsiusnarhwal.dev"
+```
+
+```toml
+[[tool.poetry.source]]
+name = "my-epic-source"
+url = "${INDEX_URL}"
+default = false
+secondary = false
+
+```
+
 If your source requires authentication, Poetry already supports defining its credentials via environment variables:
 
 ```bash
 export POETRY_HTTP_BASIC_MY_EPIC_SOURCE_USERNAME=celsiusnarhwal
 export POETRY_HTTP_BASIC_MY_EPIC_SOURCE_PASSWORD=superdupersecret
 ```
 
+## Configuration
+
+poetry-source-env's behavior can be configured via the `tool.poetry-source-env` section of `pyproject.toml`.
+
+Supported configuration options include:
+
+| **Name** | **Type** | **Description**                                                                                                                   | **Required?** | **Default**            |
+| -------- | -------- | --------------------------------------------------------------------------------------------------------------------------------- | ------------- | ---------------------- |
+| `prefix` | string   | The prefix which poetry-source-env should expect source-defining environment variables to use. Has no effect if `env` is `false`. | No            | `POETRY_REPOSITORIES_` |
+| `env`    | boolean  | Whether to read package source definitions from environment variables.                                                            | No            | `true`                 |
+| `toml`   | boolean  | Whether to expand environment variables in the `tool.poetry.source` section of `pyproject.toml`.                                  | No            | `true`                 |
+
 ## License
 
 poetry-source-env is licensed under the [MIT License](https://github.com/celsiusnarhwal/poetry-source-env/blob/main/LICENSE.md).
-
```

