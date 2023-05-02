# Comparing `tmp/nexus_utilities-0.1.4.tar.gz` & `tmp/nexus-utilities-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus_utilities-0.1.4.tar", last modified: Tue May  2 14:10:33 2023, max compression
+gzip compressed data, was "nexus-utilities-0.1.5.tar", last modified: Tue May  2 14:18:04 2023, max compression
```

## Comparing `nexus_utilities-0.1.4.tar` & `nexus-utilities-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:10:33.328845 nexus_utilities-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-02 14:10:17.000000 nexus_utilities-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-02 14:10:33.328845 nexus_utilities-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-02 14:10:17.000000 nexus_utilities-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:10:33.328845 nexus_utilities-0.1.4/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-02 14:10:33.000000 nexus_utilities-0.1.4/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-02 14:10:33.000000 nexus_utilities-0.1.4/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:10:33.000000 nexus_utilities-0.1.4/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 14:10:33.000000 nexus_utilities-0.1.4/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 14:10:33.000000 nexus_utilities-0.1.4/nexus_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:10:33.328845 nexus_utilities-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-02 14:10:17.000000 nexus_utilities-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:10:33.328845 nexus_utilities-0.1.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:10:17.000000 nexus_utilities-0.1.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-02 14:10:17.000000 nexus_utilities-0.1.4/src/package_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:18:04.252003 nexus-utilities-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-02 14:17:50.000000 nexus-utilities-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-02 14:18:04.252003 nexus-utilities-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-02 14:17:50.000000 nexus-utilities-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:18:04.252003 nexus-utilities-0.1.5/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-02 14:18:04.000000 nexus-utilities-0.1.5/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-02 14:18:04.000000 nexus-utilities-0.1.5/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:18:04.000000 nexus-utilities-0.1.5/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 14:18:04.000000 nexus-utilities-0.1.5/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 14:18:04.000000 nexus-utilities-0.1.5/nexus_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:18:04.256003 nexus-utilities-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-02 14:17:50.000000 nexus-utilities-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:18:04.252003 nexus-utilities-0.1.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:17:50.000000 nexus-utilities-0.1.5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-02 14:17:50.000000 nexus-utilities-0.1.5/src/package_utils.py
```

### Comparing `nexus_utilities-0.1.4/LICENSE.txt` & `nexus-utilities-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus_utilities-0.1.4/PKG-INFO` & `nexus-utilities-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nexus_utilities
-Version: 0.1.4
+Name: nexus-utilities
+Version: 0.1.5
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus_utils
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus_utilities-0.1.4/README.md` & `nexus-utilities-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nexus_utilities-0.1.4/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.1.5/nexus_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.1.4
+Version: 0.1.5
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus_utils
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus_utilities-0.1.4/setup.py` & `nexus-utilities-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='nexus_utilities',
-    version='0.1.4',
+    name='nexus-utilities',
+    version='0.1.5',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
     url='https://github.com/james-larsen/nexus_utils',
     packages=find_packages(),
```

### Comparing `nexus_utilities-0.1.4/src/package_utils.py` & `nexus-utilities-0.1.5/src/package_utils.py`

 * *Files identical despite different names*

