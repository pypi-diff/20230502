# Comparing `tmp/dsw-tdk-3.8.0.tar.gz` & `tmp/dsw-tdk-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-tdk-3.8.0.tar", last modified: Tue Feb  1 13:42:42 2022, max compression
+gzip compressed data, was "dsw-tdk-3.9.0.tar", last modified: Tue Mar  1 16:08:28 2022, max compression
```

## Comparing `dsw-tdk-3.8.0.tar` & `dsw-tdk-3.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-02-01 13:42:42.463385 dsw-tdk-3.8.0/
--rw-rw-rw-   0        0        0     3289 2022-02-01 13:42:34.000000 dsw-tdk-3.8.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    11558 2020-07-03 18:09:20.000000 dsw-tdk-3.8.0/LICENSE
--rw-rw-rw-   0        0        0       39 2020-11-17 18:20:12.000000 dsw-tdk-3.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6489 2022-02-01 13:42:42.463385 dsw-tdk-3.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     5401 2021-11-02 08:11:20.000000 dsw-tdk-3.8.0/README.md
-drwxrwxrwx   0        0        0        0 2022-02-01 13:42:42.449386 dsw-tdk-3.8.0/dsw_tdk/
--rw-rw-rw-   0        0        0      317 2020-11-04 13:32:00.000000 dsw-tdk-3.8.0/dsw_tdk/__init__.py
--rw-rw-rw-   0        0        0       48 2020-11-04 13:32:00.000000 dsw-tdk-3.8.0/dsw_tdk/__main__.py
--rw-rw-rw-   0        0        0    10687 2021-12-07 11:00:23.000000 dsw-tdk-3.8.0/dsw_tdk/api_client.py
--rw-rw-rw-   0        0        0    17275 2021-11-02 08:11:20.000000 dsw-tdk-3.8.0/dsw_tdk/cli.py
--rw-rw-rw-   0        0        0      623 2022-02-01 13:42:34.000000 dsw-tdk-3.8.0/dsw_tdk/consts.py
--rw-rw-rw-   0        0        0    18776 2022-02-01 13:42:34.000000 dsw-tdk-3.8.0/dsw_tdk/core.py
--rw-rw-rw-   0        0        0    16675 2021-12-07 11:00:23.000000 dsw-tdk-3.8.0/dsw_tdk/model.py
-drwxrwxrwx   0        0        0        0 2022-02-01 13:42:42.462384 dsw-tdk-3.8.0/dsw_tdk/templates/
--rw-rw-rw-   0        0        0      260 2020-11-04 13:32:00.000000 dsw-tdk-3.8.0/dsw_tdk/templates/README.md.j2
--rw-rw-rw-   0        0        0      310 2020-11-17 18:20:12.000000 dsw-tdk-3.8.0/dsw_tdk/templates/starter.j2
--rw-rw-rw-   0        0        0     5041 2021-11-02 08:11:20.000000 dsw-tdk-3.8.0/dsw_tdk/utils.py
--rw-rw-rw-   0        0        0     8234 2020-11-04 13:32:00.000000 dsw-tdk-3.8.0/dsw_tdk/validation.py
-drwxrwxrwx   0        0        0        0 2022-02-01 13:42:42.460487 dsw-tdk-3.8.0/dsw_tdk.egg-info/
--rw-rw-rw-   0        0        0     6489 2022-02-01 13:42:42.000000 dsw-tdk-3.8.0/dsw_tdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2022-02-01 13:42:42.000000 dsw-tdk-3.8.0/dsw_tdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-01 13:42:42.000000 dsw-tdk-3.8.0/dsw_tdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2022-02-01 13:42:42.000000 dsw-tdk-3.8.0/dsw_tdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2020-11-04 13:34:24.000000 dsw-tdk-3.8.0/dsw_tdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       96 2022-02-01 13:42:42.000000 dsw-tdk-3.8.0/dsw_tdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-02-01 13:42:42.000000 dsw-tdk-3.8.0/dsw_tdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2022-02-01 13:42:42.464385 dsw-tdk-3.8.0/setup.cfg
--rw-rw-rw-   0        0        0     2013 2022-02-01 13:42:34.000000 dsw-tdk-3.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-03-01 16:08:28.269867 dsw-tdk-3.9.0/
+-rw-rw-rw-   0        0        0     3359 2022-03-01 16:08:18.000000 dsw-tdk-3.9.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    11558 2020-07-03 18:09:20.000000 dsw-tdk-3.9.0/LICENSE
+-rw-rw-rw-   0        0        0       39 2020-11-17 18:20:12.000000 dsw-tdk-3.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6489 2022-03-01 16:08:28.269867 dsw-tdk-3.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5401 2021-11-02 08:11:20.000000 dsw-tdk-3.9.0/README.md
+drwxrwxrwx   0        0        0        0 2022-03-01 16:08:28.262870 dsw-tdk-3.9.0/dsw_tdk/
+-rw-rw-rw-   0        0        0      317 2020-11-04 13:32:00.000000 dsw-tdk-3.9.0/dsw_tdk/__init__.py
+-rw-rw-rw-   0        0        0       48 2020-11-04 13:32:00.000000 dsw-tdk-3.9.0/dsw_tdk/__main__.py
+-rw-rw-rw-   0        0        0    10687 2021-12-07 11:00:23.000000 dsw-tdk-3.9.0/dsw_tdk/api_client.py
+-rw-rw-rw-   0        0        0    17275 2021-11-02 08:11:20.000000 dsw-tdk-3.9.0/dsw_tdk/cli.py
+-rw-rw-rw-   0        0        0      623 2022-03-01 16:08:18.000000 dsw-tdk-3.9.0/dsw_tdk/consts.py
+-rw-rw-rw-   0        0        0    18776 2022-03-01 16:05:53.000000 dsw-tdk-3.9.0/dsw_tdk/core.py
+-rw-rw-rw-   0        0        0    16675 2021-12-07 11:00:23.000000 dsw-tdk-3.9.0/dsw_tdk/model.py
+drwxrwxrwx   0        0        0        0 2022-03-01 16:08:28.268900 dsw-tdk-3.9.0/dsw_tdk/templates/
+-rw-rw-rw-   0        0        0      260 2020-11-04 13:32:00.000000 dsw-tdk-3.9.0/dsw_tdk/templates/README.md.j2
+-rw-rw-rw-   0        0        0      310 2020-11-17 18:20:12.000000 dsw-tdk-3.9.0/dsw_tdk/templates/starter.j2
+-rw-rw-rw-   0        0        0     5041 2021-11-02 08:11:20.000000 dsw-tdk-3.9.0/dsw_tdk/utils.py
+-rw-rw-rw-   0        0        0     8234 2020-11-04 13:32:00.000000 dsw-tdk-3.9.0/dsw_tdk/validation.py
+drwxrwxrwx   0        0        0        0 2022-03-01 16:08:28.267868 dsw-tdk-3.9.0/dsw_tdk.egg-info/
+-rw-rw-rw-   0        0        0     6489 2022-03-01 16:08:28.000000 dsw-tdk-3.9.0/dsw_tdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2022-03-01 16:08:28.000000 dsw-tdk-3.9.0/dsw_tdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 16:08:28.000000 dsw-tdk-3.9.0/dsw_tdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2022-03-01 16:08:28.000000 dsw-tdk-3.9.0/dsw_tdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2020-11-04 13:34:24.000000 dsw-tdk-3.9.0/dsw_tdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       96 2022-03-01 16:08:28.000000 dsw-tdk-3.9.0/dsw_tdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-03-01 16:08:28.000000 dsw-tdk-3.9.0/dsw_tdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       70 2022-03-01 16:08:28.270234 dsw-tdk-3.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2013 2022-03-01 16:08:18.000000 dsw-tdk-3.9.0/setup.py
```

### Comparing `dsw-tdk-3.8.0/CHANGELOG.md` & `dsw-tdk-3.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [3.9.0]
+
+Released for version consistency with other DSW tools.
+
 ## [3.8.0]
 
 ### Changed
 
 - Updated with template metamodel 8
 - Updated several dependencies
 
