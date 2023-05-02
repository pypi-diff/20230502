# Comparing `tmp/dsw-config-3.22.1.tar.gz` & `tmp/dsw-config-3.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-config-3.22.1.tar", last modified: Fri Apr 14 12:55:22 2023, max compression
+gzip compressed data, was "dsw-config-3.23.0.tar", last modified: Tue May  2 09:24:20 2023, max compression
```

## Comparing `dsw-config-3.22.1.tar` & `dsw-config-3.23.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:22.036068 dsw-config-3.22.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-14 12:55:16.000000 dsw-config-3.22.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-14 12:55:22.036068 dsw-config-3.22.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-14 12:55:16.000000 dsw-config-3.22.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:22.028068 dsw-config-3.22.1/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:22.032068 dsw-config-3.22.1/dsw/config/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-14 12:55:16.000000 dsw-config-3.22.1/dsw/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-14 12:55:21.000000 dsw-config-3.22.1/dsw/config/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-14 12:55:16.000000 dsw-config-3.22.1/dsw/config/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-14 12:55:16.000000 dsw-config-3.22.1/dsw/config/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-14 12:55:16.000000 dsw-config-3.22.1/dsw/config/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:22.036068 dsw-config-3.22.1/dsw_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-14 12:55:22.000000 dsw-config-3.22.1/dsw_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-14 12:55:22.000000 dsw-config-3.22.1/dsw_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:55:22.000000 dsw-config-3.22.1/dsw_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:55:22.000000 dsw-config-3.22.1/dsw_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 12:55:22.000000 dsw-config-3.22.1/dsw_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 12:55:22.000000 dsw-config-3.22.1/dsw_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-14 12:55:16.000000 dsw-config-3.22.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:55:22.036068 dsw-config-3.22.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:55:16.000000 dsw-config-3.22.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:20.216650 dsw-config-3.23.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-02 09:24:14.000000 dsw-config-3.23.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-02 09:24:20.216650 dsw-config-3.23.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-02 09:24:14.000000 dsw-config-3.23.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:20.212650 dsw-config-3.23.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:20.212650 dsw-config-3.23.0/dsw/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 09:24:14.000000 dsw-config-3.23.0/dsw/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-02 09:24:19.000000 dsw-config-3.23.0/dsw/config/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-05-02 09:24:14.000000 dsw-config-3.23.0/dsw/config/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-02 09:24:14.000000 dsw-config-3.23.0/dsw/config/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-02 09:24:14.000000 dsw-config-3.23.0/dsw/config/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-02 09:24:14.000000 dsw-config-3.23.0/dsw/config/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-02 09:24:14.000000 dsw-config-3.23.0/dsw/config/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:20.216650 dsw-config-3.23.0/dsw_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-02 09:24:20.000000 dsw-config-3.23.0/dsw_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-02 09:24:20.000000 dsw-config-3.23.0/dsw_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:24:20.000000 dsw-config-3.23.0/dsw_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:24:20.000000 dsw-config-3.23.0/dsw_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 09:24:20.000000 dsw-config-3.23.0/dsw_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 09:24:20.000000 dsw-config-3.23.0/dsw_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-02 09:24:14.000000 dsw-config-3.23.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:24:20.216650 dsw-config-3.23.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:24:14.000000 dsw-config-3.23.0/setup.py
```

### Comparing `dsw-config-3.22.1/LICENSE` & `dsw-config-3.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-config-3.22.1/PKG-INFO` & `dsw-config-3.23.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: dsw-config
-Version: 3.22.1
+Version: 3.23.0
 Summary: Library for DSW config manipulation
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Python: <4,>=3.7
+Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Data Stewardship Wizard: Config
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ds-wizard/engine-tools)](https://github.com/ds-wizard/engine-tools/releases)
 [![PyPI](https://img.shields.io/pypi/v/dsw-config)](https://pypi.org/project/dsw-config/)
```

### Comparing `dsw-config-3.22.1/README.md` & `dsw-config-3.23.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-config-3.22.1/dsw/config/keys.py` & `dsw-config-3.23.0/dsw/config/keys.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,20 @@
 
 def cast_optional_str(value: Any) -> Optional[str]:
     if value is None:
         return None
     return str(value)
 
 
+def cast_optional_dict(value: Any) -> Optional[dict]:
+    if not isinstance(value, dict):
+        return None
+    return value
+
+
 class ConfigKey(Generic[T]):
 
     def __init__(self, yaml_path: list[str], cast: Callable[[Any], T],
                  var_names=None, default=None, required=False):
         self.yaml_path = yaml_path
         self.var_names = var_names or []  # type: list[str]
         self.default = default
@@ -118,14 +124,20 @@
     )
     format = ConfigKey(
         yaml_path=['logging', 'format'],
         var_names=['LOGGING_FORMAT'],
         default='%(asctime)s | %(levelname)8s | %(name)s: [T:%(traceId)s] %(message)s',
         cast=cast_str,
     )
+    dict_config = ConfigKey(
+        yaml_path=['logging', 'dict_config'],
+        var_names=[],
+        default=None,
+        cast=cast_optional_dict,
+    )
 
 
 class _CloudKeys(ConfigKeysContainer):
     enabled = ConfigKey(
         yaml_path=['cloud', 'enabled'],
         var_names=['CLOUD_ENABLED'],
         default=False,
@@ -138,15 +150,27 @@
         yaml_path=['sentry', 'enabled'],
         var_names=['SENTRY_ENABLED'],
         default=False,
         cast=cast_bool,
     )
     worker_dsn = ConfigKey(
         yaml_path=['sentry', 'workersDsn'],
-        var_names=['SENTRY_WORKER_DSN'],
+        var_names=['SENTRY_WORKER_DSN', 'SENTRY_DSN'],
+        default='',
+        cast=cast_str,
+    )
+    traces_sample_rate = ConfigKey(
+        yaml_path=['sentry', 'tracesSampleRate'],
+        var_names=['SENTRY_TRACES_SAMPLE_RATE'],
+        default='',
+        cast=cast_str,
+    )
+    max_breadcrumbs = ConfigKey(
+        yaml_path=['sentry', 'maxBreadcrumbs'],
+        var_names=['SENTRY_MAX_BREADCRUMBS'],
         default='',
         cast=cast_str,
     )
 
 
 class _DatabaseKeys(ConfigKeysContainer):
     connection_string = ConfigKey(
```

### Comparing `dsw-config-3.22.1/dsw/config/model.py` & `dsw-config-3.23.0/dsw/config/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pathlib
 from typing import Optional
 
+from .logging import prepare_logging, LOG_FILTER
+
 
 def _config_to_string(config: object):
     lines = [f'{type(config).__name__}']
     fields = (f for f in config.__dict__.keys() if not f.startswith('_'))
     for field in fields:
         v = str(getattr(config, field))
         t = type(getattr(config, field)).__name__
@@ -24,17 +26,20 @@
         self.environment = environment
         self.client_url = client_url
         self.secret = secret
 
 
 class SentryConfig(ConfigModel):
 
-    def __init__(self, enabled: bool, workers_dsn: Optional[str]):
+    def __init__(self, enabled: bool, workers_dsn: Optional[str],
+                 traces_sample_rate: Optional[float], max_breadcrumbs: Optional[int]):
         self.enabled = enabled
         self.workers_dsn = workers_dsn
+        self.traces_sample_rate = traces_sample_rate
+        self.max_breadcrumbs = max_breadcrumbs
 
 
 class DatabaseConfig(ConfigModel):
 
     def __init__(self, connection_string: str, connection_timeout: int, queue_timout: int):
         self.connection_string = connection_string
         self.connection_timeout = connection_timeout
@@ -50,18 +55,27 @@
         self.password = password
         self.bucket = bucket
         self.region = region
 
 
 class LoggingConfig(ConfigModel):
 
-    def __init__(self, level: str, global_level: str, message_format: str):
+    def __init__(self, level: str, global_level: str, message_format: str,
+                 dict_config: Optional[dict] = None):
         self.level = level
         self.global_level = global_level
         self.message_format = message_format
+        self.dict_config = dict_config
+
+    def apply(self):
+        prepare_logging(self)
+
+    @staticmethod
+    def set_logging_extra(key: str, value: str):
+        LOG_FILTER.set_extra(key, value)
 
 
 class CloudConfig(ConfigModel):
 
     def __init__(self, multi_tenant: bool):
         self.multi_tenant = multi_tenant
```

### Comparing `dsw-config-3.22.1/dsw/config/parser.py` & `dsw-config-3.23.0/dsw/config/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,27 +98,30 @@
 
     @property
     def logging(self) -> LoggingConfig:
         return LoggingConfig(
             level=self.get(self.keys.logging.level),
             global_level=self.get(self.keys.logging.global_level),
             message_format=self.get(self.keys.logging.format),
+            dict_config=self.get(self.keys.logging.dict_config),
         )
 
     @property
     def cloud(self) -> CloudConfig:
         return CloudConfig(
             multi_tenant=self.get(self.keys.cloud.enabled),
         )
 
     @property
     def sentry(self) -> SentryConfig:
         return SentryConfig(
             enabled=self.get(self.keys.sentry.enabled),
             workers_dsn=self.get(self.keys.sentry.worker_dsn),
+            traces_sample_rate=self.get(self.keys.sentry.traces_sample_rate),
+            max_breadcrumbs=self.get(self.keys.sentry.max_breadcrumbs),
         )
 
     @property
     def general(self) -> GeneralConfig:
         return GeneralConfig(
             environment=self.get(self.keys.general.environment),
             client_url=self.get(self.keys.general.client_url),
```

### Comparing `dsw-config-3.22.1/dsw_config.egg-info/PKG-INFO` & `dsw-config-3.23.0/dsw_config.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: dsw-config
-Version: 3.22.1
+Version: 3.23.0
 Summary: Library for DSW config manipulation
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Python: <4,>=3.7
+Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Data Stewardship Wizard: Config
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ds-wizard/engine-tools)](https://github.com/ds-wizard/engine-tools/releases)
 [![PyPI](https://img.shields.io/pypi/v/dsw-config)](https://pypi.org/project/dsw-config/)
```

### Comparing `dsw-config-3.22.1/pyproject.toml` & `dsw-config-3.23.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-config'
-version = "3.22.1"
+version = "3.23.0"
 description = 'Library for DSW config manipulation'
 readme = 'README.md'
 keywords = ['dsw', 'config', 'yaml', 'parser']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Text Processing',
     'Topic :: Utilities',
 ]
-requires-python = '>=3.7, <4'
+requires-python = '>=3.10, <4'
 dependencies = [
     'PyYAML',
+    'sentry-sdk',
 ]
 
 [project.urls]
 Homepage = 'https://ds-wizard.org'
 Repository = 'https://github.com/ds-wizard/engine-tools'
 Documentation = 'https://guide.ds-wizard.org'
```

