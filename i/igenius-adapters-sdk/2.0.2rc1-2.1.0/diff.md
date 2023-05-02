# Comparing `tmp/igenius-adapters-sdk-2.0.2rc1.tar.gz` & `tmp/igenius-adapters-sdk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igenius-adapters-sdk-2.0.2rc1.tar", last modified: Mon Mar 20 16:05:31 2023, max compression
+gzip compressed data, was "igenius-adapters-sdk-2.1.0.tar", last modified: Tue May  2 13:31:31 2023, max compression
```

## Comparing `igenius-adapters-sdk-2.0.2rc1.tar` & `igenius-adapters-sdk-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11343 2023-03-20 15:52:10.360900 igenius-adapters-sdk-2.0.2rc1/LICENSE
--rw-r--r--   0        0        0      931 2023-03-20 15:52:10.360900 igenius-adapters-sdk-2.0.2rc1/README.md
--rw-r--r--   0        0        0     1003 2023-03-20 15:56:00.661161 igenius-adapters-sdk-2.0.2rc1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-20 15:52:10.364901 igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 15:52:10.364901 igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/__init__.py
--rw-r--r--   0        0        0     6870 2023-03-20 15:52:10.364901 igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/attribute.py
--rw-r--r--   0        0        0     1192 2023-03-20 15:52:10.364901 igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/collection.py
--rw-r--r--   0        0        0     5364 2023-03-20 15:52:10.364901 igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/data.py
--rw-r--r--   0        0        0      213 2023-03-20 15:52:10.364901 igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/errors.py
--rw-r--r--   0        0        0      198 2023-03-20 15:52:10.364901 igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/i18n.py
--rw-r--r--   0        0        0     1414 2023-03-20 15:52:10.364901 igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/numeric_binning.py
--rw-r--r--   0        0        0     8319 2023-03-20 15:52:10.364901 igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/params.py
--rw-r--r--   0        0        0     2510 2023-03-20 15:52:10.364901 igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/query.py
--rw-r--r--   0        0        0     2005 2023-03-20 15:52:10.364901 igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/uri.py
--rw-r--r--   0        0        0        0 2023-03-20 15:52:10.364901 igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/tools/__init__.py
--rw-r--r--   0        0        0     1502 2023-03-20 15:52:10.364901 igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/tools/chassis.py
--rw-r--r--   0        0        0     3086 2023-03-20 15:52:10.364901 igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/tools/utils.py
--rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 igenius-adapters-sdk-2.0.2rc1/setup.py
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 igenius-adapters-sdk-2.0.2rc1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-05-02 13:27:48.952674 igenius-adapters-sdk-2.1.0/LICENSE
+-rw-r--r--   0        0        0      931 2023-05-02 13:27:48.952674 igenius-adapters-sdk-2.1.0/README.md
+-rw-r--r--   0        0        0     1000 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/__init__.py
+-rw-r--r--   0        0        0     6870 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/attribute.py
+-rw-r--r--   0        0        0     1192 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/collection.py
+-rw-r--r--   0        0        0     5364 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/data.py
+-rw-r--r--   0        0        0      213 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/errors.py
+-rw-r--r--   0        0        0      198 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/i18n.py
+-rw-r--r--   0        0        0     1414 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/numeric_binning.py
+-rw-r--r--   0        0        0     8702 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/params.py
+-rw-r--r--   0        0        0     2510 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/query.py
+-rw-r--r--   0        0        0     2005 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/uri.py
+-rw-r--r--   0        0        0        0 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/tools/__init__.py
+-rw-r--r--   0        0        0     1502 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/tools/chassis.py
+-rw-r--r--   0        0        0     3086 2023-05-02 13:27:48.956675 igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/tools/utils.py
+-rw-r--r--   0        0        0     1806 1970-01-01 00:00:00.000000 igenius-adapters-sdk-2.1.0/setup.py
+-rw-r--r--   0        0        0     1597 1970-01-01 00:00:00.000000 igenius-adapters-sdk-2.1.0/PKG-INFO
```

### Comparing `igenius-adapters-sdk-2.0.2rc1/LICENSE` & `igenius-adapters-sdk-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `igenius-adapters-sdk-2.0.2rc1/README.md` & `igenius-adapters-sdk-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `igenius-adapters-sdk-2.0.2rc1/pyproject.toml` & `igenius-adapters-sdk-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "igenius-adapters-sdk"
-version = "2.0.2rc1"
+version = "2.1.0"
 description = "The iGenius Software Development Kit to develop crystal datasource adapters."
 authors = ["iGenius Backend <backend@igenius.ai>"]
 homepage = "https://github.com/iGenius-Srl/igenius-adapters-sdk"
 license = "Apache License Version 2.0, Copyright 2021 iGenius S.r.l."
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Libraries",
```

### Comparing `igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/attribute.py` & `igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/attribute.py`

 * *Files identical despite different names*

### Comparing `igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/collection.py` & `igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/collection.py`

 * *Files identical despite different names*

### Comparing `igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/data.py` & `igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/data.py`

 * *Files identical despite different names*

### Comparing `igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/numeric_binning.py` & `igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/numeric_binning.py`

 * *Files identical despite different names*

### Comparing `igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/params.py` & `igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,22 @@
         uid="crystal.topics.data.param-operation.empty-string",
         i18n=I18n(
             name="cons-data-table-sort-operation-label-empty-string",
             description="crystal.topics.data.param-operation.empty-string.i18n.description",
         ),
         properties_schema=OperationSchemas.NO_VALUE.jsonschema,
     )