@@ -137,15 +141,15 @@
 - `new` for initializing new template project
 - `list` for listing remote templates
 - `get` for retrieving remote template and storing it locally
 - `put` for uploading local template project to DSW instance including `watch` functionality for smooth template development
 - `verify` for checking template metadata
 - `package` for creating an importable ZIP package from local project
 
-[Unreleased]: /../../compare/master...develop
+[Unreleased]: /../../compare/main...develop
 [2.8.0]: /../../tree/v2.8.0
 [2.8.1]: /../../tree/v2.8.1
 [2.9.0]: /../../tree/v2.9.0
 [2.10.0]: /../../tree/v2.10.0
 [2.11.0]: /../../tree/v2.11.0
 [2.12.0]: /../../tree/v2.12.0
 [2.12.1]: /../../tree/v2.12.1
```

### Comparing `dsw-tdk-3.8.0/LICENSE` & `dsw-tdk-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-tdk-3.8.0/PKG-INFO` & `dsw-tdk-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-tdk
-Version: 3.8.0
+Version: 3.9.0
 Summary: Data Stewardship Wizard Template Development Toolkit
 Home-page: https://github.com/ds-wizard/dsw-tdk
 Author: Marek Suchánek
 Author-email: marek.suchanek@ds-wizard.org
 License: Apache-2.0
 Keywords: dsw template toolkit jinja documents
 Platform: UNKNOWN
