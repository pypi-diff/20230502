# Comparing `tmp/PyTerm-Shell-0.1.0.tar.gz` & `tmp/PyTerm-Shell-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTerm-Shell-0.1.0.tar", last modified: Tue May  2 01:02:25 2023, max compression
+gzip compressed data, was "PyTerm-Shell-0.1.1.tar", last modified: Tue May  2 01:06:22 2023, max compression
```

## Comparing `PyTerm-Shell-0.1.0.tar` & `PyTerm-Shell-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:02:25.469005 PyTerm-Shell-0.1.0/
--rw-rw-r--   0 nick      (1000) nick      (1000)       65 2023-05-02 00:44:32.000000 PyTerm-Shell-0.1.0/MANIFEST.in
--rw-rw-r--   0 nick      (1000) nick      (1000)      356 2023-05-02 01:02:25.461001 PyTerm-Shell-0.1.0/PKG-INFO
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:02:25.444993 PyTerm-Shell-0.1.0/PyTerm/
--rw-rw-r--   0 nick      (1000) nick      (1000)    12547 2023-05-02 00:25:56.000000 PyTerm-Shell-0.1.0/PyTerm/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)       48 2023-05-02 00:50:12.000000 PyTerm-Shell-0.1.0/PyTerm/cli_assist.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:02:25.456999 PyTerm-Shell-0.1.0/PyTerm_Shell.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)      356 2023-05-02 01:02:25.000000 PyTerm-Shell-0.1.0/PyTerm_Shell.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      243 2023-05-02 01:02:25.000000 PyTerm-Shell-0.1.0/PyTerm_Shell.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-02 01:02:25.000000 PyTerm-Shell-0.1.0/PyTerm_Shell.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       50 2023-05-02 01:02:25.000000 PyTerm-Shell-0.1.0/PyTerm_Shell.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        7 2023-05-02 01:02:25.000000 PyTerm-Shell-0.1.0/PyTerm_Shell.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-02 01:02:25.469005 PyTerm-Shell-0.1.0/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)      591 2023-05-02 00:50:25.000000 PyTerm-Shell-0.1.0/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:06:22.987725 PyTerm-Shell-0.1.1/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       53 2023-05-02 01:05:57.000000 PyTerm-Shell-0.1.1/MANIFEST.in
+-rw-rw-r--   0 nick      (1000) nick      (1000)      356 2023-05-02 01:06:22.987725 PyTerm-Shell-0.1.1/PKG-INFO
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:06:22.975719 PyTerm-Shell-0.1.1/PyTerm/
+-rw-rw-r--   0 nick      (1000) nick      (1000)    12547 2023-05-02 00:25:56.000000 PyTerm-Shell-0.1.1/PyTerm/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)       48 2023-05-02 00:50:12.000000 PyTerm-Shell-0.1.1/PyTerm/cli_assist.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)       96 2023-05-01 21:20:12.000000 PyTerm-Shell-0.1.1/PyTerm/config.json
+-rw-rw-r--   0 nick      (1000) nick      (1000)      295 2023-05-01 21:20:12.000000 PyTerm-Shell-0.1.1/PyTerm/styles.css
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:06:22.987725 PyTerm-Shell-0.1.1/PyTerm_Shell.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      356 2023-05-02 01:06:22.000000 PyTerm-Shell-0.1.1/PyTerm_Shell.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      280 2023-05-02 01:06:22.000000 PyTerm-Shell-0.1.1/PyTerm_Shell.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-02 01:06:22.000000 PyTerm-Shell-0.1.1/PyTerm_Shell.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       50 2023-05-02 01:06:22.000000 PyTerm-Shell-0.1.1/PyTerm_Shell.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        7 2023-05-02 01:06:22.000000 PyTerm-Shell-0.1.1/PyTerm_Shell.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-02 01:06:22.987725 PyTerm-Shell-0.1.1/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)      592 2023-05-02 01:06:14.000000 PyTerm-Shell-0.1.1/setup.py
```

### Comparing `PyTerm-Shell-0.1.0/PyTerm/__init__.py` & `PyTerm-Shell-0.1.1/PyTerm/__init__.py`

 * *Files identical despite different names*

### Comparing `PyTerm-Shell-0.1.0/setup.py` & `PyTerm-Shell-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 
 
 setup (
  name = 'PyTerm-Shell',
  description = 'Making an aesthetic minimalist Linux shell in Python',
- version = '0.1.0',
+ version = '0.1.01',
  python_requires='>=3.7',
  entry_points = {
         'console_scripts': ['PyTerm=PyTerm.cli_assist:main'],
  },
  include_package_data=True,
  author="Nick Tsiones",
  license='MIT',
```

