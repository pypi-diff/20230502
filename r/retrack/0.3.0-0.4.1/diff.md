# Comparing `tmp/retrack-0.3.0.tar.gz` & `tmp/retrack-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retrack-0.3.0.tar", max compression
+gzip compressed data, was "retrack-0.4.1.tar", max compression
```

## Comparing `retrack-0.3.0.tar` & `retrack-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1072 2023-02-27 17:46:16.140757 retrack-0.3.0/LICENSE
--rw-r--r--   0        0        0     4906 2023-02-27 17:46:16.140757 retrack-0.3.0/README.md
--rw-r--r--   0        0        0     1518 2023-02-27 17:46:16.140757 retrack-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      366 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/__init__.py
--rw-r--r--   0        0        0        0 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/engine/__init__.py
--rw-r--r--   0        0        0     5062 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/engine/parser.py
--rw-r--r--   0        0        0     2907 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/engine/request_manager.py
--rw-r--r--   0        0        0     6010 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/engine/runner.py
--rw-r--r--   0        0        0      465 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/engine/validators/__init__.py
--rw-r--r--   0        0        0      267 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/engine/validators/base.py
--rw-r--r--   0        0        0      414 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/engine/validators/check_is_dag.py
--rw-r--r--   0        0        0     1303 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/engine/validators/node_exists.py
--rw-r--r--   0        0        0     1323 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/__init__.py
--rw-r--r--   0        0        0     1460 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/base.py
--rw-r--r--   0        0        0     2605 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/check.py
--rw-r--r--   0        0        0     2123 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/constants.py
--rw-r--r--   0        0        0      822 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/contains.py
--rw-r--r--   0        0        0      910 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/endswith.py
--rw-r--r--   0        0        0      858 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/endswithany.py
--rw-r--r--   0        0        0     1009 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/inputs.py
--rw-r--r--   0        0        0     1606 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/logic.py
--rw-r--r--   0        0        0      953 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/match.py
--rw-r--r--   0        0        0     2116 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/math.py
--rw-r--r--   0        0        0     1085 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/outputs.py
--rw-r--r--   0        0        0      581 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/start.py
--rw-r--r--   0        0        0      926 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/startswith.py
--rw-r--r--   0        0        0      874 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/nodes/startswithany.py
--rw-r--r--   0        0        0        0 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/utils/__init__.py
--rw-r--r--   0        0        0      197 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/utils/constants.py
--rw-r--r--   0        0        0     1619 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/utils/graph.py
--rw-r--r--   0        0        0     1324 2023-02-27 17:46:16.144757 retrack-0.3.0/retrack/utils/registry.py
--rw-r--r--   0        0        0     5845 2023-02-27 17:46:24.162925 retrack-0.3.0/setup.py
--rw-r--r--   0        0        0     5622 2023-02-27 17:46:24.163376 retrack-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-02 17:30:19.838518 retrack-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4914 2023-05-02 17:30:19.838518 retrack-0.4.1/README.md
+-rw-r--r--   0        0        0     1518 2023-05-02 17:30:19.838518 retrack-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      366 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/engine/__init__.py
+-rw-r--r--   0        0        0     6675 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/engine/parser.py
+-rw-r--r--   0        0        0     2907 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/engine/request_manager.py
+-rw-r--r--   0        0        0     6463 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/engine/runner.py
+-rw-r--r--   0        0        0     1322 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/__init__.py
+-rw-r--r--   0        0        0     1800 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/base.py
+-rw-r--r--   0        0        0     2574 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/check.py
+-rw-r--r--   0        0        0     2234 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/constants.py
+-rw-r--r--   0        0        0      873 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/contains.py
+-rw-r--r--   0        0        0      910 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/endswith.py
+-rw-r--r--   0        0        0      941 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/endswithany.py
+-rw-r--r--   0        0        0     1009 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/inputs.py
+-rw-r--r--   0        0        0     1606 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/logic.py
+-rw-r--r--   0        0        0     1056 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/match.py
+-rw-r--r--   0        0        0     2116 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/math.py
+-rw-r--r--   0        0        0     1085 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/outputs.py
+-rw-r--r--   0        0        0      581 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/start.py
+-rw-r--r--   0        0        0      926 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/startswith.py
+-rw-r--r--   0        0        0      957 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/nodes/startswithany.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/utils/__init__.py
+-rw-r--r--   0        0        0      197 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/utils/constants.py
+-rw-r--r--   0        0        0     1324 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/utils/registry.py
+-rw-r--r--   0        0        0      154 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/utils/transformers.py
+-rw-r--r--   0        0        0      594 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/validators/__init__.py
+-rw-r--r--   0        0        0      267 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/validators/base.py
+-rw-r--r--   0        0        0      407 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/validators/check_is_dag.py
+-rw-r--r--   0        0        0     1296 2023-05-02 17:30:19.838518 retrack-0.4.1/retrack/validators/node_exists.py
+-rw-r--r--   0        0        0     5846 2023-05-02 17:30:29.127900 retrack-0.4.1/setup.py
+-rw-r--r--   0        0        0     5630 2023-05-02 17:30:29.128374 retrack-0.4.1/PKG-INFO
```

### Comparing `retrack-0.3.0/LICENSE` & `retrack-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `retrack-0.3.0/README.md` & `retrack-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # Parse the rule/model
 parser = retrack.Parser(rule)
 
 # Create a runner
 runner = retrack.Runner(parser)
 
 # Run the rule/model passing the data
-runner(data)
+runner.execute(data)
 ```
 
 The `Parser` class parses the rule/model and creates a graph of nodes. The `Runner` class runs the rule/model using the data passed to the runner. The `data` is a dictionary or a list of dictionaries containing the data that will be used to evaluate the conditions and execute the actions. To see wich data is required for the given rule/model, check the `runner.request_model` property that is a pydantic model used to validate the data.
 
 ### Creating a rule/model
 
 A rule is a set of conditions and actions that are executed when the conditions are met. The conditions are evaluated using the data passed to the runner. The actions are executed when the conditions are met.
