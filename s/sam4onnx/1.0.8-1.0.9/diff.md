# Comparing `tmp/sam4onnx-1.0.8.tar.gz` & `tmp/sam4onnx-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam4onnx-1.0.8.tar", last modified: Tue Jun  7 23:20:02 2022, max compression
+gzip compressed data, was "sam4onnx-1.0.9.tar", last modified: Sun Jul 17 14:41:34 2022, max compression
```

## Comparing `sam4onnx-1.0.8.tar` & `sam4onnx-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 23:20:02.537935 sam4onnx-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-06-07 23:19:52.000000 sam4onnx-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9717 2022-06-07 23:20:02.537935 sam4onnx-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9263 2022-06-07 23:19:52.000000 sam4onnx-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 23:20:02.537935 sam4onnx-1.0.8/sam4onnx/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-06-07 23:19:52.000000 sam4onnx-1.0.8/sam4onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-07 23:19:52.000000 sam4onnx-1.0.8/sam4onnx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16443 2022-06-07 23:19:52.000000 sam4onnx-1.0.8/sam4onnx/onnx_attr_const_modify.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 23:20:02.537935 sam4onnx-1.0.8/sam4onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9717 2022-06-07 23:20:02.000000 sam4onnx-1.0.8/sam4onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-06-07 23:20:02.000000 sam4onnx-1.0.8/sam4onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 23:20:02.000000 sam4onnx-1.0.8/sam4onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-06-07 23:20:02.000000 sam4onnx-1.0.8/sam4onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-07 23:20:02.000000 sam4onnx-1.0.8/sam4onnx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 23:20:02.541935 sam4onnx-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-06-07 23:19:52.000000 sam4onnx-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 14:41:34.180324 sam4onnx-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-07-17 14:41:27.000000 sam4onnx-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     9758 2022-07-17 14:41:34.180324 sam4onnx-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9304 2022-07-17 14:41:27.000000 sam4onnx-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 14:41:34.180324 sam4onnx-1.0.9/sam4onnx/
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-07-17 14:41:27.000000 sam4onnx-1.0.9/sam4onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-07-17 14:41:27.000000 sam4onnx-1.0.9/sam4onnx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19733 2022-07-17 14:41:27.000000 sam4onnx-1.0.9/sam4onnx/onnx_attr_const_modify.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-17 14:41:34.180324 sam4onnx-1.0.9/sam4onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9758 2022-07-17 14:41:34.000000 sam4onnx-1.0.9/sam4onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-07-17 14:41:34.000000 sam4onnx-1.0.9/sam4onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-17 14:41:34.000000 sam4onnx-1.0.9/sam4onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-07-17 14:41:34.000000 sam4onnx-1.0.9/sam4onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-17 14:41:34.000000 sam4onnx-1.0.9/sam4onnx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-17 14:41:34.180324 sam4onnx-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-07-17 14:41:27.000000 sam4onnx-1.0.9/setup.py
```

### Comparing `sam4onnx-1.0.8/LICENSE` & `sam4onnx-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sam4onnx-1.0.8/PKG-INFO` & `sam4onnx-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sam4onnx
-Version: 1.0.8
+Version: 1.0.9
 Summary: A very simple tool to rewrite parameters such as attributes and constants for OPs in ONNX models. Simple Attribute and Constant Modifier for ONNX.
 Home-page: https://github.com/PINTO0309/sam4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
@@ -224,37 +224,39 @@
 ```
 
 ## 6. Sample
 ### 6-1. Transpose - update **`perm`**
 ![image](https://user-images.githubusercontent.com/33194443/163525107-f355bc2e-66d6-4a8e-bc54-2fcfc36107e8.png)
 ```bash
 $ sam4onnx \
---op_name Transpose_17 \
 --input_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt.onnx \
 --output_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt_mod.onnx \
