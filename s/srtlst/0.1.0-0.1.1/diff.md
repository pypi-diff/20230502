# Comparing `tmp/srtlst-0.1.0.tar.gz` & `tmp/srtlst-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srtlst-0.1.0.tar", max compression
+gzip compressed data, was "srtlst-0.1.1.tar", max compression
```

## Comparing `srtlst-0.1.0.tar` & `srtlst-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      565 2023-04-30 18:52:41.564247 srtlst-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      155 2023-04-30 18:54:26.210904 srtlst-0.1.0/src/srtlst/__init__.py
--rw-r--r--   0        0        0      154 2023-04-27 19:04:51.754352 srtlst-0.1.0/src/srtlst/protocols.py
--rw-r--r--   0        0        0        0 2023-04-30 13:23:02.474724 srtlst-0.1.0/src/srtlst/py.typed
--rw-r--r--   0        0        0     4829 2023-04-30 18:54:26.158137 srtlst-0.1.0/src/srtlst/sorted_list.py
--rw-r--r--   0        0        0      874 2023-04-30 18:54:26.188039 srtlst-0.1.0/src/srtlst/sorted_list_by_key.py
--rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 srtlst-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-05-02 11:30:15.985176 srtlst-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      821 2023-04-30 13:23:02.518546 srtlst-0.1.1/readme.md
+-rw-r--r--   0        0        0      155 2023-04-30 18:54:26.210904 srtlst-0.1.1/src/srtlst/__init__.py
+-rw-r--r--   0        0        0      154 2023-04-27 19:04:51.754352 srtlst-0.1.1/src/srtlst/protocols.py
+-rw-r--r--   0        0        0        0 2023-04-30 13:23:02.474724 srtlst-0.1.1/src/srtlst/py.typed
+-rw-r--r--   0        0        0     4829 2023-04-30 18:54:26.158137 srtlst-0.1.1/src/srtlst/sorted_list.py
+-rw-r--r--   0        0        0      874 2023-04-30 18:54:26.188039 srtlst-0.1.1/src/srtlst/sorted_list_by_key.py
+-rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 srtlst-0.1.1/PKG-INFO
```

### Comparing `srtlst-0.1.0/pyproject.toml` & `srtlst-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "srtlst"
-version = "0.1.0"
+version = "0.1.1"
 description = "a simple, type checkable, sorted list"
 authors = ["exoriente"]
 license = "MIT"
+readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.262"
 black = "^23.3.0"
```

### Comparing `srtlst-0.1.0/src/srtlst/sorted_list.py` & `srtlst-0.1.1/src/srtlst/sorted_list.py`

 * *Files identical despite different names*

### Comparing `srtlst-0.1.0/src/srtlst/sorted_list_by_key.py` & `srtlst-0.1.1/src/srtlst/sorted_list_by_key.py`

 * *Files identical despite different names*

