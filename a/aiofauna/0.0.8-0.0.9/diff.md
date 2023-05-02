# Comparing `tmp/aiofauna-0.0.8.tar.gz` & `tmp/aiofauna-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiofauna-0.0.8.tar", max compression
+gzip compressed data, was "aiofauna-0.0.9.tar", max compression
```

## Comparing `aiofauna-0.0.8.tar` & `aiofauna-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1065 2023-04-09 16:07:24.225577 aiofauna-0.0.8/aiofauna/__init__.py
--rw-r--r--   0        0        0     7816 2023-04-09 15:50:09.852936 aiofauna-0.0.8/aiofauna/application.py
--rw-r--r--   0        0        0     4881 2023-04-09 00:48:46.949196 aiofauna-0.0.8/aiofauna/client.py
--rw-r--r--   0        0        0      493 2023-04-04 07:02:54.142000 aiofauna-0.0.8/aiofauna/deprecated.py
--rw-r--r--   0        0        0     8215 2023-04-09 15:50:12.700726 aiofauna-0.0.8/aiofauna/errors.py
--rw-r--r--   0        0        0     2198 2023-04-09 16:11:33.832628 aiofauna-0.0.8/aiofauna/helpers.py
--rw-r--r--   0        0        0     6724 2023-04-09 00:48:44.968530 aiofauna-0.0.8/aiofauna/json.py
--rw-r--r--   0        0        0     1303 2023-04-09 01:04:59.396687 aiofauna-0.0.8/aiofauna/meta.py
--rw-r--r--   0        0        0     5777 2023-04-09 14:32:34.125477 aiofauna-0.0.8/aiofauna/objects.py
--rw-r--r--   0        0        0    15335 2023-04-04 07:02:51.919994 aiofauna-0.0.8/aiofauna/odm.py
--rw-r--r--   0        0        0     2624 2023-04-04 08:57:42.050368 aiofauna-0.0.8/aiofauna/page.py
--rw-r--r--   0        0        0    41509 2023-04-02 02:01:30.987614 aiofauna-0.0.8/aiofauna/query.py
--rw-r--r--   0        0        0     1132 2023-04-04 08:55:57.371956 aiofauna-0.0.8/LICENSE
--rw-r--r--   0        0        0      589 2023-04-09 16:11:51.916761 aiofauna-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      804 2023-04-09 16:12:11.357240 aiofauna-0.0.8/setup.py
--rw-r--r--   0        0        0      708 2023-04-09 16:12:11.358237 aiofauna-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-10 13:14:14.629944 aiofauna-0.0.9/aiofauna/__init__.py
+-rw-r--r--   0        0        0     7816 2023-04-09 15:50:09.852936 aiofauna-0.0.9/aiofauna/application.py
+-rw-r--r--   0        0        0     4881 2023-04-09 00:48:46.949196 aiofauna-0.0.9/aiofauna/client.py
+-rw-r--r--   0        0        0      493 2023-04-04 07:02:54.142000 aiofauna-0.0.9/aiofauna/deprecated.py
+-rw-r--r--   0        0        0     8215 2023-04-10 13:14:13.610780 aiofauna-0.0.9/aiofauna/errors.py
+-rw-r--r--   0        0        0     2198 2023-04-09 16:11:33.832628 aiofauna-0.0.9/aiofauna/helpers.py
+-rw-r--r--   0        0        0     6724 2023-04-09 00:48:44.968530 aiofauna-0.0.9/aiofauna/json.py
+-rw-r--r--   0        0        0     1303 2023-04-09 01:04:59.396687 aiofauna-0.0.9/aiofauna/meta.py
+-rw-r--r--   0        0        0     5777 2023-04-09 14:32:34.125477 aiofauna-0.0.9/aiofauna/objects.py
+-rw-r--r--   0        0        0    15914 2023-04-10 13:14:11.811186 aiofauna-0.0.9/aiofauna/odm.py
+-rw-r--r--   0        0        0     2624 2023-04-04 08:57:42.050368 aiofauna-0.0.9/aiofauna/page.py
+-rw-r--r--   0        0        0    41509 2023-04-02 02:01:30.987614 aiofauna-0.0.9/aiofauna/query.py
+-rw-r--r--   0        0        0     1132 2023-04-10 13:24:00.328399 aiofauna-0.0.9/LICENSE
+-rw-r--r--   0        0        0      589 2023-04-10 13:25:34.650690 aiofauna-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      804 2023-04-10 13:25:48.777899 aiofauna-0.0.9/setup.py
+-rw-r--r--   0        0        0      708 2023-04-10 13:25:48.777899 aiofauna-0.0.9/PKG-INFO
```

### Comparing `aiofauna-0.0.8/aiofauna/__init__.py` & `aiofauna-0.0.9/aiofauna/__init__.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.8/aiofauna/application.py` & `aiofauna-0.0.9/aiofauna/application.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.8/aiofauna/client.py` & `aiofauna-0.0.9/aiofauna/client.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.8/aiofauna/errors.py` & `aiofauna-0.0.9/aiofauna/errors.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.8/aiofauna/helpers.py` & `aiofauna-0.0.9/aiofauna/helpers.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.8/aiofauna/json.py` & `aiofauna-0.0.9/aiofauna/json.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.8/aiofauna/meta.py` & `aiofauna-0.0.9/aiofauna/meta.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.8/aiofauna/objects.py` & `aiofauna-0.0.9/aiofauna/objects.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.8/aiofauna/odm.py` & `aiofauna-0.0.9/aiofauna/odm.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,35 @@
         Runs a query in FaunaDB.
     """
 
     ref: Optional[str] = None
 
     ts: Optional[int] = None
 
+
+    def __init__(self, **data: Any) -> None:
+
+        for field in self.__fields__.values():
+
+            try:
+                
+                one_of = field.field_info.extra.get("oneOf")
+                
+                if isinstance(one_of, list):
+                
+                    if data.get(field.name) not in one_of:
+                    
+                        raise ValueError(f"{field.name} must be one of {one_of}")
+                    
+            except KeyError:
+                
+                continue
+
+        super().__init__(**data)
+
     @classmethod
     def client(cls) -> AsyncFaunaClient:
         """
 
         Returns an instance of AsyncFaunaClient to interact with FaunaDB.
