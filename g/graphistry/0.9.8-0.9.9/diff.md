# Comparing `tmp/graphistry-0.9.8.tar.gz` & `tmp/graphistry-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/graphistry-0.9.8.tar", last modified: Fri Sep  4 22:52:45 2015, max compression
+gzip compressed data, was "dist/graphistry-0.9.9.tar", last modified: Mon Sep 14 20:53:44 2015, max compression
```

## Comparing `graphistry-0.9.8.tar` & `graphistry-0.9.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tbh        (501) staff       (20)        0 2015-09-04 22:52:45.000000 graphistry-0.9.8/
-drwxr-xr-x   0 tbh        (501) staff       (20)        0 2015-09-04 22:52:45.000000 graphistry-0.9.8/graphistry/
--rw-r--r--   0 tbh        (501) staff       (20)      266 2015-08-10 21:55:34.000000 graphistry-0.9.8/graphistry/__init__.py
--rw-r--r--   0 tbh        (501) staff       (20)    18880 2015-09-04 22:43:37.000000 graphistry-0.9.8/graphistry/plotter.py
--rw-r--r--   0 tbh        (501) staff       (20)     6029 2015-09-04 22:48:23.000000 graphistry-0.9.8/graphistry/pygraphistry.py
--rw-r--r--   0 tbh        (501) staff       (20)     1294 2015-09-04 22:42:51.000000 graphistry-0.9.8/graphistry/util.py
-drwxr-xr-x   0 tbh        (501) staff       (20)        0 2015-09-04 22:52:45.000000 graphistry-0.9.8/Graphistry.egg-info/
--rw-r--r--   0 tbh        (501) staff       (20)        1 2015-09-04 22:52:45.000000 graphistry-0.9.8/Graphistry.egg-info/dependency_links.txt
--rw-r--r--   0 tbh        (501) staff       (20)     2367 2015-09-04 22:52:45.000000 graphistry-0.9.8/Graphistry.egg-info/PKG-INFO
--rw-r--r--   0 tbh        (501) staff       (20)      158 2015-09-04 22:52:45.000000 graphistry-0.9.8/Graphistry.egg-info/requires.txt
--rw-r--r--   0 tbh        (501) staff       (20)      310 2015-09-04 22:52:45.000000 graphistry-0.9.8/Graphistry.egg-info/SOURCES.txt
--rw-r--r--   0 tbh        (501) staff       (20)       11 2015-09-04 22:52:45.000000 graphistry-0.9.8/Graphistry.egg-info/top_level.txt
--rw-r--r--   0 tbh        (501) staff       (20)     2367 2015-09-04 22:52:45.000000 graphistry-0.9.8/PKG-INFO
--rw-r--r--   0 tbh        (501) staff       (20)       88 2015-09-04 22:52:45.000000 graphistry-0.9.8/setup.cfg
--rwxr-xr-x   0 tbh        (501) staff       (20)     2688 2015-09-04 22:52:05.000000 graphistry-0.9.8/setup.py
+drwxr-xr-x   0 tbh        (501) staff       (20)        0 2015-09-14 20:53:44.000000 graphistry-0.9.9/
+drwxr-xr-x   0 tbh        (501) staff       (20)        0 2015-09-14 20:53:44.000000 graphistry-0.9.9/graphistry/
+-rw-r--r--   0 tbh        (501) staff       (20)      266 2015-08-10 21:55:34.000000 graphistry-0.9.9/graphistry/__init__.py
+-rw-r--r--   0 tbh        (501) staff       (20)    18895 2015-09-14 20:24:13.000000 graphistry-0.9.9/graphistry/plotter.py
+-rw-r--r--   0 tbh        (501) staff       (20)     6227 2015-09-14 20:39:08.000000 graphistry-0.9.9/graphistry/pygraphistry.py
+-rw-r--r--   0 tbh        (501) staff       (20)     1512 2015-09-14 20:35:15.000000 graphistry-0.9.9/graphistry/util.py
+drwxr-xr-x   0 tbh        (501) staff       (20)        0 2015-09-14 20:53:44.000000 graphistry-0.9.9/Graphistry.egg-info/
+-rw-r--r--   0 tbh        (501) staff       (20)        1 2015-09-14 20:53:44.000000 graphistry-0.9.9/Graphistry.egg-info/dependency_links.txt
+-rw-r--r--   0 tbh        (501) staff       (20)     2367 2015-09-14 20:53:44.000000 graphistry-0.9.9/Graphistry.egg-info/PKG-INFO
+-rw-r--r--   0 tbh        (501) staff       (20)      158 2015-09-14 20:53:44.000000 graphistry-0.9.9/Graphistry.egg-info/requires.txt
+-rw-r--r--   0 tbh        (501) staff       (20)      310 2015-09-14 20:53:44.000000 graphistry-0.9.9/Graphistry.egg-info/SOURCES.txt
+-rw-r--r--   0 tbh        (501) staff       (20)       11 2015-09-14 20:53:44.000000 graphistry-0.9.9/Graphistry.egg-info/top_level.txt
+-rw-r--r--   0 tbh        (501) staff       (20)     2367 2015-09-14 20:53:44.000000 graphistry-0.9.9/PKG-INFO
+-rw-r--r--   0 tbh        (501) staff       (20)       88 2015-09-14 20:53:44.000000 graphistry-0.9.9/setup.cfg
+-rwxr-xr-x   0 tbh        (501) staff       (20)     2688 2015-09-14 20:40:33.000000 graphistry-0.9.9/setup.py
```

### Comparing `graphistry-0.9.8/graphistry/plotter.py` & `graphistry-0.9.9/graphistry/plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
 
         PyG = pygraphistry.PyGraphistry
         dataset = PyG._etl(dataset)
         viz_url = PyG._viz_url(dataset['name'], dataset['viztoken'], self._url_params)
 
         if util.in_ipython() is True:
             from IPython.core.display import HTML
