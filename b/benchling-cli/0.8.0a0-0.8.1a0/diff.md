# Comparing `tmp/benchling_cli-0.8.0a0.tar.gz` & `tmp/benchling_cli-0.8.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchling_cli-0.8.0a0.tar", max compression
+gzip compressed data, was "benchling_cli-0.8.1a0.tar", max compression
```

## Comparing `benchling_cli-0.8.0a0.tar` & `benchling_cli-0.8.1a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/LICENSE
--rw-r--r--   0        0        0      237 2023-04-27 19:39:14.084632 benchling_cli-0.8.0a0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 19:38:48.974339 benchling_cli-0.8.0a0/benchling_cli/__init__.py
--rw-r--r--   0        0        0       41 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/__main__.py
--rw-r--r--   0        0        0        0 2023-04-27 19:38:49.004339 benchling_cli-0.8.0a0/benchling_cli/apps/__init__.py
--rw-r--r--   0        0        0     2567 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/cli.py
--rw-r--r--   0        0        0        0 2023-04-27 19:38:49.004339 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/__init__.py
--rw-r--r--   0        0        0     2257 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/generate_dependencies_module.py
--rw-r--r--   0        0        0     5465 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/generate_models.py
--rw-r--r--   0        0        0     4333 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/helpers.py
--rw-r--r--   0        0        0    14459 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/dependencies.py.jinja2
--rw-r--r--   0        0        0     2124 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/dropdown_model.py.jinja2
--rw-r--r--   0        0        0     1167 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/enum_scalar_model.py.jinja2
--rw-r--r--   0        0        0     8395 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/schema_instance_model.py.jinja2
--rw-r--r--   0        0        0    13835 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/workflow_instance_model.py.jinja2
--rw-r--r--   0        0        0      759 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/cli.py
--rw-r--r--   0        0        0       25 2023-04-27 19:34:35.571374 benchling_cli-0.8.0a0/benchling_cli/py.typed
--rw-r--r--   0        0        0     2316 2023-04-27 19:39:14.024631 benchling_cli-0.8.0a0/pyproject.toml
--rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 benchling_cli-0.8.0a0/setup.py
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 benchling_cli-0.8.0a0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-01 22:13:53.106489 benchling_cli-0.8.1a0/LICENSE
+-rw-r--r--   0        0        0      237 2023-05-01 22:14:05.136426 benchling_cli-0.8.1a0/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 22:13:53.576486 benchling_cli-0.8.1a0/benchling_cli/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-01 22:13:53.106489 benchling_cli-0.8.1a0/benchling_cli/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:13:53.576486 benchling_cli-0.8.1a0/benchling_cli/apps/__init__.py
+-rw-r--r--   0        0        0     2567 2023-05-01 22:13:53.106489 benchling_cli-0.8.1a0/benchling_cli/apps/cli.py
+-rw-r--r--   0        0        0        0 2023-05-01 22:13:53.576486 benchling_cli-0.8.1a0/benchling_cli/apps/codegen/__init__.py
+-rw-r--r--   0        0        0     2257 2023-05-01 22:13:53.106489 benchling_cli-0.8.1a0/benchling_cli/apps/codegen/generate_dependencies_module.py
+-rw-r--r--   0        0        0     5465 2023-05-01 22:13:53.106489 benchling_cli-0.8.1a0/benchling_cli/apps/codegen/generate_models.py
+-rw-r--r--   0        0        0     4438 2023-05-01 22:13:53.106489 benchling_cli-0.8.1a0/benchling_cli/apps/codegen/helpers.py
+-rw-r--r--   0        0        0    14459 2023-05-01 22:13:53.106489 benchling_cli-0.8.1a0/benchling_cli/apps/codegen/templates/dependencies.py.jinja2
+-rw-r--r--   0        0        0     2124 2023-05-01 22:13:53.106489 benchling_cli-0.8.1a0/benchling_cli/apps/codegen/templates/dropdown_model.py.jinja2
+-rw-r--r--   0        0        0     1167 2023-05-01 22:13:53.106489 benchling_cli-0.8.1a0/benchling_cli/apps/codegen/templates/enum_scalar_model.py.jinja2
+-rw-r--r--   0        0        0     8395 2023-05-01 22:13:53.106489 benchling_cli-0.8.1a0/benchling_cli/apps/codegen/templates/schema_instance_model.py.jinja2
+-rw-r--r--   0        0        0    13835 2023-05-01 22:13:53.106489 benchling_cli-0.8.1a0/benchling_cli/apps/codegen/templates/workflow_instance_model.py.jinja2
+-rw-r--r--   0        0        0      759 2023-05-01 22:13:53.106489 benchling_cli-0.8.1a0/benchling_cli/cli.py
+-rw-r--r--   0        0        0       25 2023-05-01 22:13:53.106489 benchling_cli-0.8.1a0/benchling_cli/py.typed
+-rw-r--r--   0        0        0     2316 2023-05-01 22:14:05.096427 benchling_cli-0.8.1a0/pyproject.toml
+-rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 benchling_cli-0.8.1a0/setup.py
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 benchling_cli-0.8.1a0/PKG-INFO
```

### Comparing `benchling_cli-0.8.0a0/LICENSE` & `benchling_cli-0.8.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.8.0a0/benchling_cli/apps/cli.py` & `benchling_cli-0.8.1a0/benchling_cli/apps/cli.py`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.8.0a0/benchling_cli/apps/codegen/generate_dependencies_module.py` & `benchling_cli-0.8.1a0/benchling_cli/apps/codegen/generate_dependencies_module.py`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.8.0a0/benchling_cli/apps/codegen/generate_models.py` & `benchling_cli-0.8.1a0/benchling_cli/apps/codegen/generate_models.py`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.8.0a0/benchling_cli/apps/codegen/helpers.py` & `benchling_cli-0.8.1a0/benchling_cli/apps/codegen/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,10 +94,12 @@
     # We can't seem to handle this programmatically by checking isinstance() or field truthiness
     except NotPresentError:
         pass
     return None
 
 
 def to_enum_option(enum_value: Union[str, float, int]) -> str:
+    if isinstance(enum_value, (int, float)):
+        enum_value = str(enum_value).replace("-", "MINUS_")
     # make all uppercase, remove any symbols, and replace spaces with underscores
     option_value = "_".join([word.upper() for word in _clean_and_split(str(enum_value))]).replace(".", "_")
     return option_value
```

