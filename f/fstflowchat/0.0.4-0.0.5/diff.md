# Comparing `tmp/fstflowchat-0.0.4.tar.gz` & `tmp/fstflowchat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fstflowchat-0.0.4.tar", last modified: Mon May  1 02:51:33 2023, max compression
+gzip compressed data, was "fstflowchat-0.0.5.tar", last modified: Tue May  2 20:50:21 2023, max compression
```

## Comparing `fstflowchat-0.0.4.tar` & `fstflowchat-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-01 02:51:33.153457 fstflowchat-0.0.4/
--rw-r--r--   0 kaze7539   (503) staff       (20)     1071 2023-04-19 21:48:08.000000 fstflowchat-0.0.4/LICENSE
--rw-r--r--   0 kaze7539   (503) staff       (20)       28 2023-04-24 01:28:18.000000 fstflowchat-0.0.4/MANIFEST.in
--rw-r--r--   0 kaze7539   (503) staff       (20)     2614 2023-05-01 02:51:33.152054 fstflowchat-0.0.4/PKG-INFO
--rw-r--r--   0 kaze7539   (503) staff       (20)     1473 2023-04-24 00:59:35.000000 fstflowchat-0.0.4/README.md
--rw-r--r--   0 kaze7539   (503) staff       (20)       38 2023-05-01 02:51:33.153541 fstflowchat-0.0.4/setup.cfg
--rwxr-xr-x   0 kaze7539   (503) staff       (20)     8191 2023-05-01 02:51:17.000000 fstflowchat-0.0.4/setup.py
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-01 02:51:33.131041 fstflowchat-0.0.4/src/
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-01 02:51:33.137597 fstflowchat-0.0.4/src/fstflowchat/
--rw-r--r--   0 kaze7539   (503) staff       (20)     4007 2023-05-01 02:29:33.000000 fstflowchat-0.0.4/src/fstflowchat/__init__.py
--rw-r--r--   0 kaze7539   (503) staff       (20)     7200 2023-04-24 01:50:56.000000 fstflowchat-0.0.4/src/fstflowchat/example.py
--rw-r--r--   0 kaze7539   (503) staff       (20)      795 2023-04-23 23:37:09.000000 fstflowchat-0.0.4/src/fstflowchat/quiz.dot
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-01 02:51:33.149797 fstflowchat-0.0.4/src/fstflowchat.egg-info/
--rw-r--r--   0 kaze7539   (503) staff       (20)     2614 2023-05-01 02:51:33.000000 fstflowchat-0.0.4/src/fstflowchat.egg-info/PKG-INFO
--rw-r--r--   0 kaze7539   (503) staff       (20)      354 2023-05-01 02:51:33.000000 fstflowchat-0.0.4/src/fstflowchat.egg-info/SOURCES.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)        1 2023-05-01 02:51:33.000000 fstflowchat-0.0.4/src/fstflowchat.egg-info/dependency_links.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       65 2023-05-01 02:51:33.000000 fstflowchat-0.0.4/src/fstflowchat.egg-info/entry_points.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       11 2023-05-01 02:51:33.000000 fstflowchat-0.0.4/src/fstflowchat.egg-info/requires.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       12 2023-05-01 02:51:33.000000 fstflowchat-0.0.4/src/fstflowchat.egg-info/top_level.txt
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-02 20:50:21.629103 fstflowchat-0.0.5/
+-rw-r--r--   0 kaze7539   (503) staff       (20)     1071 2023-04-19 21:48:08.000000 fstflowchat-0.0.5/LICENSE
+-rw-r--r--   0 kaze7539   (503) staff       (20)       28 2023-04-24 01:28:18.000000 fstflowchat-0.0.5/MANIFEST.in
+-rw-r--r--   0 kaze7539   (503) staff       (20)     2614 2023-05-02 20:50:21.628473 fstflowchat-0.0.5/PKG-INFO
+-rw-r--r--   0 kaze7539   (503) staff       (20)     1473 2023-04-24 00:59:35.000000 fstflowchat-0.0.5/README.md
+-rw-r--r--   0 kaze7539   (503) staff       (20)       38 2023-05-02 20:50:21.629299 fstflowchat-0.0.5/setup.cfg
+-rwxr-xr-x   0 kaze7539   (503) staff       (20)     8199 2023-05-02 20:48:26.000000 fstflowchat-0.0.5/setup.py
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-02 20:50:21.545734 fstflowchat-0.0.5/src/
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-02 20:50:21.615668 fstflowchat-0.0.5/src/fstflowchat/
+-rw-r--r--   0 kaze7539   (503) staff       (20)     4384 2023-05-02 20:40:08.000000 fstflowchat-0.0.5/src/fstflowchat/__init__.py
+-rw-r--r--   0 kaze7539   (503) staff       (20)     7200 2023-04-24 01:50:56.000000 fstflowchat-0.0.5/src/fstflowchat/example.py
+-rw-r--r--   0 kaze7539   (503) staff       (20)      795 2023-04-23 23:37:09.000000 fstflowchat-0.0.5/src/fstflowchat/quiz.dot
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-02 20:50:21.627220 fstflowchat-0.0.5/src/fstflowchat.egg-info/
+-rw-r--r--   0 kaze7539   (503) staff       (20)     2614 2023-05-02 20:50:21.000000 fstflowchat-0.0.5/src/fstflowchat.egg-info/PKG-INFO
+-rw-r--r--   0 kaze7539   (503) staff       (20)      354 2023-05-02 20:50:21.000000 fstflowchat-0.0.5/src/fstflowchat.egg-info/SOURCES.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)        1 2023-05-02 20:50:21.000000 fstflowchat-0.0.5/src/fstflowchat.egg-info/dependency_links.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       65 2023-05-02 20:50:21.000000 fstflowchat-0.0.5/src/fstflowchat.egg-info/entry_points.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       16 2023-05-02 20:50:21.000000 fstflowchat-0.0.5/src/fstflowchat.egg-info/requires.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       12 2023-05-02 20:50:21.000000 fstflowchat-0.0.5/src/fstflowchat.egg-info/top_level.txt
```

### Comparing `fstflowchat-0.0.4/LICENSE` & `fstflowchat-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.4/PKG-INFO` & `fstflowchat-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstflowchat
-Version: 0.0.4
+Version: 0.0.5
 Summary: a small, pedagogical, fst-based dialog toolkit.
 Home-page: https://fstflowchat.readthedocs.io/en/latest/
 Author: Abe Kazemzadeh
 Project-URL: Bug Reports, https://github.com/abecode/fstflowchat/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
 Project-URL: Source, https://github.com/abecode/fstflowchat/issues
