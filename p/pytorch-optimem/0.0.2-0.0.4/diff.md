# Comparing `tmp/pytorch-optimem-0.0.2.tar.gz` & `tmp/pytorch-optimem-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jimmy/llama/pytorch-optimem/dist/.tmp-lhenr0th/pytorch-optimem-0.0.2.tar", last modified: Tue May  2 10:19:54 2023, max compression
+gzip compressed data, was "/home/jimmy/llama/pytorch-optimem/dist/.tmp-3otcfzle/pytorch-optimem-0.0.4.tar", last modified: Tue May  2 10:34:19 2023, max compression
```

## Comparing `pytorch-optimem-0.0.2.tar` & `pytorch-optimem-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jimmy     (1001) jimmy     (1002)        0 2023-05-02 10:19:54.000000 pytorch-optimem-0.0.2/
--rw-r--r--   0 jimmy     (1001) jimmy     (1002)     1066 2023-05-02 09:14:17.000000 pytorch-optimem-0.0.2/LICENSE
--rw-r--r--   0 jimmy     (1001) jimmy     (1002)      693 2023-05-02 10:19:54.000000 pytorch-optimem-0.0.2/PKG-INFO
--rw-r--r--   0 jimmy     (1001) jimmy     (1002)       83 2023-05-02 09:14:17.000000 pytorch-optimem-0.0.2/README.md
--rw-r--r--   0 jimmy     (1001) jimmy     (1002)      644 2023-05-02 10:19:40.000000 pytorch-optimem-0.0.2/pyproject.toml
--rw-r--r--   0 jimmy     (1001) jimmy     (1002)       38 2023-05-02 10:19:54.000000 pytorch-optimem-0.0.2/setup.cfg
-drwxr-xr-x   0 jimmy     (1001) jimmy     (1002)        0 2023-05-02 10:19:54.000000 pytorch-optimem-0.0.2/src/
--rw-r--r--   0 jimmy     (1001) jimmy     (1002)        0 2023-05-02 09:19:18.000000 pytorch-optimem-0.0.2/src/__init__.py
--rw-r--r--   0 jimmy     (1001) jimmy     (1002)     3424 2023-05-02 10:19:40.000000 pytorch-optimem-0.0.2/src/main.py
--rw-r--r--   0 jimmy     (1001) jimmy     (1002)     1442 2023-05-02 09:20:02.000000 pytorch-optimem-0.0.2/src/memory_utils.py
-drwxr-xr-x   0 jimmy     (1001) jimmy     (1002)        0 2023-05-02 10:19:54.000000 pytorch-optimem-0.0.2/src/pytorch_optimem.egg-info/
--rw-r--r--   0 jimmy     (1001) jimmy     (1002)      693 2023-05-02 10:19:54.000000 pytorch-optimem-0.0.2/src/pytorch_optimem.egg-info/PKG-INFO
--rw-r--r--   0 jimmy     (1001) jimmy     (1002)      294 2023-05-02 10:19:54.000000 pytorch-optimem-0.0.2/src/pytorch_optimem.egg-info/SOURCES.txt
--rw-r--r--   0 jimmy     (1001) jimmy     (1002)        1 2023-05-02 10:19:54.000000 pytorch-optimem-0.0.2/src/pytorch_optimem.egg-info/dependency_links.txt
--rw-r--r--   0 jimmy     (1001) jimmy     (1002)        6 2023-05-02 10:19:54.000000 pytorch-optimem-0.0.2/src/pytorch_optimem.egg-info/requires.txt
--rw-r--r--   0 jimmy     (1001) jimmy     (1002)       27 2023-05-02 10:19:54.000000 pytorch-optimem-0.0.2/src/pytorch_optimem.egg-info/top_level.txt
+drwxr-xr-x   0 jimmy     (1001) jimmy     (1002)        0 2023-05-02 10:34:19.000000 pytorch-optimem-0.0.4/
+-rw-r--r--   0 jimmy     (1001) jimmy     (1002)     1066 2023-05-02 09:14:17.000000 pytorch-optimem-0.0.4/LICENSE
+-rw-r--r--   0 jimmy     (1001) jimmy     (1002)      693 2023-05-02 10:34:19.000000 pytorch-optimem-0.0.4/PKG-INFO
+-rw-r--r--   0 jimmy     (1001) jimmy     (1002)       83 2023-05-02 09:14:17.000000 pytorch-optimem-0.0.4/README.md
+-rw-r--r--   0 jimmy     (1001) jimmy     (1002)      644 2023-05-02 10:34:13.000000 pytorch-optimem-0.0.4/pyproject.toml
+-rw-r--r--   0 jimmy     (1001) jimmy     (1002)       38 2023-05-02 10:34:19.000000 pytorch-optimem-0.0.4/setup.cfg
+drwxr-xr-x   0 jimmy     (1001) jimmy     (1002)        0 2023-05-02 10:34:19.000000 pytorch-optimem-0.0.4/src/
+drwxr-xr-x   0 jimmy     (1001) jimmy     (1002)        0 2023-05-02 10:34:19.000000 pytorch-optimem-0.0.4/src/optimem/
+-rw-r--r--   0 jimmy     (1001) jimmy     (1002)        0 2023-05-02 09:19:18.000000 pytorch-optimem-0.0.4/src/optimem/__init__.py
+-rw-r--r--   0 jimmy     (1001) jimmy     (1002)     3424 2023-05-02 10:19:40.000000 pytorch-optimem-0.0.4/src/optimem/main.py
+drwxr-xr-x   0 jimmy     (1001) jimmy     (1002)        0 2023-05-02 10:34:19.000000 pytorch-optimem-0.0.4/src/pytorch_optimem.egg-info/
+-rw-r--r--   0 jimmy     (1001) jimmy     (1002)      693 2023-05-02 10:34:19.000000 pytorch-optimem-0.0.4/src/pytorch_optimem.egg-info/PKG-INFO
+-rw-r--r--   0 jimmy     (1001) jimmy     (1002)      290 2023-05-02 10:34:19.000000 pytorch-optimem-0.0.4/src/pytorch_optimem.egg-info/SOURCES.txt
+-rw-r--r--   0 jimmy     (1001) jimmy     (1002)        1 2023-05-02 10:34:19.000000 pytorch-optimem-0.0.4/src/pytorch_optimem.egg-info/dependency_links.txt
+-rw-r--r--   0 jimmy     (1001) jimmy     (1002)        6 2023-05-02 10:34:19.000000 pytorch-optimem-0.0.4/src/pytorch_optimem.egg-info/requires.txt
+-rw-r--r--   0 jimmy     (1001) jimmy     (1002)        8 2023-05-02 10:34:19.000000 pytorch-optimem-0.0.4/src/pytorch_optimem.egg-info/top_level.txt
```

### Comparing `pytorch-optimem-0.0.2/LICENSE` & `pytorch-optimem-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-optimem-0.0.2/PKG-INFO` & `pytorch-optimem-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytorch-optimem
-Version: 0.0.2
+Version: 0.0.4
 Summary: Optimem is a library to reduce the GPU memory footprint of PyTorch models
 Author-email: Jimmy Li <jimmy.li@berkeley.com>, Mehul Raheja <mraheja@berkeley.edu>
 Project-URL: Homepage, https://github.com/callaunchpad/pytorch-optimem
 Project-URL: Bug Tracker, https://github.com/callaunchpad/pytorch-optimem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytorch-optimem
 A Python package for reducing memory footprint of PyTorch models
