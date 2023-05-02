# Comparing `tmp/Coquille-0.1.1.tar.gz` & `tmp/Coquille-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Coquille-0.1.1.tar", last modified: Tue May  2 20:56:59 2023, max compression
+gzip compressed data, was "Coquille-0.1.2.tar", last modified: Tue May  2 21:37:29 2023, max compression
```

## Comparing `Coquille-0.1.1.tar` & `Coquille-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 20:56:59.689721 Coquille-0.1.1/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1813 2023-05-02 17:54:21.000000 Coquille-0.1.1/.gitignore
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      550 2023-05-02 19:03:38.000000 Coquille-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2023-05-02 18:38:39.000000 Coquille-0.1.1/LICENSE
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1480 2023-05-02 20:56:59.689721 Coquille-0.1.1/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1103 2023-05-02 19:24:02.000000 Coquille-0.1.1/README.md
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 20:56:59.686388 Coquille-0.1.1/examples/
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 20:56:59.689721 Coquille-0.1.1/examples/coquille_context/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      437 2023-05-02 18:39:46.000000 Coquille-0.1.1/examples/coquille_context/__main__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    31985 2023-05-02 18:20:06.000000 Coquille-0.1.1/examples/coquille_context/screenshot.png
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      454 2023-05-02 20:56:46.000000 Coquille-0.1.1/pyproject.toml
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2023-05-02 20:56:59.689721 Coquille-0.1.1/setup.cfg
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      115 2023-05-02 20:03:01.000000 Coquille-0.1.1/setup.py
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 20:56:59.686388 Coquille-0.1.1/src/
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 20:56:59.689721 Coquille-0.1.1/src/Coquille.egg-info/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1480 2023-05-02 20:56:59.000000 Coquille-0.1.1/src/Coquille.egg-info/PKG-INFO
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      500 2023-05-02 20:56:59.000000 Coquille-0.1.1/src/Coquille.egg-info/SOURCES.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2023-05-02 20:56:59.000000 Coquille-0.1.1/src/Coquille.egg-info/dependency_links.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       23 2023-05-02 20:56:59.000000 Coquille-0.1.1/src/Coquille.egg-info/requires.txt
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        9 2023-05-02 20:56:59.000000 Coquille-0.1.1/src/Coquille.egg-info/top_level.txt
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 20:56:59.689721 Coquille-0.1.1/src/coquille/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)       32 2023-05-02 14:44:50.000000 Coquille-0.1.1/src/coquille/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     5735 2023-05-02 20:49:56.000000 Coquille-0.1.1/src/coquille/coquille.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)    10596 2023-05-02 20:27:12.000000 Coquille-0.1.1/src/coquille/sequences.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)      340 2023-05-02 18:59:39.000000 Coquille-0.1.1/src/coquille/typeshed.py
-drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 20:56:59.689721 Coquille-0.1.1/tests/
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 19:55:01.000000 Coquille-0.1.1/tests/__init__.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1081 2023-05-02 20:50:32.000000 Coquille-0.1.1/tests/coquille_test.py
--rw-r--r--   0 clarisse  (1000) clarisse  (1000)     4219 2023-05-02 20:30:32.000000 Coquille-0.1.1/tests/sequences_test.py
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.377598 Coquille-0.1.2/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1813 2023-05-02 17:54:21.000000 Coquille-0.1.2/.gitignore
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      550 2023-05-02 19:03:38.000000 Coquille-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1062 2023-05-02 18:38:39.000000 Coquille-0.1.2/LICENSE
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2348 2023-05-02 21:37:29.377598 Coquille-0.1.2/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1971 2023-05-02 21:36:06.000000 Coquille-0.1.2/README.md
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.370931 Coquille-0.1.2/examples/
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.374265 Coquille-0.1.2/examples/coquille_context/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      437 2023-05-02 18:39:46.000000 Coquille-0.1.2/examples/coquille_context/__main__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)    31985 2023-05-02 18:20:06.000000 Coquille-0.1.2/examples/coquille_context/screenshot.png
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.374265 Coquille-0.1.2/examples/coquille_print/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      436 2023-05-02 21:36:06.000000 Coquille-0.1.2/examples/coquille_print/__main__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       45 2023-05-02 21:36:06.000000 Coquille-0.1.2/examples/coquille_print/output.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)    35689 2023-05-02 21:36:06.000000 Coquille-0.1.2/examples/coquille_print/screenshot.png
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      454 2023-05-02 21:36:13.000000 Coquille-0.1.2/pyproject.toml
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       38 2023-05-02 21:37:29.377598 Coquille-0.1.2/setup.cfg
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      115 2023-05-02 21:08:25.000000 Coquille-0.1.2/setup.py
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.370931 Coquille-0.1.2/src/
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.374265 Coquille-0.1.2/src/Coquille.egg-info/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     2348 2023-05-02 21:37:29.000000 Coquille-0.1.2/src/Coquille.egg-info/PKG-INFO
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      610 2023-05-02 21:37:29.000000 Coquille-0.1.2/src/Coquille.egg-info/SOURCES.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        1 2023-05-02 21:37:29.000000 Coquille-0.1.2/src/Coquille.egg-info/dependency_links.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       23 2023-05-02 21:37:29.000000 Coquille-0.1.2/src/Coquille.egg-info/requires.txt
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        9 2023-05-02 21:37:29.000000 Coquille-0.1.2/src/Coquille.egg-info/top_level.txt
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.377598 Coquille-0.1.2/src/coquille/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)       32 2023-05-02 14:44:50.000000 Coquille-0.1.2/src/coquille/__init__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     5731 2023-05-02 21:36:06.000000 Coquille-0.1.2/src/coquille/coquille.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)    10596 2023-05-02 21:08:25.000000 Coquille-0.1.2/src/coquille/sequences.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)      340 2023-05-02 18:59:39.000000 Coquille-0.1.2/src/coquille/typeshed.py
+drwxr-xr-x   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:37:29.377598 Coquille-0.1.2/tests/
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)        0 2023-05-02 21:08:25.000000 Coquille-0.1.2/tests/__init__.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     1081 2023-05-02 21:08:25.000000 Coquille-0.1.2/tests/coquille_test.py
+-rw-r--r--   0 clarisse  (1000) clarisse  (1000)     4219 2023-05-02 21:08:25.000000 Coquille-0.1.2/tests/sequences_test.py
```

### Comparing `Coquille-0.1.1/.gitignore` & `Coquille-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.1/.pre-commit-config.yaml` & `Coquille-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.1/LICENSE` & `Coquille-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.1/PKG-INFO` & `Coquille-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 0.1.1
+Version: 0.1.2
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -17,14 +17,40 @@
 
 ## Notes
 
 Requires Python 3.9 or higher.
 
 This library attempts to cover as many escape sequences as possible ; but it is not an exhaustive list, some might be missing. Also, you might find that few have no effect on your terminal emulator.
 
