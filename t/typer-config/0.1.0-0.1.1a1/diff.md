# Comparing `tmp/typer_config-0.1.0.tar.gz` & `tmp/typer_config-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_config-0.1.0.tar", max compression
+gzip compressed data, was "typer_config-0.1.1a1.tar", max compression
```

## Comparing `typer_config-0.1.0.tar` & `typer_config-0.1.1a1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2023-05-01 18:19:39.198935 typer_config-0.1.0/LICENSE
--rw-r--r--   0        0        0     3687 2023-05-01 20:41:02.213226 typer_config-0.1.0/README.md
--rw-r--r--   0        0        0      766 2023-05-01 19:10:49.507873 typer_config-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1300 2023-05-01 20:43:39.935630 typer_config-0.1.0/typer_config/__init__.py
--rw-r--r--   0        0        0     1699 2023-05-01 20:42:35.792792 typer_config-0.1.0/typer_config/loaders.py
--rw-r--r--   0        0        0     4582 1970-01-01 00:00:00.000000 typer_config-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-01 22:06:08.946924 typer_config-0.1.1a1/LICENSE
+-rw-r--r--   0        0        0     3693 2023-05-01 22:06:08.946924 typer_config-0.1.1a1/README.md
+-rw-r--r--   0        0        0      786 2023-05-01 22:06:08.946924 typer_config-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0     1306 2023-05-01 22:06:08.946924 typer_config-0.1.1a1/typer_config/__init__.py
+-rw-r--r--   0        0        0     1705 2023-05-01 22:06:08.946924 typer_config-0.1.1a1/typer_config/loaders.py
+-rw-r--r--   0        0        0     4640 1970-01-01 00:00:00.000000 typer_config-0.1.1a1/PKG-INFO
```

### Comparing `typer_config-0.1.0/LICENSE` & `typer_config-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_config-0.1.0/README.md` & `typer_config-0.1.1a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,17 @@
 Then, we can read the values in our typer CLI:
 
 ```python
 # typer_config.py
 import typer
 import typer_config
 
-from typing import Any
+from typing import Any, Dict
 
-def pyproject_loader(path: str) -> dict[str, Any]:
+def pyproject_loader(path: str) -> Dict[str, Any]:
     if not path: # set a default path to read from
         path = "pyproject.toml"
         
     pyproject = toml.load("pyproject.toml")
     conf = pyproject["tool"]["my_tool"]
     return conf
```

