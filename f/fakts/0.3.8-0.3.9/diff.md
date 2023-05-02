# Comparing `tmp/fakts-0.3.8.tar.gz` & `tmp/fakts-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakts-0.3.8.tar", max compression
+gzip compressed data, was "fakts-0.3.9.tar", max compression
```

## Comparing `fakts-0.3.8.tar` & `fakts-0.3.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     3465 2022-11-21 11:13:02.484118 fakts-0.3.8/README.md
--rw-r--r--   0        0        0      263 2022-11-20 14:08:10.639283 fakts-0.3.8/fakts/__init__.py
--rw-r--r--   0        0        0     1854 2022-11-21 10:34:53.263821 fakts-0.3.8/fakts/cli/main.py
--rw-r--r--   0        0        0      116 2022-11-21 10:33:13.031539 fakts-0.3.8/fakts/discovery/__init__.py
--rw-r--r--   0        0        0     4832 2023-01-17 09:16:51.487491 fakts-0.3.8/fakts/discovery/advertised.py
--rw-r--r--   0        0        0      720 2023-01-16 16:16:06.159933 fakts-0.3.8/fakts/discovery/base.py
--rw-r--r--   0        0        0      232 2022-11-21 10:35:02.323846 fakts-0.3.8/fakts/discovery/beacon/__init__.py
--rw-r--r--   0        0        0     4590 2022-11-21 10:32:28.059513 fakts-0.3.8/fakts/discovery/beacon/beacon.py
--rw-r--r--   0        0        0        0 2022-05-16 14:37:58.382355 fakts-0.3.8/fakts/discovery/qt/__init__.py
--rw-r--r--   0        0        0     5929 2023-01-18 14:45:01.934170 fakts-0.3.8/fakts/discovery/qt/selectable_beacon.py
--rw-r--r--   0        0        0      296 2022-11-21 10:31:31.975480 fakts-0.3.8/fakts/discovery/static.py
--rw-r--r--   0        0        0      279 2022-11-21 10:33:48.715629 fakts-0.3.8/fakts/errors.py
--rw-r--r--   0        0        0       43 2022-11-17 17:49:20.358443 fakts-0.3.8/fakts/fakt/__init__.py
--rw-r--r--   0        0        0      309 2022-09-28 15:00:44.341579 fakts-0.3.8/fakts/fakt/base.py
--rw-r--r--   0        0        0     7106 2023-01-19 09:11:14.533654 fakts-0.3.8/fakts/fakts.py
--rw-r--r--   0        0        0      290 2022-11-18 15:43:40.386023 fakts-0.3.8/fakts/grants/__init__.py
--rw-r--r--   0        0        0      646 2022-11-21 10:33:48.715629 fakts-0.3.8/fakts/grants/base.py
--rw-r--r--   0        0        0     1217 2022-11-18 15:35:11.413064 fakts-0.3.8/fakts/grants/env.py
--rw-r--r--   0        0        0      120 2022-11-18 14:56:49.493394 fakts-0.3.8/fakts/grants/errors.py
--rw-r--r--   0        0        0        0 2022-05-16 14:16:00.394593 fakts-0.3.8/fakts/grants/io/__init__.py
--rw-r--r--   0        0        0     1620 2022-11-20 12:21:45.996177 fakts-0.3.8/fakts/grants/io/qt/yaml.py
--rw-r--r--   0        0        0      268 2022-11-18 14:03:15.348626 fakts-0.3.8/fakts/grants/io/toml.py
--rw-r--r--   0        0        0      292 2022-11-18 13:39:59.149493 fakts-0.3.8/fakts/grants/io/yaml.py
--rw-r--r--   0        0        0      162 2022-11-18 15:32:42.992740 fakts-0.3.8/fakts/grants/meta/__init__.py
--rw-r--r--   0        0        0     2086 2023-01-16 15:55:56.940626 fakts-0.3.8/fakts/grants/meta/cache.py
--rw-r--r--   0        0        0      712 2022-11-18 15:37:31.969349 fakts-0.3.8/fakts/grants/meta/failsafe.py
--rw-r--r--   0        0        0      729 2022-11-17 17:24:28.127678 fakts-0.3.8/fakts/grants/meta/parallel.py
--rw-r--r--   0        0        0      416 2022-11-18 14:13:28.045466 fakts-0.3.8/fakts/grants/remote/__init__.py
--rw-r--r--   0        0        0     4415 2023-01-17 08:54:44.591642 fakts-0.3.8/fakts/grants/remote/base.py
--rw-r--r--   0        0        0     5651 2023-01-16 16:33:21.157569 fakts-0.3.8/fakts/grants/remote/device_code.py
--rw-r--r--   0        0        0      137 2022-11-18 15:37:01.885289 fakts-0.3.8/fakts/grants/remote/errors.py
--rw-r--r--   0        0        0     1907 2023-01-17 09:09:04.877363 fakts-0.3.8/fakts/grants/remote/retrieve.py
--rw-r--r--   0        0        0     1163 2022-11-21 16:58:55.186635 fakts-0.3.8/fakts/grants/remote/static.py
--rw-r--r--   0        0        0      600 2022-11-18 14:56:05.781347 fakts-0.3.8/fakts/utils.py
--rw-r--r--   0        0        0     1398 2023-01-25 09:07:28.300644 fakts-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     4575 1970-01-01 00:00:00.000000 fakts-0.3.8/setup.py
--rw-r--r--   0        0        0     4315 1970-01-01 00:00:00.000000 fakts-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     3465 2022-11-21 11:13:02.484118 fakts-0.3.9/README.md
+-rw-r--r--   0        0        0      263 2022-11-20 14:08:10.639283 fakts-0.3.9/fakts/__init__.py
+-rw-r--r--   0        0        0     1854 2022-11-21 10:34:53.263821 fakts-0.3.9/fakts/cli/main.py
+-rw-r--r--   0        0        0      116 2022-11-21 10:33:13.031539 fakts-0.3.9/fakts/discovery/__init__.py
+-rw-r--r--   0        0        0     4832 2023-01-17 09:16:51.487491 fakts-0.3.9/fakts/discovery/advertised.py
+-rw-r--r--   0        0        0      720 2023-01-16 16:16:06.159933 fakts-0.3.9/fakts/discovery/base.py
+-rw-r--r--   0        0        0      232 2022-11-21 10:35:02.323846 fakts-0.3.9/fakts/discovery/beacon/__init__.py
+-rw-r--r--   0        0        0     4590 2022-11-21 10:32:28.059513 fakts-0.3.9/fakts/discovery/beacon/beacon.py
+-rw-r--r--   0        0        0        0 2022-05-16 14:37:58.382355 fakts-0.3.9/fakts/discovery/qt/__init__.py
+-rw-r--r--   0        0        0     5929 2023-01-18 14:45:01.934170 fakts-0.3.9/fakts/discovery/qt/selectable_beacon.py
+-rw-r--r--   0        0        0      296 2022-11-21 10:31:31.975480 fakts-0.3.9/fakts/discovery/static.py
+-rw-r--r--   0        0        0      279 2022-11-21 10:33:48.715629 fakts-0.3.9/fakts/errors.py
+-rw-r--r--   0        0        0       43 2022-11-17 17:49:20.358443 fakts-0.3.9/fakts/fakt/__init__.py
+-rw-r--r--   0        0        0      309 2022-09-28 15:00:44.341579 fakts-0.3.9/fakts/fakt/base.py
+-rw-r--r--   0        0        0     7106 2023-01-19 09:11:14.533654 fakts-0.3.9/fakts/fakts.py
+-rw-r--r--   0        0        0      290 2022-11-18 15:43:40.386023 fakts-0.3.9/fakts/grants/__init__.py
+-rw-r--r--   0        0        0      646 2022-11-21 10:33:48.715629 fakts-0.3.9/fakts/grants/base.py
+-rw-r--r--   0        0        0     1217 2022-11-18 15:35:11.413064 fakts-0.3.9/fakts/grants/env.py
+-rw-r--r--   0        0        0      120 2022-11-18 14:56:49.493394 fakts-0.3.9/fakts/grants/errors.py
+-rw-r--r--   0        0        0        0 2022-05-16 14:16:00.394593 fakts-0.3.9/fakts/grants/io/__init__.py
+-rw-r--r--   0        0        0     1620 2022-11-20 12:21:45.996177 fakts-0.3.9/fakts/grants/io/qt/yaml.py
+-rw-r--r--   0        0        0      268 2022-11-18 14:03:15.348626 fakts-0.3.9/fakts/grants/io/toml.py
+-rw-r--r--   0        0        0      292 2022-11-18 13:39:59.149493 fakts-0.3.9/fakts/grants/io/yaml.py
+-rw-r--r--   0        0        0      162 2022-11-18 15:32:42.992740 fakts-0.3.9/fakts/grants/meta/__init__.py
+-rw-r--r--   0        0        0     2086 2023-01-16 15:55:56.940626 fakts-0.3.9/fakts/grants/meta/cache.py
+-rw-r--r--   0        0        0      712 2022-11-18 15:37:31.969349 fakts-0.3.9/fakts/grants/meta/failsafe.py
+-rw-r--r--   0        0        0      729 2022-11-17 17:24:28.127678 fakts-0.3.9/fakts/grants/meta/parallel.py
+-rw-r--r--   0        0        0      416 2022-11-18 14:13:28.045466 fakts-0.3.9/fakts/grants/remote/__init__.py
+-rw-r--r--   0        0        0     4415 2023-01-17 08:54:44.591642 fakts-0.3.9/fakts/grants/remote/base.py
+-rw-r--r--   0        0        0     5651 2023-01-25 16:33:16.670670 fakts-0.3.9/fakts/grants/remote/device_code.py
+-rw-r--r--   0        0        0      137 2022-11-18 15:37:01.885289 fakts-0.3.9/fakts/grants/remote/errors.py
+-rw-r--r--   0        0        0     1907 2023-01-17 09:09:04.877363 fakts-0.3.9/fakts/grants/remote/retrieve.py
+-rw-r--r--   0        0        0     1163 2022-11-21 16:58:55.186635 fakts-0.3.9/fakts/grants/remote/static.py
+-rw-r--r--   0        0        0      600 2022-11-18 14:56:05.781347 fakts-0.3.9/fakts/utils.py
+-rw-r--r--   0        0        0     1398 2023-02-03 10:21:07.335950 fakts-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4575 1970-01-01 00:00:00.000000 fakts-0.3.9/setup.py
+-rw-r--r--   0        0        0     4315 1970-01-01 00:00:00.000000 fakts-0.3.9/PKG-INFO
```

### Comparing `fakts-0.3.8/README.md` & `fakts-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/cli/main.py` & `fakts-0.3.9/fakts/cli/main.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/discovery/advertised.py` & `fakts-0.3.9/fakts/discovery/advertised.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/discovery/base.py` & `fakts-0.3.9/fakts/discovery/base.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/discovery/beacon/beacon.py` & `fakts-0.3.9/fakts/discovery/beacon/beacon.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/discovery/qt/selectable_beacon.py` & `fakts-0.3.9/fakts/discovery/qt/selectable_beacon.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/fakts.py` & `fakts-0.3.9/fakts/fakts.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/grants/base.py` & `fakts-0.3.9/fakts/grants/base.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/grants/env.py` & `fakts-0.3.9/fakts/grants/env.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/grants/io/qt/yaml.py` & `fakts-0.3.9/fakts/grants/io/qt/yaml.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/grants/meta/cache.py` & `fakts-0.3.9/fakts/grants/meta/cache.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/grants/meta/failsafe.py` & `fakts-0.3.9/fakts/grants/meta/failsafe.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/grants/meta/parallel.py` & `fakts-0.3.9/fakts/grants/meta/parallel.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/grants/remote/base.py` & `fakts-0.3.9/fakts/grants/remote/base.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/grants/remote/device_code.py` & `fakts-0.3.9/fakts/grants/remote/device_code.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/grants/remote/retrieve.py` & `fakts-0.3.9/fakts/grants/remote/retrieve.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/grants/remote/static.py` & `fakts-0.3.9/fakts/grants/remote/static.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/fakts/utils.py` & `fakts-0.3.9/fakts/utils.py`

 * *Files identical despite different names*

### Comparing `fakts-0.3.8/pyproject.toml` & `fakts-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fakts"
-version = "0.3.8"
+version = "0.3.9"
 description = "asynchronous configuration provider ( tailored to support dynamic client-server relations)"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 readme = "README.md"
 packages = [{ include = "fakts" }]
 
 [tool.poetry.dependencies]
