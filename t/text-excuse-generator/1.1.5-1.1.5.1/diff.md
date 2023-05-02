# Comparing `tmp/text_excuse_generator-1.1.5.tar.gz` & `tmp/text_excuse_generator-1.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_excuse_generator-1.1.5.tar", last modified: Tue May  2 05:31:08 2023, max compression
+gzip compressed data, was "text_excuse_generator-1.1.5.1.tar", last modified: Tue May  2 05:41:49 2023, max compression
```

## Comparing `text_excuse_generator-1.1.5.tar` & `text_excuse_generator-1.1.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-05-02 05:31:08.074087 text_excuse_generator-1.1.5/
--rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 text_excuse_generator-1.1.5/LICENSE
--rw-r--r--   0 Huck       (503) staff       (20)    12367 2023-05-02 05:31:08.073909 text_excuse_generator-1.1.5/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)       38 2023-05-02 05:31:08.074141 text_excuse_generator-1.1.5/setup.cfg
--rw-r--r--   0 Huck       (503) staff       (20)     1089 2023-05-02 05:31:07.000000 text_excuse_generator-1.1.5/setup.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-05-02 05:31:08.072842 text_excuse_generator-1.1.5/text_excuse_generator/
--rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 03:34:45.000000 text_excuse_generator-1.1.5/text_excuse_generator/__init__.py
--rw-r--r--   0 Huck       (503) staff       (20)    12322 2023-05-02 05:19:07.000000 text_excuse_generator-1.1.5/text_excuse_generator/excuse_generator.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-05-02 05:31:08.073685 text_excuse_generator-1.1.5/text_excuse_generator.egg-info/
--rw-r--r--   0 Huck       (503) staff       (20)    12367 2023-05-02 05:31:08.000000 text_excuse_generator-1.1.5/text_excuse_generator.egg-info/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)      316 2023-05-02 05:31:08.000000 text_excuse_generator-1.1.5/text_excuse_generator.egg-info/SOURCES.txt
--rw-r--r--   0 Huck       (503) staff       (20)        1 2023-05-02 05:31:08.000000 text_excuse_generator-1.1.5/text_excuse_generator.egg-info/dependency_links.txt
--rw-r--r--   0 Huck       (503) staff       (20)       41 2023-05-02 05:31:08.000000 text_excuse_generator-1.1.5/text_excuse_generator.egg-info/requires.txt
--rw-r--r--   0 Huck       (503) staff       (20)       22 2023-05-02 05:31:08.000000 text_excuse_generator-1.1.5/text_excuse_generator.egg-info/top_level.txt
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-05-02 05:41:49.119761 text_excuse_generator-1.1.5.1/
+-rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 text_excuse_generator-1.1.5.1/LICENSE
+-rw-r--r--   0 Huck       (503) staff       (20)    12461 2023-05-02 05:41:49.119519 text_excuse_generator-1.1.5.1/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)       38 2023-05-02 05:41:49.119813 text_excuse_generator-1.1.5.1/setup.cfg
+-rw-r--r--   0 Huck       (503) staff       (20)     1091 2023-05-02 05:41:48.000000 text_excuse_generator-1.1.5.1/setup.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-05-02 05:41:49.118039 text_excuse_generator-1.1.5.1/text_excuse_generator/
+-rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 03:34:45.000000 text_excuse_generator-1.1.5.1/text_excuse_generator/__init__.py
+-rw-r--r--   0 Huck       (503) staff       (20)    12322 2023-05-02 05:19:07.000000 text_excuse_generator-1.1.5.1/text_excuse_generator/excuse_generator.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-05-02 05:41:49.119007 text_excuse_generator-1.1.5.1/text_excuse_generator.egg-info/
+-rw-r--r--   0 Huck       (503) staff       (20)    12461 2023-05-02 05:41:49.000000 text_excuse_generator-1.1.5.1/text_excuse_generator.egg-info/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)      316 2023-05-02 05:41:49.000000 text_excuse_generator-1.1.5.1/text_excuse_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 Huck       (503) staff       (20)        1 2023-05-02 05:41:49.000000 text_excuse_generator-1.1.5.1/text_excuse_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       41 2023-05-02 05:41:49.000000 text_excuse_generator-1.1.5.1/text_excuse_generator.egg-info/requires.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       22 2023-05-02 05:41:49.000000 text_excuse_generator-1.1.5.1/text_excuse_generator.egg-info/top_level.txt
```

### Comparing `text_excuse_generator-1.1.5/LICENSE` & `text_excuse_generator-1.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `text_excuse_generator-1.1.5/PKG-INFO` & `text_excuse_generator-1.1.5.1/text_excuse_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: text_excuse_generator
-Version: 1.1.5
+Name: text-excuse-generator
+Version: 1.1.5.1
 Summary: Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it
 Home-page: https://github.com/Huckdirks/text-excuse-generator
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 Keywords: text excuse generator,openai,twilio,text message,GPT-3.5
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
@@ -105,14 +105,16 @@
 Simply run:
 ```bash
 pip install text-excuse-generator
 ```
 To import the module into your python file, put this at the top of your file:
 ```python
 from text_excuse_generator.excuse_generator import *
+# or
+import text_excuse_generator.excuse_generator as teg # or whatever you want to call it
 ```
 Or you can import the individual functions.
 
 #### `generate_excuse()` takes in:
 ```python
 generate_excuse(USER: str, RECIPIENT: str, PROBLEM: str, EXCUSE: str, SEND_TEXT: bool) -> (str | None)
 ```
```

### Comparing `text_excuse_generator-1.1.5/setup.py` & `text_excuse_generator-1.1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 README_PATH = join(dirname(__file__), "docs/README.md")
 
 with open(README_PATH, "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 setup(
     name = "text_excuse_generator",
-	version = "1.1.5",
+	version = "1.1.5.1",
     author = "Huck Dirksmeier",
     author_email = "Huckdirks@gmail.com",
     description = "Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it",
     long_description = LONG_DESCRIPTION,
     long_description_content_type = "text/markdown",
     url = "https://github.com/Huckdirks/text-excuse-generator",
     packages = find_packages(),
```

### Comparing `text_excuse_generator-1.1.5/text_excuse_generator/excuse_generator.py` & `text_excuse_generator-1.1.5.1/text_excuse_generator/excuse_generator.py`

 * *Files identical despite different names*

### Comparing `text_excuse_generator-1.1.5/text_excuse_generator.egg-info/PKG-INFO` & `text_excuse_generator-1.1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: text-excuse-generator
-Version: 1.1.5
+Name: text_excuse_generator
+Version: 1.1.5.1
 Summary: Uses Open AI's GPT-3.5 model to create an excuse from given parameters & text it
 Home-page: https://github.com/Huckdirks/text-excuse-generator
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
 Keywords: text excuse generator,openai,twilio,text message,GPT-3.5
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
@@ -105,14 +105,16 @@
 Simply run:
 ```bash
 pip install text-excuse-generator
 ```
 To import the module into your python file, put this at the top of your file:
 ```python
 from text_excuse_generator.excuse_generator import *
+# or
+import text_excuse_generator.excuse_generator as teg # or whatever you want to call it
 ```
 Or you can import the individual functions.
 
 #### `generate_excuse()` takes in:
 ```python
 generate_excuse(USER: str, RECIPIENT: str, PROBLEM: str, EXCUSE: str, SEND_TEXT: bool) -> (str | None)
 ```
```

