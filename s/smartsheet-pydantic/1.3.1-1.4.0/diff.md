# Comparing `tmp/smartsheet-pydantic-1.3.1.tar.gz` & `tmp/smartsheet-pydantic-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartsheet-pydantic-1.3.1.tar", last modified: Fri Apr 28 21:13:44 2023, max compression
+gzip compressed data, was "smartsheet-pydantic-1.4.0.tar", last modified: Mon May  1 22:50:21 2023, max compression
```

## Comparing `smartsheet-pydantic-1.3.1.tar` & `smartsheet-pydantic-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-28 21:13:44.062747 smartsheet-pydantic-1.3.1/
--rw-r--r--   0 tak       (1000) tak       (1000)     1091 2023-04-22 15:28:56.000000 smartsheet-pydantic-1.3.1/LICENSE
--rw-r--r--   0 tak       (1000) tak       (1000)     8575 2023-04-28 21:13:44.062747 smartsheet-pydantic-1.3.1/PKG-INFO
--rw-r--r--   0 tak       (1000) tak       (1000)     6925 2023-04-28 21:12:54.000000 smartsheet-pydantic-1.3.1/README.md
--rw-r--r--   0 tak       (1000) tak       (1000)      811 2023-04-28 21:12:54.000000 smartsheet-pydantic-1.3.1/pyproject.toml
--rw-r--r--   0 tak       (1000) tak       (1000)       38 2023-04-28 21:13:44.062747 smartsheet-pydantic-1.3.1/setup.cfg
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-28 21:13:44.062747 smartsheet-pydantic-1.3.1/src/
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-28 21:13:44.062747 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/
--rw-r--r--   0 tak       (1000) tak       (1000)        0 2023-04-22 14:53:46.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/__init__.py
--rw-r--r--   0 tak       (1000) tak       (1000)     6740 2023-04-23 22:32:42.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/controller.py
--rw-r--r--   0 tak       (1000) tak       (1000)      493 2023-04-22 14:53:20.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/debug_logger.py
--rw-r--r--   0 tak       (1000) tak       (1000)     2816 2023-04-22 15:44:48.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/filters.py
--rw-r--r--   0 tak       (1000) tak       (1000)    12396 2023-04-23 15:11:22.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/smartmodels.py
--rw-r--r--   0 tak       (1000) tak       (1000)     2309 2023-04-23 16:37:59.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/sources.py
--rw-r--r--   0 tak       (1000) tak       (1000)     2329 2023-04-28 21:12:54.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/transformer.py
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-28 21:13:44.062747 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/
--rw-r--r--   0 tak       (1000) tak       (1000)     8575 2023-04-28 21:13:44.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 tak       (1000) tak       (1000)      622 2023-04-28 21:13:44.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 tak       (1000) tak       (1000)        1 2023-04-28 21:13:44.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 tak       (1000) tak       (1000)      102 2023-04-28 21:13:44.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/requires.txt
--rw-r--r--   0 tak       (1000) tak       (1000)       20 2023-04-28 21:13:44.000000 smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/top_level.txt
-drwxr-xr-x   0 tak       (1000) tak       (1000)        0 2023-04-28 21:13:44.062747 smartsheet-pydantic-1.3.1/tests/
--rw-r--r--   0 tak       (1000) tak       (1000)     4686 2023-04-23 22:32:42.000000 smartsheet-pydantic-1.3.1/tests/test_controller.py
--rw-r--r--   0 tak       (1000) tak       (1000)     3527 2023-04-22 16:01:06.000000 smartsheet-pydantic-1.3.1/tests/test_filters.py
--rw-r--r--   0 tak       (1000) tak       (1000)    13872 2023-04-23 15:11:22.000000 smartsheet-pydantic-1.3.1/tests/test_smartmodel.py
--rw-r--r--   0 tak       (1000) tak       (1000)     1714 2023-04-23 16:37:59.000000 smartsheet-pydantic-1.3.1/tests/test_sources.py
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-01 22:50:21.665284 smartsheet-pydantic-1.4.0/
+-rw-rw-r--   0 agile     (1000) agile     (1000)     1091 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/LICENSE
+-rw-rw-r--   0 agile     (1000) agile     (1000)     8575 2023-05-01 22:50:21.665284 smartsheet-pydantic-1.4.0/PKG-INFO
+-rw-rw-r--   0 agile     (1000) agile     (1000)     6925 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/README.md
+-rw-rw-r--   0 agile     (1000) agile     (1000)      811 2023-05-01 22:46:50.000000 smartsheet-pydantic-1.4.0/pyproject.toml
+-rw-rw-r--   0 agile     (1000) agile     (1000)       38 2023-05-01 22:50:21.665284 smartsheet-pydantic-1.4.0/setup.cfg
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-01 22:50:21.665284 smartsheet-pydantic-1.4.0/src/
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-01 22:50:21.665284 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/
+-rw-rw-r--   0 agile     (1000) agile     (1000)        0 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/__init__.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     6740 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/controller.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)      493 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/debug_logger.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     2816 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/filters.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)    12396 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/smartmodels.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     3087 2023-05-01 22:41:52.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/sources.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     2329 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/transformer.py
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-01 22:50:21.665284 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/
+-rw-rw-r--   0 agile     (1000) agile     (1000)     8575 2023-05-01 22:50:21.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/PKG-INFO
+-rw-rw-r--   0 agile     (1000) agile     (1000)      622 2023-05-01 22:50:21.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 agile     (1000) agile     (1000)        1 2023-05-01 22:50:21.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 agile     (1000) agile     (1000)      102 2023-05-01 22:50:21.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/requires.txt
+-rw-rw-r--   0 agile     (1000) agile     (1000)       20 2023-05-01 22:50:21.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/top_level.txt
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-01 22:50:21.665284 smartsheet-pydantic-1.4.0/tests/
+-rw-rw-r--   0 agile     (1000) agile     (1000)     4686 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/tests/test_controller.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     3527 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/tests/test_filters.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)    13872 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/tests/test_smartmodel.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     1714 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/tests/test_sources.py
```

### Comparing `smartsheet-pydantic-1.3.1/LICENSE` & `smartsheet-pydantic-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.1/PKG-INFO` & `smartsheet-pydantic-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsheet-pydantic
-Version: 1.3.1
+Version: 1.4.0
 Summary: Smartsheet Python SDK and Pydantic Wrapper
 Author: Takahiro Watanabe
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `smartsheet-pydantic-1.3.1/README.md` & `smartsheet-pydantic-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.1/pyproject.toml` & `smartsheet-pydantic-1.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=67.7.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "smartsheet-pydantic"
-version = "1.3.1"
+version = "1.4.0"
 description = "Smartsheet Python SDK and Pydantic Wrapper"
 readme = "README.md"
 authors = [{ name = "Takahiro Watanabe" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/controller.py` & `smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/controller.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/filters.py` & `smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/filters.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/smartmodels.py` & `smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/smartmodels.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/sources.py` & `smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/sources.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+from databricks import sql
 import logging
 import psycopg2
 import requests
 from typing import TypedDict
 
 
 class SourceType(TypedDict):
@@ -102,7 +103,46 @@
         Query the PostgreSQL database, and convert the list[tuple] type into
         list[dict] type, using the given columns attribute.
         """
         results = []
         for row in self._query():
             results.append(dict(zip(self.columns, row)))
         return results
+
+
+class DataSourceDatabricks(DataSource):
+
+    @property
+    @abstractmethod
+    def host(self) -> str:
+        ...
+
+    @property
+    @abstractmethod
+    def http_path(self) -> str:
+        ...
+
+    @property
+    @abstractmethod
+    def access_token(self) -> str:
+        ...
+
+    @property
+    @abstractmethod
+    def query(self) -> str:
+        ...
+
+    @records_count
+    def get(self) -> list[dict]:
+        connection = sql.connect(
+            server_hostname=self.host,
+            http_path=self.http_path,
+            access_token=self.access_token,
+        )
+        cursor = connection.cursor()
+        cursor.execute(self.query)
+        result = cursor.fetchall()
+
+        cursor.close()
+        connection.close()
+
+        return result
```

### Comparing `smartsheet-pydantic-1.3.1/src/smartsheet_pydantic/transformer.py` & `smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/transformer.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/PKG-INFO` & `smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsheet-pydantic
-Version: 1.3.1
+Version: 1.4.0
 Summary: Smartsheet Python SDK and Pydantic Wrapper
 Author: Takahiro Watanabe
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `smartsheet-pydantic-1.3.1/src/smartsheet_pydantic.egg-info/SOURCES.txt` & `smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.1/tests/test_controller.py` & `smartsheet-pydantic-1.4.0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.1/tests/test_filters.py` & `smartsheet-pydantic-1.4.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.1/tests/test_smartmodel.py` & `smartsheet-pydantic-1.4.0/tests/test_smartmodel.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.3.1/tests/test_sources.py` & `smartsheet-pydantic-1.4.0/tests/test_sources.py`

 * *Files identical despite different names*