+--op_name Transpose_17 \
 --attributes perm int64 [0,1]
 ```
 ![image](https://user-images.githubusercontent.com/33194443/163525149-64da02af-754f-40e5-916a-20f581ff0034.png)
 
 ### 6-2. Mul - update **`Constant (170)`** - From: **`2`**, To: **`1`**
 ![image](https://user-images.githubusercontent.com/33194443/163560084-9541140a-6368-4f4f-aced-ebdf7bf43c70.png)
 ```bash
 $ sam4onnx \
 --input_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt.onnx \
 --output_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt_mod.onnx \
+--op_name Mul_5 \
 --input_constants 170 float32 1
 ```
 ![image](https://user-images.githubusercontent.com/33194443/163560202-15584279-58d7-4c96-b1c3-7366d165ba21.png)
 
 ### 6-3. Reshape - update **`Constant (241)`** - From: **`[-1]`**, To: **`[1]`**
 ![image](https://user-images.githubusercontent.com/33194443/163560715-21e0ab88-7859-4b52-adb4-c4d902525ac3.png)
 ```bash
 $ sam4onnx \
 --input_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt.onnx \
 --output_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt_mod.onnx \
+--op_name Reshape_34 \
 --input_constants 241 int64 [1]
 ```
 ![image](https://user-images.githubusercontent.com/33194443/163561022-2e3dae84-7c6e-4ed0-9644-2248f91ab2ab.png)
 
 ## 7. Issues
 https://github.com/PINTO0309/simple-onnx-processing-tools/issues
```

### Comparing `sam4onnx-1.0.8/README.md` & `sam4onnx-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -210,36 +210,38 @@
 ```
 
 ## 6. Sample
 ### 6-1. Transpose - update **`perm`**
 ![image](https://user-images.githubusercontent.com/33194443/163525107-f355bc2e-66d6-4a8e-bc54-2fcfc36107e8.png)
 ```bash
 $ sam4onnx \
---op_name Transpose_17 \
 --input_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt.onnx \
 --output_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt_mod.onnx \
+--op_name Transpose_17 \
 --attributes perm int64 [0,1]
 ```
 ![image](https://user-images.githubusercontent.com/33194443/163525149-64da02af-754f-40e5-916a-20f581ff0034.png)
 
 ### 6-2. Mul - update **`Constant (170)`** - From: **`2`**, To: **`1`**
 ![image](https://user-images.githubusercontent.com/33194443/163560084-9541140a-6368-4f4f-aced-ebdf7bf43c70.png)
 ```bash
 $ sam4onnx \
 --input_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt.onnx \
 --output_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt_mod.onnx \
+--op_name Mul_5 \
 --input_constants 170 float32 1
 ```
 ![image](https://user-images.githubusercontent.com/33194443/163560202-15584279-58d7-4c96-b1c3-7366d165ba21.png)
 
 ### 6-3. Reshape - update **`Constant (241)`** - From: **`[-1]`**, To: **`[1]`**
 ![image](https://user-images.githubusercontent.com/33194443/163560715-21e0ab88-7859-4b52-adb4-c4d902525ac3.png)
 ```bash
 $ sam4onnx \
 --input_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt.onnx \
 --output_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt_mod.onnx \
+--op_name Reshape_34 \
 --input_constants 241 int64 [1]
 ```
 ![image](https://user-images.githubusercontent.com/33194443/163561022-2e3dae84-7c6e-4ed0-9644-2248f91ab2ab.png)
 
 ## 7. Issues
 https://github.com/PINTO0309/simple-onnx-processing-tools/issues
```

### Comparing `sam4onnx-1.0.8/sam4onnx/onnx_attr_const_modify.py` & `sam4onnx-1.0.9/sam4onnx/onnx_attr_const_modify.py`

 * *Files 15% similar despite different names*

