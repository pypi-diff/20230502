# Comparing `tmp/graphdisplay-0.1.1.tar.gz` & `tmp/graphdisplay-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdisplay-0.1.1.tar", last modified: Tue May  2 19:43:57 2023, max compression
+gzip compressed data, was "graphdisplay-0.1.2.tar", last modified: Tue May  2 21:05:13 2023, max compression
```

## Comparing `graphdisplay-0.1.1.tar` & `graphdisplay-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 19:43:57.591688 graphdisplay-0.1.1/
--rw-rw-rw-   0        0        0     1051 2023-05-02 19:43:57.590688 graphdisplay-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-05-02 18:43:09.000000 graphdisplay-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 19:43:57.582722 graphdisplay-0.1.1/graphdisplay/
--rw-rw-rw-   0        0        0       34 2023-04-24 21:08:03.000000 graphdisplay-0.1.1/graphdisplay/__init__.py
--rw-rw-rw-   0        0        0     4920 2023-05-02 18:37:35.000000 graphdisplay-0.1.1/graphdisplay/graph.py
--rw-rw-rw-   0        0        0     9863 2023-05-02 18:40:09.000000 graphdisplay-0.1.1/graphdisplay/graphdisplay.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:43:57.589691 graphdisplay-0.1.1/graphdisplay.egg-info/
--rw-rw-rw-   0        0        0     1051 2023-05-02 19:43:57.000000 graphdisplay-0.1.1/graphdisplay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-05-02 19:43:57.000000 graphdisplay-0.1.1/graphdisplay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 19:43:57.000000 graphdisplay-0.1.1/graphdisplay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 19:43:57.000000 graphdisplay-0.1.1/graphdisplay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 19:43:57.591688 graphdisplay-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1842 2023-05-02 19:42:24.000000 graphdisplay-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:05:13.439128 graphdisplay-0.1.2/
+-rw-rw-rw-   0        0        0     1051 2023-05-02 21:05:13.438130 graphdisplay-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-05-02 18:43:09.000000 graphdisplay-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 21:05:13.420178 graphdisplay-0.1.2/graphdisplay/
+-rw-rw-rw-   0        0        0       34 2023-04-24 21:08:03.000000 graphdisplay-0.1.2/graphdisplay/__init__.py
+-rw-rw-rw-   0        0        0     4927 2023-05-02 21:02:58.000000 graphdisplay-0.1.2/graphdisplay/graph.py
+-rw-rw-rw-   0        0        0    10026 2023-05-02 21:02:40.000000 graphdisplay-0.1.2/graphdisplay/graphdisplay.py
+drwxrwxrwx   0        0        0        0 2023-05-02 21:05:13.437157 graphdisplay-0.1.2/graphdisplay.egg-info/
+-rw-rw-rw-   0        0        0     1051 2023-05-02 21:05:13.000000 graphdisplay-0.1.2/graphdisplay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-02 21:05:13.000000 graphdisplay-0.1.2/graphdisplay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 21:05:13.000000 graphdisplay-0.1.2/graphdisplay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 21:05:13.000000 graphdisplay-0.1.2/graphdisplay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 21:05:13.439128 graphdisplay-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1842 2023-05-02 21:02:40.000000 graphdisplay-0.1.2/setup.py
```

### Comparing `graphdisplay-0.1.1/PKG-INFO` & `graphdisplay-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.1.1
+Version: 0.1.2
 Summary: Librería para representar visualmente grafos de tipo diccionario
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `graphdisplay-0.1.1/graphdisplay/graph.py` & `graphdisplay-0.1.2/graphdisplay/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                     break
         return lst_origins
 
 
 if __name__ == '__main__':
 
     labels = ['A', 'B', 'C', 'D', 'E']
-    g = Graph(labels)
+    g = Graph(labels, False)
 
     # Now, we add the edges
     g.add_edge('A', 'C', 12)  # A->(12)C
     g.add_edge('A', 'D', 60)  # A->(60)D
     g.add_edge('B', 'A', 10)  # B->(10)A
     g.add_edge('C', 'B', 20)  # C->(20)B
     g.add_edge('C', 'D', 32)  # C->(32)D
```

### Comparing `graphdisplay-0.1.1/graphdisplay/graphdisplay.py` & `graphdisplay-0.1.2/graphdisplay/graphdisplay.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,25 +64,29 @@
                     if node.id == str(adj.vertex):
                         self.edges.append(Edge(self.canvas, self.nodes[i], node, adj.weight))
                         node.asociated_edges_IN.append(self.edges[-1])
                         self.nodes[i].asociated_edges_OUT.append(self.edges[-1])
             i += 1
 
         # Display the edges
-        for edge in self.edges:
-            edge_start_node = edge.start_node
-            edge_end_node = edge.end_node
-            found = False
-            for i in edge_start_node.asociated_edges_IN:
-                if i.start_node == edge_end_node:
-                    found = True
-                    edge.overlaped = True
+        if self.graph._directed:
+            for edge in self.edges:
+                edge_start_node = edge.start_node
+                edge_end_node = edge.end_node
+                found = False
+                for i in edge_start_node.asociated_edges_IN:
+                    if i.start_node == edge_end_node:
+                        found = True
+                        edge.overlaped = True
+                        edge.show()
+                        break
+                if not found:
                     edge.show()
-                    break
-            if not found:
+        else:
+            for edge in self.edges:
                 edge.show()
 
         self.canvas.tag_bind("movil", "<ButtonPress-1>", self.on_press)
         self.canvas.tag_bind("movil", "<Button1-Motion>", self.move)
         self.selected_node = None
 
         """label =  tk.Label(self.canvas, text="Ventana de prueba", background="Red")
```

### Comparing `graphdisplay-0.1.1/graphdisplay.egg-info/PKG-INFO` & `graphdisplay-0.1.2/graphdisplay.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.1.1
+Version: 0.1.2
 Summary: Librería para representar visualmente grafos de tipo diccionario
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `graphdisplay-0.1.1/setup.py` & `graphdisplay-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.1' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.1.2' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'graphdisplay' #Debe coincidir con el nombre de la carpeta
 AUTHOR = 'Alberto Penas Díaz' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'albertopenasdiaz@gmail.com' #Modificar con vuestros datos
 URL = 'https://github.com/seniorbeto' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Librería para representar visualmente grafos de tipo diccionario' #Descripción corta
```

