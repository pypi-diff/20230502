# Comparing `tmp/latex_input-0.3.0.tar.gz` & `tmp/latex_input-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex_input-0.3.0.tar", last modified: Tue May  2 04:08:34 2023, max compression
+gzip compressed data, was "latex_input-0.3.1.tar", last modified: Tue May  2 04:12:38 2023, max compression
```

## Comparing `latex_input-0.3.0.tar` & `latex_input-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2023-05-02 04:08:34.863424 latex_input-0.3.0/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    35149 2023-05-01 02:54:53.000000 latex_input-0.3.0/LICENSE
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1498 2023-05-02 04:08:34.863424 latex_input-0.3.0/PKG-INFO
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      979 2023-05-01 02:54:53.000000 latex_input-0.3.0/README.md
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2023-05-02 04:08:34.863424 latex_input-0.3.0/latex_input/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     7673 2023-05-02 03:48:05.000000 latex_input-0.3.0/latex_input/__main__.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    58755 2023-05-01 02:54:53.000000 latex_input-0.3.0/latex_input/cached_unicode_data.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2023-05-02 04:08:34.863424 latex_input-0.3.0/latex_input/data/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)   105776 2023-05-01 02:54:53.000000 latex_input-0.3.0/latex_input/data/icon.ico
--rw-rw-r--   0 kevin     (1000) kevin     (1000)   105634 2023-05-01 02:54:53.000000 latex_input-0.3.0/latex_input/data/icon_activated.ico
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     4705 2023-05-02 03:45:34.000000 latex_input-0.3.0/latex_input/input_client_linux.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3713 2023-05-02 03:45:43.000000 latex_input-0.3.0/latex_input/input_client_win.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    10440 2023-05-01 02:54:53.000000 latex_input-0.3.0/latex_input/latex_converter.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1222 2023-05-01 02:54:53.000000 latex_input-0.3.0/latex_input/listener.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     3441 2023-05-01 02:54:53.000000 latex_input-0.3.0/latex_input/parse_unicode_data.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)    67693 2023-05-02 03:18:50.000000 latex_input-0.3.0/latex_input/unicode_data.py
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      372 2023-05-01 02:54:53.000000 latex_input-0.3.0/latex_input/unicode_structs.py
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2023-05-02 04:08:34.863424 latex_input-0.3.0/latex_input.egg-info/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     1498 2023-05-02 04:08:34.000000 latex_input-0.3.0/latex_input.egg-info/PKG-INFO
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      564 2023-05-02 04:08:34.000000 latex_input-0.3.0/latex_input.egg-info/SOURCES.txt
--rw-rw-r--   0 kevin     (1000) kevin     (1000)        1 2023-05-02 04:08:34.000000 latex_input-0.3.0/latex_input.egg-info/dependency_links.txt
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       38 2023-05-02 04:08:34.000000 latex_input-0.3.0/latex_input.egg-info/requires.txt
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       12 2023-05-02 04:08:34.000000 latex_input-0.3.0/latex_input.egg-info/top_level.txt
--rw-rw-r--   0 kevin     (1000) kevin     (1000)      750 2023-05-02 04:08:07.000000 latex_input-0.3.0/pyproject.toml
--rw-rw-r--   0 kevin     (1000) kevin     (1000)       38 2023-05-02 04:08:34.863424 latex_input-0.3.0/setup.cfg
-drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2023-05-02 04:08:34.863424 latex_input-0.3.0/test/
--rw-rw-r--   0 kevin     (1000) kevin     (1000)     5420 2023-05-01 02:54:53.000000 latex_input-0.3.0/test/test_converter.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2023-05-02 04:12:38.959217 latex_input-0.3.1/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    35149 2023-05-01 02:54:53.000000 latex_input-0.3.1/LICENSE
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1498 2023-05-02 04:12:38.959217 latex_input-0.3.1/PKG-INFO
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      979 2023-05-01 02:54:53.000000 latex_input-0.3.1/README.md
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2023-05-02 04:12:38.959217 latex_input-0.3.1/latex_input/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     7673 2023-05-02 03:48:05.000000 latex_input-0.3.1/latex_input/__main__.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    58755 2023-05-01 02:54:53.000000 latex_input-0.3.1/latex_input/cached_unicode_data.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2023-05-02 04:12:38.959217 latex_input-0.3.1/latex_input/data/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)   105776 2023-05-01 02:54:53.000000 latex_input-0.3.1/latex_input/data/icon.ico
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)   105634 2023-05-01 02:54:53.000000 latex_input-0.3.1/latex_input/data/icon_activated.ico
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     4705 2023-05-02 03:45:34.000000 latex_input-0.3.1/latex_input/input_client_linux.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3713 2023-05-02 03:45:43.000000 latex_input-0.3.1/latex_input/input_client_win.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    10440 2023-05-01 02:54:53.000000 latex_input-0.3.1/latex_input/latex_converter.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1222 2023-05-01 02:54:53.000000 latex_input-0.3.1/latex_input/listener.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     3441 2023-05-01 02:54:53.000000 latex_input-0.3.1/latex_input/parse_unicode_data.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)    67693 2023-05-02 03:18:50.000000 latex_input-0.3.1/latex_input/unicode_data.py
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      372 2023-05-01 02:54:53.000000 latex_input-0.3.1/latex_input/unicode_structs.py
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2023-05-02 04:12:38.959217 latex_input-0.3.1/latex_input.egg-info/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     1498 2023-05-02 04:12:38.000000 latex_input-0.3.1/latex_input.egg-info/PKG-INFO
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      564 2023-05-02 04:12:38.000000 latex_input-0.3.1/latex_input.egg-info/SOURCES.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)        1 2023-05-02 04:12:38.000000 latex_input-0.3.1/latex_input.egg-info/dependency_links.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       45 2023-05-02 04:12:38.000000 latex_input-0.3.1/latex_input.egg-info/requires.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       12 2023-05-02 04:12:38.000000 latex_input-0.3.1/latex_input.egg-info/top_level.txt
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)      764 2023-05-02 04:12:16.000000 latex_input-0.3.1/pyproject.toml
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)       38 2023-05-02 04:12:38.959217 latex_input-0.3.1/setup.cfg
+drwxrwxr-x   0 kevin     (1000) kevin     (1000)        0 2023-05-02 04:12:38.959217 latex_input-0.3.1/test/
+-rw-rw-r--   0 kevin     (1000) kevin     (1000)     5420 2023-05-01 02:54:53.000000 latex_input-0.3.1/test/test_converter.py
```

### Comparing `latex_input-0.3.0/LICENSE` & `latex_input-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `latex_input-0.3.0/PKG-INFO` & `latex_input-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex_input
-Version: 0.3.0
+Version: 0.3.1
 Summary: Use LaTeX-style inputs to write the equivalent unicode characters anywhere
 Author-email: kmgb <kevinmgb@proton.me>
 Project-URL: Homepage, https://github.com/kmgb/latex_input
 Project-URL: Bug Tracker, https://github.com/kmgb/latex_input/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
```

