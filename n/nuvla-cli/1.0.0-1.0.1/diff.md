# Comparing `tmp/nuvla_cli-1.0.0.tar.gz` & `tmp/nuvla_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvla_cli-1.0.0.tar", max compression
+gzip compressed data, was "nuvla_cli-1.0.1.tar", max compression
```

## Comparing `nuvla_cli-1.0.0.tar` & `nuvla_cli-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    11357 2023-05-02 09:55:36.938818 nuvla_cli-1.0.0/LICENSE
--rw-r--r--   0        0        0     1953 2023-05-02 09:55:36.938818 nuvla_cli-1.0.0/README.md
--rw-r--r--   0        0        0     1497 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/__init__.py
--rw-r--r--   0        0        0       40 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/__main__.py
--rw-r--r--   0        0        0        0 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/common/__init__.py
--rw-r--r--   0        0        0      637 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/common/cli_builder.py
--rw-r--r--   0        0        0     1126 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/common/common.py
--rw-r--r--   0        0        0     1342 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/common/constants.py
--rw-r--r--   0        0        0     2808 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/common/geo_location.py
--rw-r--r--   0        0        0        0 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/entity_action_cmd/__init__.py
--rw-r--r--   0        0        0     6248 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/entity_action_cmd/edge.py
--rw-r--r--   0        0        0     3148 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/entity_action_cmd/fleet.py
--rw-r--r--   0        0        0     1769 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/entity_action_cmd/user.py
--rw-r--r--   0        0        0        0 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/nuvlaio/__init__.py
--rw-r--r--   0        0        0     2458 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/nuvlaio/cli_api.py
--rw-r--r--   0        0        0      428 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/nuvlaio/device/__init__.py
--rw-r--r--   0        0        0     1619 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/nuvlaio/device/device.py
--rw-r--r--   0        0        0     1827 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/nuvlaio/device/dummy.py
--rw-r--r--   0        0        0     2342 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/nuvlaio/device/local.py
--rw-r--r--   0        0        0     4749 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/nuvlaio/device/release_control.py
--rw-r--r--   0        0        0     2045 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/nuvlaio/device/remote.py
--rw-r--r--   0        0        0     8641 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/nuvlaio/edge.py
--rw-r--r--   0        0        0     7752 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/nuvlaio/nuvlaedge_engine.py
--rw-r--r--   0        0        0     3387 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/nuvlaio/nuvlaio_cli.py
--rw-r--r--   0        0        0       98 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/schemas/__init__.py
--rw-r--r--   0        0        0      683 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/schemas/edge_schema.py
--rw-r--r--   0        0        0      897 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/schemas/engine_schema.py
--rw-r--r--   0        0        0      893 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/schemas/nuvla_schema.py
--rw-r--r--   0        0        0     1184 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/nuvla_cli/schemas/user_schema.py
--rw-r--r--   0        0        0      756 2023-05-02 09:55:36.986818 nuvla_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 nuvla_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 11:08:38.352162 nuvla_cli-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1953 2023-05-02 11:08:38.352162 nuvla_cli-1.0.1/README.md
+-rw-r--r--   0        0        0     1991 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/common/__init__.py
+-rw-r--r--   0        0        0      637 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/common/cli_builder.py
+-rw-r--r--   0        0        0     1126 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/common/common.py
+-rw-r--r--   0        0        0     1342 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/common/constants.py
+-rw-r--r--   0        0        0     2808 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/common/geo_location.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/entity_action_cmd/__init__.py
+-rw-r--r--   0        0        0     6248 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/entity_action_cmd/edge.py
+-rw-r--r--   0        0        0     3148 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/entity_action_cmd/fleet.py
+-rw-r--r--   0        0        0     1769 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/entity_action_cmd/user.py
+-rw-r--r--   0        0        0        0 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/nuvlaio/__init__.py
+-rw-r--r--   0        0        0     2458 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/nuvlaio/cli_api.py
+-rw-r--r--   0        0        0      428 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/nuvlaio/device/__init__.py
+-rw-r--r--   0        0        0     1619 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/nuvlaio/device/device.py
+-rw-r--r--   0        0        0     1827 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/nuvlaio/device/dummy.py
+-rw-r--r--   0        0        0     2342 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/nuvlaio/device/local.py
+-rw-r--r--   0        0        0     4749 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/nuvlaio/device/release_control.py
+-rw-r--r--   0        0        0     2045 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/nuvlaio/device/remote.py
+-rw-r--r--   0        0        0     8641 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/nuvlaio/edge.py
+-rw-r--r--   0        0        0     7752 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/nuvlaio/nuvlaedge_engine.py
+-rw-r--r--   0        0        0     3387 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/nuvlaio/nuvlaio_cli.py
+-rw-r--r--   0        0        0       98 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/schemas/__init__.py
+-rw-r--r--   0        0        0      683 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/schemas/edge_schema.py
+-rw-r--r--   0        0        0      897 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/schemas/engine_schema.py
+-rw-r--r--   0        0        0      893 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/schemas/nuvla_schema.py
+-rw-r--r--   0        0        0     1184 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/nuvla_cli/schemas/user_schema.py
+-rw-r--r--   0        0        0      756 2023-05-02 11:08:38.396163 nuvla_cli-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 nuvla_cli-1.0.1/PKG-INFO
```

### Comparing `nuvla_cli-1.0.0/LICENSE` & `nuvla_cli-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/README.md` & `nuvla_cli-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/__init__.py` & `nuvla_cli-1.0.1/nuvla_cli/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 """ Nuvla CLI main script """
 import logging
