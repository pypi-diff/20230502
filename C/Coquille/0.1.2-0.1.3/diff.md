# Comparing `tmp/Coquille-0.1.2.tar.gz` & `tmp/Coquille-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Coquille-0.1.2.tar", last modified: Tue May  2 21:37:29 2023, max compression
+gzip compressed data, was "Coquille-0.1.3.tar", last modified: Tue May  2 21:50:24 2023, max compression
```

## Comparing `Coquille-0.1.2.tar` & `Coquille-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.377598 Coquille-0.1.2/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1813 2023-05-02 17:54:21.000000 Coquille-0.1.2/.gitignore
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      550 2023-05-02 19:03:38.000000 Coquille-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2023-05-02 18:38:39.000000 Coquille-0.1.2/LICENSE
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2348 2023-05-02 21:37:29.377598 Coquille-0.1.2/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1971 2023-05-02 21:36:06.000000 Coquille-0.1.2/README.md
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.370931 Coquille-0.1.2/examples/
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.374265 Coquille-0.1.2/examples/coquille_context/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      437 2023-05-02 18:39:46.000000 Coquille-0.1.2/examples/coquille_context/__main__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    31985 2023-05-02 18:20:06.000000 Coquille-0.1.2/examples/coquille_context/screenshot.png
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.374265 Coquille-0.1.2/examples/coquille_print/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      436 2023-05-02 21:36:06.000000 Coquille-0.1.2/examples/coquille_print/__main__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       45 2023-05-02 21:36:06.000000 Coquille-0.1.2/examples/coquille_print/output.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    35689 2023-05-02 21:36:06.000000 Coquille-0.1.2/examples/coquille_print/screenshot.png
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      454 2023-05-02 21:36:13.000000 Coquille-0.1.2/pyproject.toml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2023-05-02 21:37:29.377598 Coquille-0.1.2/setup.cfg
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      115 2023-05-02 21:08:25.000000 Coquille-0.1.2/setup.py
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.370931 Coquille-0.1.2/src/
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.374265 Coquille-0.1.2/src/Coquille.egg-info/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2348 2023-05-02 21:37:29.000000 Coquille-0.1.2/src/Coquille.egg-info/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      610 2023-05-02 21:37:29.000000 Coquille-0.1.2/src/Coquille.egg-info/SOURCES.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2023-05-02 21:37:29.000000 Coquille-0.1.2/src/Coquille.egg-info/dependency_links.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       23 2023-05-02 21:37:29.000000 Coquille-0.1.2/src/Coquille.egg-info/requires.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        9 2023-05-02 21:37:29.000000 Coquille-0.1.2/src/Coquille.egg-info/top_level.txt
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.377598 Coquille-0.1.2/src/coquille/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       32 2023-05-02 14:44:50.000000 Coquille-0.1.2/src/coquille/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     5731 2023-05-02 21:36:06.000000 Coquille-0.1.2/src/coquille/coquille.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    10596 2023-05-02 21:08:25.000000 Coquille-0.1.2/src/coquille/sequences.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      340 2023-05-02 18:59:39.000000 Coquille-0.1.2/src/coquille/typeshed.py
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.377598 Coquille-0.1.2/tests/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:08:25.000000 Coquille-0.1.2/tests/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1081 2023-05-02 21:08:25.000000 Coquille-0.1.2/tests/coquille_test.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     4219 2023-05-02 21:08:25.000000 Coquille-0.1.2/tests/sequences_test.py
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.454930 Coquille-0.1.3/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1813 2023-05-02 17:54:21.000000 Coquille-0.1.3/.gitignore
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      550 2023-05-02 19:03:38.000000 Coquille-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2023-05-02 18:38:39.000000 Coquille-0.1.3/LICENSE
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2892 2023-05-02 21:50:24.454930 Coquille-0.1.3/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2515 2023-05-02 21:48:53.000000 Coquille-0.1.3/README.md
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.451597 Coquille-0.1.3/examples/
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.454930 Coquille-0.1.3/examples/coquille_context/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      437 2023-05-02 18:39:46.000000 Coquille-0.1.3/examples/coquille_context/__main__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)    31985 2023-05-02 18:20:06.000000 Coquille-0.1.3/examples/coquille_context/screenshot.png
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.454930 Coquille-0.1.3/examples/coquille_print/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      436 2023-05-02 21:36:06.000000 Coquille-0.1.3/examples/coquille_print/__main__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       45 2023-05-02 21:36:06.000000 Coquille-0.1.3/examples/coquille_print/output.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)    35689 2023-05-02 21:36:06.000000 Coquille-0.1.3/examples/coquille_print/screenshot.png
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      454 2023-05-02 21:50:18.000000 Coquille-0.1.3/pyproject.toml
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2023-05-02 21:50:24.454930 Coquille-0.1.3/setup.cfg
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      115 2023-05-02 21:08:25.000000 Coquille-0.1.3/setup.py
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.451597 Coquille-0.1.3/src/
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.454930 Coquille-0.1.3/src/Coquille.egg-info/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2892 2023-05-02 21:50:24.000000 Coquille-0.1.3/src/Coquille.egg-info/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      610 2023-05-02 21:50:24.000000 Coquille-0.1.3/src/Coquille.egg-info/SOURCES.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2023-05-02 21:50:24.000000 Coquille-0.1.3/src/Coquille.egg-info/dependency_links.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       23 2023-05-02 21:50:24.000000 Coquille-0.1.3/src/Coquille.egg-info/requires.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        9 2023-05-02 21:50:24.000000 Coquille-0.1.3/src/Coquille.egg-info/top_level.txt
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.454930 Coquille-0.1.3/src/coquille/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       32 2023-05-02 14:44:50.000000 Coquille-0.1.3/src/coquille/__init__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     5731 2023-05-02 21:36:06.000000 Coquille-0.1.3/src/coquille/coquille.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)    10596 2023-05-02 21:08:25.000000 Coquille-0.1.3/src/coquille/sequences.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      340 2023-05-02 18:59:39.000000 Coquille-0.1.3/src/coquille/typeshed.py
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:50:24.454930 Coquille-0.1.3/tests/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:08:25.000000 Coquille-0.1.3/tests/__init__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1081 2023-05-02 21:08:25.000000 Coquille-0.1.3/tests/coquille_test.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     4219 2023-05-02 21:08:25.000000 Coquille-0.1.3/tests/sequences_test.py
```

### Comparing `Coquille-0.1.2/.gitignore` & `Coquille-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.2/.pre-commit-config.yaml` & `Coquille-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.2/LICENSE` & `Coquille-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.2/PKG-INFO` & `Coquille-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,22 @@
-Metadata-Version: 2.1
-Name: Coquille
-Version: 0.1.2
-Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
-Author: Qexat
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Coquille
 
 Coquille (IPA: `/kɔ.kij/`, english: 'shell' or 'typo') is a library that wraps terminal escape sequences to easily apply them to a stream.
 
 ## Notes
 
 Requires Python 3.9 or higher.
 
 This library attempts to cover as many escape sequences as possible ; but it is not an exhaustive list, some might be missing. Also, you might find that few have no effect on your terminal emulator.
 