```

### Comparing `dsw-tdk-3.8.0/README.md` & `dsw-tdk-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-tdk-3.8.0/dsw_tdk/api_client.py` & `dsw-tdk-3.9.0/dsw_tdk/api_client.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-3.8.0/dsw_tdk/cli.py` & `dsw-tdk-3.9.0/dsw_tdk/cli.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-3.8.0/dsw_tdk/consts.py` & `dsw-tdk-3.9.0/dsw_tdk/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pathspec  # type: ignore
 import re
 
 APP = 'dsw-tdk'
-VERSION = '3.8.0'
+VERSION = '3.9.0'
 METAMODEL_VERSION = 8
 
 REGEX_SEMVER = re.compile(r'^[0-9]+\.[0-9]+\.[0-9]+$')
 REGEX_ORGANIZATION_ID = re.compile(r'^(?![.])(?!.*[.]$)[a-zA-Z0-9.]+$')
 REGEX_TEMPLATE_ID = re.compile(r'^(?![-])(?!.*[-]$)[a-zA-Z0-9-]+$')
 REGEX_KM_ID = REGEX_TEMPLATE_ID
 REGEX_MIME_TYPE = re.compile(r'^(?![-])(?!.*[-]$)[-\w.]+/[-\w.]+$')
```

### Comparing `dsw-tdk-3.8.0/dsw_tdk/core.py` & `dsw-tdk-3.9.0/dsw_tdk/core.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-3.8.0/dsw_tdk/model.py` & `dsw-tdk-3.9.0/dsw_tdk/model.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-3.8.0/dsw_tdk/utils.py` & `dsw-tdk-3.9.0/dsw_tdk/utils.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-3.8.0/dsw_tdk/validation.py` & `dsw-tdk-3.9.0/dsw_tdk/validation.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-3.8.0/dsw_tdk.egg-info/PKG-INFO` & `dsw-tdk-3.9.0/dsw_tdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-tdk
-Version: 3.8.0
+Version: 3.9.0
 Summary: Data Stewardship Wizard Template Development Toolkit
 Home-page: https://github.com/ds-wizard/dsw-tdk
 Author: Marek Suchánek
 Author-email: marek.suchanek@ds-wizard.org
 License: Apache-2.0
 Keywords: dsw template toolkit jinja documents
 Platform: UNKNOWN
```

### Comparing `dsw-tdk-3.8.0/setup.py` & `dsw-tdk-3.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = ''.join(f.readlines())
 
 setup(
     name='dsw-tdk',
-    version='3.8.0',
+    version='3.9.0',
     keywords='dsw template toolkit jinja documents',
     description='Data Stewardship Wizard Template Development Toolkit',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Marek Suchánek',
     author_email='marek.suchanek@ds-wizard.org',
     url='https://github.com/ds-wizard/dsw-tdk',
```

