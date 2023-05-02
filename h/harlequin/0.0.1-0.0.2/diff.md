# Comparing `tmp/harlequin-0.0.1.tar.gz` & `tmp/harlequin-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlequin-0.0.1.tar", max compression
+gzip compressed data, was "harlequin-0.0.2.tar", max compression
```

## Comparing `harlequin-0.0.1.tar` & `harlequin-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-05-02 16:40:24.975336 harlequin-0.0.1/LICENSE
--rw-r--r--   0        0        0       45 2023-05-02 16:40:24.975336 harlequin-0.0.1/README.md
--rw-r--r--   0        0        0      652 2023-05-02 16:40:24.975336 harlequin-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 16:40:24.975336 harlequin-0.0.1/src/harlequin/__init__.py
--rw-r--r--   0        0        0      313 2023-05-02 16:40:24.975336 harlequin-0.0.1/src/harlequin/cli.py
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 harlequin-0.0.1/setup.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 harlequin-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-02 20:18:52.433412 harlequin-0.0.2/LICENSE
+-rw-r--r--   0        0        0      826 2023-05-02 20:18:52.433412 harlequin-0.0.2/README.md
+-rw-r--r--   0        0        0      652 2023-05-02 20:18:52.433412 harlequin-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/__init__.py
+-rw-r--r--   0        0        0      388 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/cli.py
+-rw-r--r--   0        0        0      204 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/tui/__init__.py
+-rw-r--r--   0        0        0      403 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/tui/code_editor.py
+-rw-r--r--   0        0        0       81 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/tui/results_viewer.py
+-rw-r--r--   0        0        0     1300 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/tui/schema_viewer.py
+-rw-r--r--   0        0        0      155 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/tui/sql_client.css
+-rw-r--r--   0        0        0     1399 2023-05-02 20:18:52.433412 harlequin-0.0.2/src/harlequin/tui/sql_client.py
+-rw-r--r--   0        0        0     1737 1970-01-01 00:00:00.000000 harlequin-0.0.2/setup.py
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 harlequin-0.0.2/PKG-INFO
```

### Comparing `harlequin-0.0.1/LICENSE` & `harlequin-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.1/pyproject.toml` & `harlequin-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harlequin"
-version = "0.0.1"
+version = "0.0.2"
 description = "A Text User Interface for DuckDB"
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "harlequin", from = "src" },
 ]
```