-            return HTML(util.make_iframe(viz_url, self._height))
+            return HTML(util.make_iframe(viz_url, self._height, PyG._protocol))
         else:
             print('Url: http://%s' % viz_url)
             import webbrowser
             webbrowser.open(viz_url)
             return self
 
     def pandas2igraph(self, edges, directed=True):
```

### Comparing `graphistry-0.9.8/graphistry/pygraphistry.py` & `graphistry-0.9.9/graphistry/pygraphistry.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,52 +18,55 @@
 
 
 class PyGraphistry(object):
     api_key = None
     _tag = util.fingerprint()
     _dataset_prefix = 'PyGraphistry/'
     _hostname = 'localhost:3000'
+    _protocol = None
 
     @staticmethod
-    def register(key, server='labs'):
+    def register(key, server='labs', protocol=None):
         """API key registration and server selection
 
         Changing the key effects all derived Plotter instances.
 
         :param key: API key.
         :type key: String.
         :param server: URL of the visualization server.
         :type server: Optional string.
+        :param protocol: Protocol used to contact visualization server
+        :type protocol: Optional string.
         :returns: None.
         :rtype: None.
 
 
         **Example: Standard**
                 ::
 
                     import graphistry
                     graphistry.register(key="my api key")
 
         **Example: Developer**
                 ::
 
                     import graphistry
-                    graphistry.register('my api key', 'staging')
-
+                    graphistry.register('my api key', 'staging', 'https')
 
         """
 
         shortcuts = {'localhost': 'localhost:3000',
                      'staging': 'proxy-staging.graphistry.com',
                      'labs': 'proxy-labs.graphistry.com'}
         if server in shortcuts:
             PyGraphistry._hostname = shortcuts[server]
         else:
             PyGraphistry._hostname = server
         PyGraphistry.api_key = key.strip()
+        PyGraphistry._protocol = protocol
         PyGraphistry._check_key()
 
     @staticmethod
     def bind(node=None, source=None, destination=None,
              edge_title=None, edge_label=None, edge_color=None, edge_weight=None,
              point_title=None, point_label=None, point_color=None, point_size=None):
         """Create a base plotter.
```

### Comparing `graphistry-0.9.8/graphistry/util.py` & `graphistry-0.9.9/graphistry/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 from builtins import str
 
 import sys
 import platform as p
 import uuid
 import hashlib
 
-def make_iframe(raw_url, height):
+def make_iframe(raw_url, height, protocol=None):
+    if protocol:
+        return '''<iframe src="%s"
+                          style="width:100%%; height:%dpx; border: 1px solid #DDD">
+                </iframe>''' % (protocol + ':' + raw_url, height)
+
     id = uuid.uuid4()
     script = '''<script>var p = document.location.protocol;
                         if(p === "file:") {p = "http:";}
                         $("#%s").attr("src", p + "%s").show();
                 </script>''' % (id, raw_url)
     iframe = '''<iframe id="%s"
                         style="display:none; width:100%%; height:%dpx; border: 1px solid #DDD">
```

### Comparing `graphistry-0.9.8/Graphistry.egg-info/PKG-INFO` & `graphistry-0.9.9/Graphistry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: graphistry
-Version: 0.9.8
+Version: 0.9.9
 Summary: Visualize node-link graphs using Graphistry's cloud
 Home-page: https://github.com/graphistry/pygraphistry
 Author: The Graphistry Team
 Author-email: pygraphistry@graphistry.com
 License: BSD
 Download-URL: https://pypi.python.org/pypi/graphistry/
 Description:
```

### Comparing `graphistry-0.9.8/PKG-INFO` & `graphistry-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: graphistry
-Version: 0.9.8
+Version: 0.9.9
 Summary: Visualize node-link graphs using Graphistry's cloud
 Home-page: https://github.com/graphistry/pygraphistry
 Author: The Graphistry Team
 Author-email: pygraphistry@graphistry.com
 License: BSD
 Download-URL: https://pypi.python.org/pypi/graphistry/
 Description:
```

### Comparing `graphistry-0.9.8/setup.py` & `graphistry-0.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 Tutorial and API docs are on
 `https://github.com/graphistry/pygraphistry <https://github.com/graphistry/pygraphistry>`_
 """
 
 setup(
     name='graphistry',
-    version='0.9.8',
+    version='0.9.9',
     packages = ['graphistry'],
     platforms='any',
     description = 'Visualize node-link graphs using Graphistry\'s cloud',
     long_description=long_description,
     url='https://github.com/graphistry/pygraphistry',
     download_url= 'https://pypi.python.org/pypi/graphistry/',
     author='The Graphistry Team',
```

