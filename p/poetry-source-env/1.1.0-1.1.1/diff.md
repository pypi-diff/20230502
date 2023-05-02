# Comparing `tmp/poetry_source_env-1.1.0.tar.gz` & `tmp/poetry_source_env-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_source_env-1.1.0.tar", max compression
+gzip compressed data, was "poetry_source_env-1.1.1.tar", max compression
```

## Comparing `poetry_source_env-1.1.0.tar` & `poetry_source_env-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1099 2023-05-01 22:54:07.793303 poetry_source_env-1.1.0/LICENSE.md
--rw-r--r--   0        0        0     4042 2023-05-01 22:54:07.793303 poetry_source_env-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-01 22:54:07.793303 poetry_source_env-1.1.0/poetry_source_env/__init__.py
--rw-r--r--   0        0        0     2634 2023-05-01 22:54:07.793303 poetry_source_env-1.1.0/poetry_source_env/plugin.py
--rw-r--r--   0        0        0      737 2023-05-01 22:54:07.793303 poetry_source_env-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4873 1970-01-01 00:00:00.000000 poetry_source_env-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-02 21:30:00.136706 poetry_source_env-1.1.1/LICENSE.md
+-rw-r--r--   0        0        0     4005 2023-05-02 21:30:00.136706 poetry_source_env-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 21:30:00.136706 poetry_source_env-1.1.1/poetry_source_env/__init__.py
+-rw-r--r--   0        0        0     2624 2023-05-02 21:30:00.136706 poetry_source_env-1.1.1/poetry_source_env/plugin.py
+-rw-r--r--   0        0        0      737 2023-05-02 21:30:00.136706 poetry_source_env-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4836 1970-01-01 00:00:00.000000 poetry_source_env-1.1.1/PKG-INFO
```

### Comparing `poetry_source_env-1.1.0/LICENSE.md` & `poetry_source_env-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `poetry_source_env-1.1.0/README.md` & `poetry_source_env-1.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -21,51 +21,52 @@
 
 ## Usage
 
 Normally, you would define a package source in `pyproject.toml` like this:
 
 ```toml
 [[tool.poetry.source]]
-name = "my-epic-source"
-url = "https://pkg.celsiusnarhwal.dev"
+name = "foo"
+url = "https://foo.bar/simple"
 default = false
 secondary = false
 
 ```
 
 With poetry-source-env, you can define this source via environment variables, similar to how you can already
 configure [publishable repositories](https://python-poetry.org/docs/repositories/#publishable-repositories:~:text=Alternatively%2C%20you%20can%20use%20environment%20variables%20to%20provide%20the%20credentials%3A):
 
 ```bash
-export POETRY_REPOSITORIES_MY_EPIC_SOURCE_URL=https://pkg.celsiusnarhwal.dev
-export POETRY_REPOSITORIES_MY_EPIC_SOURCE_DEFAULT=false
-export POETRY_REPOSITORIES_MY_EPIC_SOURCE_SECONDARY=false
+export POETRY_REPOSITORIES_FOO_URL=https://foo.bar/simple
+export POETRY_REPOSITORIES_FOO_DEFAULT=false
+export POETRY_REPOSITORIES_FOO_SECONDARY=false
 ```
 
-If you prefer to keep the source defined in `pyproject.toml`, you can opt to conceal parts of its definition behind
-environment variables:
+If you prefer to keep the source defined in `pyproject.toml`, you can opt to conceal its name or URL, in whole or
+in part, behind environment variables:
 
 ```bash
-export INDEX_URL="https://pkg.celsiusnarhwal.dev"
+export FOO_INDEX_NAME="foo"
+export FOO_INDEX_URL="https://foo.bar/simple"
 ```
 
 ```toml
 [[tool.poetry.source]]
-name = "my-epic-source"
-url = "${INDEX_URL}"
+name = "${FOO_INDEX_NAME}"
+url = "${FOO_INDEX_URL}"
 default = false
 secondary = false
 
 ```
 
 If your source requires authentication, Poetry already supports defining its credentials via environment variables:
 
 ```bash
-export POETRY_HTTP_BASIC_MY_EPIC_SOURCE_USERNAME=celsiusnarhwal
-export POETRY_HTTP_BASIC_MY_EPIC_SOURCE_PASSWORD=superdupersecret
+export POETRY_HTTP_BASIC_FOO_USERNAME=celsiusnarhwal
+export POETRY_HTTP_BASIC_FOO_PASSWORD=superdupersecret
 ```
 
 ## Configuration
 
 poetry-source-env's behavior can be configured via the `tool.poetry-source-env` section of `pyproject.toml`.
 
 Supported configuration options include:
```