+    NOT_EMPTY_STRING = ParamOperationSpecs(
+        uid="crystal.topics.data.param-operation.not-empty-string",
+        i18n=I18n(
+            name="cons-data-table-sort-operation-label-not-empty-string",
+            description="crystal.topics.data.param-operation.not-empty-string.i18n.description",
+        ),
+        properties_schema=OperationSchemas.NO_VALUE.jsonschema,
+    )
 
     @classmethod
     def from_uid(cls, uid: str) -> ParamOperationSpecs:
         """Given a param operation uid, returns its complete spec if found,
         otherwise raises ValueError."""
         try:
             return next(
```

### Comparing `igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/query.py` & `igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/query.py`

 * *Files identical despite different names*

### Comparing `igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/entities/uri.py` & `igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/entities/uri.py`

 * *Files identical despite different names*

### Comparing `igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/tools/chassis.py` & `igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/tools/chassis.py`

 * *Files identical despite different names*

### Comparing `igenius-adapters-sdk-2.0.2rc1/src/igenius_adapters_sdk/tools/utils.py` & `igenius-adapters-sdk-2.1.0/src/igenius_adapters_sdk/tools/utils.py`

 * *Files identical despite different names*

### Comparing `igenius-adapters-sdk-2.0.2rc1/setup.py` & `igenius-adapters-sdk-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.7.2,<2.0.0', 'typing-extensions>=3.10.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'igenius-adapters-sdk',
-    'version': '2.0.2rc1',
+    'version': '2.1.0',
     'description': 'The iGenius Software Development Kit to develop crystal datasource adapters.',
     'long_description': '# iGenius Adapters SDK\n\nThis is the Software Development Kit for iGenius Web Connectors development.  \nYou can use our SDK in your project to be able to handle correctly the data structures that will be used by iGenius services to call your web connector adapter.\nFurther information about SDK can be found in the [official documentation](https://webconnectors.crystal.ai/sdk/latest/), instead check [What is a Web Connector](https://webconnectors.crystal.ai/docs/latest/) to know more \nabout the data sharing with _Crystal_.\n\n## Installation\n\nWith Poetry\n\n```bash\npoetry add igenius-adapters-sdk\n```\n\nWith pip\n\n```bash\npip install igenius-adapters-sdk\n```\n\n## Releases\n\nSee the [CHANGELOG.md](/CHANGELOG.md) file.\n\n## License\n\nAll the content in this repository is licensed under the [Apache license, version 2.0](http://www.apache.org/licenses/LICENSE-2.0.txt). The full license text can be found in the [LICENSE](/LICENSE) file.',
     'author': 'iGenius Backend',
     'author_email': 'backend@igenius.ai',
     'url': 'https://github.com/iGenius-Srl/igenius-adapters-sdk',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `igenius-adapters-sdk-2.0.2rc1/PKG-INFO` & `igenius-adapters-sdk-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igenius-adapters-sdk
-Version: 2.0.2rc1
+Version: 2.1.0
 Summary: The iGenius Software Development Kit to develop crystal datasource adapters.
 Home-page: https://github.com/iGenius-Srl/igenius-adapters-sdk
 Author: iGenius Backend
 Author-email: backend@igenius.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

