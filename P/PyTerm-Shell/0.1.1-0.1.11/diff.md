# Comparing `tmp/PyTerm-Shell-0.1.1.tar.gz` & `tmp/PyTerm-Shell-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTerm-Shell-0.1.1.tar", last modified: Tue May  2 01:06:22 2023, max compression
+gzip compressed data, was "PyTerm-Shell-0.1.11.tar", last modified: Tue May  2 01:16:02 2023, max compression
```

## Comparing `PyTerm-Shell-0.1.1.tar` & `PyTerm-Shell-0.1.11.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:06:22.987725 PyTerm-Shell-0.1.1/
--rw-rw-r--   0 nick      (1000) nick      (1000)       53 2023-05-02 01:05:57.000000 PyTerm-Shell-0.1.1/MANIFEST.in
--rw-rw-r--   0 nick      (1000) nick      (1000)      356 2023-05-02 01:06:22.987725 PyTerm-Shell-0.1.1/PKG-INFO
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:06:22.975719 PyTerm-Shell-0.1.1/PyTerm/
--rw-rw-r--   0 nick      (1000) nick      (1000)    12547 2023-05-02 00:25:56.000000 PyTerm-Shell-0.1.1/PyTerm/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)       48 2023-05-02 00:50:12.000000 PyTerm-Shell-0.1.1/PyTerm/cli_assist.py
--rw-rw-r--   0 nick      (1000) nick      (1000)       96 2023-05-01 21:20:12.000000 PyTerm-Shell-0.1.1/PyTerm/config.json
--rw-rw-r--   0 nick      (1000) nick      (1000)      295 2023-05-01 21:20:12.000000 PyTerm-Shell-0.1.1/PyTerm/styles.css
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:06:22.987725 PyTerm-Shell-0.1.1/PyTerm_Shell.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)      356 2023-05-02 01:06:22.000000 PyTerm-Shell-0.1.1/PyTerm_Shell.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      280 2023-05-02 01:06:22.000000 PyTerm-Shell-0.1.1/PyTerm_Shell.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-02 01:06:22.000000 PyTerm-Shell-0.1.1/PyTerm_Shell.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       50 2023-05-02 01:06:22.000000 PyTerm-Shell-0.1.1/PyTerm_Shell.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        7 2023-05-02 01:06:22.000000 PyTerm-Shell-0.1.1/PyTerm_Shell.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-02 01:06:22.987725 PyTerm-Shell-0.1.1/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)      592 2023-05-02 01:06:14.000000 PyTerm-Shell-0.1.1/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:16:02.037128 PyTerm-Shell-0.1.11/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       53 2023-05-02 01:05:57.000000 PyTerm-Shell-0.1.11/MANIFEST.in
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2756 2023-05-02 01:16:02.037128 PyTerm-Shell-0.1.11/PKG-INFO
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:16:02.025122 PyTerm-Shell-0.1.11/PyTerm/
+-rw-rw-r--   0 nick      (1000) nick      (1000)    12547 2023-05-02 00:25:56.000000 PyTerm-Shell-0.1.11/PyTerm/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)       48 2023-05-02 00:50:12.000000 PyTerm-Shell-0.1.11/PyTerm/cli_assist.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)       96 2023-05-01 21:20:12.000000 PyTerm-Shell-0.1.11/PyTerm/config.json
+-rw-rw-r--   0 nick      (1000) nick      (1000)      295 2023-05-01 21:20:12.000000 PyTerm-Shell-0.1.11/PyTerm/styles.css
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:16:02.037128 PyTerm-Shell-0.1.11/PyTerm_Shell.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2756 2023-05-02 01:16:02.000000 PyTerm-Shell-0.1.11/PyTerm_Shell.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      290 2023-05-02 01:16:02.000000 PyTerm-Shell-0.1.11/PyTerm_Shell.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-02 01:16:02.000000 PyTerm-Shell-0.1.11/PyTerm_Shell.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       50 2023-05-02 01:16:02.000000 PyTerm-Shell-0.1.11/PyTerm_Shell.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        7 2023-05-02 01:16:02.000000 PyTerm-Shell-0.1.11/PyTerm_Shell.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2421 2023-05-02 01:13:29.000000 PyTerm-Shell-0.1.11/README.md
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-02 01:16:02.037128 PyTerm-Shell-0.1.11/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)      803 2023-05-02 01:15:50.000000 PyTerm-Shell-0.1.11/setup.py
```

### Comparing `PyTerm-Shell-0.1.1/PyTerm/__init__.py` & `PyTerm-Shell-0.1.11/PyTerm/__init__.py`

 * *Files identical despite different names*