### Comparing `benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/dependencies.py.jinja2` & `benchling_cli-0.8.1a0/benchling_cli/apps/codegen/templates/dependencies.py.jinja2`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/dropdown_model.py.jinja2` & `benchling_cli-0.8.1a0/benchling_cli/apps/codegen/templates/dropdown_model.py.jinja2`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/enum_scalar_model.py.jinja2` & `benchling_cli-0.8.1a0/benchling_cli/apps/codegen/templates/enum_scalar_model.py.jinja2`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/schema_instance_model.py.jinja2` & `benchling_cli-0.8.1a0/benchling_cli/apps/codegen/templates/schema_instance_model.py.jinja2`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.8.0a0/benchling_cli/apps/codegen/templates/workflow_instance_model.py.jinja2` & `benchling_cli-0.8.1a0/benchling_cli/apps/codegen/templates/workflow_instance_model.py.jinja2`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.8.0a0/benchling_cli/cli.py` & `benchling_cli-0.8.1a0/benchling_cli/cli.py`

 * *Files identical despite different names*

### Comparing `benchling_cli-0.8.0a0/pyproject.toml` & `benchling_cli-0.8.1a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "benchling-cli"
-version = "0.8.0a0"   # NOTE: This version number is ignored and does not correspond to releases (see README)
+version = "0.8.1a0"   # NOTE: This version number is ignored and does not correspond to releases (see README)
 description = "CLI for assistance in developing with the Benchling Platform."
 authors = ["Benchling Support <support@benchling.com>"]
 packages = [{include = "benchling_cli"}]
 include = [
     "LICENSE", "benchling_cli/py.typed"
 ]
 license = "Apache-2.0"
```

### Comparing `benchling_cli-0.8.0a0/setup.py` & `benchling_cli-0.8.1a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'typer>=0.6.1,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['benchling-cli = benchling_cli.cli:cli']}
 
 setup_kwargs = {
     'name': 'benchling-cli',
-    'version': '0.8.0a0',
+    'version': '0.8.1a0',
     'description': 'CLI for assistance in developing with the Benchling Platform.',
     'long_description': 'Benchling CLI\n-------------\n\nA Python 3.8+ CLI for the [Benchling](https://www.benchling.com/) platform designed to assist in developing against the\nBenchling platform\n\nTo see all commands available in the CLI, use `benchling-cli --help`',
     'author': 'Benchling Support',
     'author_email': 'support@benchling.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `benchling_cli-0.8.0a0/PKG-INFO` & `benchling_cli-0.8.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchling-cli
-Version: 0.8.0a0
+Version: 0.8.1a0
 Summary: CLI for assistance in developing with the Benchling Platform.
 License: Apache-2.0
 Author: Benchling Support
 Author-email: support@benchling.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

