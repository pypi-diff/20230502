# Comparing `tmp/bal-tools-1.2.9.tar.gz` & `tmp/bal-tools-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bal-tools-1.2.9.tar", last modified: Tue Apr  4 15:20:22 2023, max compression
+gzip compressed data, was "bal-tools-1.3.1.tar", last modified: Tue May  2 09:43:09 2023, max compression
```

## Comparing `bal-tools-1.2.9.tar` & `bal-tools-1.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 egvo      (1000) root         (0)        0 2023-04-04 15:20:22.376299 bal-tools-1.2.9/
--rwxrwxrwx   0 egvo      (1000) root         (0)      623 2023-04-04 15:20:22.376093 bal-tools-1.2.9/PKG-INFO
--rwxrwxrwx   0 egvo      (1000) root         (0)       30 2021-07-12 15:20:15.000000 bal-tools-1.2.9/README.md
-drwxrwxrwx   0 egvo      (1000) root         (0)        0 2023-04-04 15:20:22.369213 bal-tools-1.2.9/bal_tools/
--rwxrwxrwx   0 egvo      (1000) root         (0)       21 2023-04-04 15:20:20.000000 bal-tools-1.2.9/bal_tools/__init__.py
--rwxrwxrwx   0 egvo      (1000) root         (0)     1984 2021-07-12 15:20:15.000000 bal-tools-1.2.9/bal_tools/avito_api.py
--rwxrwxrwx   0 egvo      (1000) root         (0)      535 2021-07-12 15:20:15.000000 bal-tools-1.2.9/bal_tools/common.py
-drwxrwxrwx   0 egvo      (1000) root         (0)        0 2023-04-04 15:20:22.374102 bal-tools-1.2.9/bal_tools/flask/
--rwxrwxrwx   0 egvo      (1000) root         (0)        0 2021-07-12 15:20:15.000000 bal-tools-1.2.9/bal_tools/flask/__init__.py
--rwxrwxrwx   0 egvo      (1000) root         (0)     2989 2021-07-12 16:13:31.000000 bal-tools-1.2.9/bal_tools/flask/api.py
--rwxrwxrwx   0 egvo      (1000) root         (0)     5751 2021-07-12 15:20:15.000000 bal-tools-1.2.9/bal_tools/flask/sessions.py
-drwxrwxrwx   0 egvo      (1000) root         (0)        0 2023-04-04 15:20:22.375333 bal-tools-1.2.9/bal_tools/flask/test_case/
--rwxrwxrwx   0 egvo      (1000) root         (0)        0 2021-07-12 15:20:15.000000 bal-tools-1.2.9/bal_tools/flask/test_case/__init__.py
--rwxrwxrwx   0 egvo      (1000) root         (0)    22803 2023-04-04 15:20:20.000000 bal-tools-1.2.9/bal_tools/flask/test_case/nosql.py
--rwxrwxrwx   0 egvo      (1000) root         (0)     3908 2021-07-12 15:20:15.000000 bal-tools-1.2.9/bal_tools/sbr_api.py
--rwxrwxrwx   0 egvo      (1000) root         (0)      732 2021-07-12 15:20:15.000000 bal-tools-1.2.9/bal_tools/tg_event_messeger.py
-drwxrwxrwx   0 egvo      (1000) root         (0)        0 2023-04-04 15:20:22.372204 bal-tools-1.2.9/bal_tools.egg-info/
--rwxrwxrwx   0 egvo      (1000) root         (0)      623 2023-04-04 15:20:22.000000 bal-tools-1.2.9/bal_tools.egg-info/PKG-INFO
--rwxrwxrwx   0 egvo      (1000) root         (0)      451 2023-04-04 15:20:22.000000 bal-tools-1.2.9/bal_tools.egg-info/SOURCES.txt
--rwxrwxrwx   0 egvo      (1000) root         (0)        1 2023-04-04 15:20:22.000000 bal-tools-1.2.9/bal_tools.egg-info/dependency_links.txt
--rwxrwxrwx   0 egvo      (1000) root         (0)        1 2023-04-04 14:59:28.000000 bal-tools-1.2.9/bal_tools.egg-info/not-zip-safe
--rwxrwxrwx   0 egvo      (1000) root         (0)       10 2023-04-04 15:20:22.000000 bal-tools-1.2.9/bal_tools.egg-info/top_level.txt
--rwxrwxrwx   0 egvo      (1000) root         (0)       38 2023-04-04 15:20:22.376380 bal-tools-1.2.9/setup.cfg
--rwxrwxrwx   0 egvo      (1000) root         (0)      965 2023-04-04 15:20:20.000000 bal-tools-1.2.9/setup.py
+drwxrwxrwx   0 egvo      (1000) root         (0)        0 2023-05-02 09:43:09.660903 bal-tools-1.3.1/
+-rwxrwxrwx   0 egvo      (1000) root         (0)      623 2023-05-02 09:43:09.660474 bal-tools-1.3.1/PKG-INFO
+-rwxrwxrwx   0 egvo      (1000) root         (0)       30 2021-07-12 15:20:15.000000 bal-tools-1.3.1/README.md
+drwxrwxrwx   0 egvo      (1000) root         (0)        0 2023-05-02 09:43:09.654103 bal-tools-1.3.1/bal_tools/
+-rwxrwxrwx   0 egvo      (1000) root         (0)       21 2023-05-02 09:43:05.000000 bal-tools-1.3.1/bal_tools/__init__.py
+-rwxrwxrwx   0 egvo      (1000) root         (0)     1984 2021-07-12 15:20:15.000000 bal-tools-1.3.1/bal_tools/avito_api.py
+-rwxrwxrwx   0 egvo      (1000) root         (0)      535 2021-07-12 15:20:15.000000 bal-tools-1.3.1/bal_tools/common.py
+drwxrwxrwx   0 egvo      (1000) root         (0)        0 2023-05-02 09:43:09.658407 bal-tools-1.3.1/bal_tools/flask/
+-rwxrwxrwx   0 egvo      (1000) root         (0)        0 2021-07-12 15:20:15.000000 bal-tools-1.3.1/bal_tools/flask/__init__.py
+-rwxrwxrwx   0 egvo      (1000) root         (0)     2989 2021-07-12 16:13:31.000000 bal-tools-1.3.1/bal_tools/flask/api.py
+-rwxrwxrwx   0 egvo      (1000) root         (0)     5751 2021-07-12 15:20:15.000000 bal-tools-1.3.1/bal_tools/flask/sessions.py
+drwxrwxrwx   0 egvo      (1000) root         (0)        0 2023-05-02 09:43:09.659730 bal-tools-1.3.1/bal_tools/flask/test_case/
+-rwxrwxrwx   0 egvo      (1000) root         (0)        0 2021-07-12 15:20:15.000000 bal-tools-1.3.1/bal_tools/flask/test_case/__init__.py
+-rwxrwxrwx   0 egvo      (1000) root         (0)    22840 2023-05-02 09:43:05.000000 bal-tools-1.3.1/bal_tools/flask/test_case/nosql.py
+-rwxrwxrwx   0 egvo      (1000) root         (0)     3908 2021-07-12 15:20:15.000000 bal-tools-1.3.1/bal_tools/sbr_api.py
+-rwxrwxrwx   0 egvo      (1000) root         (0)      732 2021-07-12 15:20:15.000000 bal-tools-1.3.1/bal_tools/tg_event_messeger.py
+drwxrwxrwx   0 egvo      (1000) root         (0)        0 2023-05-02 09:43:09.656913 bal-tools-1.3.1/bal_tools.egg-info/
+-rwxrwxrwx   0 egvo      (1000) root         (0)      623 2023-05-02 09:43:09.000000 bal-tools-1.3.1/bal_tools.egg-info/PKG-INFO
+-rwxrwxrwx   0 egvo      (1000) root         (0)      451 2023-05-02 09:43:09.000000 bal-tools-1.3.1/bal_tools.egg-info/SOURCES.txt
+-rwxrwxrwx   0 egvo      (1000) root         (0)        1 2023-05-02 09:43:09.000000 bal-tools-1.3.1/bal_tools.egg-info/dependency_links.txt
+-rwxrwxrwx   0 egvo      (1000) root         (0)        1 2023-04-04 14:59:28.000000 bal-tools-1.3.1/bal_tools.egg-info/not-zip-safe
+-rwxrwxrwx   0 egvo      (1000) root         (0)       10 2023-05-02 09:43:09.000000 bal-tools-1.3.1/bal_tools.egg-info/top_level.txt
+-rwxrwxrwx   0 egvo      (1000) root         (0)       38 2023-05-02 09:43:09.661058 bal-tools-1.3.1/setup.cfg
+-rwxrwxrwx   0 egvo      (1000) root         (0)      965 2023-05-02 09:43:05.000000 bal-tools-1.3.1/setup.py
```

### Comparing `bal-tools-1.2.9/PKG-INFO` & `bal-tools-1.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bal-tools
-Version: 1.2.9
+Version: 1.3.1
 Summary: Black Acorn Labs tools library
 Home-page: https://github.com/blackacornlabs/bal_tools
 Author: BlackAcornLabs
 Author-email: git@blackacorn.io
 License: UNKNOWN
 Description: Black Acorn Labs tools library
 Platform: UNKNOWN
