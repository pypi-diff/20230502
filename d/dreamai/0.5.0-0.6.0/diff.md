# Comparing `tmp/dreamai-0.5.0.tar.gz` & `tmp/dreamai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai-0.5.0.tar", last modified: Mon May  1 20:38:28 2023, max compression
+gzip compressed data, was "dreamai-0.6.0.tar", last modified: Tue May  2 01:43:38 2023, max compression
```

## Comparing `dreamai-0.5.0.tar` & `dreamai-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-01 20:38:28.787012 dreamai-0.5.0/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2022-09-05 16:31:43.000000 dreamai-0.5.0/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2022-09-05 16:31:43.000000 dreamai-0.5.0/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-01 20:38:28.787012 dreamai-0.5.0/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      130 2023-04-28 13:32:56.000000 dreamai-0.5.0/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-01 20:38:28.783012 dreamai-0.5.0/dreamai/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-01 20:38:22.000000 dreamai-0.5.0/dreamai/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8109 2023-05-01 20:38:22.000000 dreamai-0.5.0/dreamai/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8778 2023-05-01 20:38:22.000000 dreamai-0.5.0/dreamai/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      636 2023-05-01 20:31:14.000000 dreamai-0.5.0/dreamai/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     8258 2023-05-01 20:38:22.000000 dreamai-0.5.0/dreamai/vision.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-01 20:38:28.787012 dreamai-0.5.0/dreamai.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-01 20:38:28.000000 dreamai-0.5.0/dreamai.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      361 2023-05-01 20:38:28.000000 dreamai-0.5.0/dreamai.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-01 20:38:28.000000 dreamai-0.5.0/dreamai.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       36 2023-05-01 20:38:28.000000 dreamai-0.5.0/dreamai.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-01-18 11:49:09.000000 dreamai-0.5.0/dreamai.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      483 2023-05-01 20:38:28.000000 dreamai-0.5.0/dreamai.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        8 2023-05-01 20:38:28.000000 dreamai-0.5.0/dreamai.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1143 2023-05-01 20:34:56.000000 dreamai-0.5.0/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-01 20:38:28.787012 dreamai-0.5.0/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2641 2023-01-25 20:45:57.000000 dreamai-0.5.0/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 01:43:38.862010 dreamai-0.6.0/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2022-09-05 16:31:43.000000 dreamai-0.6.0/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2022-09-05 16:31:43.000000 dreamai-0.6.0/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-02 01:43:38.862010 dreamai-0.6.0/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      130 2023-05-02 01:42:31.000000 dreamai-0.6.0/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 01:43:38.858010 dreamai-0.6.0/dreamai/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-02 01:43:22.000000 dreamai-0.6.0/dreamai/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     7897 2023-05-02 01:43:22.000000 dreamai-0.6.0/dreamai/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     8737 2023-05-02 01:43:22.000000 dreamai-0.6.0/dreamai/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      811 2023-05-02 01:33:15.000000 dreamai-0.6.0/dreamai/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     8258 2023-05-02 01:43:22.000000 dreamai-0.6.0/dreamai/vision.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-02 01:43:38.862010 dreamai-0.6.0/dreamai.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      869 2023-05-02 01:43:38.000000 dreamai-0.6.0/dreamai.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      361 2023-05-02 01:43:38.000000 dreamai-0.6.0/dreamai.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-02 01:43:38.000000 dreamai-0.6.0/dreamai.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       36 2023-05-02 01:43:38.000000 dreamai-0.6.0/dreamai.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-01-18 11:49:09.000000 dreamai-0.6.0/dreamai.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      483 2023-05-02 01:43:38.000000 dreamai-0.6.0/dreamai.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        8 2023-05-02 01:43:38.000000 dreamai-0.6.0/dreamai.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1143 2023-05-02 01:43:12.000000 dreamai-0.6.0/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-02 01:43:38.862010 dreamai-0.6.0/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2641 2023-01-25 20:45:57.000000 dreamai-0.6.0/setup.py
```

### Comparing `dreamai-0.5.0/LICENSE` & `dreamai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai-0.5.0/PKG-INFO` & `dreamai-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai
-Version: 0.5.0
+Version: 0.6.0
 Summary: A bunch of cool and convenient utility functions.
 Home-page: https://github.com/HamzaFarhan/dreamai
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai-0.5.0/dreamai/_modidx.py` & `dreamai-0.6.0/dreamai/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,25 @@
                               'dreamai.core.is_img': ('core.html#is_img', 'dreamai/core.py'),
                               'dreamai.core.is_int': ('core.html#is_int', 'dreamai/core.py'),
                               'dreamai.core.is_iter': ('core.html#is_iter', 'dreamai/core.py'),
                               'dreamai.core.is_list': ('core.html#is_list', 'dreamai/core.py'),
                               'dreamai.core.is_norm': ('core.html#is_norm', 'dreamai/core.py'),
                               'dreamai.core.is_path': ('core.html#is_path', 'dreamai/core.py'),
                               'dreamai.core.is_pilimage': ('core.html#is_pilimage', 'dreamai/core.py'),
