# Comparing `tmp/pytest_oar-2.0.1.tar.gz` & `tmp/pytest_oar-2.0.2.tar.gz`

## Comparing `pytest_oar-2.0.1.tar` & `pytest_oar-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/requirements.txt
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/setup.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/oar/__init__.py
--rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/oar/client.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/oar/config.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/oar/consts.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/oar/models.py
--rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/oar/plugin.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/oar/report.py
--rw-r--r--   0        0        0    12969 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/tests/conftest.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/tests/test_client.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/tests/test_config.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/tests/test_models.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/tests/test_report.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/.gitignore
--rw-r--r--   0        0        0    10939 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/README.md
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 pytest_oar-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/requirements.txt
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/setup.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/oar/__init__.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/oar/client.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/oar/config.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/oar/consts.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/oar/models.py
+-rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/oar/plugin.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/oar/report.py
+-rw-r--r--   0        0        0    12969 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/tests/test_client.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/tests/test_config.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/tests/test_models.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/tests/test_report.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/.gitignore
+-rw-r--r--   0        0        0    10939 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/README.md
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 pytest_oar-2.0.2/PKG-INFO
```

### Comparing `pytest_oar-2.0.1/oar/client.py` & `pytest_oar-2.0.2/oar/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             logger.error("Max retries reached for adding test result, continuing but you should probably look at this!")
             return  # Will silently fail
 
         self.__log_error_if_not_ok(response)
         test_id = response.json() if response.ok else None
         return test_id
 
-    def query(self, query: TestQuery) -> str:
+    def query(self, query: TestQuery) -> str | None:
         """
         Will call the ``/query`` endpoint with a TestQuery and return a base64 encoded string to use as the "query"
         parameter for the ``/tests`` methods.
 
         Notes
         -----
         This is here for a complete interface, but you will not need to use this if just working in Python.
@@ -102,20 +102,20 @@
         Parameters
         ----------
         query : TestQuery
             Query to encode
 
         Returns
         -------
-        query_string : str
-            base64 encoded string returned from the endpoint
+        query_string : str | None
+            base64 encoded string returned from the endpoint. None if request failed
         """
         response = self.session.post(self.query_route, json=query.as_request_body())
         self.__log_error_if_not_ok(response)
-        return response.json()
+        return response.json() if response.ok else None
 
     def get_tests(self, query: TestQuery, offset: int = 0, limit: int = 250) -> TestQueryResult | None:
         """
         Sends a GET to the ``/tests`` endpoint to return the results of the test query.
 
         Parameters
         ----------
```

### Comparing `pytest_oar-2.0.1/oar/config.py` & `pytest_oar-2.0.2/oar/config.py`

 * *Files identical despite different names*

### Comparing `pytest_oar-2.0.1/oar/consts.py` & `pytest_oar-2.0.2/oar/consts.py`

 * *Files identical despite different names*

### Comparing `pytest_oar-2.0.1/oar/plugin.py` & `pytest_oar-2.0.2/oar/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_oar-2.0.1/oar/report.py` & `pytest_oar-2.0.2/oar/report.py`

 * *Files identical despite different names*

### Comparing `pytest_oar-2.0.1/tests/conftest.py` & `pytest_oar-2.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_oar-2.0.1/tests/test_config.py` & `pytest_oar-2.0.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pytest_oar-2.0.1/tests/test_models.py` & `pytest_oar-2.0.2/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,8 +84,9 @@
         ----------
         valid_query : dict[str, typing.Any]
             Valid test query
         """
         query = oar.TestQuery(**valid_query)
         request_body = query.as_request_body()
         request_body_query = oar.TestQuery(**request_body)  # Should go both ways
+
         assert query == request_body_query
```

### Comparing `pytest_oar-2.0.1/README.md` & `pytest_oar-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_oar-2.0.1/pyproject.toml` & `pytest_oar-2.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytest-oar"
-version = "2.0.1"
+version = "2.0.2"
 description = "PyTest plugin for the OAR testing framework"
 license = "MIT"
 authors = [
   { name="Ryan de Marigny", email="ryandemarigny@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `pytest_oar-2.0.1/PKG-INFO` & `pytest_oar-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-oar
-Version: 2.0.1
+Version: 2.0.2
 Summary: PyTest plugin for the OAR testing framework
 Project-URL: Homepage, https://github.com/ryandem1/oar
 Project-URL: Bug Tracker, https://github.com/ryandem1/oar/issues
 Author-email: Ryan de Marigny <ryandemarigny@gmail.com>
 License-Expression: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