```

### Comparing `pytorch-optimem-0.0.2/pyproject.toml` & `pytorch-optimem-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "pytorch-optimem"
-version = "0.0.2"
+version = "0.0.4"
 authors = [
   { name="Jimmy Li", email="jimmy.li@berkeley.com" }, { name="Mehul Raheja", email="mraheja@berkeley.edu" },
 ]
 description = "Optimem is a library to reduce the GPU memory footprint of PyTorch models"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
```

### Comparing `pytorch-optimem-0.0.2/src/main.py` & `pytorch-optimem-0.0.4/src/optimem/main.py`

 * *Files identical despite different names*

### Comparing `pytorch-optimem-0.0.2/src/pytorch_optimem.egg-info/PKG-INFO` & `pytorch-optimem-0.0.4/src/pytorch_optimem.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytorch-optimem
-Version: 0.0.2
+Version: 0.0.4
 Summary: Optimem is a library to reduce the GPU memory footprint of PyTorch models
 Author-email: Jimmy Li <jimmy.li@berkeley.com>, Mehul Raheja <mraheja@berkeley.edu>
 Project-URL: Homepage, https://github.com/callaunchpad/pytorch-optimem
 Project-URL: Bug Tracker, https://github.com/callaunchpad/pytorch-optimem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytorch-optimem
 A Python package for reducing memory footprint of PyTorch models
```

