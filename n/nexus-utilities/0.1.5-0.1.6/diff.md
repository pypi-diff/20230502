# Comparing `tmp/nexus-utilities-0.1.5.tar.gz` & `tmp/nexus-utilities-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.1.5.tar", last modified: Tue May  2 14:18:04 2023, max compression
+gzip compressed data, was "nexus-utilities-0.1.6.tar", last modified: Tue May  2 14:33:44 2023, max compression
```

## Comparing `nexus-utilities-0.1.5.tar` & `nexus-utilities-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:18:04.252003 nexus-utilities-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-02 14:17:50.000000 nexus-utilities-0.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-02 14:18:04.252003 nexus-utilities-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-02 14:17:50.000000 nexus-utilities-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:18:04.252003 nexus-utilities-0.1.5/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-02 14:18:04.000000 nexus-utilities-0.1.5/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-02 14:18:04.000000 nexus-utilities-0.1.5/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:18:04.000000 nexus-utilities-0.1.5/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 14:18:04.000000 nexus-utilities-0.1.5/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 14:18:04.000000 nexus-utilities-0.1.5/nexus_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:18:04.256003 nexus-utilities-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-02 14:17:50.000000 nexus-utilities-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:18:04.252003 nexus-utilities-0.1.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:17:50.000000 nexus-utilities-0.1.5/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-02 14:17:50.000000 nexus-utilities-0.1.5/src/package_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:33:44.013285 nexus-utilities-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-02 14:33:21.000000 nexus-utilities-0.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 14:33:44.013285 nexus-utilities-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-02 14:33:21.000000 nexus-utilities-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:33:44.013285 nexus-utilities-0.1.6/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 14:33:43.000000 nexus-utilities-0.1.6/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-02 14:33:43.000000 nexus-utilities-0.1.6/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:33:43.000000 nexus-utilities-0.1.6/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 14:33:43.000000 nexus-utilities-0.1.6/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 14:33:43.000000 nexus-utilities-0.1.6/nexus_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:33:44.013285 nexus-utilities-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-02 14:33:21.000000 nexus-utilities-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:33:44.013285 nexus-utilities-0.1.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:33:21.000000 nexus-utilities-0.1.6/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-02 14:33:21.000000 nexus-utilities-0.1.6/src/package_utils.py
```

### Comparing `nexus-utilities-0.1.5/LICENSE.txt` & `nexus-utilities-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.1.5/PKG-INFO` & `nexus-utilities-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.1.5
+Version: 0.1.6
 Summary: Common python utilities
-Home-page: https://github.com/james-larsen/nexus_utils
+Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexus-utilities-0.1.5/README.md` & `nexus-utilities-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.1.5/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.1.6/nexus_utilities.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.1.5
+Version: 0.1.6
 Summary: Common python utilities
-Home-page: https://github.com/james-larsen/nexus_utils
+Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexus-utilities-0.1.5/setup.py` & `nexus-utilities-0.1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-utilities',
-    version='0.1.5',
+    version='0.1.6',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
-    url='https://github.com/james-larsen/nexus_utils',
+    url='https://github.com/james-larsen/nexus-utilities',
     packages=find_packages(),
     install_requires=[
         'boto3>=1.26.45',
         'twine>=3.4.0'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `nexus-utilities-0.1.5/src/package_utils.py` & `nexus-utilities-0.1.6/src/package_utils.py`

 * *Files identical despite different names*