```

### Comparing `bal-tools-1.2.9/bal_tools/avito_api.py` & `bal-tools-1.3.1/bal_tools/avito_api.py`

 * *Files identical despite different names*

### Comparing `bal-tools-1.2.9/bal_tools/common.py` & `bal-tools-1.3.1/bal_tools/common.py`

 * *Files identical despite different names*

### Comparing `bal-tools-1.2.9/bal_tools/flask/api.py` & `bal-tools-1.3.1/bal_tools/flask/api.py`

 * *Files identical despite different names*

### Comparing `bal-tools-1.2.9/bal_tools/flask/sessions.py` & `bal-tools-1.3.1/bal_tools/flask/sessions.py`

 * *Files identical despite different names*

### Comparing `bal-tools-1.2.9/bal_tools/flask/test_case/nosql.py` & `bal-tools-1.3.1/bal_tools/flask/test_case/nosql.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     authorized = False
     url = None
     request_method = None
     test_docs = []
     test_data_file_name = None
     _base_dir = None
     models_map = None
-    counter_map = {}
     template_url = None
     user_for_auth = None
     password_for_auth = 'test_pass'
 
     @classmethod
     def setUpClass(cls, create_app, config, db, *args):
         """
@@ -43,14 +42,15 @@
         # Start flask app
         app = create_app(config)
         cls.client = app.test_client()
         cls.app_context = app.app_context()
         cls.app_context.push()
         cls.db = db
         cls._prepare_database(config=config, db=db)
+        cls.counter_map = {}
 
     @classmethod
     def _prepare_database(cls, config, db):
         """Prepare test database"""
         cls.test_db_name = db.connection._MongoClient__default_database_name
 
         # Check test database name in test db
@@ -63,14 +63,15 @@
 
     @classmethod
     def tearDownClass(cls):
         """Delete test data and stop Flask app"""
         # Удаление тестовой базы и завершение Flask приложения
         cls.db.connection.drop_database(cls.test_db_name)
         cls.app_context.pop()
+        cls.counter_map = {}
 
     @classmethod
     def setUp(cls):
         if not cls.request_method:
             raise AssertionError("Not found request method!")
 
     @classmethod
```

### Comparing `bal-tools-1.2.9/bal_tools/sbr_api.py` & `bal-tools-1.3.1/bal_tools/sbr_api.py`

 * *Files identical despite different names*

### Comparing `bal-tools-1.2.9/bal_tools/tg_event_messeger.py` & `bal-tools-1.3.1/bal_tools/tg_event_messeger.py`

 * *Files identical despite different names*

### Comparing `bal-tools-1.2.9/bal_tools.egg-info/PKG-INFO` & `bal-tools-1.3.1/bal_tools.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bal-tools
-Version: 1.2.9
+Version: 1.3.1
 Summary: Black Acorn Labs tools library
 Home-page: https://github.com/blackacornlabs/bal_tools
 Author: BlackAcornLabs
 Author-email: git@blackacorn.io
 License: UNKNOWN
 Description: Black Acorn Labs tools library
 Platform: UNKNOWN
```

### Comparing `bal-tools-1.2.9/setup.py` & `bal-tools-1.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='bal-tools',
-      version='1.2.9',
+      version='1.3.1',
       url='https://github.com/blackacornlabs/bal_tools',
       long_description=README,
       description='Black Acorn Labs tools library',
       long_description_content_type="text/markdown",
       packages=setuptools.find_packages(),
       author='BlackAcornLabs',
       author_email='git@blackacorn.io',
```

