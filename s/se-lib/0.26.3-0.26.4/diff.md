# Comparing `tmp/se_lib-0.26.3.tar.gz` & `tmp/se_lib-0.26.4.tar.gz`

## Comparing `se_lib-0.26.3.tar` & `se_lib-0.26.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.26.3/.DS_Store
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.26.3/.gitattributes
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.26.3/selib/.DS_Store
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 se_lib-0.26.3/selib/__init__.py
--rw-r--r--   0        0        0    74813 2020-02-02 00:00:00.000000 se_lib-0.26.3/selib/selib.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.26.3/LICENSE
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 se_lib-0.26.3/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 se_lib-0.26.3/pyproject.toml
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 se_lib-0.26.3/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.26.4/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.26.4/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.26.4/selib/.DS_Store
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 se_lib-0.26.4/selib/__init__.py
+-rw-r--r--   0        0        0    74890 2020-02-02 00:00:00.000000 se_lib-0.26.4/selib/selib.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.26.4/LICENSE
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 se_lib-0.26.4/README.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 se_lib-0.26.4/pyproject.toml
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 se_lib-0.26.4/PKG-INFO
```

### Comparing `se_lib-0.26.3/.DS_Store` & `se_lib-0.26.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.3/selib/.DS_Store` & `se_lib-0.26.4/selib/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.3/selib/selib.py` & `se_lib-0.26.4/selib/selib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-se-lib Version .26.3
+se-lib Version .26.4
 
 Copyright (c) 2022-2023 Ray Madachy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
@@ -1684,26 +1684,31 @@
 
 
 def init_de_model():
     """
     Instantiates a discrete event model for simulation
     """
     global env, entity_num, entity_data, run_specs, model_type
+    network.clear()
+    run_specs.clear()
+    entity_num = 0
+    entity_data.clear()
+    
     # create simulation environment
     env = simpy.Environment()
     model_type = "discrete"
 
 def add_server(name, connections, service_time, capacity=1):
     """
     Add a server to a discrete event model. 
 
     Parameters
     ----------
     name: string
-    	A name for server.
+    	A name for the server.
     connections: dictionary
     	A dictionary of the node connections after the server.  The node names are the keys and the values are the relative probabilities of traversing the connection.
     capacity: integer
     	The number of resource usage slots in the server
     """
     network[name] = {
         'type': 'server',
@@ -1717,19 +1722,19 @@
 def add_delay(name, connections, delay_time):
     """
     Add a delay to a discrete event model. 
 
     Parameters
     ----------
     name: string
-    	A name for delay.
+    	A name for the delay.
     connections: dictionary
     	A dictionary of the node connections after the delay.  The node names are the keys and the values are the relative probabilities of traversing the connections.
-    delay_time: the time delay for entities to traverse.  May be a constant or random function.
-    	The number of resource usage slots in the server
+    delay_time: float
+    	The time delay for entities to traverse.  May be a constant or random function.
     """
     network[name] = {
         'type': 'delay',
         'connections': connections,
         'delay_time': delay_time,
     }
 
@@ -1737,19 +1742,21 @@
 def add_source(name, connections, num_entities, interarrival_time):
     """
     Add a source node to a discrete event model to generate entities. 
 
     Parameters
     ----------
     name: string
-    	A name for the source.
+    	A name for the the source.
     connections: dictionary
     	A dictionary of the node connections after the source.  The node names are the keys and the values are the relative probabilities of traversing the connections.
-    interarrival_time: the time between entity arrrivals into the system.  May be a constant or random function.
-    	The number of resource usage slots in the server
+    num_entities: integer
+    	Number of entities to be generated.
+    interarrival_time: float
+    	The time between entity arrrivals into the system.  May be a constant or random function.
     """
 
     network[name] = {
         'type': 'source',
         'connections': connections,
         'interarrival_time': interarrival_time,
     }
@@ -1890,11 +1897,8 @@
             graph.edge(
                 node_name,
                 connection,
             )
     if filename is not None:
         graph.render(
         )  # render and save file, clean up temporary dot source file (no extension) after successful rendering with (cleanup=True) doesn't work on windows "permission denied"
-    return graph
-
-	
-	
+    return graph
```

### Comparing `se_lib-0.26.3/LICENSE` & `se_lib-0.26.4/LICENSE`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.3/README.md` & `se_lib-0.26.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Systems Engineering Library (se-lib)
-Version .26.3
+Version .26.4
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `se_lib-0.26.3/pyproject.toml` & `se_lib-0.26.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "se-lib"
-version = "0.26.3"
+version = "0.26.4"
 authors = [
   { name="se-lib Development Team", email="info@se-lib.org" },
 ]
 description = "Systems Engineering Library (se-lib)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `se_lib-0.26.3/PKG-INFO` & `se_lib-0.26.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: se-lib
-Version: 0.26.3
+Version: 0.26.4
 Summary: Systems Engineering Library (se-lib)
 Project-URL: Homepage, http://se-lib.org
 Author-email: se-lib Development Team <info@se-lib.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: netcdf4
 Requires-Dist: pandas
 Requires-Dist: pysd
 Description-Content-Type: text/markdown
 
 # Systems Engineering Library (se-lib)
-Version .26.3
+Version .26.4
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