```

### Comparing `retrack-0.3.0/pyproject.toml` & `retrack-0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retrack"
-version = "0.3.0"
+version = "0.4.1"
 description = "A business rules engine"
 authors = ["Gabriel Guarisa <gabrielguarisa@gmail.com>", "Nathalia Trotte <nathaliatrotte@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gabrielguarisa/retrack"
 homepage = "https://github.com/gabrielguarisa/retrack"
 keywords = ["rules", "models", "business", "node", "graph"]
```

### Comparing `retrack-0.3.0/retrack/engine/request_manager.py` & `retrack-0.4.1/retrack/engine/request_manager.py`

 * *Files identical despite different names*

### Comparing `retrack-0.3.0/retrack/engine/runner.py` & `retrack-0.4.1/retrack/engine/runner.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,103 +2,103 @@
 
 import numpy as np
 import pandas as pd
 import pydantic
 
 from retrack.engine.parser import Parser
 from retrack.engine.request_manager import RequestManager
-from retrack.nodes.base import NodeKind
-from retrack.utils import constants, graph
+from retrack.nodes.base import NodeKind, NodeMemoryType
+from retrack.utils import constants
 
 
 class Runner:
     def __init__(self, parser: Parser):
         self._parser = parser
+        self.reset()
+        self._set_constants()
+        self._set_input_columns()
+        self._request_manager = RequestManager(self._parser.get_by_kind(NodeKind.INPUT))
 
-        input_nodes = self._parser.get_nodes_by_kind(NodeKind.INPUT)
-        self._input_new_columns = {
-            f"{node.id}@{constants.INPUT_OUTPUT_VALUE_CONNECTOR_NAME}": node.data.name
-            for node in input_nodes
-        }
-        self._request_manager = RequestManager(input_nodes)
-
-        self._execution_order = graph.get_execution_order(self._parser)
-        self._state_df = None
-
-        self._filters = {}
+    @property
+    def parser(self) -> Parser:
+        return self._parser
 
     @property
     def request_manager(self) -> RequestManager:
         return self._request_manager
 
     @property
     def request_model(self) -> pydantic.BaseModel:
         return self._request_manager.model
 
     @property
-    def state_df(self) -> pd.DataFrame:
-        return self._state_df
-
-    @property
-    def states(self) -> list:
-        return self._state_df.to_dict(orient="records")
+    def states(self) -> pd.DataFrame:
+        return self._states
 
     @property
     def filters(self) -> dict:
         return self._filters
 
     @property
-    def filter_df(self) -> pd.DataFrame:
-        return pd.DataFrame(self._filters)
+    def constants(self) -> dict:
+        return self._constants
+
+    def _set_constants(self):
+        constant_nodes = self.parser.get_by_memory_type(NodeMemoryType.CONSTANT)
+        self._constants = {}
+        for node in constant_nodes:
+            for output_connector_name, _ in node.outputs:
+                self._constants[f"{node.id}@{output_connector_name}"] = node.data.value
+
+    @property
+    def input_columns(self) -> dict:
+        return self._input_columns
+
+    def _set_input_columns(self):
+        input_nodes = self._parser.get_by_kind(NodeKind.INPUT)
+        self._input_columns = {
+            f"{node.id}@{constants.INPUT_OUTPUT_VALUE_CONNECTOR_NAME}": node.data.name
+            for node in input_nodes
+        }
+
+    def reset(self):
+        self._states = None
+        self._filters = {}
+
+    def __set_output_connection_filters(
+        self, node_id: str, filter: typing.Any, filter_by_connector=None
+    ):
+        if filter is not None:
+            output_connections = self.parser.get_node_connections(
+                node_id, is_input=False, filter_by_connector=filter_by_connector
+            )
+            for output_connection_id in output_connections:
+                if self._filters.get(output_connection_id, None) is None:
+                    self._filters[output_connection_id] = filter
+                else:
+                    self._filters[output_connection_id] = (
+                        self._filters[output_connection_id] & filter
+                    )
 
-    def __get_initial_state_df(self, payload: typing.Union[dict, list]) -> pd.DataFrame:
+    def _create_initial_state_from_payload(
+        self, payload: typing.Union[dict, list]
+    ) -> pd.DataFrame:
+        """Create initial state from payload. This is the first step of the runner."""
         validated_payload = self.request_manager.validate(payload)
         validated_payload = pd.DataFrame([p.dict() for p in validated_payload])
 
         state_df = pd.DataFrame([])
-        for node_id, input_name in self._input_new_columns.items():
+        for node_id, input_name in self.input_columns.items():
             state_df[node_id] = validated_payload[input_name]
 
         state_df[constants.OUTPUT_REFERENCE_COLUMN] = np.nan
         state_df[constants.OUTPUT_MESSAGE_REFERENCE_COLUMN] = np.nan
 
         return state_df
 
-    @staticmethod
-    def __get_output_state_df(state_df: pd.DataFrame) -> pd.DataFrame:
-        output_state_df = state_df[
-            [
-                constants.OUTPUT_REFERENCE_COLUMN,
-                constants.OUTPUT_MESSAGE_REFERENCE_COLUMN,
-            ]
-        ].copy()
-
-        output_state_df = output_state_df.rename(
-            columns={
-                constants.OUTPUT_REFERENCE_COLUMN: "output",
-                constants.OUTPUT_MESSAGE_REFERENCE_COLUMN: "message",
-            }
-        )
-
-        return output_state_df
-
-    def __set_output_connection_filters(
-        self, node, value: typing.Any, filter_by_connector=None
-    ):
-        output_connections = graph.get_node_connections(
-            node, is_input=False, filter_by_connector=filter_by_connector
-        )
-        for output_connection_id in output_connections:
-            if self._filters.get(output_connection_id, None) is None:
-                self._filters[output_connection_id] = value
-            else:
-                self._filters[output_connection_id] = (
-                    self._filters[output_connection_id] & value
-                )
-
     def __get_input_params(
         self, node_dict: dict, current_node_filter: pd.Series
     ) -> dict:
         input_params = {}
 
         for connector_name, connections in node_dict.get("inputs", {}).items():
             if connector_name.endswith(constants.NULL_SUFFIX):
@@ -107,66 +107,76 @@
             for connection in connections["connections"]:
                 input_params[connector_name] = self.__get_state_data(
                     f"{connection['node']}@{connection['output']}", current_node_filter
                 )
 
         return input_params
 
-    def __get_state_data(self, column: str, filter_by: typing.Any = None):
-        if filter_by is None:
-            return self._state_df[column]
-        else:
-            return self._state_df.loc[filter_by, column]
-
     def __set_state_data(
         self, column: str, value: typing.Any, filter_by: typing.Any = None
     ):
         if filter_by is None:
-            self._state_df[column] = value
+            self._states[column] = value
         else:
-            self._state_df.loc[filter_by, column] = value
+            self._states.loc[filter_by, column] = value
+
+    def __get_state_data(self, column: str, filter_by: typing.Any = None):
+        if column in self._constants:
+            return self._constants[column]
+
+        if filter_by is None:
+            return self._states[column]
+
+        return self._states.loc[filter_by, column]
 
     def __run_node(self, node_id: str):
-        node = self._parser.get_node_by_id(node_id)
         current_node_filter = self._filters.get(node_id, None)
+        # if there is a filter, we need to set the children nodes to receive filtered data
+        self.__set_output_connection_filters(node_id, current_node_filter)
+
+        node = self.parser.get_by_id(node_id)
+
+        if node.memory_type == NodeMemoryType.CONSTANT:
+            return
 
         input_params = self.__get_input_params(
             node.dict(by_alias=True), current_node_filter
         )
-
-        if (
-            current_node_filter is not None
-        ):  # if there is a filter, we need to set the children nodes to receive filtered data
-            self.__set_output_connection_filters(node, current_node_filter)
-
         output = node.run(**input_params)
+
         for output_name, output_value in output.items():
             if (
                 output_name == constants.OUTPUT_REFERENCE_COLUMN
                 or output_name == constants.OUTPUT_MESSAGE_REFERENCE_COLUMN
             ):  # Setting output values
                 self.__set_state_data(output_name, output_value, current_node_filter)
             elif output_name.endswith(constants.FILTER_SUFFIX):  # Setting filters
-                self.__set_output_connection_filters(node, output_value, output_name)
+                self.__set_output_connection_filters(node_id, output_value, output_name)
             else:  # Setting node outputs to be used as inputs by other nodes
                 self.__set_state_data(
                     f"{node_id}@{output_name}", output_value, current_node_filter
                 )
 
-    def __call__(
-        self, payload: typing.Union[dict, list], to_dict: bool = True
-    ) -> pd.DataFrame:
-        self._state_df = self.__get_initial_state_df(payload)
-        self._filters = {}
+    def __get_output_states(self) -> pd.DataFrame:
+        """Returns a dataframe with the final states of the flow"""
+        return pd.DataFrame(
+            {
+                "output": self.states[constants.OUTPUT_REFERENCE_COLUMN],
+                "message": self.states[constants.OUTPUT_MESSAGE_REFERENCE_COLUMN],
+            }
+        )
+
+    def execute(self, payload: typing.Union[dict, list]) -> pd.DataFrame:
+        """Executes the flow with the given payload"""
+        self.reset()
+        self._states = self._create_initial_state_from_payload(payload)
 
-        for node_id in self._execution_order:
+        for node_id in self.parser.execution_order:
             try:
                 self.__run_node(node_id)
             except Exception as e:
-                raise e  # TODO: Handle errors
-            if self._state_df[constants.OUTPUT_REFERENCE_COLUMN].isna().sum() == 0:
+                print(f"Error running node {node_id}")
+                raise e
+            if self.states[constants.OUTPUT_REFERENCE_COLUMN].isna().sum() == 0:
                 break
 
-        if to_dict:
-            return self.__get_output_state_df(self._state_df).to_dict(orient="records")
-
-        return Runner.__get_output_state_df(self._state_df)
+        return self.__get_output_states()
```

### Comparing `retrack-0.3.0/retrack/engine/validators/node_exists.py` & `retrack-0.4.1/retrack/validators/node_exists.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from retrack.engine.validators.base import BaseValidator
+from retrack.validators.base import BaseValidator
 
 
 class NodeExistsValidator(BaseValidator):
     """Validator that checks if a node exists in the graph."""
 
     def __init__(
         self, node_name: str, max_quantity: int = None, min_quantity: int = None
```

### Comparing `retrack-0.3.0/retrack/nodes/__init__.py` & `retrack-0.4.1/retrack/nodes/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,28 +10,37 @@
 from retrack.nodes.math import Math
 from retrack.nodes.outputs import Output
 from retrack.nodes.start import Start
 from retrack.nodes.startswith import StartsWith
 from retrack.nodes.startswithany import StartsWithAny
 from retrack.utils.registry import Registry
 
-registry = Registry()
+_registry = Registry()
 
-registry.register("Input", Input)
-registry.register("Start", Start)
-registry.register("Constant", Constant)
-registry.register("List", List)
-registry.register("Bool", Bool)
-registry.register("Output", Output)
-registry.register("Check", Check)
-registry.register("If", If)
-registry.register("And", And)
-registry.register("Or", Or)
-registry.register("Not", Not)
-registry.register("Math", Math)
-registry.register("StartsWith", StartsWith)
-registry.register("EndsWith", EndsWith)
-registry.register("StartsWithAny", StartsWithAny)
-registry.register("EndsWithAny", EndsWithAny)
-registry.register("Contains", Contains)
 
-__all__ = ["registry", "BaseNode"]
+def registry() -> Registry:
+    return _registry
+
+
+def register(name: str, node: BaseNode) -> None:
+    registry().register(name, node)
+
+
+register("Input", Input)
+register("Start", Start)
+register("Constant", Constant)
+register("List", List)
+register("Bool", Bool)
+register("Output", Output)
+register("Check", Check)
+register("If", If)
+register("And", And)
+register("Or", Or)
+register("Not", Not)
+register("Math", Math)
+register("StartsWith", StartsWith)
+register("EndsWith", EndsWith)
+register("StartsWithAny", StartsWithAny)
+register("EndsWithAny", EndsWithAny)
+register("Contains", Contains)
+
+__all__ = ["registry", "register", "BaseNode"]
```

### Comparing `retrack-0.3.0/retrack/nodes/check.py` & `retrack-0.4.1/retrack/nodes/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 import typing
 
 import enum
 
 import pandas as pd
 import pydantic
 
-from retrack.nodes.base import (
-    BaseNode,
-    InputConnectionModel,
-    NodeKind,
-    OutputConnectionModel,
-)
+from retrack.nodes.base import BaseNode, InputConnectionModel, OutputConnectionModel
 
 ###############################################################
 # Check Metadata Models
 ###############################################################
 
 
 class CheckOperator(str, enum.Enum):
```

### Comparing `retrack-0.3.0/retrack/nodes/constants.py` & `retrack-0.4.1/retrack/nodes/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import pydantic
 
 from retrack.nodes.base import (
     BaseNode,
     InputConnectionModel,
     NodeKind,
+    NodeMemoryType,
     OutputConnectionModel,
 )
 
 #######################################################
 # Constant Metadata Models
 #######################################################
 
@@ -74,15 +75,18 @@
 
 
 class List(BaseConstant):
     data: ListMetadataModel
     outputs: ListOutputsModel
 
     def run(self, **kwargs) -> typing.Dict[str, typing.Any]:
-        return {"output_list": self.data.value}
+        return {}  # {"output_list": self.data.value}
+
+    def memory_type(self) -> NodeMemoryType:
+        return NodeMemoryType.CONSTANT
 
 
 class Bool(BaseConstant):
     data: BoolMetadataModel = BoolMetadataModel(value=False)
     outputs: BoolOutputsModel
 
     def run(self, **kwargs) -> typing.Dict[str, typing.Any]:
```

### Comparing `retrack-0.3.0/retrack/nodes/contains.py` & `retrack-0.4.1/retrack/nodes/contains.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 import pydantic
 
 from retrack.nodes.base import BaseNode, InputConnectionModel, OutputConnectionModel
+from retrack.utils import transformers
 
 ################################################
 # Contains Inputs Outputs
 ################################################
 
 
 class ContainsInputsModel(pydantic.BaseModel):
@@ -23,8 +24,8 @@
 
 
 class Contains(BaseNode):
     inputs: ContainsInputsModel
     outputs: ContainsOutputsModel
 
     def run(self, input_list: pd.Series, input_value: pd.Series) -> pd.Series:
-        return {"output_bool": input_value.isin(input_list.to_list())}
+        return {"output_bool": input_value.isin(transformers.to_list(input_list))}
```

### Comparing `retrack-0.3.0/retrack/nodes/endswith.py` & `retrack-0.4.1/retrack/nodes/endswith.py`

 * *Files identical despite different names*

### Comparing `retrack-0.3.0/retrack/nodes/inputs.py` & `retrack-0.4.1/retrack/nodes/inputs.py`

 * *Files identical despite different names*

### Comparing `retrack-0.3.0/retrack/nodes/logic.py` & `retrack-0.4.1/retrack/nodes/logic.py`

 * *Files identical despite different names*

### Comparing `retrack-0.3.0/retrack/nodes/match.py` & `retrack-0.4.1/retrack/nodes/match.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pandas as pd
 import pydantic
 
 from retrack.nodes.base import (
     BaseNode,
     InputConnectionModel,
     NodeKind,
+    NodeMemoryType,
     OutputConnectionModel,
 )
 
 ################################################
 # If Inputs and Outputs
 ################################################
 
@@ -37,7 +38,10 @@
         return NodeKind.FILTER
 
     def run(self, input_bool: pd.Series) -> typing.Dict[str, pd.Series]:
         return {
             f"output_then_filter": input_bool,
             f"output_else_filter": ~input_bool,
         }
+
+    def memory_type(self) -> NodeMemoryType:
+        return NodeMemoryType.FILTER
```

### Comparing `retrack-0.3.0/retrack/nodes/math.py` & `retrack-0.4.1/retrack/nodes/math.py`

 * *Files identical despite different names*

### Comparing `retrack-0.3.0/retrack/nodes/outputs.py` & `retrack-0.4.1/retrack/nodes/outputs.py`

 * *Files identical despite different names*

### Comparing `retrack-0.3.0/retrack/nodes/start.py` & `retrack-0.4.1/retrack/nodes/start.py`

 * *Files identical despite different names*

### Comparing `retrack-0.3.0/retrack/nodes/startswith.py` & `retrack-0.4.1/retrack/nodes/startswith.py`

 * *Files identical despite different names*

### Comparing `retrack-0.3.0/retrack/nodes/startswithany.py` & `retrack-0.4.1/retrack/nodes/startswithany.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 import pydantic
 
 from retrack.nodes.base import BaseNode, InputConnectionModel, OutputConnectionModel
+from retrack.utils import transformers
 
 ################################################
 # StartsWithAny Inputs Outputs
 ################################################
 
 
 class StartsWithAnyInputsModel(pydantic.BaseModel):
@@ -23,8 +24,9 @@
 
 
 class StartsWithAny(BaseNode):
     inputs: StartsWithAnyInputsModel
     outputs: StartsWithAnyOutputsModel
 
     def run(self, input_value: pd.Series, input_list: pd.Series) -> pd.Series:
-        return {"output_bool": input_value.str.startswith(tuple(input_list.to_list()))}
+        input_list = transformers.to_list(input_list)
+        return {"output_bool": input_value.str.startswith(tuple(input_list))}
```

### Comparing `retrack-0.3.0/retrack/utils/registry.py` & `retrack-0.4.1/retrack/utils/registry.py`

 * *Files identical despite different names*

### Comparing `retrack-0.3.0/setup.py` & `retrack-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['retrack',
  'retrack.engine',
- 'retrack.engine.validators',
  'retrack.nodes',
- 'retrack.utils']
+ 'retrack.utils',
+ 'retrack.validators']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['networkx>=3.0,<4.0', 'pandas>=1.5.2,<2.0.0', 'pydantic>=1.10.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'retrack',
-    'version': '0.3.0',
+    'version': '0.4.1',
     'description': 'A business rules engine',
-    'long_description': '<p align="center">\n  <a href="https://github.com/gabrielguarisa/retrack"><img src="https://raw.githubusercontent.com/gabrielguarisa/retrack/main/logo.png" alt="retrack"></a>\n</p>\n<p align="center">\n    <em>A business rules engine</em>\n</p>\n\n<div align="center">\n\n[![Package version](https://img.shields.io/pypi/v/retrack?color=%2334D058&label=pypi%20package)](https://pypi.org/project/retrack/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/gabrielguarisa/retrack/releases)\n[![License](https://img.shields.io/github/license/gabrielguarisa/retrack)](https://github.com/gabrielguarisa/retrack/blob/main/LICENSE)\n\n</div>\n\n\n## Installation\n\n```bash\npip install retrack\n```\n\n## Usage\n\n```python\nimport retrack\n\n# Parse the rule/model\nparser = retrack.Parser(rule)\n\n# Create a runner\nrunner = retrack.Runner(parser)\n\n# Run the rule/model passing the data\nrunner(data)\n```\n\nThe `Parser` class parses the rule/model and creates a graph of nodes. The `Runner` class runs the rule/model using the data passed to the runner. The `data` is a dictionary or a list of dictionaries containing the data that will be used to evaluate the conditions and execute the actions. To see wich data is required for the given rule/model, check the `runner.request_model` property that is a pydantic model used to validate the data.\n\n### Creating a rule/model\n\nA rule is a set of conditions and actions that are executed when the conditions are met. The conditions are evaluated using the data passed to the runner. The actions are executed when the conditions are met.\n\nEach rule is composed of many nodes. To see each node type, check the [nodes](https://github.com/gabrielguarisa/retrack/tree/main/retrack/nodes) folder.\n\nTo create a rule, you need to create a JSON file with the following structure:\n\n```json\n{\n  "nodes": {\n\t\t"node id": {\n\t\t\t"id": "node id",\n\t\t\t"data": {},\n\t\t\t"inputs": {},\n\t\t\t"outputs": {},\n\t\t\t"name": "node name",\n\t\t},\n    // ... more nodes\n  }\n}\n```\n\nThe `nodes` key is a dictionary of nodes. Each node has the following properties:\n\n- `id`: The node id. This is used to reference the node in the `inputs` and `outputs` properties.\n- `data`: The node data. This is used as a metadata for the node.\n- `inputs`: The node inputs. This is used to reference the node inputs.\n- `outputs`: The node outputs. This is used to reference the node outputs.\n- `name`: The node name. This is used to define the node type.\n\nThe `inputs` and `outputs` properties are dictionaries of node connections. Each connection has the following properties:\n\n- `node`: The node id that is connected to the current node.\n- `input`: The input name of the connection that is connected to the current node. This is only used in the `inputs` property.\n- `output`: The output name of the connection that is connected to the current node. This is only used in the `outputs` property.\n\nTo see some examples, check the [examples](https://github.com/gabrielguarisa/retrack/tree/main/examples) folder.\n\n### Creating a custom node\n\nTo create a custom node, you need to create a class that inherits from the `BaseNode` class. Each node is a pydantic model, so you can use pydantic features to create your custom node. To see the available features, check the [pydantic documentation](https://pydantic-docs.helpmanual.io/).\n\nTo create a custom node you need to define the inputs and outputs of the node. To do this, you need to define the `inputs` and `outputs` class attributes. Let\'s see an example of a custom node that has two inputs, sum them and return the result:\n\n```python\nimport retrack\nimport pydantic\nimport pandas as pd\nimport typing\n\n\nclass SumInputsModel(pydantic.BaseModel):\n    input_value_0: retrack.InputConnectionModel\n    input_value_1: retrack.InputConnectionModel\n\n\nclass SumOutputsModel(pydantic.BaseModel):\n    output_value: retrack.OutputConnectionModel\n\n\nclass SumNode(retrack.BaseNode):\n    inputs: SumInputsModel\n    outputs: SumOutputsModel\n\n    def run(self, input_value_0: pd.Series,\n        input_value_1: pd.Series,\n    ) -> typing.Dict[str, pd.Series]:\n        output_value = input_value_0.astype(float) + input_value_1.astype(float)\n        return {\n            "output_value": output_value,\n        }\n```\n\nAfter creating the custom node, you need to register it in the nodes registry and pass the registry to the parser. Let\'s see an example:\n\n```python\nimport retrack\n\n# Register the custom node\nretrack.component_registry.register_node("sum", SumNode)\n\n# Parse the rule/model\nparser = Parser(rule, component_registry=retrack.component_registry)\n```\n\n## Contributing\n\nContributions are welcome! Please read the [contributing guidelines](https://github.com/gabrielguarisa/retrack/tree/main/CONTRIBUTING.md) first.',
+    'long_description': '<p align="center">\n  <a href="https://github.com/gabrielguarisa/retrack"><img src="https://raw.githubusercontent.com/gabrielguarisa/retrack/main/logo.png" alt="retrack"></a>\n</p>\n<p align="center">\n    <em>A business rules engine</em>\n</p>\n\n<div align="center">\n\n[![Package version](https://img.shields.io/pypi/v/retrack?color=%2334D058&label=pypi%20package)](https://pypi.org/project/retrack/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/gabrielguarisa/retrack/releases)\n[![License](https://img.shields.io/github/license/gabrielguarisa/retrack)](https://github.com/gabrielguarisa/retrack/blob/main/LICENSE)\n\n</div>\n\n\n## Installation\n\n```bash\npip install retrack\n```\n\n## Usage\n\n```python\nimport retrack\n\n# Parse the rule/model\nparser = retrack.Parser(rule)\n\n# Create a runner\nrunner = retrack.Runner(parser)\n\n# Run the rule/model passing the data\nrunner.execute(data)\n```\n\nThe `Parser` class parses the rule/model and creates a graph of nodes. The `Runner` class runs the rule/model using the data passed to the runner. The `data` is a dictionary or a list of dictionaries containing the data that will be used to evaluate the conditions and execute the actions. To see wich data is required for the given rule/model, check the `runner.request_model` property that is a pydantic model used to validate the data.\n\n### Creating a rule/model\n\nA rule is a set of conditions and actions that are executed when the conditions are met. The conditions are evaluated using the data passed to the runner. The actions are executed when the conditions are met.\n\nEach rule is composed of many nodes. To see each node type, check the [nodes](https://github.com/gabrielguarisa/retrack/tree/main/retrack/nodes) folder.\n\nTo create a rule, you need to create a JSON file with the following structure:\n\n```json\n{\n  "nodes": {\n\t\t"node id": {\n\t\t\t"id": "node id",\n\t\t\t"data": {},\n\t\t\t"inputs": {},\n\t\t\t"outputs": {},\n\t\t\t"name": "node name",\n\t\t},\n    // ... more nodes\n  }\n}\n```\n\nThe `nodes` key is a dictionary of nodes. Each node has the following properties:\n\n- `id`: The node id. This is used to reference the node in the `inputs` and `outputs` properties.\n- `data`: The node data. This is used as a metadata for the node.\n- `inputs`: The node inputs. This is used to reference the node inputs.\n- `outputs`: The node outputs. This is used to reference the node outputs.\n- `name`: The node name. This is used to define the node type.\n\nThe `inputs` and `outputs` properties are dictionaries of node connections. Each connection has the following properties:\n\n- `node`: The node id that is connected to the current node.\n- `input`: The input name of the connection that is connected to the current node. This is only used in the `inputs` property.\n- `output`: The output name of the connection that is connected to the current node. This is only used in the `outputs` property.\n\nTo see some examples, check the [examples](https://github.com/gabrielguarisa/retrack/tree/main/examples) folder.\n\n### Creating a custom node\n\nTo create a custom node, you need to create a class that inherits from the `BaseNode` class. Each node is a pydantic model, so you can use pydantic features to create your custom node. To see the available features, check the [pydantic documentation](https://pydantic-docs.helpmanual.io/).\n\nTo create a custom node you need to define the inputs and outputs of the node. To do this, you need to define the `inputs` and `outputs` class attributes. Let\'s see an example of a custom node that has two inputs, sum them and return the result:\n\n```python\nimport retrack\nimport pydantic\nimport pandas as pd\nimport typing\n\n\nclass SumInputsModel(pydantic.BaseModel):\n    input_value_0: retrack.InputConnectionModel\n    input_value_1: retrack.InputConnectionModel\n\n\nclass SumOutputsModel(pydantic.BaseModel):\n    output_value: retrack.OutputConnectionModel\n\n\nclass SumNode(retrack.BaseNode):\n    inputs: SumInputsModel\n    outputs: SumOutputsModel\n\n    def run(self, input_value_0: pd.Series,\n        input_value_1: pd.Series,\n    ) -> typing.Dict[str, pd.Series]:\n        output_value = input_value_0.astype(float) + input_value_1.astype(float)\n        return {\n            "output_value": output_value,\n        }\n```\n\nAfter creating the custom node, you need to register it in the nodes registry and pass the registry to the parser. Let\'s see an example:\n\n```python\nimport retrack\n\n# Register the custom node\nretrack.component_registry.register_node("sum", SumNode)\n\n# Parse the rule/model\nparser = Parser(rule, component_registry=retrack.component_registry)\n```\n\n## Contributing\n\nContributions are welcome! Please read the [contributing guidelines](https://github.com/gabrielguarisa/retrack/tree/main/CONTRIBUTING.md) first.',
     'author': 'Gabriel Guarisa',
     'author_email': 'gabrielguarisa@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/gabrielguarisa/retrack',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['retrack',
-'retrack.engine', 'retrack.engine.validators', 'retrack.nodes',
-'retrack.utils'] package_data = \ {'': ['*']} install_requires = \
-['networkx>=3.0,<4.0', 'pandas>=1.5.2,<2.0.0', 'pydantic>=1.10.4,<2.0.0']
-setup_kwargs = { 'name': 'retrack', 'version': '0.3.0', 'description': 'A
-business rules engine', 'long_description': '
+'retrack.engine', 'retrack.nodes', 'retrack.utils', 'retrack.validators']
+package_data = \ {'': ['*']} install_requires = \ ['networkx>=3.0,<4.0',
+'pandas>=1.5.2,<2.0.0', 'pydantic>=1.10.4,<2.0.0'] setup_kwargs = { 'name':
+'retrack', 'version': '0.4.1', 'description': 'A business rules engine',
+'long_description': '
                                 \n [retrack]\n
 \n
                          \n A business rules engine\n
 \n\n
             \n\n[![Package version](https://img.shields.io/pypi/v/
    retrack?color=%2334D058&label=pypi%20package)](https://pypi.org/project/
   retrack/)\n[![Code style: black](https://img.shields.io/badge/code%20style-
@@ -15,52 +15,53 @@
    /img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-
  e10079.svg)](https://github.com/gabrielguarisa/retrack/releases)\n[![License]
    (https://img.shields.io/github/license/gabrielguarisa/retrack)](https://
            github.com/gabrielguarisa/retrack/blob/main/LICENSE)\n\n
 \n\n\n## Installation\n\n```bash\npip install retrack\n```\n\n##
 Usage\n\n```python\nimport retrack\n\n# Parse the rule/model\nparser =
 retrack.Parser(rule)\n\n# Create a runner\nrunner = retrack.Runner(parser)\n\n#
-Run the rule/model passing the data\nrunner(data)\n```\n\nThe `Parser` class
-parses the rule/model and creates a graph of nodes. The `Runner` class runs the
-rule/model using the data passed to the runner. The `data` is a dictionary or a
-list of dictionaries containing the data that will be used to evaluate the
-conditions and execute the actions. To see wich data is required for the given
-rule/model, check the `runner.request_model` property that is a pydantic model
-used to validate the data.\n\n### Creating a rule/model\n\nA rule is a set of
-conditions and actions that are executed when the conditions are met. The
-conditions are evaluated using the data passed to the runner. The actions are
-executed when the conditions are met.\n\nEach rule is composed of many nodes.
-To see each node type, check the [nodes](https://github.com/gabrielguarisa/
-retrack/tree/main/retrack/nodes) folder.\n\nTo create a rule, you need to
-create a JSON file with the following structure:\n\n```json\n{\n "nodes":
-{\n\t\t"node id": {\n\t\t\t"id": "node id",\n\t\t\t"data": {},\n\t\t\t"inputs":
-{},\n\t\t\t"outputs": {},\n\t\t\t"name": "node name",\n\t\t},\n // ... more
-nodes\n }\n}\n```\n\nThe `nodes` key is a dictionary of nodes. Each node has
-the following properties:\n\n- `id`: The node id. This is used to reference the
-node in the `inputs` and `outputs` properties.\n- `data`: The node data. This
-is used as a metadata for the node.\n- `inputs`: The node inputs. This is used
-to reference the node inputs.\n- `outputs`: The node outputs. This is used to
-reference the node outputs.\n- `name`: The node name. This is used to define
-the node type.\n\nThe `inputs` and `outputs` properties are dictionaries of
-node connections. Each connection has the following properties:\n\n- `node`:
-The node id that is connected to the current node.\n- `input`: The input name
-of the connection that is connected to the current node. This is only used in
-the `inputs` property.\n- `output`: The output name of the connection that is
-connected to the current node. This is only used in the `outputs`
-property.\n\nTo see some examples, check the [examples](https://github.com/
-gabrielguarisa/retrack/tree/main/examples) folder.\n\n### Creating a custom
-node\n\nTo create a custom node, you need to create a class that inherits from
-the `BaseNode` class. Each node is a pydantic model, so you can use pydantic
-features to create your custom node. To see the available features, check the
-[pydantic documentation](https://pydantic-docs.helpmanual.io/).\n\nTo create a
-custom node you need to define the inputs and outputs of the node. To do this,
-you need to define the `inputs` and `outputs` class attributes. Let\'s see an
-example of a custom node that has two inputs, sum them and return the result:
-\n\n```python\nimport retrack\nimport pydantic\nimport pandas as pd\nimport
-typing\n\n\nclass SumInputsModel(pydantic.BaseModel):\n input_value_0:
+Run the rule/model passing the data\nrunner.execute(data)\n```\n\nThe `Parser`
+class parses the rule/model and creates a graph of nodes. The `Runner` class
+runs the rule/model using the data passed to the runner. The `data` is a
+dictionary or a list of dictionaries containing the data that will be used to
+evaluate the conditions and execute the actions. To see wich data is required
+for the given rule/model, check the `runner.request_model` property that is a
+pydantic model used to validate the data.\n\n### Creating a rule/model\n\nA
+rule is a set of conditions and actions that are executed when the conditions
+are met. The conditions are evaluated using the data passed to the runner. The
+actions are executed when the conditions are met.\n\nEach rule is composed of
+many nodes. To see each node type, check the [nodes](https://github.com/
+gabrielguarisa/retrack/tree/main/retrack/nodes) folder.\n\nTo create a rule,
+you need to create a JSON file with the following structure:\n\n```json\n{\n
+"nodes": {\n\t\t"node id": {\n\t\t\t"id": "node id",\n\t\t\t"data":
+{},\n\t\t\t"inputs": {},\n\t\t\t"outputs": {},\n\t\t\t"name": "node
+name",\n\t\t},\n // ... more nodes\n }\n}\n```\n\nThe `nodes` key is a
+dictionary of nodes. Each node has the following properties:\n\n- `id`: The
+node id. This is used to reference the node in the `inputs` and `outputs`
+properties.\n- `data`: The node data. This is used as a metadata for the
+node.\n- `inputs`: The node inputs. This is used to reference the node
+inputs.\n- `outputs`: The node outputs. This is used to reference the node
+outputs.\n- `name`: The node name. This is used to define the node type.\n\nThe
+`inputs` and `outputs` properties are dictionaries of node connections. Each
+connection has the following properties:\n\n- `node`: The node id that is
+connected to the current node.\n- `input`: The input name of the connection
+that is connected to the current node. This is only used in the `inputs`
+property.\n- `output`: The output name of the connection that is connected to
+the current node. This is only used in the `outputs` property.\n\nTo see some
+examples, check the [examples](https://github.com/gabrielguarisa/retrack/tree/
+main/examples) folder.\n\n### Creating a custom node\n\nTo create a custom
+node, you need to create a class that inherits from the `BaseNode` class. Each
+node is a pydantic model, so you can use pydantic features to create your
+custom node. To see the available features, check the [pydantic documentation]
+(https://pydantic-docs.helpmanual.io/).\n\nTo create a custom node you need to
+define the inputs and outputs of the node. To do this, you need to define the
+`inputs` and `outputs` class attributes. Let\'s see an example of a custom node
+that has two inputs, sum them and return the result:\n\n```python\nimport
+retrack\nimport pydantic\nimport pandas as pd\nimport typing\n\n\nclass
+SumInputsModel(pydantic.BaseModel):\n input_value_0:
 retrack.InputConnectionModel\n input_value_1:
 retrack.InputConnectionModel\n\n\nclass SumOutputsModel(pydantic.BaseModel):\n
 output_value: retrack.OutputConnectionModel\n\n\nclass SumNode
 (retrack.BaseNode):\n inputs: SumInputsModel\n outputs: SumOutputsModel\n\n def
 run(self, input_value_0: pd.Series,\n input_value_1: pd.Series,\n ) -
 > typing.Dict[str, pd.Series]:\n output_value = input_value_0.astype(float) +
 input_value_1.astype(float)\n return {\n "output_value": output_value,\n
```

### Comparing `retrack-0.3.0/PKG-INFO` & `retrack-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retrack
-Version: 0.3.0
+Version: 0.4.1
 Summary: A business rules engine
 Home-page: https://github.com/gabrielguarisa/retrack
 License: MIT
 Keywords: rules,models,business,node,graph
 Author: Gabriel Guarisa
 Author-email: gabrielguarisa@gmail.com
 Requires-Python: >=3.8.16,<4.0.0
@@ -49,15 +49,15 @@
 # Parse the rule/model
 parser = retrack.Parser(rule)
 
 # Create a runner
 runner = retrack.Runner(parser)
 
 # Run the rule/model passing the data
-runner(data)
+runner.execute(data)
 ```
 
 The `Parser` class parses the rule/model and creates a graph of nodes. The `Runner` class runs the rule/model using the data passed to the runner. The `data` is a dictionary or a list of dictionaries containing the data that will be used to evaluate the conditions and execute the actions. To see wich data is required for the given rule/model, check the `runner.request_model` property that is a pydantic model used to validate the data.
 
 ### Creating a rule/model
 
 A rule is a set of conditions and actions that are executed when the conditions are met. The conditions are evaluated using the data passed to the runner. The actions are executed when the conditions are met.
```

