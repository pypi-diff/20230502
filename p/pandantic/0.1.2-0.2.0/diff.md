# Comparing `tmp/pandantic-0.1.2.tar.gz` & `tmp/pandantic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandantic-0.1.2.tar", max compression
+gzip compressed data, was "pandantic-0.2.0.tar", max compression
```

## Comparing `pandantic-0.1.2.tar` & `pandantic-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3519 2023-04-14 15:22:28.796652 pandantic-0.1.2/README.md
--rw-r--r--   0        0        0      711 2023-04-14 15:22:35.877363 pandantic-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-12 19:53:14.255729 pandantic-0.1.2/src/pandantic/__init__.py
--rw-r--r--   0        0        0     2833 2023-04-14 14:30:26.856805 pandantic-0.1.2/src/pandantic/basemodel.py
--rw-r--r--   0        0        0     3939 1970-01-01 00:00:00.000000 pandantic-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3512 2023-05-02 19:16:57.940573 pandantic-0.2.0/README.md
+-rw-r--r--   0        0        0      840 2023-05-02 19:16:59.720597 pandantic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-05-02 19:16:57.940573 pandantic-0.2.0/src/pandantic/__init__.py
+-rw-r--r--   0        0        0     4541 2023-05-02 19:16:57.940573 pandantic-0.2.0/src/pandantic/basemodel.py
+-rw-r--r--   0        0        0     4029 1970-01-01 00:00:00.000000 pandantic-0.2.0/PKG-INFO
```

### Comparing `pandantic-0.1.2/README.md` & `pandantic-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 
 `pandantic` introduces the ability to validate (`pandas`) DataFrames using `pydantic.BaseModel`s. The `pandantic` package is using the V2 version of `pydantic` as it has significant improvements over its V1 versions (a performance increase up to 50 times).
 
 First, install `pandantic` by using pip (or any other package managing tool).
 
 ```pip install pandantic```
 
-## parse_df 
+## parse_df
 
 To validate `pd.DataFrame`s using Pydantic `BaseModel`s make sure to import the `BaseModel` class from the `pandantic` package.
 
 ```from pandantic import BaseModel```
 
 The `pandantic.BaseModel` subclasses the original `pydantic.BaseModel` which means the `pandantic.BaseModel` includes all functionality from the original `pydantic.BaseModel` but it adds the `parse_df` class method which should be used to parse DataFrames.
 
 ## A quick example
 
 Enough of the talking, lets just make things easier by showing a very minor but quick example. Make sure to import the `BaseModel` class from `pandantic` and create a schema like we normally would when using `pydantic`.
 
 ```
-from pandantic import BaseModel
 from pydantic.types import StrictInt
 
+from pandantic import BaseModel
+
 
 class DataFrameSchema(BaseModel):
     """Example schema for testing."""
-    
+
     example_str: str
     example_int: StrictInt
 ```
 
 Let's try this schema on a simple `pandas.DataFrame`. Use the class method `parse_df` from the freshly defined `DataFrameSchema` and specify the `dataframe` that should be validated using the arguments of the method. In this example, we want to `filter` out the bad records (there are more options like the good old `raise` to raise a ValueError after validating the whole DataFrame). In this case, only the second record would be kept in the returned DataFrame.
 
 ```
@@ -83,10 +84,7 @@
     dataframe=example_df_invalid,
     errors="raise",
 )
 ```
 ## Docs
 
 Need to work on this, I know. I do wrote an [Medium blogpost](https://duckduckgo.com) about the usage and possibilites of the `pandantic` package (including some benchmarks).
-
-
-
```

### Comparing `pandantic-0.1.2/pyproject.toml` & `pandantic-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 [tool.poetry]
 name = "pandantic"
-version = "0.1.2"
+version = "0.2.0"
 description = ""
 authors = ["wessel.huising <wessel.huising@mollie.com>"]
 readme = "README.md"
 
 packages = [
     { include = "pandantic", from = "src" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 pandas = "^2.0.0"
 pydantic = "2.0a2"
-
+multiprocess = "^0.70.14"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 pre-commit = "^3.2.2"
 black = "^23.3.0"
 pylint = "^2.17.2"
 isort = "^5.12.0"
 mypy = "^1.2.0"
 pre-commit-hooks = "^4.4.0"
 safety = "^2.3.5"
+scikit-learn = "^1.2.2"
+pandera = "^0.14.5"
+pandas-stubs = "^2.0.0.230412"
 
 [tool.mypy]
 strict = true
 warn_unreachable = true
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
+ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pandantic-0.1.2/PKG-INFO` & `pandantic-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 Metadata-Version: 2.1
 Name: pandantic
-Version: 0.1.2
+Version: 0.2.0
 Summary: 
 Author: wessel.huising
 Author-email: wessel.huising@mollie.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: multiprocess (>=0.70.14,<0.71.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pydantic (==2.0a2)
 Description-Content-Type: text/markdown
 
 # pandantic
 
 `pandantic` introduces the ability to validate (`pandas`) DataFrames using `pydantic.BaseModel`s. The `pandantic` package is using the V2 version of `pydantic` as it has significant improvements over its V1 versions (a performance increase up to 50 times).
 
 First, install `pandantic` by using pip (or any other package managing tool).
 
 ```pip install pandantic```
 
-## parse_df 
+## parse_df
 
 To validate `pd.DataFrame`s using Pydantic `BaseModel`s make sure to import the `BaseModel` class from the `pandantic` package.
 
 ```from pandantic import BaseModel```
 
 The `pandantic.BaseModel` subclasses the original `pydantic.BaseModel` which means the `pandantic.BaseModel` includes all functionality from the original `pydantic.BaseModel` but it adds the `parse_df` class method which should be used to parse DataFrames.
 
 ## A quick example
 
 Enough of the talking, lets just make things easier by showing a very minor but quick example. Make sure to import the `BaseModel` class from `pandantic` and create a schema like we normally would when using `pydantic`.
 
 ```
-from pandantic import BaseModel
 from pydantic.types import StrictInt
 
+from pandantic import BaseModel
+
 
 class DataFrameSchema(BaseModel):
     """Example schema for testing."""
-    
+
     example_str: str
     example_int: StrictInt
 ```
 
 Let's try this schema on a simple `pandas.DataFrame`. Use the class method `parse_df` from the freshly defined `DataFrameSchema` and specify the `dataframe` that should be validated using the arguments of the method. In this example, we want to `filter` out the bad records (there are more options like the good old `raise` to raise a ValueError after validating the whole DataFrame). In this case, only the second record would be kept in the returned DataFrame.
 
 ```
@@ -98,10 +101,7 @@
     errors="raise",
 )
 ```
 ## Docs
 
 Need to work on this, I know. I do wrote an [Medium blogpost](https://duckduckgo.com) about the usage and possibilites of the `pandantic` package (including some benchmarks).
 
-
-
-
```