```

### Comparing `fstflowchat-0.0.4/README.md` & `fstflowchat-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.4/setup.py` & `fstflowchat-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.4",  # Required
+    version="0.0.5",  # Required
     
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="a small, pedagogical, fst-based dialog toolkit.",  # Optional
     
     # This is an optional longer description of your project that represents
@@ -129,15 +129,15 @@
     
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
-    install_requires=["pygraphviz"],  # Optional
+    install_requires=["pygraphviz", "rich"],  # Optional
     
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
```

### Comparing `fstflowchat-0.0.4/src/fstflowchat/__init__.py` & `fstflowchat-0.0.5/src/fstflowchat/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import sys
 import pygraphviz as pgv
 
 
 # for rich colored printing
 from rich.console import Console
 from rich.theme import Theme
@@ -50,59 +51,73 @@
                            self.get_graph_functions()))
         else:
             all_implemented = True
             for e in self.edges_iter():
                 transitionfn, outputfn = e.attr['label'].split(':')
                 if not self.is_implemented(transitionfn, env):
                     all_implemented = False
-                    print(f"# {transitionfn} for {e} is not implemented")
+                    print(f"# {transitionfn} for edge {e} is not implemented")
                     print(transition_function_tmpl.format(transitionfn))
                 if not self.is_implemented(outputfn, env):
                     all_implemented = False
-                    print(f"# {outputfn} for {e} is not implemented")
+                    print(f"# {outputfn} for edge {e} is not implemented")
                     print(output_function_tmpl.format(outputfn))
             return all_implemented
         
                 
 
 class FST():
     def __init__(self, graph, start, end, env={}):
         self.graph = graph
-        self.start = self.currentstate = start
+        self.start = self.current_state = start
         self.end = end
         self.is_running = True
         self._env = env
 
     def __call__(self, input_: str) -> str:
-        console.print(f"currentstate: {self.currentstate}", style="info")
-        neighbor_edges = self.graph.out_edges(self.currentstate)
-        console.print("\tneighbor_edges", style="info")
+
+        # use this dict to store info for debugging
+        transition_info = {"current_state": self.current_state,
+                           "input_": input_,
+                           "edges": []}
+        
+        neighbor_edges = self.graph.out_edges(self.current_state)
         valid_edges = []
         output_fns = []
         for e in neighbor_edges:
-            console.print("\t\t", e, style="info")
             test_fn, out_fn = e.attr['label'].split(":")
-            console.print("\t\t", test_fn, out_fn, style="info")
+            edge_logging_info = {"to": e[0],
+                                 "from": e[1],
+                                 "transition_fn": test_fn,
+                                 "output_fn": out_fn,
+                                 "valid": False}
+
             if self._env[test_fn](input_):
                 valid_edges.append(e)
                 output_fns.append(out_fn)
-        console.print("\tthere are " + str(len(valid_edges)) + " valid next states",
-                      style="info")
-        console.print("\t\t", valid_edges,
-                      style="info")
+                edge_logging_info['valid'] = True
+
+            transition_info["edges"].append(edge_logging_info)
 
+        #transition_info["valid_next_states"] = list(map(lambda x: x[1], valid_edges))
         
         if len(valid_edges) == 0:
             print("no valid transitions", file=sys.stderr)
             exit(-1)
         
         # we will pick the first True test function
-        self.currentstate = valid_edges[0][1]
-        console.print(f"currentstate {self.currentstate}", style="info")
-        return self._env[output_fns[0]](input_)
+        self.current_state = valid_edges[0][1]
+        transition_info["next_state"] = self.current_state
+
+        output = self._env[output_fns[0]](input_)
+        transition_info["output"] = output
+
+        console.print(json.dumps(transition_info, indent=2), style="info")
+
+        return output
 
     def run(self) -> None:
         agent_output = self("") # prime the agent because it needs input to start
         console.print(agent_output, style="warning")
         user_input = input()
         while(self.is_running):
             agent_output = self(user_input)
```

### Comparing `fstflowchat-0.0.4/src/fstflowchat/example.py` & `fstflowchat-0.0.5/src/fstflowchat/example.py`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.4/src/fstflowchat/quiz.dot` & `fstflowchat-0.0.5/src/fstflowchat/quiz.dot`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.4/src/fstflowchat.egg-info/PKG-INFO` & `fstflowchat-0.0.5/src/fstflowchat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstflowchat
-Version: 0.0.4
+Version: 0.0.5
 Summary: a small, pedagogical, fst-based dialog toolkit.
 Home-page: https://fstflowchat.readthedocs.io/en/latest/
 Author: Abe Kazemzadeh
 Project-URL: Bug Reports, https://github.com/abecode/fstflowchat/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
 Project-URL: Source, https://github.com/abecode/fstflowchat/issues
```