+## Install
+
+### Normal installation
+
+```sh
+pip install coquille
+```
+
+### Dev installation
+
+```sh
+pip install coquille[dev]
+```
+
+This allows you to run the tests:
+
+```sh
+coverage run -m pytest
+```
+
+Then check the coverage:
+
+```sh
+coverage report -m
+```
+
 ## Examples
 
 ### Coquille context manager
 
 ```py
 from coquille import Coquille
 from coquille.sequences import bold, fg_magenta, italic
@@ -40,10 +66,29 @@
 print("Oh, we are back to normal now...")
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_context/screenshot.png)
 
 Source code: [examples/coquille_context/](https://github.com/qexat/Coquille/blob/main/examples/coquille_context/__main__.py)
 
+### Coquille.print()
+
+```py
+from coquille import Coquille
+from coquille.sequences import bold, fg_blue, fg_magenta, italic
+
+print("Hello World!")
+
+Coquille.print("Hello World, but in magenta and italic!", fg_magenta, italic)
+
+with open("examples/coquille_print/output.txt", "w") as my_file:
+    Coquille.print("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
+
+```
+
+![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_print/screenshot.png)
+
+Source code: [examples/coquille_print/](https://github.com/qexat/Coquille/blob/main/examples/coquille_print/__main__.py)
+
 ## Documentation
 
 Coming soon! 🚧
```

### Comparing `Coquille-0.1.1/examples/coquille_context/screenshot.png` & `Coquille-0.1.2/examples/coquille_context/screenshot.png`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.1/src/Coquille.egg-info/PKG-INFO` & `Coquille-0.1.2/src/Coquille.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 0.1.1
+Version: 0.1.2
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -17,14 +17,40 @@
 
 ## Notes
 
 Requires Python 3.9 or higher.
 
 This library attempts to cover as many escape sequences as possible ; but it is not an exhaustive list, some might be missing. Also, you might find that few have no effect on your terminal emulator.
 
+## Install
+
+### Normal installation
+
+```sh
+pip install coquille
+```
+
+### Dev installation
+
+```sh
+pip install coquille[dev]
+```
+
+This allows you to run the tests:
+
+```sh
+coverage run -m pytest
+```
+
+Then check the coverage:
+
+```sh
+coverage report -m
+```
+
 ## Examples
 
 ### Coquille context manager
 
 ```py
 from coquille import Coquille
 from coquille.sequences import bold, fg_magenta, italic
@@ -40,10 +66,29 @@
 print("Oh, we are back to normal now...")
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_context/screenshot.png)
 
 Source code: [examples/coquille_context/](https://github.com/qexat/Coquille/blob/main/examples/coquille_context/__main__.py)
 
+### Coquille.print()
+
+```py
+from coquille import Coquille
+from coquille.sequences import bold, fg_blue, fg_magenta, italic
+
+print("Hello World!")
+
+Coquille.print("Hello World, but in magenta and italic!", fg_magenta, italic)
+
+with open("examples/coquille_print/output.txt", "w") as my_file:
+    Coquille.print("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
+
+```
+
+![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_print/screenshot.png)
+
+Source code: [examples/coquille_print/](https://github.com/qexat/Coquille/blob/main/examples/coquille_print/__main__.py)
+
 ## Documentation
 
 Coming soon! 🚧
```

### Comparing `Coquille-0.1.1/src/coquille/coquille.py` & `Coquille-0.1.2/src/coquille/coquille.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         text: str,
         *sequences: EscapeSequence,
         end: str | None = "\n",
         file: SupportsWrite[str] | None = None,
     ) -> None:
         """
         A function relatively similar to built-in `print`, but with
-        support of escape sequences that are prepended before the printed
+        support of escape sequences that are prepended to the printed
         text.
 
         Example:
         ```py
         >>> from coquille.sequences import fg_magenta, italic
         >>> Coquille.print("Hello World!", fg_magenta, italic)
         Hello World!
```

### Comparing `Coquille-0.1.1/src/coquille/sequences.py` & `Coquille-0.1.2/src/coquille/sequences.py`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.1/tests/coquille_test.py` & `Coquille-0.1.2/tests/coquille_test.py`

 * *Files identical despite different names*

### Comparing `Coquille-0.1.1/tests/sequences_test.py` & `Coquille-0.1.2/tests/sequences_test.py`

 * *Files identical despite different names*

