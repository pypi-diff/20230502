# Comparing `tmp/core-braincube-dev-0.0.8.tar.gz` & `tmp/core-braincube-dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core-braincube-dev-0.0.8.tar", last modified: Tue May  2 12:08:19 2023, max compression
+gzip compressed data, was "core-braincube-dev-0.0.9.tar", last modified: Tue May  2 12:26:38 2023, max compression
```

## Comparing `core-braincube-dev-0.0.8.tar` & `core-braincube-dev-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:08:19.607303 core-braincube-dev-0.0.8/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 09:45:18.000000 core-braincube-dev-0.0.8/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     5235 2023-05-02 12:08:19.607537 core-braincube-dev-0.0.8/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4291 2023-05-02 11:38:16.000000 core-braincube-dev-0.0.8/README.md
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:08:19.594381 core-braincube-dev-0.0.8/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:08:19.596972 core-braincube-dev-0.0.8/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1497 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    20547 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:08:19.599120 core-braincube-dev-0.0.8/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3472 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:08:19.601376 core-braincube-dev-0.0.8/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1112 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3026 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-02 11:05:30.000000 core-braincube-dev-0.0.8/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:08:19.604126 core-braincube-dev-0.0.8/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1111 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.8/core/utils/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:08:19.606867 core-braincube-dev-0.0.8/core_braincube_dev.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     5235 2023-05-02 12:08:19.000000 core-braincube-dev-0.0.8/core_braincube_dev.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      604 2023-05-02 12:08:19.000000 core-braincube-dev-0.0.8/core_braincube_dev.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-02 12:08:19.000000 core-braincube-dev-0.0.8/core_braincube_dev.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-02 12:08:19.000000 core-braincube-dev-0.0.8/core_braincube_dev.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-02 12:08:19.000000 core-braincube-dev-0.0.8/core_braincube_dev.egg-info/top_level.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1021 2023-05-02 12:08:19.608435 core-braincube-dev-0.0.8/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 11:28:19.000000 core-braincube-dev-0.0.8/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:26:38.554182 core-braincube-dev-0.0.9/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 09:45:18.000000 core-braincube-dev-0.0.9/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     6830 2023-05-02 12:26:38.554424 core-braincube-dev-0.0.9/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     5886 2023-05-02 12:22:49.000000 core-braincube-dev-0.0.9/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 12:13:15.000000 core-braincube-dev-0.0.9/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1080 2023-05-02 12:26:38.555367 core-braincube-dev-0.0.9/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 11:28:19.000000 core-braincube-dev-0.0.9/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:26:38.538569 core-braincube-dev-0.0.9/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:26:38.540656 core-braincube-dev-0.0.9/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:26:38.543836 core-braincube-dev-0.0.9/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1497 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    20547 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:26:38.546257 core-braincube-dev-0.0.9/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3472 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:26:38.549075 core-braincube-dev-0.0.9/src/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1112 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3026 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-02 11:05:30.000000 core-braincube-dev-0.0.9/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:26:38.551226 core-braincube-dev-0.0.9/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1111 2023-04-29 11:58:44.000000 core-braincube-dev-0.0.9/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-02 12:26:38.553827 core-braincube-dev-0.0.9/src/core_braincube_dev.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     6830 2023-05-02 12:26:38.000000 core-braincube-dev-0.0.9/src/core_braincube_dev.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      703 2023-05-02 12:26:38.000000 core-braincube-dev-0.0.9/src/core_braincube_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-02 12:26:38.000000 core-braincube-dev-0.0.9/src/core_braincube_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-02 12:26:38.000000 core-braincube-dev-0.0.9/src/core_braincube_dev.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-02 12:26:38.000000 core-braincube-dev-0.0.9/src/core_braincube_dev.egg-info/top_level.txt
```

### Comparing `core-braincube-dev-0.0.8/LICENSE` & `core-braincube-dev-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.8/PKG-INFO` & `core-braincube-dev-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-braincube-dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: spresvias@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -52,22 +52,72 @@
 sam deploy --guided --profile analog_user --region eu-west-1
 ```
 
 ### PostgresRepository usage
 
 ```python
 from core.rest.data import HTTPRequest
-from core.dal.data import Key
-from core.dal.postgres_connection import get_pool
+from core.utils.data import Order, OrderType
+from core.dal.data import Key, Schema, Column, Relation, SimpleColumn, JoinType, JoinThrough, StatementField
+from core.dal.postgres_connection import get_pool, Pool
 from core.dal.postgres_repository import PostgresRepository
 
