# Comparing `tmp/nmodl_preprocessor-1.0.5.tar.gz` & `tmp/nmodl_preprocessor-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmodl_preprocessor-1.0.5.tar", last modified: Mon May  1 22:39:03 2023, max compression
+gzip compressed data, was "nmodl_preprocessor-1.0.6.tar", last modified: Mon May  1 22:42:00 2023, max compression
```

## Comparing `nmodl_preprocessor-1.0.5.tar` & `nmodl_preprocessor-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-01 22:39:03.243815 nmodl_preprocessor-1.0.5/
--rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-19 23:44:54.000000 nmodl_preprocessor-1.0.5/.gitignore
--rw-rw-r--   0 dm        (1000) dm        (1000)    37883 2023-04-19 23:02:12.000000 nmodl_preprocessor-1.0.5/DETAILS.pdf
--rw-rw-r--   0 dm        (1000) dm        (1000)     1076 2023-03-28 16:31:04.000000 nmodl_preprocessor-1.0.5/LICENSE.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)     2030 2023-05-01 22:39:03.243815 nmodl_preprocessor-1.0.5/PKG-INFO
--rw-rw-r--   0 dm        (1000) dm        (1000)     1289 2023-04-20 22:05:56.000000 nmodl_preprocessor-1.0.5/README.md
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-01 22:39:03.243815 nmodl_preprocessor-1.0.5/nmodl_preprocessor/
--rw-rw-r--   0 dm        (1000) dm        (1000)    20861 2023-05-01 15:35:14.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor/__main__.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     1642 2023-04-29 16:57:39.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor/cpp_keywords.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     4533 2023-04-30 22:51:37.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor/nmodl_to_python.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     3700 2023-05-01 00:53:22.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor/rw_patterns.py
--rw-rw-r--   0 dm        (1000) dm        (1000)      550 2023-05-01 00:53:17.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor/utils.py
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-01 22:39:03.243815 nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/
--rw-rw-r--   0 dm        (1000) dm        (1000)     2030 2023-05-01 22:39:03.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/PKG-INFO
--rw-rw-r--   0 dm        (1000) dm        (1000)      479 2023-05-01 22:39:03.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/SOURCES.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)        1 2023-05-01 22:39:03.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/dependency_links.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)       80 2023-05-01 22:39:03.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/entry_points.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)        6 2023-05-01 22:39:03.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/requires.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)       19 2023-05-01 22:39:03.000000 nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/top_level.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)      957 2023-05-01 22:38:08.000000 nmodl_preprocessor-1.0.5/pyproject.toml
--rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-05-01 22:39:03.243815 nmodl_preprocessor-1.0.5/setup.cfg
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-01 22:42:00.951285 nmodl_preprocessor-1.0.6/
+-rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-19 23:44:54.000000 nmodl_preprocessor-1.0.6/.gitignore
+-rw-rw-r--   0 dm        (1000) dm        (1000)    37883 2023-04-19 23:02:12.000000 nmodl_preprocessor-1.0.6/DETAILS.pdf
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1076 2023-03-28 16:31:04.000000 nmodl_preprocessor-1.0.6/LICENSE.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)     2030 2023-05-01 22:42:00.951285 nmodl_preprocessor-1.0.6/PKG-INFO
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1289 2023-04-20 22:05:56.000000 nmodl_preprocessor-1.0.6/README.md
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-01 22:42:00.951285 nmodl_preprocessor-1.0.6/nmodl_preprocessor/
+-rw-rw-r--   0 dm        (1000) dm        (1000)    20861 2023-05-01 15:35:14.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor/__main__.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1642 2023-04-29 16:57:39.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor/cpp_keywords.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     4533 2023-04-30 22:51:37.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor/nmodl_to_python.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     3700 2023-05-01 00:53:22.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor/rw_patterns.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)      550 2023-05-01 00:53:17.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor/utils.py
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-05-01 22:42:00.951285 nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/
+-rw-rw-r--   0 dm        (1000) dm        (1000)     2030 2023-05-01 22:42:00.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/PKG-INFO
+-rw-rw-r--   0 dm        (1000) dm        (1000)      479 2023-05-01 22:42:00.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/SOURCES.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)        1 2023-05-01 22:42:00.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/dependency_links.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)       80 2023-05-01 22:42:00.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/entry_points.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)        6 2023-05-01 22:42:00.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/requires.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)       19 2023-05-01 22:42:00.000000 nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/top_level.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)      957 2023-05-01 22:41:13.000000 nmodl_preprocessor-1.0.6/pyproject.toml
+-rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-05-01 22:42:00.951285 nmodl_preprocessor-1.0.6/setup.cfg
```

### Comparing `nmodl_preprocessor-1.0.5/DETAILS.pdf` & `nmodl_preprocessor-1.0.6/DETAILS.pdf`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.5/LICENSE.txt` & `nmodl_preprocessor-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.5/PKG-INFO` & `nmodl_preprocessor-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nmodl_preprocessor
-Version: 1.0.5
+Version: 1.0.6
 Summary: Optimize NMODL files for the NEURON simulator
 Author-email: David McDougall <dam1784@rit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/ctrl-z-9000-times/nmodl_preprocessor
 Keywords: nmodl,neuron
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # nmodl_preprocessor
 
 This program optimizes NMODL files for the NEURON simulator.  
 It performs the following optimizations to ".mod" files:
```

### Comparing `nmodl_preprocessor-1.0.5/README.md` & `nmodl_preprocessor-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.5/nmodl_preprocessor/__main__.py` & `nmodl_preprocessor-1.0.6/nmodl_preprocessor/__main__.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.5/nmodl_preprocessor/cpp_keywords.py` & `nmodl_preprocessor-1.0.6/nmodl_preprocessor/cpp_keywords.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.5/nmodl_preprocessor/nmodl_to_python.py` & `nmodl_preprocessor-1.0.6/nmodl_preprocessor/nmodl_to_python.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.5/nmodl_preprocessor/rw_patterns.py` & `nmodl_preprocessor-1.0.6/nmodl_preprocessor/rw_patterns.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.5/nmodl_preprocessor/utils.py` & `nmodl_preprocessor-1.0.6/nmodl_preprocessor/utils.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.5/nmodl_preprocessor.egg-info/PKG-INFO` & `nmodl_preprocessor-1.0.6/nmodl_preprocessor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nmodl-preprocessor
-Version: 1.0.5
+Version: 1.0.6
 Summary: Optimize NMODL files for the NEURON simulator
 Author-email: David McDougall <dam1784@rit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/ctrl-z-9000-times/nmodl_preprocessor
 Keywords: nmodl,neuron
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # nmodl_preprocessor
 
 This program optimizes NMODL files for the NEURON simulator.  
 It performs the following optimizations to ".mod" files:
```

### Comparing `nmodl_preprocessor-1.0.5/pyproject.toml` & `nmodl_preprocessor-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["nmodl_preprocessor"]
 
 [project]
 name = "nmodl_preprocessor"
-version = "1.0.5"
+version = "1.0.6"
 description = "Optimize NMODL files for the NEURON simulator"
 readme = "README.md"
 license = {text = "MIT"}
 authors = [
     {name = "David McDougall", email = "dam1784@rit.edu"},
 ]
 urls = {Homepage = "https://github.com/ctrl-z-9000-times/nmodl_preprocessor"}
@@ -22,10 +22,10 @@
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Development Status :: 5 - Production/Stable",
     "Natural Language :: English",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = ["nmodl"]
 scripts = {nmodl_preprocessor = "nmodl_preprocessor:__main__._placeholder"}
```

