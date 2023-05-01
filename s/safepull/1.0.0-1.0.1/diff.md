# Comparing `tmp/safepull-1.0.0.tar.gz` & `tmp/safepull-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safepull-1.0.0.tar", last modified: Mon May  1 23:06:00 2023, max compression
+gzip compressed data, was "safepull-1.0.1.tar", last modified: Mon May  1 23:28:05 2023, max compression
```

## Comparing `safepull-1.0.0.tar` & `safepull-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 rem       (1000) rem       (1000)        0 2023-05-01 23:06:00.901172 safepull-1.0.0/
--rw-rw-r--   0 rem       (1000) rem       (1000)     1060 2023-05-01 23:04:18.000000 safepull-1.0.0/LICENSE
--rw-rw-r--   0 rem       (1000) rem       (1000)      652 2023-05-01 23:06:00.901172 safepull-1.0.0/PKG-INFO
--rw-rw-r--   0 rem       (1000) rem       (1000)      270 2023-05-01 23:04:18.000000 safepull-1.0.0/README.md
--rw-rw-r--   0 rem       (1000) rem       (1000)      552 2023-05-01 23:04:18.000000 safepull-1.0.0/pyproject.toml
--rw-rw-r--   0 rem       (1000) rem       (1000)       38 2023-05-01 23:06:00.901172 safepull-1.0.0/setup.cfg
-drwxrwxr-x   0 rem       (1000) rem       (1000)        0 2023-05-01 23:06:00.901172 safepull-1.0.0/src/
-drwxrwxr-x   0 rem       (1000) rem       (1000)        0 2023-05-01 23:06:00.901172 safepull-1.0.0/src/safepull/
--rw-rw-r--   0 rem       (1000) rem       (1000)        0 2023-05-01 23:04:18.000000 safepull-1.0.0/src/safepull/__init__.py
--rw-rw-r--   0 rem       (1000) rem       (1000)       64 2023-05-01 23:04:18.000000 safepull-1.0.0/src/safepull/__main__.py
--rw-rw-r--   0 rem       (1000) rem       (1000)     5087 2023-05-01 23:04:18.000000 safepull-1.0.0/src/safepull/safepull.py
-drwxrwxr-x   0 rem       (1000) rem       (1000)        0 2023-05-01 23:06:00.901172 safepull-1.0.0/src/safepull.egg-info/
--rw-rw-r--   0 rem       (1000) rem       (1000)      652 2023-05-01 23:06:00.000000 safepull-1.0.0/src/safepull.egg-info/PKG-INFO
--rw-rw-r--   0 rem       (1000) rem       (1000)      325 2023-05-01 23:06:00.000000 safepull-1.0.0/src/safepull.egg-info/SOURCES.txt
--rw-rw-r--   0 rem       (1000) rem       (1000)        1 2023-05-01 23:06:00.000000 safepull-1.0.0/src/safepull.egg-info/dependency_links.txt
--rw-rw-r--   0 rem       (1000) rem       (1000)       51 2023-05-01 23:06:00.000000 safepull-1.0.0/src/safepull.egg-info/entry_points.txt
--rw-rw-r--   0 rem       (1000) rem       (1000)       17 2023-05-01 23:06:00.000000 safepull-1.0.0/src/safepull.egg-info/requires.txt
--rw-rw-r--   0 rem       (1000) rem       (1000)        9 2023-05-01 23:06:00.000000 safepull-1.0.0/src/safepull.egg-info/top_level.txt
+drwxrwxr-x   0 rem       (1000) rem       (1000)        0 2023-05-01 23:28:05.278447 safepull-1.0.1/
+-rw-rw-r--   0 rem       (1000) rem       (1000)     1060 2023-05-01 23:04:18.000000 safepull-1.0.1/LICENSE
+-rw-rw-r--   0 rem       (1000) rem       (1000)     1516 2023-05-01 23:28:05.278447 safepull-1.0.1/PKG-INFO
+-rw-rw-r--   0 rem       (1000) rem       (1000)     1134 2023-05-01 23:26:22.000000 safepull-1.0.1/README.md
+-rw-rw-r--   0 rem       (1000) rem       (1000)      552 2023-05-01 23:27:47.000000 safepull-1.0.1/pyproject.toml
+-rw-rw-r--   0 rem       (1000) rem       (1000)       38 2023-05-01 23:28:05.278447 safepull-1.0.1/setup.cfg
+drwxrwxr-x   0 rem       (1000) rem       (1000)        0 2023-05-01 23:28:05.278447 safepull-1.0.1/src/
+drwxrwxr-x   0 rem       (1000) rem       (1000)        0 2023-05-01 23:28:05.278447 safepull-1.0.1/src/safepull/
+-rw-rw-r--   0 rem       (1000) rem       (1000)        0 2023-05-01 23:04:18.000000 safepull-1.0.1/src/safepull/__init__.py
+-rw-rw-r--   0 rem       (1000) rem       (1000)       64 2023-05-01 23:04:18.000000 safepull-1.0.1/src/safepull/__main__.py
+-rw-rw-r--   0 rem       (1000) rem       (1000)     5087 2023-05-01 23:04:18.000000 safepull-1.0.1/src/safepull/safepull.py
+drwxrwxr-x   0 rem       (1000) rem       (1000)        0 2023-05-01 23:28:05.278447 safepull-1.0.1/src/safepull.egg-info/
+-rw-rw-r--   0 rem       (1000) rem       (1000)     1516 2023-05-01 23:28:05.000000 safepull-1.0.1/src/safepull.egg-info/PKG-INFO
+-rw-rw-r--   0 rem       (1000) rem       (1000)      325 2023-05-01 23:28:05.000000 safepull-1.0.1/src/safepull.egg-info/SOURCES.txt
+-rw-rw-r--   0 rem       (1000) rem       (1000)        1 2023-05-01 23:28:05.000000 safepull-1.0.1/src/safepull.egg-info/dependency_links.txt
+-rw-rw-r--   0 rem       (1000) rem       (1000)       51 2023-05-01 23:28:05.000000 safepull-1.0.1/src/safepull.egg-info/entry_points.txt
+-rw-rw-r--   0 rem       (1000) rem       (1000)       17 2023-05-01 23:28:05.000000 safepull-1.0.1/src/safepull.egg-info/requires.txt
+-rw-rw-r--   0 rem       (1000) rem       (1000)        9 2023-05-01 23:28:05.000000 safepull-1.0.1/src/safepull.egg-info/top_level.txt
```

### Comparing `safepull-1.0.0/LICENSE` & `safepull-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `safepull-1.0.0/pyproject.toml` & `safepull-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "safepull"
-version = "1.0.0"
+version = "1.0.1"
 description = "A quick and dirty command-line script to pull down and extract .py files out of tarballs and wheels without interfacing with the setup.py file."
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.10"
 dependencies = [
     "requests~=2.28.2",
 ]
```

### Comparing `safepull-1.0.0/src/safepull/safepull.py` & `safepull-1.0.1/src/safepull/safepull.py`

 * *Files identical despite different names*