### Comparing `poetry_source_env-1.1.0/poetry_source_env/plugin.py` & `poetry_source_env-1.1.1/poetry_source_env/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,19 +39,19 @@
                         "env_name": match.group("name"),
                         "url": os.environ[env_key],
                     }
 
             for name, repository in repositories.items():
                 repo = LegacyRepository(name, repository["url"])
                 default = (
-                    os.getenv(f"POETRY_REPOSITORIES_{repository['env_name']}_DEFAULT")
+                    os.getenv(f"{config.prefix}{repository['env_name']}_DEFAULT")
                     == "true"
                 )
                 secondary = (
-                    os.getenv(f"POETRY_REPOSITORIES_{repository['env_name']}_SECONDARY")
+                    os.getenv(f"{config.prefix}{repository['env_name']}_SECONDARY")
                     == "true"
                 )
 
                 poetry.pool.add_repository(repo, default, secondary)
 
         if config.toml:
             for repository in poetry.pool.repositories:
```

### Comparing `poetry_source_env-1.1.0/pyproject.toml` & `poetry_source_env-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-source-env"
-version = "1.1.0"
+version = "1.1.1"
 description = "Load Poetry package sources from environment variables"
 authors = ["celsius narhwal <hello@celsiusnarhwal.dev>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/celsiusnarhwal/poetry-source-env"
 repository = "https://github.com/celsiusnarhwal/poetry-source-env"
```

### Comparing `poetry_source_env-1.1.0/PKG-INFO` & `poetry_source_env-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-source-env
-Version: 1.1.0
+Version: 1.1.1
 Summary: Load Poetry package sources from environment variables
 Home-page: https://github.com/celsiusnarhwal/poetry-source-env
 License: MIT
 Author: celsius narhwal
 Author-email: hello@celsiusnarhwal.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -42,51 +42,52 @@
 
 ## Usage
 
 Normally, you would define a package source in `pyproject.toml` like this:
 
 ```toml
 [[tool.poetry.source]]
-name = "my-epic-source"
-url = "https://pkg.celsiusnarhwal.dev"
+name = "foo"
+url = "https://foo.bar/simple"
 default = false
 secondary = false
 
 ```
 
 With poetry-source-env, you can define this source via environment variables, similar to how you can already
 configure [publishable repositories](https://python-poetry.org/docs/repositories/#publishable-repositories:~:text=Alternatively%2C%20you%20can%20use%20environment%20variables%20to%20provide%20the%20credentials%3A):
 
 ```bash
-export POETRY_REPOSITORIES_MY_EPIC_SOURCE_URL=https://pkg.celsiusnarhwal.dev
-export POETRY_REPOSITORIES_MY_EPIC_SOURCE_DEFAULT=false
-export POETRY_REPOSITORIES_MY_EPIC_SOURCE_SECONDARY=false
+export POETRY_REPOSITORIES_FOO_URL=https://foo.bar/simple
+export POETRY_REPOSITORIES_FOO_DEFAULT=false
+export POETRY_REPOSITORIES_FOO_SECONDARY=false
 ```
 
-If you prefer to keep the source defined in `pyproject.toml`, you can opt to conceal parts of its definition behind
-environment variables:
+If you prefer to keep the source defined in `pyproject.toml`, you can opt to conceal its name or URL, in whole or
+in part, behind environment variables:
 
 ```bash
-export INDEX_URL="https://pkg.celsiusnarhwal.dev"
+export FOO_INDEX_NAME="foo"
+export FOO_INDEX_URL="https://foo.bar/simple"
 ```
 
 ```toml
 [[tool.poetry.source]]
-name = "my-epic-source"
-url = "${INDEX_URL}"
+name = "${FOO_INDEX_NAME}"
+url = "${FOO_INDEX_URL}"
 default = false
 secondary = false
 
 ```
 
 If your source requires authentication, Poetry already supports defining its credentials via environment variables:
 
 ```bash
-export POETRY_HTTP_BASIC_MY_EPIC_SOURCE_USERNAME=celsiusnarhwal
-export POETRY_HTTP_BASIC_MY_EPIC_SOURCE_PASSWORD=superdupersecret
+export POETRY_HTTP_BASIC_FOO_USERNAME=celsiusnarhwal
+export POETRY_HTTP_BASIC_FOO_PASSWORD=superdupersecret
 ```
 
 ## Configuration
 
 poetry-source-env's behavior can be configured via the `tool.poetry-source-env` section of `pyproject.toml`.
 
 Supported configuration options include:
```

