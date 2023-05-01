# Comparing `tmp/typer_config-0.1.1.tar.gz` & `tmp/typer_config-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_config-0.1.1.tar", max compression
+gzip compressed data, was "typer_config-0.1.1a1.tar", max compression
```

## Comparing `typer_config-0.1.1.tar` & `typer_config-0.1.1a1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2023-05-01 22:10:24.591238 typer_config-0.1.1/LICENSE
--rw-r--r--   0        0        0     3693 2023-05-01 22:10:24.591238 typer_config-0.1.1/README.md
--rw-r--r--   0        0        0      784 2023-05-01 22:10:24.591238 typer_config-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1306 2023-05-01 22:10:24.591238 typer_config-0.1.1/typer_config/__init__.py
--rw-r--r--   0        0        0     1705 2023-05-01 22:10:24.591238 typer_config-0.1.1/typer_config/loaders.py
--rw-r--r--   0        0        0     4638 1970-01-01 00:00:00.000000 typer_config-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-01 22:06:08.946924 typer_config-0.1.1a1/LICENSE
+-rw-r--r--   0        0        0     3693 2023-05-01 22:06:08.946924 typer_config-0.1.1a1/README.md
+-rw-r--r--   0        0        0      786 2023-05-01 22:06:08.946924 typer_config-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0     1306 2023-05-01 22:06:08.946924 typer_config-0.1.1a1/typer_config/__init__.py
+-rw-r--r--   0        0        0     1705 2023-05-01 22:06:08.946924 typer_config-0.1.1a1/typer_config/loaders.py
+-rw-r--r--   0        0        0     4640 1970-01-01 00:00:00.000000 typer_config-0.1.1a1/PKG-INFO
```

### Comparing `typer_config-0.1.1/LICENSE` & `typer_config-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_config-0.1.1/README.md` & `typer_config-0.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `typer_config-0.1.1/pyproject.toml` & `typer_config-0.1.1a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typer-config"
-version = "0.1.1"
+version = "0.1.1a1"
 description = "Utilities for working with configuration files in typer CLIs. "
 authors = ["Matt Anderson <matt@manderscience.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "typer_config"}]
 repository = "https://github.com/maxb2/typer-config"
 keywords = ["typer"]
```

### Comparing `typer_config-0.1.1/typer_config/__init__.py` & `typer_config-0.1.1a1/typer_config/__init__.py`

 * *Files identical despite different names*

### Comparing `typer_config-0.1.1/typer_config/loaders.py` & `typer_config-0.1.1a1/typer_config/loaders.py`

 * *Files identical despite different names*

### Comparing `typer_config-0.1.1/PKG-INFO` & `typer_config-0.1.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer-config
-Version: 0.1.1
+Version: 0.1.1a1
 Summary: Utilities for working with configuration files in typer CLIs. 
 Home-page: https://github.com/maxb2/typer-config
 License: MIT
 Keywords: typer
 Author: Matt Anderson
 Author-email: matt@manderscience.com
 Requires-Python: >=3.8,<4.0
```

