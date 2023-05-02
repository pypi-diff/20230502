# Comparing `tmp/cfg-argparser-1.0.5.tar.gz` & `tmp/cfg-argparser-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfg-argparser-1.0.5.tar", last modified: Fri Apr 14 04:14:49 2023, max compression
+gzip compressed data, was "cfg-argparser-1.1.0.tar", last modified: Tue May  2 16:16:12 2023, max compression
```

## Comparing `cfg-argparser-1.0.5.tar` & `cfg-argparser-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-04-14 04:14:49.875022 cfg-argparser-1.0.5/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.0.5/LICENSE
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1493 2023-04-14 04:14:49.875022 cfg-argparser-1.0.5/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      962 2023-04-14 03:38:02.000000 cfg-argparser-1.0.5/README.md
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      597 2023-04-14 04:14:31.000000 cfg-argparser-1.0.5/pyproject.toml
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-04-14 04:14:49.875022 cfg-argparser-1.0.5/setup.cfg
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-04-14 04:14:49.875022 cfg-argparser-1.0.5/src/
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-04-14 04:14:49.875022 cfg-argparser-1.0.5/src/cfg_argparser/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      104 2023-04-12 21:18:54.000000 cfg-argparser-1.0.5/src/cfg_argparser/__init__.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)    11355 2023-04-14 04:09:51.000000 cfg-argparser-1.0.5/src/cfg_argparser/config_arg_parser.py
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-04-14 04:14:49.875022 cfg-argparser-1.0.5/src/cfg_argparser.egg-info/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1493 2023-04-14 04:14:49.000000 cfg-argparser-1.0.5/src/cfg_argparser.egg-info/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      265 2023-04-14 04:14:49.000000 cfg-argparser-1.0.5/src/cfg_argparser.egg-info/SOURCES.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-04-14 04:14:49.000000 cfg-argparser-1.0.5/src/cfg_argparser.egg-info/dependency_links.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-04-14 04:14:49.000000 cfg-argparser-1.0.5/src/cfg_argparser.egg-info/top_level.txt
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-02 16:16:12.678932 cfg-argparser-1.1.0/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.1.0/LICENSE
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2118 2023-05-02 16:16:12.675598 cfg-argparser-1.1.0/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1285 2023-04-14 06:48:50.000000 cfg-argparser-1.1.0/README.md
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      874 2023-04-19 02:49:09.000000 cfg-argparser-1.1.0/pyproject.toml
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-05-02 16:16:12.678932 cfg-argparser-1.1.0/setup.cfg
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-02 16:16:12.675598 cfg-argparser-1.1.0/src/
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-02 16:16:12.675598 cfg-argparser-1.1.0/src/cfg_argparser/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      104 2023-04-12 21:18:54.000000 cfg-argparser-1.1.0/src/cfg_argparser/__init__.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)    11665 2023-05-02 16:08:37.000000 cfg-argparser-1.1.0/src/cfg_argparser/config_arg_parser.py
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-05-02 16:16:12.675598 cfg-argparser-1.1.0/src/cfg_argparser.egg-info/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2118 2023-05-02 16:16:12.000000 cfg-argparser-1.1.0/src/cfg_argparser.egg-info/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      265 2023-05-02 16:16:12.000000 cfg-argparser-1.1.0/src/cfg_argparser.egg-info/SOURCES.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-05-02 16:16:12.000000 cfg-argparser-1.1.0/src/cfg_argparser.egg-info/dependency_links.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-05-02 16:16:12.000000 cfg-argparser-1.1.0/src/cfg_argparser.egg-info/top_level.txt
```

### Comparing `cfg-argparser-1.0.5/LICENSE` & `cfg-argparser-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.0.5/src/cfg_argparser/config_arg_parser.py` & `cfg-argparser-1.1.0/src/cfg_argparser/config_arg_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,27 @@
 from sys import exit as sys_exit
 
 # from pprint import pprint
 # from rich import print as rprint
 
 
 class CfgDict(dict):
-    def __init__(self, cfg_path, config: dict = {}):
+    """
+    A subclass of `dict` with some useful changes, most notably 
+    storing a path to save, and saving methods
+    """
+    def __init__(self, cfg_path, config: dict = {}, save_on_change: bool =False):
         super().__init__()
         self.cfg_path = cfg_path
+        self.save_on_change = save_on_change
         self.load()
         self.update(config)
 
     def set_path(self, path):
         self.cfg_path = path
-        self.load()
         return self
 
     def save(self, out_dict=None, indent=4):
         if not isinstance(out_dict, dict):
             out_dict = self
         with open(self.cfg_path, 'w+') as f:
             f.write(json.dumps(out_dict, indent=indent))
@@ -46,14 +50,19 @@
                     self.update(json.loads(data))
                 except (json.decoder.JSONDecodeError, TypeError):
                     print(f'[!] failed to load config.orjson from {self.cfg_path}')
         else:
             self.save({})
         return self
 
+    def __setitem__(self, key, value):
+        super().__setitem__(key, value)
+        if self.save_on_change:
+            self.save()
+
 
 class ParserTree(dict):
     def __init__(self, argparser: ArgumentParser):
         super().__init__()
         self.parser = argparser
         self.update(ParserTree.parser_to_tree(argparser))
 
@@ -222,15 +231,15 @@
             the path to the json file.
         cfgObject : CfgDict, optional
             if desired, update an existing CfgDict object, by default None
         exit_on_change : bool, optional
             exits when set, reset, or reset_all is called, by default False
         argument_group_name : str, optional
             name of the argument group, by default "Config options"
-        
+
         """
 
         # parent parser
         self.parser = parser
         self.default_prefix = self.parser.prefix_chars[0]
         self.exit_on_change = exit_on_change
         self.file = cfgObject or CfgDict(config_path)
```