+import importlib.metadata
+from typing import Optional
+from typing_extensions import Annotated
 
 import typer
+from rich.pretty import pprint
 
 from nuvla_cli.common.cli_builder import build_entity_action
 from nuvla_cli.nuvlaio.edge import Edge
 
 
+__version__ = importlib.metadata.version("nuvla-cli")
+
 app_cli = typer.Typer(no_args_is_help=True)
 
 build_entity_action(app_cli)
 
 
 logging.basicConfig(
         level=logging.WARNING,
@@ -38,7 +44,23 @@
         edge: Edge = Edge()
         edges_in_nuvla = edge.nuvla_api.search('nuvlabox',
                                                filter={"tags=='cli.created=True'"})
 
         for nuvla_edge in edges_in_nuvla.resources:
             logger.info(f'Bulk remove Edge {nuvla_edge}')
             edge.remove_edge(nuvla_edge.data.get('id'), force=True)
+
+
+def version_callback(flag: bool):
+    if flag:
+        pprint(f'Nuvla-CLI Version: {__version__}')
+        raise typer.Exit(0)
+
+
+@app_cli.callback()
+def main(
+    version: Annotated[
+            Optional[bool],
+            typer.Option("--version", '-v', callback=version_callback)
+        ] = None,
+):
+    pass
```

### Comparing `nuvla_cli-1.0.0/nuvla_cli/common/cli_builder.py` & `nuvla_cli-1.0.1/nuvla_cli/common/cli_builder.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/common/common.py` & `nuvla_cli-1.0.1/nuvla_cli/common/common.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/common/constants.py` & `nuvla_cli-1.0.1/nuvla_cli/common/constants.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/common/geo_location.py` & `nuvla_cli-1.0.1/nuvla_cli/common/geo_location.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/entity_action_cmd/edge.py` & `nuvla_cli-1.0.1/nuvla_cli/entity_action_cmd/edge.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/entity_action_cmd/fleet.py` & `nuvla_cli-1.0.1/nuvla_cli/entity_action_cmd/fleet.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/entity_action_cmd/user.py` & `nuvla_cli-1.0.1/nuvla_cli/entity_action_cmd/user.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/nuvlaio/cli_api.py` & `nuvla_cli-1.0.1/nuvla_cli/nuvlaio/cli_api.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/nuvlaio/device/device.py` & `nuvla_cli-1.0.1/nuvla_cli/nuvlaio/device/device.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/nuvlaio/device/dummy.py` & `nuvla_cli-1.0.1/nuvla_cli/nuvlaio/device/dummy.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/nuvlaio/device/local.py` & `nuvla_cli-1.0.1/nuvla_cli/nuvlaio/device/local.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/nuvlaio/device/release_control.py` & `nuvla_cli-1.0.1/nuvla_cli/nuvlaio/device/release_control.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/nuvlaio/device/remote.py` & `nuvla_cli-1.0.1/nuvla_cli/nuvlaio/device/remote.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/nuvlaio/edge.py` & `nuvla_cli-1.0.1/nuvla_cli/nuvlaio/edge.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/nuvlaio/nuvlaedge_engine.py` & `nuvla_cli-1.0.1/nuvla_cli/nuvlaio/nuvlaedge_engine.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/nuvlaio/nuvlaio_cli.py` & `nuvla_cli-1.0.1/nuvla_cli/nuvlaio/nuvlaio_cli.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/schemas/edge_schema.py` & `nuvla_cli-1.0.1/nuvla_cli/schemas/edge_schema.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/schemas/engine_schema.py` & `nuvla_cli-1.0.1/nuvla_cli/schemas/engine_schema.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/schemas/nuvla_schema.py` & `nuvla_cli-1.0.1/nuvla_cli/schemas/nuvla_schema.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/nuvla_cli/schemas/user_schema.py` & `nuvla_cli-1.0.1/nuvla_cli/schemas/user_schema.py`

 * *Files identical despite different names*

### Comparing `nuvla_cli-1.0.0/pyproject.toml` & `nuvla_cli-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nuvla-cli"
-version = "1.0.0"
+version = "1.0.1"
 description = "CLI tool for local management of Nuvla and NuvlaEdges via terminal"
 authors = ["Nacho <nacho@sixsq.com>"]
 readme = "README.md"
 packages = [{include = "nuvla_cli"}]
 repository = "https://github.com/nuvla/cli"
 license = "Apache-2.0"
```

### Comparing `nuvla_cli-1.0.0/PKG-INFO` & `nuvla_cli-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuvla-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: CLI tool for local management of Nuvla and NuvlaEdges via terminal
 Home-page: https://github.com/nuvla/cli
 License: Apache-2.0
 Author: Nacho
 Author-email: nacho@sixsq.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