-                              'dreamai.core.is_sequential': ('core.html#is_sequential', 'dreamai/core.py'),
                               'dreamai.core.is_set': ('core.html#is_set', 'dreamai/core.py'),
                               'dreamai.core.is_str': ('core.html#is_str', 'dreamai/core.py'),
                               'dreamai.core.is_subscriptable': ('core.html#is_subscriptable', 'dreamai/core.py'),
                               'dreamai.core.is_tuple': ('core.html#is_tuple', 'dreamai/core.py'),
                               'dreamai.core.is_unfrozen': ('core.html#is_unfrozen', 'dreamai/core.py'),
                               'dreamai.core.last_modified': ('core.html#last_modified', 'dreamai/core.py'),
                               'dreamai.core.list_map': ('core.html#list_map', 'dreamai/core.py'),
                               'dreamai.core.list_or_tuple': ('core.html#list_or_tuple', 'dreamai/core.py'),
                               'dreamai.core.load_obj': ('core.html#load_obj', 'dreamai/core.py'),
                               'dreamai.core.load_yaml': ('core.html#load_yaml', 'dreamai/core.py'),
                               'dreamai.core.locals_to_params': ('core.html#locals_to_params', 'dreamai/core.py'),
-                              'dreamai.core.merge_dicts': ('core.html#merge_dicts', 'dreamai/core.py'),
                               'dreamai.core.model_children': ('core.html#model_children', 'dreamai/core.py'),
                               'dreamai.core.next_batch': ('core.html#next_batch', 'dreamai/core.py'),
                               'dreamai.core.noop': ('core.html#noop', 'dreamai/core.py'),
                               'dreamai.core.params': ('core.html#params', 'dreamai/core.py'),
                               'dreamai.core.path_name': ('core.html#path_name', 'dreamai/core.py'),
                               'dreamai.core.path_or_str': ('core.html#path_or_str', 'dreamai/core.py'),
                               'dreamai.core.path_stem': ('core.html#path_stem', 'dreamai/core.py'),
```

### Comparing `dreamai-0.5.0/dreamai/core.py` & `dreamai-0.6.0/dreamai/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
 __all__ = ['flatten_list', 'noop', 'is_list', 'is_tuple', 'list_or_tuple', 'is_iter', 'is_dict', 'is_df', 'is_str', 'is_int',
            'is_float', 'is_array', 'is_pilimage', 'is_img', 'is_set', 'is_path', 'path_or_str', 'is_norm', 'params',
-           'is_frozen', 'is_unfrozen', 'is_subscriptable', 'is_sequential', 'is_clip', 'path_name', 'path_stem',
-           'path_suffix', 'extend_path_name', 'end_of_path', 'last_modified', 'load_yaml', 'save_obj', 'load_obj',
-           'resolve_data_path', 'yml_to_pip', 'set_pip_req', 'merge_dicts', 'dict_values', 'dict_keys', 'sort_dict',
-           'locals_to_params', 'list_map', 'next_batch', 'model_children', 'replace_dict_key', 'proc_fn', 'filter_dict',
-           'setify', 'get_files']
+           'is_frozen', 'is_unfrozen', 'is_subscriptable', 'is_clip', 'path_name', 'path_stem', 'path_suffix',
+           'extend_path_name', 'end_of_path', 'last_modified', 'load_yaml', 'save_obj', 'load_obj', 'resolve_data_path',
+           'yml_to_pip', 'set_pip_req', 'dict_values', 'dict_keys', 'sort_dict', 'locals_to_params', 'list_map',
+           'next_batch', 'model_children', 'replace_dict_key', 'proc_fn', 'filter_dict', 'setify', 'get_files']
 
 # %% ../nbs/00_core.ipynb 3
 from .imports import *
 
 # %% ../nbs/00_core.ipynb 4
 # def default_device(device=None):
     # if device is None:
@@ -56,16 +55,20 @@
 
 def is_int(x):
     return isinstance(x, int)    
 
 def is_float(x):
     return isinstance(x, float)
 
+# def is_array(x):
+#     return isinstance(x, np.ndarray)
+
 def is_array(x):
-    return isinstance(x, np.ndarray)
+    "`True` if `x` supports `__array__` or `iloc`"
+    return hasattr(x,'__array__') or hasattr(x,'iloc')
 
 def is_pilimage(x):
     return 'PIL' in str(type(x))
 
 def is_img(x):
     return is_array(x) or is_pilimage(x)
 
@@ -93,16 +96,16 @@
 
 def is_unfrozen(model):
     return np.array([p.requires_grad for p in (params(model))]).all()
 
 def is_subscriptable(x):
     return hasattr(x, '__getitem__')
 
-def is_sequential(x):
-    return isinstance(x, nn.Sequential)
+# def is_sequential(x):
+    # return isinstance(x, nn.Sequential)
 
 def is_clip(x):
     return type(x).__name__ == 'ProntoClip' or 'moviepy' in str(type(x))
 
 def path_name(x):
     return Path(x).name
 
@@ -140,15 +143,15 @@
 
 def load_obj(path):
     with open(path, 'rb') as f:
         return pickle.load(f)
 
 def resolve_data_path(data_path):
     if not is_list(data_path): data_path = [data_path]
-    data_path = flatten_list(data_path)
+    data_path = flatten(data_path)
     paths = []
     for dp in data_path:
         if path_or_str(dp):
             dp = Path(dp)
             if not dp.exists():
                 raise Exception(f'Path {dp} does not exist.')
             if dp.is_dir():
@@ -177,22 +180,14 @@
     config = ConfigParser(delimiters=['='], allow_no_value=True)
     config.read(settings)
     cfg = config['DEFAULT']
     config.set('DEFAULT', 'pip_requirements', env_pip)
     with open(settings, 'w') as configfile:
         config.write(configfile)
 
-def merge_dicts(d1,d2):
-    d = {}
-    for k in d1:
-        d[k] = d1[k]
-    for k in d2:
-        d[k] = d2[k]
-    return d
-
 def dict_values(d):
     "Get the values of a dictionary sorted by key."
     return [v for _,v in sorted(d.items(), key=lambda x:x[0])]
 
 def dict_keys(d):
     "Get the sorted keys of a dictionary."
     return [k for k,_ in sorted(d.items(), key=lambda x:x[0])]
```

### Comparing `dreamai-0.5.0/dreamai/imports.py` & `dreamai-0.6.0/dreamai/imports.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,7 +19,11 @@
 from yaml import load, Loader
 import matplotlib.pyplot as plt
 from collections import OrderedDict
 from configparser import ConfigParser
 from imutils import resize as resize_img
 from PIL import Image, ImageDraw, ImageFont
 from typing import Iterable,Generator,Sequence,Iterator,List,Set,Dict,Union,Optional,Tuple
+
+from fastcore.foundation import is_bool, L
+from fastcore.basics import merge as merge_dicts
+from fastcore.basics import chunked, store_attr, camel2snake, snake2camel, flatten
```

### Comparing `dreamai-0.5.0/dreamai/vision.py` & `dreamai-0.6.0/dreamai/vision.py`

 * *Files identical despite different names*

### Comparing `dreamai-0.5.0/dreamai.egg-info/PKG-INFO` & `dreamai-0.6.0/dreamai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai
-Version: 0.5.0
+Version: 0.6.0
 Summary: A bunch of cool and convenient utility functions.
 Home-page: https://github.com/HamzaFarhan/dreamai
 Author: HamzaFarhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai-0.5.0/settings.ini` & `dreamai-0.6.0/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dreamai
 lib_name = %(repo)s
-version = 0.5.0
+version = 0.6.0
 min_python = 3.8
 license = apache2
 doc_path = _docs
 lib_path = dreamai
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `dreamai-0.5.0/setup.py` & `dreamai-0.6.0/setup.py`

 * *Files identical despite different names*