### Comparing `typer_config-0.1.0/pyproject.toml` & `typer_config-0.1.1a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "typer-config"
-version = "0.1.0"
+version = "0.1.1a1"
 description = "Utilities for working with configuration files in typer CLIs. "
 authors = ["Matt Anderson <matt@manderscience.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "typer_config"}]
 repository = "https://github.com/maxb2/typer-config"
 keywords = ["typer"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 typer = "^0.8.0"
 toml = {version = "^0.10.2", optional = true}
 pyyaml = {version = "^6.0", optional = true}
 
 [tool.poetry.extras]
 toml = ["toml"]
 yaml = ["pyyaml"]
 all = ["toml", "pyyaml"]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.263"
 pylint = "^2.17.3"
 black = "^23.3.0"
 isort = "^5.12.0"
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `typer_config-0.1.0/typer_config/__init__.py` & `typer_config-0.1.1a1/typer_config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
 Typer Configuration Utilities
 """
 
-from typing import Any, Callable
+from typing import Any, Callable, Dict
 
 import typer
 
 from .loaders import json_loader, toml_loader, yaml_loader
 
 
 def conf_callback_factory(
-    loader: Callable[[Any], dict[str, Any]]
+    loader: Callable[[Any], Dict[str, Any]]
 ) -> Callable[[typer.Context, typer.CallbackParam, Any], Any]:
     """Configuration callback factory
 
     Parameters
     ----------
-    loader : Callable[[Any], dict[str, Any]]
+    loader : Callable[[Any], Dict[str, Any]]
         Loader function that takes the value passed to the typer CLI and
         returns a dictionary that is applied to the click context's default map.
 
     Returns
     -------
     Callable[[typer.Context, typer.CallbackParam, Any], Any]
         Configuration callback function.
     """
 
     def _callback(ctx: typer.Context, param: typer.CallbackParam, value: Any) -> Any:
         try:
             conf = loader(value)  # Load config file
             ctx.default_map = ctx.default_map or {}  # Initialize the default map
-            ctx.default_map.update(conf)  # Merge the config dict into default_map
+            ctx.default_map.update(conf)  # Merge the config Dict into default_map
         except Exception as ex:
             raise typer.BadParameter(param) from ex
         return value
 
     return _callback
```

### Comparing `typer_config-0.1.0/typer_config/loaders.py` & `typer_config-0.1.1a1/typer_config/loaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Configuration File Loaders.
 
-These loaders must follow the signature: Callable[[Any], dict[str, Any]]
+These loaders must follow the signature: Callable[[Any], Dict[str, Any]]
 """
 
-from typing import Any
+from typing import Any, Dict
 
 try:
     # Only available for python>=3.11
     import tomllib as toml
 except ImportError:
     try:
         # Third-party toml parsing library
@@ -21,81 +21,81 @@
 except ImportError:
     yaml = None
 
 import json
 
 
 # pylint: disable-next=unused-argument
-def dummy_loader(path: str) -> dict[str, Any]:
+def dummy_loader(path: str) -> Dict[str, Any]:
     """Dummy loader to show the required interface.
 
     Parameters
     ----------
     path : str
         path of file to load
 
     Returns
     -------
-    dict
+    Dict
         dictionary loaded from file
     """
     return {}
 
 
-def yaml_loader(path: str) -> dict[str, Any]:
+def yaml_loader(path: str) -> Dict[str, Any]:
     """YAML file loader
 
     Parameters
     ----------
     path : str
         path of YAML file
 
     Returns
     -------
-    dict
+    Dict
         dictionary loaded from file
     """
 
     with open(path, "r", encoding="utf-8") as _file:
         conf = yaml.safe_load(_file)
 
     return conf
 
 
-def json_loader(path: str) -> dict[str, Any]:
+def json_loader(path: str) -> Dict[str, Any]:
     """JSON file loader
 
     Parameters
     ----------
     path : str
         path of JSON file
 
     Returns
     -------
-    dict
+    Dict
         dictionary loaded from file
     """
 
     with open(path, "r", encoding="utf-8") as _file:
         conf = json.load(_file)
 
     return conf
 
 
-def toml_loader(path: str) -> dict[str, Any]:
+def toml_loader(path: str) -> Dict[str, Any]:
     """TOML file loader
 
     Parameters
     ----------
     path : str
         path of TOML file
 
     Returns
     -------
-    dict
+    Dict
         dictionary loaded from file
     """
 
     with open(path, "r", encoding="utf-8") as _file:
         conf = toml.load(_file)
 
     return conf
```

### Comparing `typer_config-0.1.0/PKG-INFO` & `typer_config-0.1.1a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: typer-config
-Version: 0.1.0
+Version: 0.1.1a1
 Summary: Utilities for working with configuration files in typer CLIs. 
 Home-page: https://github.com/maxb2/typer-config
 License: MIT
 Keywords: typer
 Author: Matt Anderson
 Author-email: matt@manderscience.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: toml
 Provides-Extra: yaml
 Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "yaml" or extra == "all"
@@ -107,17 +108,17 @@
 Then, we can read the values in our typer CLI:
 
 ```python
 # typer_config.py
 import typer
 import typer_config
 
-from typing import Any
+from typing import Any, Dict
 
-def pyproject_loader(path: str) -> dict[str, Any]:
+def pyproject_loader(path: str) -> Dict[str, Any]:
     if not path: # set a default path to read from
         path = "pyproject.toml"
         
     pyproject = toml.load("pyproject.toml")
     conf = pyproject["tool"]["my_tool"]
     return conf
```