```diff
@@ -63,48 +63,77 @@
     'complex64': np.complex64,
     'complex128': np.complex128,
 }
 
 
 def __search_op_constant_from_input_constant_name(
     graph: onnx_graphsurgeon.Graph,
-    input_constant_name: str
+    input_constant_name: str,
+    op_name: str,
 ):
     """
     Parameters
     ----------
     graph: onnx_graphsurgeon.Graph
         Graphs to be explored.
 
     input_constant_name: str
         input_constant_name of the search target.
 
+    op_name: str
+        op_name of the search target.
+
     Returns
     -------
-    input_constant_to_change:
+    input_constant_to_change: gs.Node
         constant found.
         If not found, return an None.
+
+    new_constant_name: str
+        A new name to be given only to the constant
+        with the corresponding op_name if there are
+        multiple constants with the same name in the model.
     """
     # Search for variable matching variable_name
     input_constant_to_change = None
-    for graph_node in graph.nodes:
+    graph_nodes = None
+    if op_name:
+        graph_nodes = [graph_node for graph_node in graph.nodes if graph_node.name == op_name]
+    else:
+        graph_nodes = graph.nodes
+
+    for graph_node in graph_nodes:
         for input in graph_node.inputs:
             if isinstance(input, Constant) and input.name == input_constant_name:
                 input_constant_to_change = input
                 break
             elif isinstance(input, Variable) and input.name == input_constant_name:
                 if input.inputs[0].op == 'Constant':
                     input_constant_to_change = input.inputs[0]
                     break
         else:
             continue
         break
 
+    # If the same input_constant_name constant exists in the model,
+    # a new name is given only to the constant with the corresponding op_name.
+    new_constant_name = None
+    if input_constant_to_change is not None and op_name:
+        num_of_const_with_the_same_name = sum(
+            [
+                1 for graph_node in graph.nodes \
+                    for input in graph_node.inputs \
+                        if input.name == input_constant_name
+            ]
+        )
+        if num_of_const_with_the_same_name > 1:
+            new_constant_name = f'{input_constant_name}_mod_{num_of_const_with_the_same_name}'
+
     # Return variable
-    return input_constant_to_change
+    return input_constant_to_change, new_constant_name
 
 
 def modify(
     input_onnx_file_path: Optional[str] = '',
     output_onnx_file_path: Optional[str] = '',
     onnx_graph: Optional[onnx.ModelProto] = None,
     op_name: Optional[str] = '',
@@ -251,22 +280,65 @@
             Variable (170): (shape=None, dtype=None)
         ]
     Attributes: OrderedDict([('value', Constant (): (shape=[], dtype=<class 'numpy.float32'>)
     LazyValues (shape=[], dtype=float32))])
     """
     if input_constants:
         for input_constant_name, input_constant_value in input_constants.items():
-            constant = __search_op_constant_from_input_constant_name(graph, input_constant_name)
-            if hasattr(constant, "attrs"):
-                constant.attrs['value'] = gs.Constant(
-                    name='',
-                    values=input_constant_value
-                )
+            constant, new_constant_name = __search_op_constant_from_input_constant_name(
+                graph,
+                input_constant_name,
+                op_name,
+            )
+            if constant is not None:
+                if hasattr(constant, "attrs"):
+                    constant.attrs['value'] = gs.Constant(
+                        name='' if new_constant_name is None else new_constant_name,
+                        values=input_constant_value
+                    )
+                else:
+                    if new_constant_name is None:
+                        constant.values = input_constant_value
+                    else:
+                        if op_name:
+                            new_constant = gs.Constant(
+                                name=new_constant_name,
+                                values=input_constant_value
+                            )
+                            graph_nodes = [graph_node for graph_node in graph.nodes if graph_node.name == op_name]
+                            target_node = None
+                            target_input_idx = -1
+                            for graph_node in graph_nodes:
+                                for idx, graph_node_input in enumerate(graph_node.inputs):
+                                    if graph_node_input.name == input_constant_name:
+                                        target_node = graph_node
+                                        target_input_idx = idx
+                                        break
+                                else:
+                                    continue
+                                break
+                            if target_node and target_input_idx > -1:
+                                target_node.inputs[target_input_idx] = new_constant
+                            else:
+                                pass
+                        else:
+                            constant.values = input_constant_value
+
             else:
-                constant.values = input_constant_value
+                if not non_verbose:
+                    if op_name:
+                        print(
+                            f'{Color.YELLOW}WARNING:{Color.RESET} '+
+                            f'op_name: {op_name}, input_constant_name: {input_constant_name} did not exist in the model.'
+                        )
+                    else:
+                        print(
+                            f'{Color.YELLOW}WARNING:{Color.RESET} '+
+                            f'input_constant_name: {input_constant_name} did not exist in the model.'
+                        )
 
     # Cleanup
     graph.cleanup().toposort()
     modified_graph = gs.export_onnx(graph)
 
     # Optimize
     new_model = None
@@ -432,15 +504,15 @@
     # input constants
     # input_constant = [constant_name, numpy.dtype, value]
     input_constants_tmp = None
     if input_constants:
         input_constants_tmp = {}
         for input_constant in input_constants:
             # Search for OPs corresponding to the name of input_constant
-            constant = __search_op_constant_from_input_constant_name(graph, input_constant[0])
+            constant, _ = __search_op_constant_from_input_constant_name(graph, input_constant[0], op_name)
 
             # None: Not found
             if not constant:
                 print(
                     f'{Color.RED}ERROR:{Color.RESET} '+
                     f'input_constants not found. input_constant: {input_constant}'
                 )
```

