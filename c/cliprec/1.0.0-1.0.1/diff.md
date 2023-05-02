# Comparing `tmp/cliprec-1.0.0.tar.gz` & `tmp/cliprec-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliprec-1.0.0.tar", last modified: Mon May  1 17:42:30 2023, max compression
+gzip compressed data, was "cliprec-1.0.1.tar", last modified: Tue May  2 17:15:36 2023, max compression
```

## Comparing `cliprec-1.0.0.tar` & `cliprec-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 17:42:30.807820 cliprec-1.0.0/
--rw-rw-rw-   0        0        0     3238 2023-05-01 17:13:01.000000 cliprec-1.0.0/.gitignore
--rw-rw-rw-   0        0        0    35823 2023-05-01 17:13:01.000000 cliprec-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    43254 2023-05-01 17:42:30.806821 cliprec-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1101 2023-05-01 17:34:56.000000 cliprec-1.0.0/README.md
--rw-rw-rw-   0        0        0     1134 2023-05-01 17:24:27.000000 cliprec-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 17:42:30.807820 cliprec-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 17:42:30.772629 cliprec-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 17:42:30.782617 cliprec-1.0.0/src/cliprec/
--rw-rw-rw-   0        0        0     1109 2023-05-01 17:37:10.000000 cliprec-1.0.0/src/cliprec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 17:42:30.803820 cliprec-1.0.0/src/cliprec.egg-info/
--rw-rw-rw-   0        0        0    43254 2023-05-01 17:42:30.000000 cliprec-1.0.0/src/cliprec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-01 17:42:30.000000 cliprec-1.0.0/src/cliprec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 17:42:30.000000 cliprec-1.0.0/src/cliprec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-01 17:42:30.000000 cliprec-1.0.0/src/cliprec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 17:15:36.062692 cliprec-1.0.1/
+-rw-rw-rw-   0        0        0     3238 2023-05-01 17:13:01.000000 cliprec-1.0.1/.gitignore
+-rw-rw-rw-   0        0        0    35823 2023-05-01 17:13:01.000000 cliprec-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    43254 2023-05-02 17:15:36.062692 cliprec-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1101 2023-05-01 17:34:56.000000 cliprec-1.0.1/README.md
+-rwxrwxrwx   0        0        0  7794838 2023-05-01 17:38:03.000000 cliprec-1.0.1/cliprec.exe
+-rw-rw-rw-   0        0        0     1177 2023-05-02 17:07:58.000000 cliprec-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 17:15:36.062692 cliprec-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 17:15:36.000215 cliprec-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 17:15:36.031436 cliprec-1.0.1/src/cliprec/
+-rw-rw-rw-   0        0        0     1109 2023-05-02 17:08:11.000000 cliprec-1.0.1/src/cliprec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:15:36.062692 cliprec-1.0.1/src/cliprec.egg-info/
+-rw-rw-rw-   0        0        0    43254 2023-05-02 17:15:35.000000 cliprec-1.0.1/src/cliprec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-05-02 17:15:35.000000 cliprec-1.0.1/src/cliprec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 17:15:35.000000 cliprec-1.0.1/src/cliprec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-02 17:15:35.000000 cliprec-1.0.1/src/cliprec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 17:15:35.000000 cliprec-1.0.1/src/cliprec.egg-info/top_level.txt
```

### Comparing `cliprec-1.0.0/.gitignore` & `cliprec-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cliprec-1.0.0/LICENSE` & `cliprec-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cliprec-1.0.0/PKG-INFO` & `cliprec-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliprec
-Version: 1.0.0
+Version: 1.0.1
 Summary: A cross-platform clipboard monitoring and recording tool. Uses pyperclip. Only works for text.
 Author-email: Al Sweigart <al@inventwithpython.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cliprec-1.0.0/README.md` & `cliprec-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cliprec-1.0.0/pyproject.toml` & `cliprec-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm"]
+requires = ["setuptools", "setuptools-scm", "pyperclip"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cliprec"
 authors = [
     {name = "Al Sweigart", email = "al@inventwithpython.com"},
 ]
@@ -21,14 +21,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 2",
     "Programming Language :: Python :: 3",
 ]
 requires-python = ">=2.7"
 dynamic = ["version"]
+dependencies = ['pyperclip']
 
 [project.urls]
 "Homepage" = "https://github.com/asweigart/cliprec"
 "Bug Tracker" = "https://github.com/asweigart/cliprec/issues"
 
 [tool.setuptools.dynamic]
 version = {attr = "cliprec.__version__"}
```

### Comparing `cliprec-1.0.0/src/cliprec/__init__.py` & `cliprec-1.0.1/src/cliprec/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """A cross-platform clipboard monitoring and recording tool. Uses pyperclip. Only works for text.
 By Al Sweigart al@inventwithpython.com"""
 
 import pyperclip
 import time
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 def main():
     print('Recording clipboard... (Ctrl-C to stop)')
     all_content = []
     previous_content = pyperclip.paste()  # Ignore current clipboard contents.
     try:
         while True:
```

### Comparing `cliprec-1.0.0/src/cliprec.egg-info/PKG-INFO` & `cliprec-1.0.1/src/cliprec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliprec
-Version: 1.0.0
+Version: 1.0.1
 Summary: A cross-platform clipboard monitoring and recording tool. Uses pyperclip. Only works for text.
 Author-email: Al Sweigart <al@inventwithpython.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

