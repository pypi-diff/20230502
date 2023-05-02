# Comparing `tmp/notion-graph-0.1.1.tar.gz` & `tmp/notion-graph-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-graph-0.1.1.tar", last modified: Sat Feb 18 05:26:28 2023, max compression
+gzip compressed data, was "notion-graph-0.1.2.tar", last modified: Tue May  2 05:29:07 2023, max compression
```

## Comparing `notion-graph-0.1.1.tar` & `notion-graph-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     3579 2023-01-23 09:07:31.524157 notion-graph-0.1.1/README.md
--rw-r--r--   0        0        0      634 2023-01-23 09:07:31.524157 notion-graph-0.1.1/notion_graph/__init__.py
--rw-r--r--   0        0        0       61 2023-01-23 09:07:31.524157 notion-graph-0.1.1/notion_graph/__main__.py
--rw-r--r--   0        0        0      759 2023-01-23 09:07:31.524157 notion-graph-0.1.1/notion_graph/cli.py
--rw-r--r--   0        0        0      251 2023-01-23 09:07:31.524157 notion-graph-0.1.1/notion_graph/helper.py
--rw-r--r--   0        0        0    11211 2023-02-18 05:21:46.080462 notion-graph-0.1.1/notion_graph/parser.py
--rw-r--r--   0        0        0      523 2023-02-18 05:25:50.700429 notion-graph-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3840 1970-01-01 00:00:00.000000 notion-graph-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-02 02:00:02.124145 notion-graph-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3579 2023-01-23 09:07:31.524157 notion-graph-0.1.2/README.md
+-rw-r--r--   0        0        0      634 2023-01-23 09:07:31.524157 notion-graph-0.1.2/notion_graph/__init__.py
+-rw-r--r--   0        0        0       61 2023-01-23 09:07:31.524157 notion-graph-0.1.2/notion_graph/__main__.py
+-rw-r--r--   0        0        0      762 2023-05-02 05:25:33.092879 notion-graph-0.1.2/notion_graph/cli.py
+-rw-r--r--   0        0        0      251 2023-01-23 09:07:31.524157 notion-graph-0.1.2/notion_graph/helper.py
+-rw-r--r--   0        0        0    11346 2023-05-02 05:26:20.512874 notion-graph-0.1.2/notion_graph/parser.py
+-rw-r--r--   0        0        0      523 2023-05-02 05:27:17.202868 notion-graph-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3840 1970-01-01 00:00:00.000000 notion-graph-0.1.2/PKG-INFO
```

### Comparing `notion-graph-0.1.1/README.md` & `notion-graph-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `notion-graph-0.1.1/notion_graph/__init__.py` & `notion-graph-0.1.2/notion_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.1.1/notion_graph/cli.py` & `notion-graph-0.1.2/notion_graph/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 def main():
     parser = argparse.ArgumentParser(prog="notion-graph")
 
     parser.add_argument('--page', '-p', help='Notion page ID', required=True)
     parser.add_argument(
         '--token', '-t', help='Notion integration token', required=True)
     parser.add_argument(
-        '--serve', '-s', help='Running a web page to display graph view', required=False)
-    parser.add_argument(
         '--out', '-o', help='Image output path, e.g. `./graph_out.png`', required=False, default="./graph_out.png")
+    parser.add_argument(
+        '--font', '-f', help='Specify font family e.g. `SimSun`', required=False)
     args = parser.parse_args()
     parser = Parser(NOTION_VERSION, args.token)
     parser.parse(args.page)
-    parser.export_to_png(args.out)
+    parser.export_to_png(args.out, args.font)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `notion-graph-0.1.1/notion_graph/parser.py` & `notion-graph-0.1.2/notion_graph/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,22 +34,27 @@
         self._graph = nx.Graph()
         self._caching_ids = set()
 
     def parse(self, root_id: str) -> nx.Graph:
         self._parse_block(root_id)
         return self._graph
 
-    def export_to_png(self, png_path: str):
+    def export_to_png(self, png_path: str, font: str):
         pos = nx.spring_layout(self._graph)
         labels = nx.get_node_attributes(self._graph, 'title')
+        font_family = 'sans-serif'
+        if font:
+            font_family = font
+
         options = {
             "node_size": 10,
             "node_color": "black",
             "edge_color": "tab:gray",
             "linewidths": 0.5,
+            "font_family": font_family,
             "font_size": 6,
             "font_color": "black",
             "width": 0.5,
             "with_labels": True,
             "labels": labels,
             "alpha": 0.7,
             "verticalalignment": 'bottom',
```

### Comparing `notion-graph-0.1.1/pyproject.toml` & `notion-graph-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.pdm.scripts]
 start = "python -m notion_graph"
 
 [project]
 name = "notion-graph"
-version = "0.1.1"
+version = "0.1.2"
 description = "Generate a roam research like network graph view from your Notion pages."
 authors = [
     { name = "Steve Sun", email = "sund.chn@gmail.com" },
 ]
 dependencies = [
     "notion-client>=2.0.0",
     "networkx>=3.0",
```

### Comparing `notion-graph-0.1.1/PKG-INFO` & `notion-graph-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-graph
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate a roam research like network graph view from your Notion pages.
 License: MIT
 Author-email: Steve Sun <sund.chn@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 ![](images/snap.png)
```

