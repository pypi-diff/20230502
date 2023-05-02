# Comparing `tmp/fastphrase-0.0.4.tar.gz` & `tmp/fastphrase-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastphrase-0.0.4.tar", last modified: Tue May  2 08:28:15 2023, max compression
+gzip compressed data, was "fastphrase-0.0.5.tar", last modified: Tue May  2 08:54:57 2023, max compression
```

## Comparing `fastphrase-0.0.4.tar` & `fastphrase-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       63 2023-04-30 14:14:30.770025 fastphrase-0.0.4/README.md
--rw-r--r--   0        0        0       49 2023-05-02 08:28:00.049969 fastphrase-0.0.4/fastphrase/__about__.py
--rw-r--r--   0        0        0        0 2023-04-29 08:06:05.177892 fastphrase-0.0.4/fastphrase/__init__.py
--rw-r--r--   0        0        0      138 2023-05-01 16:04:06.354595 fastphrase-0.0.4/fastphrase/__main__.py
--rw-r--r--   0        0        0       35 2023-04-30 14:14:47.325952 fastphrase-0.0.4/fastphrase/cli/__init__.py
--rw-r--r--   0        0        0     2991 2023-05-01 16:14:19.800097 fastphrase-0.0.4/fastphrase/cli/app.py
--rw-r--r--   0        0        0        0 2023-04-29 10:06:36.749726 fastphrase-0.0.4/fastphrase/core/__init__.py
--rw-r--r--   0        0        0     2131 2023-05-01 15:06:03.898947 fastphrase-0.0.4/fastphrase/core/passphraser.py
--rw-r--r--   0        0        0     1094 2023-05-02 08:27:44.390384 fastphrase-0.0.4/fastphrase/core/pathkeeper.py
--rw-r--r--   0        0        0     1485 2023-05-01 15:06:03.906947 fastphrase-0.0.4/fastphrase/core/wordlist.py
--rw-r--r--   0        0        0    13116 2023-04-30 10:58:56.712620 fastphrase-0.0.4/fastphrase/data/dict/bip0039.txt
--rw-r--r--   0        0        0    62144 2023-04-29 13:31:18.523600 fastphrase-0.0.4/fastphrase/data/dict/eff_long.txt
--rw-r--r--   0        0        0    13660 2023-04-30 10:02:38.978774 fastphrase-0.0.4/fastphrase/data/dict/eff_short1.txt
--rw-r--r--   0        0        0    17258 2023-04-30 10:02:56.114630 fastphrase-0.0.4/fastphrase/data/dict/eff_short2.txt
--rw-r--r--   0        0        0     2929 2023-05-02 08:28:15.449572 fastphrase-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 fastphrase-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       63 2023-04-30 14:14:30.770025 fastphrase-0.0.5/README.md
+-rw-r--r--   0        0        0       49 2023-05-02 08:54:17.365806 fastphrase-0.0.5/fastphrase/__about__.py
+-rw-r--r--   0        0        0        0 2023-04-29 08:06:05.177892 fastphrase-0.0.5/fastphrase/__init__.py
+-rw-r--r--   0        0        0      138 2023-05-02 08:52:13.546342 fastphrase-0.0.5/fastphrase/__main__.py
+-rw-r--r--   0        0        0       35 2023-04-30 14:14:47.325952 fastphrase-0.0.5/fastphrase/cli/__init__.py
+-rw-r--r--   0        0        0     2991 2023-05-01 16:14:19.800097 fastphrase-0.0.5/fastphrase/cli/app.py
+-rw-r--r--   0        0        0        0 2023-04-29 10:06:36.749726 fastphrase-0.0.5/fastphrase/core/__init__.py
+-rw-r--r--   0        0        0     2131 2023-05-01 15:06:03.898947 fastphrase-0.0.5/fastphrase/core/passphraser.py
+-rw-r--r--   0        0        0     1130 2023-05-02 08:52:05.062380 fastphrase-0.0.5/fastphrase/core/pathkeeper.py
+-rw-r--r--   0        0        0     1485 2023-05-01 15:06:03.906947 fastphrase-0.0.5/fastphrase/core/wordlist.py
+-rw-r--r--   0        0        0    13116 2023-04-30 10:58:56.712620 fastphrase-0.0.5/fastphrase/data/dict/bip0039.txt
+-rw-r--r--   0        0        0    62144 2023-04-29 13:31:18.523600 fastphrase-0.0.5/fastphrase/data/dict/eff_long.txt
+-rw-r--r--   0        0        0    13660 2023-04-30 10:02:38.978774 fastphrase-0.0.5/fastphrase/data/dict/eff_short1.txt
+-rw-r--r--   0        0        0    17258 2023-04-30 10:02:56.114630 fastphrase-0.0.5/fastphrase/data/dict/eff_short2.txt
+-rw-r--r--   0        0        0     2934 2023-05-02 08:54:57.201641 fastphrase-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 fastphrase-0.0.5/PKG-INFO
```

### Comparing `fastphrase-0.0.4/fastphrase/cli/app.py` & `fastphrase-0.0.5/fastphrase/cli/app.py`

 * *Files identical despite different names*

### Comparing `fastphrase-0.0.4/fastphrase/core/passphraser.py` & `fastphrase-0.0.5/fastphrase/core/passphraser.py`

 * *Files identical despite different names*

### Comparing `fastphrase-0.0.4/fastphrase/core/pathkeeper.py` & `fastphrase-0.0.5/fastphrase/core/pathkeeper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 from functools import cache
 from pathlib import Path
 
 
 class PathKeeper:
     """PathKeeper."""
```

### Comparing `fastphrase-0.0.4/fastphrase/core/wordlist.py` & `fastphrase-0.0.5/fastphrase/core/wordlist.py`

 * *Files identical despite different names*

### Comparing `fastphrase-0.0.4/fastphrase/data/dict/bip0039.txt` & `fastphrase-0.0.5/fastphrase/data/dict/bip0039.txt`

 * *Files identical despite different names*

### Comparing `fastphrase-0.0.4/fastphrase/data/dict/eff_long.txt` & `fastphrase-0.0.5/fastphrase/data/dict/eff_long.txt`

 * *Files identical despite different names*

### Comparing `fastphrase-0.0.4/fastphrase/data/dict/eff_short1.txt` & `fastphrase-0.0.5/fastphrase/data/dict/eff_short1.txt`

 * *Files identical despite different names*

### Comparing `fastphrase-0.0.4/fastphrase/data/dict/eff_short2.txt` & `fastphrase-0.0.5/fastphrase/data/dict/eff_short2.txt`

 * *Files identical despite different names*

### Comparing `fastphrase-0.0.4/pyproject.toml` & `fastphrase-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "fastphrase"
 description = "Fastphrase - passphrase generator by worldlists."
 authors = [
     { name = "Alexander Lavrov", email = "admin@egnod.dev" },
 ]
 dependencies = []
-requires-python = ">=3.11"
+requires-python = ">=3.9,<3.12"
 readme = "README.md"
 dynamic = []
-version = "0.0.4"
+version = "0.0.5"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 fastphrase = "fastphrase.__main__:start"
 
@@ -92,15 +92,15 @@
 disable_error_code = [
     "valid-type",
     "call-arg",
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.0.4"
+version = "0.0.5"
 version_files = [
     "fastphrase/__about__.py:__version__",
 ]
 style = [
     [
         "qmark",
         "fg:#ff9d00 bold",
```