+# schema definition
+equities = Schema(
+    table="equities",
+    alias="e",
+    primary_key=["id"],
+    order=[Order(type=OrderType.asc, alias="name")],
+    statement_fields=[
+        StatementField(alias="isTypeOne",
+                       statement="CASE WHEN e.type = 1 then True else False END",
+                       relations_aliases=[])
+    ],
+    columns=[
+        Column(name="id", updatable=False, insertable=False),
+        Column(name="name"),
+        Column(name="type"),
+        Column(name="issuer_id", alias="issuerId"),
+        Column(name="industry_sector", alias="industrySector"),
+        Column(name="isin"),
+        Column(name="reference"),
+        Column(name="bloomberg_code", alias="bloombergCode"),
+        Column(name="market_symbol", alias="marketSymbol"),
+        Column(name="currency"),
+        Column(name="country", ),
+        Column(name="min_amount", alias="minAmount"),
+    ],
+    relations=[
+        Relation(
+            table="parties",
+            alias="p",
+            force_join=False,
+            columns=[
+                SimpleColumn(name="name"),
+                SimpleColumn(name="short_name", alias="shortName"),
+            ],
+            join_type=JoinType.left,
+            through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
+        )
+    ]
+)
+
+
+# repository definition
+class EquitiesRepo(PostgresRepository):
+
+    def __init__(self, pool: Pool):
+        super().__init__(pool, equities)
+
+
+# repository usage
+
 request = HTTPRequest()
 
