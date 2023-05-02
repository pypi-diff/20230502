# Comparing `tmp/dsw-database-3.22.1.tar.gz` & `tmp/dsw-database-3.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-database-3.22.1.tar", last modified: Fri Apr 14 12:55:32 2023, max compression
+gzip compressed data, was "dsw-database-3.23.0.tar", last modified: Tue May  2 09:24:20 2023, max compression
```

## Comparing `dsw-database-3.22.1.tar` & `dsw-database-3.23.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:32.658208 dsw-database-3.22.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-14 12:55:28.000000 dsw-database-3.22.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-14 12:55:32.654209 dsw-database-3.22.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-14 12:55:28.000000 dsw-database-3.22.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:32.654209 dsw-database-3.22.1/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:32.654209 dsw-database-3.22.1/dsw/database/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 12:55:28.000000 dsw-database-3.22.1/dsw/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-14 12:55:32.000000 dsw-database-3.22.1/dsw/database/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-04-14 12:55:28.000000 dsw-database-3.22.1/dsw/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    12483 2023-04-14 12:55:28.000000 dsw-database-3.22.1/dsw/database/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:32.654209 dsw-database-3.22.1/dsw_database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-14 12:55:32.000000 dsw-database-3.22.1/dsw_database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-14 12:55:32.000000 dsw-database-3.22.1/dsw_database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:55:32.000000 dsw-database-3.22.1/dsw_database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:55:32.000000 dsw-database-3.22.1/dsw_database.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-14 12:55:32.000000 dsw-database-3.22.1/dsw_database.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 12:55:32.000000 dsw-database-3.22.1/dsw_database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 12:55:28.000000 dsw-database-3.22.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:55:32.658208 dsw-database-3.22.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:55:28.000000 dsw-database-3.22.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:20.786551 dsw-database-3.23.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-02 09:24:12.000000 dsw-database-3.23.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-02 09:24:20.786551 dsw-database-3.23.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-02 09:24:12.000000 dsw-database-3.23.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:20.782551 dsw-database-3.23.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:20.786551 dsw-database-3.23.0/dsw/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-02 09:24:12.000000 dsw-database-3.23.0/dsw/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-02 09:24:20.000000 dsw-database-3.23.0/dsw/database/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20894 2023-05-02 09:24:12.000000 dsw-database-3.23.0/dsw/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-05-02 09:24:12.000000 dsw-database-3.23.0/dsw/database/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:24:20.786551 dsw-database-3.23.0/dsw_database.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-02 09:24:20.000000 dsw-database-3.23.0/dsw_database.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-02 09:24:20.000000 dsw-database-3.23.0/dsw_database.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:24:20.000000 dsw-database-3.23.0/dsw_database.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:24:20.000000 dsw-database-3.23.0/dsw_database.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 09:24:20.000000 dsw-database-3.23.0/dsw_database.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 09:24:20.000000 dsw-database-3.23.0/dsw_database.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-02 09:24:12.000000 dsw-database-3.23.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:24:20.786551 dsw-database-3.23.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:24:12.000000 dsw-database-3.23.0/setup.py
```

### Comparing `dsw-database-3.22.1/LICENSE` & `dsw-database-3.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-database-3.22.1/PKG-INFO` & `dsw-database-3.23.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: dsw-database
-Version: 3.22.1
+Version: 3.23.0
 Summary: Library for managing DSW database
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,database
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Utilities
-Requires-Python: <4,>=3.7
+Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Data Stewardship Wizard: Database
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ds-wizard/engine-tools)](https://github.com/ds-wizard/engine-tools/releases)
 [![PyPI](https://img.shields.io/pypi/v/dsw-database)](https://pypi.org/project/dsw-database/)
```

### Comparing `dsw-database-3.22.1/README.md` & `dsw-database-3.23.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-database-3.22.1/dsw/database/database.py` & `dsw-database-3.23.0/dsw/database/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,32 +60,34 @@
     SELECT_COMPONENT_INFO = 'SELECT * FROM component WHERE name = %(name)s;'
     SUM_FILE_SIZES = 'SELECT (SELECT COALESCE(SUM(file_size)::bigint, 0) ' \
                      'FROM document WHERE app_uuid = %(app_uuid)s) ' \
                      '+ (SELECT COALESCE(SUM(file_size)::bigint, 0) ' \
                      'FROM document_template_asset WHERE app_uuid = %(app_uuid)s) ' \
                      'as result;'
 
-    def __init__(self, cfg: DatabaseConfig):
+    def __init__(self, cfg: DatabaseConfig, connect: bool = True):
         self.cfg = cfg
         LOG.info('Preparing PostgreSQL connection for QUERY')
         self.conn_query = PostgresConnection(
             name='query',
             dsn=self.cfg.connection_string,
             timeout=self.cfg.connection_timeout,
             autocommit=False,
         )
-        self.conn_query.connect()
+        if connect:
+            self.conn_query.connect()
         LOG.info('Preparing PostgreSQL connection for QUEUE')
         self.conn_queue = PostgresConnection(
             name='queue',
             dsn=self.cfg.connection_string,
             timeout=self.cfg.connection_timeout,
             autocommit=True,
         )
-        self.conn_queue.connect()
+        if connect:
+            self.conn_queue.connect()
 
     def connect(self):
         self.conn_query.connect()
         self.conn_queue.connect()
 
     @tenacity.retry(
         reraise=True,
```

### Comparing `dsw-database-3.22.1/dsw/database/model.py` & `dsw-database-3.23.0/dsw/database/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,15 @@
     @staticmethod
     def from_dict_row(data: dict):
         return DBAppConfig(
             uuid=str(data['uuid']),
             organization=data['organization'],
             authentication=data['authentication'],
             privacy_and_support=data['privacy_and_support'],
-            dashboard=data['dashboard'],
+            dashboard=data['dashboard_and_login_screen'],
             look_and_feel=data['look_and_feel'],
             registry=data['registry'],
             knowledge_model=data['knowledge_model'],
             questionnaire=data['questionnaire'],
             submission=data['submission'],
             feature=data['feature'],
             owl=data['owl'],
```

### Comparing `dsw-database-3.22.1/dsw_database.egg-info/PKG-INFO` & `dsw-database-3.23.0/dsw_database.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: dsw-database
-Version: 3.22.1
+Version: 3.23.0
 Summary: Library for managing DSW database
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,database
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Utilities
-Requires-Python: <4,>=3.7
+Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Data Stewardship Wizard: Database
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ds-wizard/engine-tools)](https://github.com/ds-wizard/engine-tools/releases)
 [![PyPI](https://img.shields.io/pypi/v/dsw-database)](https://pypi.org/project/dsw-database/)
```

### Comparing `dsw-database-3.22.1/pyproject.toml` & `dsw-database-3.23.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-database'
-version = "3.22.1"
+version = "3.23.0"
 description = 'Library for managing DSW database'
 readme = 'README.md'
 keywords = ['dsw', 'database']
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
     'Topic :: Database',
     'Topic :: Utilities',
 ]
-requires-python = '>=3.7, <4'
+requires-python = '>=3.10, <4'
 dependencies = [
     'psycopg[binary]',
     'tenacity',
     # DSW
-    "dsw-config==3.22.1",
+    "dsw-config==3.23.0",
 ]
 
 [project.urls]
 Homepage = 'https://ds-wizard.org'
 Repository = 'https://github.com/ds-wizard/engine-tools'
 Documentation = 'https://guide.ds-wizard.org'
```