### Comparing `latex_input-0.3.0/README.md` & `latex_input-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `latex_input-0.3.0/latex_input/__main__.py` & `latex_input-0.3.1/latex_input/__main__.py`

 * *Files identical despite different names*

### Comparing `latex_input-0.3.0/latex_input/cached_unicode_data.py` & `latex_input-0.3.1/latex_input/cached_unicode_data.py`

 * *Files identical despite different names*

### Comparing `latex_input-0.3.0/latex_input/data/icon.ico` & `latex_input-0.3.1/latex_input/data/icon.ico`

 * *Files identical despite different names*

### Comparing `latex_input-0.3.0/latex_input/data/icon_activated.ico` & `latex_input-0.3.1/latex_input/data/icon_activated.ico`

 * *Files identical despite different names*

### Comparing `latex_input-0.3.0/latex_input/input_client_linux.py` & `latex_input-0.3.1/latex_input/input_client_linux.py`

 * *Files identical despite different names*

### Comparing `latex_input-0.3.0/latex_input/input_client_win.py` & `latex_input-0.3.1/latex_input/input_client_win.py`

 * *Files identical despite different names*

### Comparing `latex_input-0.3.0/latex_input/latex_converter.py` & `latex_input-0.3.1/latex_input/latex_converter.py`

 * *Files identical despite different names*

### Comparing `latex_input-0.3.0/latex_input/listener.py` & `latex_input-0.3.1/latex_input/listener.py`

 * *Files identical despite different names*

### Comparing `latex_input-0.3.0/latex_input/parse_unicode_data.py` & `latex_input-0.3.1/latex_input/parse_unicode_data.py`

 * *Files identical despite different names*

### Comparing `latex_input-0.3.0/latex_input/unicode_data.py` & `latex_input-0.3.1/latex_input/unicode_data.py`

 * *Files identical despite different names*

### Comparing `latex_input-0.3.0/latex_input.egg-info/PKG-INFO` & `latex_input-0.3.1/latex_input.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex-input
-Version: 0.3.0
+Version: 0.3.1
 Summary: Use LaTeX-style inputs to write the equivalent unicode characters anywhere
 Author-email: kmgb <kevinmgb@proton.me>
 Project-URL: Homepage, https://github.com/kmgb/latex_input
 Project-URL: Bug Tracker, https://github.com/kmgb/latex_input/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
```

### Comparing `latex_input-0.3.0/latex_input.egg-info/SOURCES.txt` & `latex_input-0.3.1/latex_input.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `latex_input-0.3.0/pyproject.toml` & `latex_input-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "latex_input"
 description = "Use LaTeX-style inputs to write the equivalent unicode characters anywhere"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     { name = "kmgb", email = "kevinmgb@proton.me" }
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "PyQt6",
     "ahk",
     "ahk-binary",
+    "pynput",
     "keyboard==0.13.5"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 ]
```

### Comparing `latex_input-0.3.0/test/test_converter.py` & `latex_input-0.3.1/test/test_converter.py`

 * *Files identical despite different names*