-pool = await get_pool()
-repo = PostgresRepository(pool)
+repo = EquitiesRepo(await get_pool())
 
 await repo.find_by_id(key=Key(request.path_parameters["id"]), aliases=request.query_parameters.fields)
 
 await repo.exists_by_id(key=Key("9448a57b-f686-4935-b152-566baab712db"))
 
 await repo.find_one(
     aliases=request.query_parameters.fields,
```

### Comparing `core-braincube-dev-0.0.8/README.md` & `core-braincube-dev-0.0.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -28,22 +28,72 @@
 sam deploy --guided --profile analog_user --region eu-west-1
 ```
 
 ### PostgresRepository usage
 
 ```python
 from core.rest.data import HTTPRequest
-from core.dal.data import Key
-from core.dal.postgres_connection import get_pool
+from core.utils.data import Order, OrderType
+from core.dal.data import Key, Schema, Column, Relation, SimpleColumn, JoinType, JoinThrough, StatementField
+from core.dal.postgres_connection import get_pool, Pool
 from core.dal.postgres_repository import PostgresRepository
 
+# schema definition
+equities = Schema(
+    table="equities",
+    alias="e",
+    primary_key=["id"],
+    order=[Order(type=OrderType.asc, alias="name")],
+    statement_fields=[
+        StatementField(alias="isTypeOne",
+                       statement="CASE WHEN e.type = 1 then True else False END",
+                       relations_aliases=[])
+    ],
+    columns=[
+        Column(name="id", updatable=False, insertable=False),
+        Column(name="name"),
+        Column(name="type"),
+        Column(name="issuer_id", alias="issuerId"),
+        Column(name="industry_sector", alias="industrySector"),
+        Column(name="isin"),
+        Column(name="reference"),
+        Column(name="bloomberg_code", alias="bloombergCode"),
+        Column(name="market_symbol", alias="marketSymbol"),
+        Column(name="currency"),
+        Column(name="country", ),
+        Column(name="min_amount", alias="minAmount"),
+    ],
+    relations=[
+        Relation(
+            table="parties",
+            alias="p",
+            force_join=False,
+            columns=[
+                SimpleColumn(name="name"),
+                SimpleColumn(name="short_name", alias="shortName"),
+            ],
+            join_type=JoinType.left,
+            through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
+        )
+    ]
+)
+
+
+# repository definition
+class EquitiesRepo(PostgresRepository):
+
+    def __init__(self, pool: Pool):
+        super().__init__(pool, equities)
+
+
+# repository usage
+
 request = HTTPRequest()
 
-pool = await get_pool()
-repo = PostgresRepository(pool)
+repo = EquitiesRepo(await get_pool())
 
 await repo.find_by_id(key=Key(request.path_parameters["id"]), aliases=request.query_parameters.fields)
 
 await repo.exists_by_id(key=Key("9448a57b-f686-4935-b152-566baab712db"))
 
 await repo.find_one(
     aliases=request.query_parameters.fields,
```

### Comparing `core-braincube-dev-0.0.8/core/dal/data.py` & `core-braincube-dev-0.0.9/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.8/core/dal/postgres_connection.py` & `core-braincube-dev-0.0.9/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.8/core/dal/postgres_repository.py` & `core-braincube-dev-0.0.9/src/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.8/core/di/data.py` & `core-braincube-dev-0.0.9/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.8/core/di/injector.py` & `core-braincube-dev-0.0.9/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.8/core/rest/app_controller.py` & `core-braincube-dev-0.0.9/src/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.8/core/rest/app_module.py` & `core-braincube-dev-0.0.9/src/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.8/core/rest/data.py` & `core-braincube-dev-0.0.9/src/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.8/core/utils/convert.py` & `core-braincube-dev-0.0.9/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.8/core/utils/data.py` & `core-braincube-dev-0.0.9/src/core/utils/data.py`

 * *Files identical despite different names*

### Comparing `core-braincube-dev-0.0.8/core_braincube_dev.egg-info/PKG-INFO` & `core-braincube-dev-0.0.9/src/core_braincube_dev.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-braincube-dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: spresvias@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -52,22 +52,72 @@
 sam deploy --guided --profile analog_user --region eu-west-1
 ```
 
 ### PostgresRepository usage
 
 ```python
 from core.rest.data import HTTPRequest
-from core.dal.data import Key
-from core.dal.postgres_connection import get_pool
+from core.utils.data import Order, OrderType
+from core.dal.data import Key, Schema, Column, Relation, SimpleColumn, JoinType, JoinThrough, StatementField
+from core.dal.postgres_connection import get_pool, Pool
 from core.dal.postgres_repository import PostgresRepository
 
+# schema definition
+equities = Schema(
+    table="equities",
+    alias="e",
+    primary_key=["id"],
+    order=[Order(type=OrderType.asc, alias="name")],
+    statement_fields=[
+        StatementField(alias="isTypeOne",
+                       statement="CASE WHEN e.type = 1 then True else False END",
+                       relations_aliases=[])
+    ],
+    columns=[
+        Column(name="id", updatable=False, insertable=False),
+        Column(name="name"),
+        Column(name="type"),
+        Column(name="issuer_id", alias="issuerId"),
+        Column(name="industry_sector", alias="industrySector"),
+        Column(name="isin"),
+        Column(name="reference"),
+        Column(name="bloomberg_code", alias="bloombergCode"),
+        Column(name="market_symbol", alias="marketSymbol"),
+        Column(name="currency"),
+        Column(name="country", ),
+        Column(name="min_amount", alias="minAmount"),
+    ],
+    relations=[
+        Relation(
+            table="parties",
+            alias="p",
+            force_join=False,
+            columns=[
+                SimpleColumn(name="name"),
+                SimpleColumn(name="short_name", alias="shortName"),
+            ],
+            join_type=JoinType.left,
+            through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
+        )
+    ]
+)
+
+
+# repository definition
+class EquitiesRepo(PostgresRepository):
+
+    def __init__(self, pool: Pool):
+        super().__init__(pool, equities)
+
+
+# repository usage
+
 request = HTTPRequest()
 
-pool = await get_pool()
-repo = PostgresRepository(pool)
+repo = EquitiesRepo(await get_pool())
 
 await repo.find_by_id(key=Key(request.path_parameters["id"]), aliases=request.query_parameters.fields)
 
 await repo.exists_by_id(key=Key("9448a57b-f686-4935-b152-566baab712db"))
 
 await repo.find_one(
     aliases=request.query_parameters.fields,
```

### Comparing `core-braincube-dev-0.0.8/setup.cfg` & `core-braincube-dev-0.0.9/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = core-braincube-dev
-version = 0.0.8
-url = https://bitbucket.org/braincube-common/core-aws.git
+version = 0.0.9
 author = Braincube
 author_email = spresvias@braincube.gr
-license = MIT
-license_files = LICENSE
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
+url = https://bitbucket.org/braincube-common/core-aws.git
+license = MIT
+license_files = LICENSE
 classifiers = 
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
@@ -20,18 +20,23 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 keywords = python, amazon, aws, lambda, routing, dal, injection
 
 [options]
+package_dir = 
+	= src
+packages = find:
 python_requires = >=3.7, <4
 install_requires = 
 	asyncpg==0.27.0
 	pypika==0.48.9
 	pydantic==1.10.7
-packages = find:
+
+[options.packages.find]
+where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