+This library is based on the following resources:
+
+- The Wikipedia page: <https://en.m.wikipedia.org/wiki/ANSI_escape_code>
+- Some Microsoft documentation about console virtual terminal sequences: <https://learn.microsoft.com/en-us/windows/console/console-virtual-terminal-sequences>
+
 ## Install
 
 ### Normal installation
 
 ```sh
 pip install coquille
 ```
@@ -45,14 +37,16 @@
 
 ```sh
 coverage report -m
 ```
 
 ## Examples
 
+Even though the examples are mostly showcasing [SGR escape sequences](https://en.wikipedia.org/wiki/ANSI_escape_code#SGR_(Select_Graphic_Rendition)_parameters) (because they are pretty visible), Coquille can do more! See the [documentation](#documentation).
+
 ### Coquille context manager
 
 ```py
 from coquille import Coquille
 from coquille.sequences import bold, fg_magenta, italic
 
 print("Hello World!")
```

### Comparing `Coquille-0.1.2/examples/coquille_context/screenshot.png` & `Coquille-0.1.3/examples/coquille_context/screenshot.png`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.2/examples/coquille_print/screenshot.png` & `Coquille-0.1.3/examples/coquille_print/screenshot.png`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.2/src/Coquille.egg-info/PKG-INFO` & `Coquille-0.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 0.1.2
+Version: 0.1.3
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -17,14 +17,19 @@
 
 ## Notes
 
 Requires Python 3.9 or higher.
 
 This library attempts to cover as many escape sequences as possible ; but it is not an exhaustive list, some might be missing. Also, you might find that few have no effect on your terminal emulator.
 
+This library is based on the following resources:
+
+- The Wikipedia page: <https://en.m.wikipedia.org/wiki/ANSI_escape_code>
+- Some Microsoft documentation about console virtual terminal sequences: <https://learn.microsoft.com/en-us/windows/console/console-virtual-terminal-sequences>
+
 ## Install
 
 ### Normal installation
 
 ```sh
 pip install coquille
 ```
@@ -45,14 +50,16 @@
 
 ```sh
 coverage report -m
 ```
 
 ## Examples
 
+Even though the examples are mostly showcasing [SGR escape sequences](https://en.wikipedia.org/wiki/ANSI_escape_code#SGR_(Select_Graphic_Rendition)_parameters) (because they are pretty visible), Coquille can do more! See the [documentation](#documentation).
+
 ### Coquille context manager
 
 ```py
 from coquille import Coquille
 from coquille.sequences import bold, fg_magenta, italic
 
 print("Hello World!")
```

### Comparing `Coquille-0.1.2/src/Coquille.egg-info/SOURCES.txt` & `Coquille-0.1.3/src/Coquille.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.2/src/coquille/coquille.py` & `Coquille-0.1.3/src/coquille/coquille.py`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.2/src/coquille/sequences.py` & `Coquille-0.1.3/src/coquille/sequences.py`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.2/tests/coquille_test.py` & `Coquille-0.1.3/tests/coquille_test.py`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.2/tests/sequences_test.py` & `Coquille-0.1.3/tests/sequences_test.py`

 * *Files identical despite different names*

