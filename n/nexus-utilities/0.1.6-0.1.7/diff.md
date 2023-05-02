# Comparing `tmp/nexus-utilities-0.1.6.tar.gz` & `tmp/nexus-utilities-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.1.6.tar", last modified: Tue May  2 14:33:44 2023, max compression
+gzip compressed data, was "nexus-utilities-0.1.7.tar", last modified: Tue May  2 15:41:01 2023, max compression
```

## Comparing `nexus-utilities-0.1.6.tar` & `nexus-utilities-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:33:44.013285 nexus-utilities-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-02 14:33:21.000000 nexus-utilities-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 14:33:44.013285 nexus-utilities-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-02 14:33:21.000000 nexus-utilities-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:33:44.013285 nexus-utilities-0.1.6/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 14:33:43.000000 nexus-utilities-0.1.6/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-02 14:33:43.000000 nexus-utilities-0.1.6/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:33:43.000000 nexus-utilities-0.1.6/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 14:33:43.000000 nexus-utilities-0.1.6/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 14:33:43.000000 nexus-utilities-0.1.6/nexus_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:33:44.013285 nexus-utilities-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-02 14:33:21.000000 nexus-utilities-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:33:44.013285 nexus-utilities-0.1.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:33:21.000000 nexus-utilities-0.1.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-02 14:33:21.000000 nexus-utilities-0.1.6/src/package_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:41:01.869062 nexus-utilities-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-02 15:40:45.000000 nexus-utilities-0.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 15:41:01.869062 nexus-utilities-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-02 15:40:45.000000 nexus-utilities-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:41:01.869062 nexus-utilities-0.1.7/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 15:41:01.000000 nexus-utilities-0.1.7/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-02 15:41:01.000000 nexus-utilities-0.1.7/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:41:01.000000 nexus-utilities-0.1.7/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 15:41:01.000000 nexus-utilities-0.1.7/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 15:41:01.000000 nexus-utilities-0.1.7/nexus_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:41:01.869062 nexus-utilities-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-02 15:40:45.000000 nexus-utilities-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:41:01.869062 nexus-utilities-0.1.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:40:45.000000 nexus-utilities-0.1.7/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-02 15:40:45.000000 nexus-utilities-0.1.7/src/package_utils.py
```

### Comparing `nexus-utilities-0.1.6/LICENSE.txt` & `nexus-utilities-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.1.6/PKG-INFO` & `nexus-utilities-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.1.6
+Version: 0.1.7
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.1.6/README.md` & `nexus-utilities-0.1.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# nexus_utils<!-- omit in toc -->
+# nexus-utilities<!-- omit in toc -->
 This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.  Feel free to use these if you find them valuable and I welcome any feedback.
 
 ## Table of Contents <!-- omit in toc -->
 
 - [Installation](#installation)
 - [package\_utils.py](#package_utilspy)
   - [**add\_package\_to\_path()**](#add_package_to_path)
@@ -10,17 +10,19 @@
 - [About the Author](#about-the-author)
 
 ---
 
 ## Installation
 
 ```python
-pip3 install nexus_utils
+pip3 install nexus-utilities
 ```
 
+After installation, use "import nexus_utils" to access the various functions.
+
 ---
 
 ## package_utils.py
 
 This module contains functions for working with Python packages.
 
 ### **add_package_to_path()**
```

### Comparing `nexus-utilities-0.1.6/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.1.7/nexus_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.1.6
+Version: 0.1.7
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.1.6/src/package_utils.py` & `nexus-utilities-0.1.7/src/package_utils.py`

 * *Files identical despite different names*

