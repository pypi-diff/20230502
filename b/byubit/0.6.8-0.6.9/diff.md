# Comparing `tmp/byubit-0.6.8.tar.gz` & `tmp/byubit-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byubit-0.6.8.tar", max compression
+gzip compressed data, was "byubit-0.6.9.tar", max compression
```

## Comparing `byubit-0.6.8.tar` & `byubit-0.6.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2021-12-10 23:51:45.656173 byubit-0.6.8/LICENSE
--rw-r--r--   0        0        0      218 2023-01-03 21:11:26.814854 byubit-0.6.8/byubit/__init__.py
--rw-r--r--   0        0        0    13696 2023-01-03 21:11:26.821168 byubit-0.6.8/byubit/bit.py
--rw-r--r--   0        0        0     5274 2023-01-03 21:11:26.831328 byubit-0.6.8/byubit/core.py
--rw-r--r--   0        0        0     8484 2023-01-03 21:11:26.842357 byubit-0.6.8/byubit/renderers.py
--rw-r--r--   0        0        0      400 2023-01-03 21:11:26.933701 byubit-0.6.8/pyproject.toml
--rw-r--r--   0        0        0      652 2023-01-03 21:12:09.593342 byubit-0.6.8/setup.py
--rw-r--r--   0        0        0      531 2023-01-03 21:12:09.593578 byubit-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2021-12-10 23:51:45.656173 byubit-0.6.9/LICENSE
+-rw-r--r--   0        0        0      218 2023-01-03 21:11:26.814854 byubit-0.6.9/byubit/__init__.py
+-rw-r--r--   0        0        0    13696 2023-01-03 21:11:26.821168 byubit-0.6.9/byubit/bit.py
+-rw-r--r--   0        0        0     5274 2023-01-03 21:11:26.831328 byubit-0.6.9/byubit/core.py
+-rw-r--r--   0        0        0     8503 2023-01-06 21:56:23.807563 byubit-0.6.9/byubit/renderers.py
+-rw-r--r--   0        0        0      400 2023-01-06 21:58:05.594763 byubit-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0      652 2023-01-06 21:58:33.257487 byubit-0.6.9/setup.py
+-rw-r--r--   0        0        0      531 2023-01-06 21:58:33.257626 byubit-0.6.9/PKG-INFO
```

### Comparing `byubit-0.6.8/LICENSE` & `byubit-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `byubit-0.6.8/byubit/bit.py` & `byubit-0.6.9/byubit/bit.py`

 * *Files identical despite different names*

### Comparing `byubit-0.6.8/byubit/core.py` & `byubit-0.6.9/byubit/core.py`

 * *Files identical despite different names*

### Comparing `byubit-0.6.8/byubit/renderers.py` & `byubit-0.6.9/byubit/renderers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+import os
+
 import matplotlib
 from matplotlib import pyplot as plt
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from matplotlib.figure import Figure
 
 import tkinter as tk
 from tkinter import ttk
 
 from typing import List, Tuple
 
 from byubit.core import BitHistoryRecord, BitHistoryRenderer, draw_record, determine_figure_size
 
-matplotlib.use("TkAgg")
-
 
 def print_histories(histories: List[Tuple[str, List[BitHistoryRecord]]]):
     for name, history in histories:
         print(name)
         print('-' * len(name))
         for num, record in enumerate(history):
             print(f"{num}: {record.name}")
@@ -250,14 +250,16 @@
     def __init__(self, verbose=False):
         self.verbose = verbose
 
     def render(self, histories: List[Tuple[str, List[BitHistoryRecord]]]):
         """
         Run TKinter application
         """
+        matplotlib.use("TkAgg")
+
         root = tk.Tk()
         root.title('CS 110 Bit')
 
         bit_panel = MainWindow(root, histories, self.verbose)
         bit_panel.pack()
 
         root.protocol('WM_DELETE_WINDOW', root.quit)
```

### Comparing `byubit-0.6.8/setup.py` & `byubit-0.6.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.5.1,<4.0.0', 'numpy>=1.22.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'byubit',
-    'version': '0.6.8',
+    'version': '0.6.9',
     'description': 'A library for teaching beginners how to program',
     'long_description': None,
     'author': 'Gordon Bean',
     'author_email': 'gbean@cs.byu.edu',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `byubit-0.6.8/PKG-INFO` & `byubit-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byubit
-Version: 0.6.8
+Version: 0.6.9
 Summary: A library for teaching beginners how to program
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