### Comparing `sam4onnx-1.0.8/sam4onnx.egg-info/PKG-INFO` & `sam4onnx-1.0.9/sam4onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sam4onnx
-Version: 1.0.8
+Version: 1.0.9
 Summary: A very simple tool to rewrite parameters such as attributes and constants for OPs in ONNX models. Simple Attribute and Constant Modifier for ONNX.
 Home-page: https://github.com/PINTO0309/sam4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
@@ -224,37 +224,39 @@
 ```
 
 ## 6. Sample
 ### 6-1. Transpose - update **`perm`**
 ![image](https://user-images.githubusercontent.com/33194443/163525107-f355bc2e-66d6-4a8e-bc54-2fcfc36107e8.png)
 ```bash
 $ sam4onnx \
---op_name Transpose_17 \
 --input_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt.onnx \
 --output_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt_mod.onnx \
+--op_name Transpose_17 \
 --attributes perm int64 [0,1]
 ```
 ![image](https://user-images.githubusercontent.com/33194443/163525149-64da02af-754f-40e5-916a-20f581ff0034.png)
 
 ### 6-2. Mul - update **`Constant (170)`** - From: **`2`**, To: **`1`**
 ![image](https://user-images.githubusercontent.com/33194443/163560084-9541140a-6368-4f4f-aced-ebdf7bf43c70.png)
 ```bash
 $ sam4onnx \
 --input_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt.onnx \
 --output_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt_mod.onnx \
+--op_name Mul_5 \
 --input_constants 170 float32 1
 ```
 ![image](https://user-images.githubusercontent.com/33194443/163560202-15584279-58d7-4c96-b1c3-7366d165ba21.png)
 
 ### 6-3. Reshape - update **`Constant (241)`** - From: **`[-1]`**, To: **`[1]`**
 ![image](https://user-images.githubusercontent.com/33194443/163560715-21e0ab88-7859-4b52-adb4-c4d902525ac3.png)
 ```bash
 $ sam4onnx \
 --input_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt.onnx \
 --output_onnx_file_path hitnet_sf_finalpass_720x1280_nonopt_mod.onnx \
+--op_name Reshape_34 \
 --input_constants 241 int64 [1]
 ```
 ![image](https://user-images.githubusercontent.com/33194443/163561022-2e3dae84-7c6e-4ed0-9644-2248f91ab2ab.png)
 
 ## 7. Issues
 https://github.com/PINTO0309/simple-onnx-processing-tools/issues
```

### Comparing `sam4onnx-1.0.8/setup.py` & `sam4onnx-1.0.9/setup.py`

 * *Files identical despite different names*