```

### Comparing `aiofauna-0.0.8/aiofauna/page.py` & `aiofauna-0.0.9/aiofauna/page.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.8/aiofauna/query.py` & `aiofauna-0.0.9/aiofauna/query.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.8/LICENSE` & `aiofauna-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.8/pyproject.toml` & `aiofauna-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiofauna"
-version = "0.0.8"
+version = "0.0.9"
 description = "A developer friendly yet versatile asynchronous Object-Document Mapper for FaunaDB"
 authors = ["Oscar Bahamonde <oscar.bahamonde.dev@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pydantic = {extras = ["dotenv","email"], version = "^1.10.7"}
 aiohttp = "^3.8.4"
```

### Comparing `aiofauna-0.0.8/setup.py` & `aiofauna-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'aiohttp-sse>=2.1.0,<3.0.0',
  'aiohttp>=3.8.4,<4.0.0',
  'iso8601>=1.1.0,<2.0.0',
  'pydantic[dotenv,email]>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'aiofauna',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'A developer friendly yet versatile asynchronous Object-Document Mapper for FaunaDB',
     'long_description': None,
     'author': 'Oscar Bahamonde',
     'author_email': 'oscar.bahamonde.dev@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `aiofauna-0.0.8/PKG-INFO` & `aiofauna-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiofauna
-Version: 0.0.8
+Version: 0.0.9
 Summary: A developer friendly yet versatile asynchronous Object-Document Mapper for FaunaDB
 Author: Oscar Bahamonde
 Author-email: oscar.bahamonde.dev@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

