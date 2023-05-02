# Comparing `tmp/dsw-models-3.22.1.tar.gz` & `tmp/dsw-models-3.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-models-3.22.1.tar", last modified: Fri Apr 14 12:55:25 2023, max compression
+gzip compressed data, was "dsw-models-3.23.0.tar", last modified: Tue May  2 09:24:40 2023, max compression
```

## Comparing `dsw-models-3.22.1.tar` & `dsw-models-3.23.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:25.522484 dsw-models-3.22.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-14 12:55:22.000000 dsw-models-3.22.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-14 12:55:25.522484 dsw-models-3.22.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-14 12:55:22.000000 dsw-models-3.22.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:25.518484 dsw-models-3.22.1/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:25.522484 dsw-models-3.22.1/dsw/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:22.000000 dsw-models-3.22.1/dsw/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-14 12:55:25.000000 dsw-models-3.22.1/dsw/models/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-14 12:55:22.000000 dsw-models-3.22.1/dsw/models/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:25.522484 dsw-models-3.22.1/dsw/models/km/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:22.000000 dsw-models-3.22.1/dsw/models/km/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    90332 2023-04-14 12:55:22.000000 dsw-models-3.22.1/dsw/models/km/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-14 12:55:22.000000 dsw-models-3.22.1/dsw/models/km/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:25.522484 dsw-models-3.22.1/dsw_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-14 12:55:25.000000 dsw-models-3.22.1/dsw_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-14 12:55:25.000000 dsw-models-3.22.1/dsw_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:55:25.000000 dsw-models-3.22.1/dsw_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:55:25.000000 dsw-models-3.22.1/dsw_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 12:55:25.000000 dsw-models-3.22.1/dsw_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-14 12:55:22.000000 dsw-models-3.22.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:55:25.522484 dsw-models-3.22.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:55:22.000000 dsw-models-3.22.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:40.908227 dsw-models-3.23.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-02 09:24:28.000000 dsw-models-3.23.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-02 09:24:40.908227 dsw-models-3.23.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-02 09:24:28.000000 dsw-models-3.23.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:40.904226 dsw-models-3.23.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:40.908227 dsw-models-3.23.0/dsw/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:28.000000 dsw-models-3.23.0/dsw/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-02 09:24:40.000000 dsw-models-3.23.0/dsw/models/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-02 09:24:28.000000 dsw-models-3.23.0/dsw/models/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:40.908227 dsw-models-3.23.0/dsw/models/km/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:28.000000 dsw-models-3.23.0/dsw/models/km/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90332 2023-05-02 09:24:28.000000 dsw-models-3.23.0/dsw/models/km/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-02 09:24:28.000000 dsw-models-3.23.0/dsw/models/km/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:40.908227 dsw-models-3.23.0/dsw_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-02 09:24:40.000000 dsw-models-3.23.0/dsw_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-02 09:24:40.000000 dsw-models-3.23.0/dsw_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:24:40.000000 dsw-models-3.23.0/dsw_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:24:40.000000 dsw-models-3.23.0/dsw_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 09:24:40.000000 dsw-models-3.23.0/dsw_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-02 09:24:28.000000 dsw-models-3.23.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:24:40.908227 dsw-models-3.23.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:24:28.000000 dsw-models-3.23.0/setup.py
```

### Comparing `dsw-models-3.22.1/LICENSE` & `dsw-models-3.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-models-3.22.1/PKG-INFO` & `dsw-models-3.23.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: dsw-models
-Version: 3.22.1
+Version: 3.23.0
 Summary: Library with DSW models and basic IO operations
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Python: <4,>=3.8
+Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Data Stewardship Wizard: Models
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ds-wizard/engine-tools)](https://github.com/ds-wizard/engine-tools/releases)
 [![PyPI](https://img.shields.io/pypi/v/dsw-config)](https://pypi.org/project/dsw-config/)
```

### Comparing `dsw-models-3.22.1/README.md` & `dsw-models-3.23.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-models-3.22.1/dsw/models/km/events.py` & `dsw-models-3.23.0/dsw/models/km/events.py`

 * *Files identical despite different names*

### Comparing `dsw-models-3.22.1/dsw/models/km/package.py` & `dsw-models-3.23.0/dsw/models/km/package.py`

 * *Files identical despite different names*

### Comparing `dsw-models-3.22.1/dsw_models.egg-info/PKG-INFO` & `dsw-models-3.23.0/dsw_models.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: dsw-models
-Version: 3.22.1
+Version: 3.23.0
 Summary: Library with DSW models and basic IO operations
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Python: <4,>=3.8
+Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Data Stewardship Wizard: Models
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ds-wizard/engine-tools)](https://github.com/ds-wizard/engine-tools/releases)
 [![PyPI](https://img.shields.io/pypi/v/dsw-config)](https://pypi.org/project/dsw-config/)
```

### Comparing `dsw-models-3.22.1/pyproject.toml` & `dsw-models-3.23.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-models'
-version = "3.22.1"
+version = "3.23.0"
 description = 'Library with DSW models and basic IO operations'
 readme = 'README.md'
 keywords = ['dsw', 'config', 'yaml', 'parser']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
 classifiers = [
     'Development Status :: 4 - Beta',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Topic :: Text Processing',
     'Topic :: Utilities',
 ]
-requires-python = '>=3.8, <4'
+requires-python = '>=3.10, <4'
 dependencies = [
 ]
 
 [project.urls]
 Homepage = 'https://ds-wizard.org'
 Repository = 'https://github.com/ds-wizard/engine-tools'
 Documentation = 'https://guide.ds-wizard.org'
```

