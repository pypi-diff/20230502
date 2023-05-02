# Comparing `tmp/cfg-argparser-1.1.0.tar.gz` & `tmp/cfg-argparser-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfg-argparser-1.1.0.tar", last modified: Tue May  2 16:16:12 2023, max compression
+gzip compressed data, was "cfg-argparser-1.1.1.tar", last modified: Tue May  2 16:30:46 2023, max compression
```

## Comparing `cfg-argparser-1.1.0.tar` & `cfg-argparser-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-02 16:16:12.678932 cfg-argparser-1.1.0/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.1.0/LICENSE
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2118 2023-05-02 16:16:12.675598 cfg-argparser-1.1.0/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1285 2023-04-14 06:48:50.000000 cfg-argparser-1.1.0/README.md
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      874 2023-04-19 02:49:09.000000 cfg-argparser-1.1.0/pyproject.toml
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-05-02 16:16:12.678932 cfg-argparser-1.1.0/setup.cfg
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-02 16:16:12.675598 cfg-argparser-1.1.0/src/
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-02 16:16:12.675598 cfg-argparser-1.1.0/src/cfg_argparser/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      104 2023-04-12 21:18:54.000000 cfg-argparser-1.1.0/src/cfg_argparser/__init__.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)    11665 2023-05-02 16:08:37.000000 cfg-argparser-1.1.0/src/cfg_argparser/config_arg_parser.py
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-02 16:16:12.675598 cfg-argparser-1.1.0/src/cfg_argparser.egg-info/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2118 2023-05-02 16:16:12.000000 cfg-argparser-1.1.0/src/cfg_argparser.egg-info/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      265 2023-05-02 16:16:12.000000 cfg-argparser-1.1.0/src/cfg_argparser.egg-info/SOURCES.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-05-02 16:16:12.000000 cfg-argparser-1.1.0/src/cfg_argparser.egg-info/dependency_links.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-05-02 16:16:12.000000 cfg-argparser-1.1.0/src/cfg_argparser.egg-info/top_level.txt
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-02 16:30:46.978921 cfg-argparser-1.1.1/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.1.1/LICENSE
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2118 2023-05-02 16:30:46.978921 cfg-argparser-1.1.1/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1285 2023-04-14 06:48:50.000000 cfg-argparser-1.1.1/README.md
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      874 2023-05-02 16:30:35.000000 cfg-argparser-1.1.1/pyproject.toml
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-05-02 16:30:46.978921 cfg-argparser-1.1.1/setup.cfg
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-02 16:30:46.975588 cfg-argparser-1.1.1/src/
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-02 16:30:46.975588 cfg-argparser-1.1.1/src/cfg_argparser/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      104 2023-04-12 21:18:54.000000 cfg-argparser-1.1.1/src/cfg_argparser/__init__.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)    11984 2023-05-02 16:29:40.000000 cfg-argparser-1.1.1/src/cfg_argparser/config_arg_parser.py
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-02 16:30:46.978921 cfg-argparser-1.1.1/src/cfg_argparser.egg-info/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2118 2023-05-02 16:30:46.000000 cfg-argparser-1.1.1/src/cfg_argparser.egg-info/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      265 2023-05-02 16:30:46.000000 cfg-argparser-1.1.1/src/cfg_argparser.egg-info/SOURCES.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-05-02 16:30:46.000000 cfg-argparser-1.1.1/src/cfg_argparser.egg-info/dependency_links.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-05-02 16:30:46.000000 cfg-argparser-1.1.1/src/cfg_argparser.egg-info/top_level.txt
```

### Comparing `cfg-argparser-1.1.0/LICENSE` & `cfg-argparser-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.1.0/PKG-INFO` & `cfg-argparser-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfg-argparser
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package designed to simplify configurable defaults from argparse.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `cfg-argparser-1.1.0/README.md` & `cfg-argparser-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.1.0/pyproject.toml` & `cfg-argparser-1.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cfg-argparser"
-version = "1.1.0"
+version = "1.1.1"
 authors = [{ name = "Zeptofine", email = "zeptofine@gmail.com" }]
 description = "A package designed to simplify configurable defaults from argparse."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
```

### Comparing `cfg-argparser-1.1.0/src/cfg_argparser/config_arg_parser.py` & `cfg-argparser-1.1.1/src/cfg_argparser/config_arg_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 
 class CfgDict(dict):
     """
     A subclass of `dict` with some useful changes, most notably 
     storing a path to save, and saving methods
     """
-    def __init__(self, cfg_path, config: dict = {}, save_on_change: bool =False):
+
+    def __init__(self, cfg_path, config: dict = {}, save_on_change: bool = False):
         super().__init__()
         self.cfg_path = cfg_path
         self.save_on_change = save_on_change
         self.load()
         self.update(config)
 
     def set_path(self, path):
@@ -26,20 +27,28 @@
     def save(self, out_dict=None, indent=4):
         if not isinstance(out_dict, dict):
             out_dict = self
         with open(self.cfg_path, 'w+') as f:
             f.write(json.dumps(out_dict, indent=indent))
         return self
 
+    def _save_on_change(self):
+        if self.save_on_change:
+            self.save()
+            return True
+        return False
+
     def update(self, *args, **kwargs):
         super().update(*args, **kwargs)
+        self._save_on_change()
         return self
 
     def pop(self, *args, **kwargs):
         super().pop(*args, **kwargs)
+        self._save_on_change()
         return self
 
     def clear(self):
         super().clear()
         return self
 
     def load(self):
@@ -55,14 +64,19 @@
         return self
 
     def __setitem__(self, key, value):
         super().__setitem__(key, value)
         if self.save_on_change:
             self.save()
 
+    def __delitem__(self, key):
+        super().__delitem__(key)
+        if self.save_on_change:
+            self.save()
+
 
 class ParserTree(dict):
     def __init__(self, argparser: ArgumentParser):
         super().__init__()
         self.parser = argparser
         self.update(ParserTree.parser_to_tree(argparser))
```

### Comparing `cfg-argparser-1.1.0/src/cfg_argparser.egg-info/PKG-INFO` & `cfg-argparser-1.1.1/src/cfg_argparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfg-argparser
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package designed to simplify configurable defaults from argparse.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