```

### Comparing `fakts-0.3.8/setup.py` & `fakts-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ['PyYAML>=5.2', 'QtPy>=2.0.1,<3.0.0', 'koil>=0.2.10', 'pydantic>1.8.2']
 
 extras_require = \
 {'remote': ['aiohttp>=3.8.2,<4.0.0', 'certifi>2021']}
 
 setup_kwargs = {
     'name': 'fakts',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'asynchronous configuration provider ( tailored to support dynamic client-server relations)',
     'long_description': '# fakts\n\n[![codecov](https://codecov.io/gh/jhnnsrs/fakts/branch/master/graph/badge.svg?token=UGXEA2THBV)](https://codecov.io/gh/jhnnsrs/fakts)\n[![PyPI version](https://badge.fury.io/py/fakts.svg)](https://pypi.org/project/fakts/)\n[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://pypi.org/project/fakts/)\n![Maintainer](https://img.shields.io/badge/maintainer-jhnnsrs-blue)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/fakts.svg)](https://pypi.python.org/pypi/fakts/)\n[![PyPI status](https://img.shields.io/pypi/status/fakts.svg)](https://pypi.python.org/pypi/fakts/)\n[![PyPI download day](https://img.shields.io/pypi/dm/fakts.svg)](https://pypi.python.org/pypi/fakts/)\n\n### DEVELOPMENT\n\n## Inspiration\n\nFakts was designed to make configuration of apps compatible with concurrency pattern, it is designed to allow\nfor asynchronous retrieval of configuration from various sources, may it be a config file, environmental variables\nor a remote server.\n\n# Core Design\n\nFakts uses Grants to obtain configuration asynchronously, a grant is a way of retrieving the configuration from a\nspecific source. It can be a local config file (eg. yaml, toml, json), environemnt variables, a remote configuration (eg. from a fakts server), a database.\nThe fakts class then wraps the grant to ensure both a sychronous and asychronous interface that is threadsafe.\n\nGrants are designed to be composable through MetaGrants so by desigining a specifc grant structure, one can\nhighly customize the retrieval logic. Please check out the\n\n# Example:\n\n```python\nasync with Fakts(grant=YamlGrant("config.yaml")) as fakts:\n    config = await fakts.aget("group_name")\n```\n\nor\n\n```python\nwith Fakts(grant=YamlGrant("config.yaml")) as fakts:\n    config = fakts.get("group_name")\n```\n\nFakts should be used as a context manager, and will set the current fakts context variable to itself, letting\nyou access the current fakts instance from anywhere in your code (async or sync) without specifically passing a referece.\nTo understand how the async sync code access work, please check out the documentation for koil.\n\n# Composability\n\nYou can compose grants through meta grants in order to load configuration from multiple sources (eg. a local, file\nthat can be overwritten by a remote configuration, or some envionment variables).\n\nExample:\n\n```python\nasync with Fakts(grant=FailsafeGrant(\n    grants=[\n        EnvGrant(),\n        YamlGrant("config.yaml")\n    ]\n)) as fakts:\n    config = await fakts.get("group_name")\n```\n\nIn this example fakts will load the configuration from the environment variables first, and if that fails,\nit will load it from the yaml file.\n\n## Special Use Case: Dynamic Server Relations\n\nFakts provides the remote grant protocol for retrieval of configuration in dynamic client-server relationships.\nWith these grants you provide a software manifest for a configuration server (fakts-server), that then grants\nthe configuration (either through user approval (similar to device code grant)). These grants are mainly used\nto setup or claim an oauth2 application on the backend securely that then can be used to identify the application in the\nfuture. These grants are at the moment highly specific to the arkitekt platform and subject to change.\n\n# Sister packages\n\nThese packages provide contrib modules to support auto\nconfiguration through a fakts instance\n\n- herre: oauth2 client\n- rath: graphql client (typed through turms)\n',
     'author': 'jhnnsrs',
     'author_email': 'jhnnsrs@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fakts-0.3.8/PKG-INFO` & `fakts-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakts
-Version: 0.3.8
+Version: 0.3.9
 Summary: asynchronous configuration provider ( tailored to support dynamic client-server relations)
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

