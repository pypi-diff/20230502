# Comparing `tmp/embedbase-1.0.9.tar.gz` & `tmp/embedbase-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.0.9.tar", max compression
+gzip compressed data, was "embedbase-1.1.0.tar", max compression
```

## Comparing `embedbase-1.0.9.tar` & `embedbase-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-05-01 15:27:18.259174 embedbase-1.0.9/LICENSE
--rw-r--r--   0        0        0     5952 2023-05-01 15:27:18.259174 embedbase-1.0.9/README.md
--rw-r--r--   0        0        0      121 2023-05-01 15:27:18.311175 embedbase-1.0.9/embedbase/__init__.py
--rw-r--r--   0        0        0     1658 2023-05-01 15:27:18.311175 embedbase-1.0.9/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-05-01 15:27:18.311175 embedbase-1.0.9/embedbase/api.py
--rw-r--r--   0        0        0    16796 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/__init__.py
--rw-r--r--   0        0        0     2463 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/base.py
--rw-r--r--   0        0        0     1903 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/db_utils.py
--rw-r--r--   0        0        0     4823 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/memory_db.py
--rw-r--r--   0        0        0      504 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/pinecone_db.py
--rw-r--r--   0        0        0     8011 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     4479 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0      411 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/weaviate_db.py
--rw-r--r--   0        0        0       77 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/logging_utils.py
--rw-r--r--   0        0        0      743 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/utils.py
--rw-r--r--   0        0        0     3585 2023-05-01 15:27:18.315175 embedbase-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     7433 1970-01-01 00:00:00.000000 embedbase-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-02 14:23:45.366326 embedbase-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6149 2023-05-02 14:23:45.366326 embedbase-1.1.0/README.md
+-rw-r--r--   0        0        0      121 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/__init__.py
+-rw-r--r--   0        0        0     1658 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/api.py
+-rw-r--r--   0        0        0    16796 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     2848 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/database/base.py
+-rw-r--r--   0        0        0     1903 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/database/db_utils.py
+-rw-r--r--   0        0        0     4763 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0     7946 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     4375 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      743 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/utils.py
+-rw-r--r--   0        0        0     3636 2023-05-02 14:23:45.434331 embedbase-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7587 1970-01-01 00:00:00.000000 embedbase-1.1.0/PKG-INFO
```

### Comparing `embedbase-1.0.9/LICENSE` & `embedbase-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.9/README.md` & `embedbase-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,18 @@
     <a href="https://discord.gg/pMNeuGrDky"><img alt="Discord" src="https://img.shields.io/discord/1066022656845025310?color=black&style=for-the-badge"></a>
     <a href="https://badge.fury.io/py/embedbase"><img alt="PyPI" src="https://img.shields.io/pypi/v/embedbase?color=black&style=for-the-badge"></a>
     <br />
     <a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase-render">
       <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
     </a>
     <br />
+    <a href="https://replit.com/@benjaminshafii/Embedbase-Quickstart-JS?v=1">
+      <img src="https://replit.com/badge?caption=Try%20with%20Replit" alt="Try with Replit Badge">
+    </a>
+    <br />
     <a target="_blank" href="https://colab.research.google.com/github/different-ai/embedbase/blob/main/notebooks/Embedbase_Getting_started.ipynb">
       <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     </a>
     <p align="center">Open-source API & SDK to sync your data and easily hook them up to LLMs</p>
     <p align="center">Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
     <div align="center">
       <a href="https://app.embedbase.xyz/signup">Try Embedbase Cloud now</a>
```

### Comparing `embedbase-1.0.9/embedbase/__main__.py` & `embedbase-1.1.0/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.9/embedbase/api.py` & `embedbase-1.1.0/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.9/embedbase/app.py` & `embedbase-1.1.0/embedbase/app.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.9/embedbase/database/base.py` & `embedbase-1.1.0/embedbase/database/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,33 @@
 from abc import ABC, abstractmethod
+from dataclasses import dataclass
 from typing import Coroutine, List, Optional
 from pandas import DataFrame
 
+@dataclass
+class Dataset:
+    dataset_id: str
+    documents_count: int
+
+@dataclass
+class SearchResponse:
+    score: float
+    id: str
+    data: str
+    hash: str
+    embedding: List[float]
+    metadata: dict
+
+@dataclass
+class SelectResponse:
+    id: str
+    data: str
+    hash: str
+    embedding: List[float]
+    metadata: dict
 
 class VectorDatabase(ABC):
     """
     Base class for all vector databases
     """
     def __init__(self, dimensions: int = 1536):
         self._dimensions = dimensions
@@ -14,15 +36,15 @@
     async def select(
         self,
         ids: List[str] = [],
         hashes: List[str] = [],
         dataset_id: Optional[str] = None,
         user_id: Optional[str] = None,
         distinct: bool = True,
-    ) -> List[dict]:
+    ) -> List[SelectResponse]:
         """
         :param ids: list of ids
         :param hashes: list of hashes
         :param dataset_id: dataset id
         :param user_id: user id
         :param distinct: distinct
         :return: list of documents
@@ -61,15 +83,15 @@
     @abstractmethod
     async def search(
         self,
         vector: List[float],
         top_k: Optional[int],
         dataset_ids: List[str],
         user_id: Optional[str] = None,
-    ) -> List[dict]:
+    ) -> List[SearchResponse]:
         """
         :param vector: vector
         :param top_k: top k
         :param dataset_id: dataset id
         :param user_id: user id
         :return: list of documents
         """
@@ -80,13 +102,13 @@
         """
         :param dataset_id: dataset id
         :param user_id: user id
         """
         raise NotImplementedError
 
     @abstractmethod
-    async def get_datasets(self, user_id: Optional[str] = None) -> List[dict]:
+    async def get_datasets(self, user_id: Optional[str] = None) -> List[Dataset]:
         """
         :param user_id: user id
         :return: list of datasets
         """
         raise NotImplementedError
```

### Comparing `embedbase-1.0.9/embedbase/database/db_utils.py` & `embedbase-1.1.0/embedbase/database/db_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.9/embedbase/database/memory_db.py` & `embedbase-1.1.0/embedbase/database/memory_db.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,14 @@
                 "data": row.data if store_data else None,
                 "embedding": self._np.array(row.embedding),
                 "metadata": row.metadata,
                 "dataset_id": dataset_id,
                 "user_id": user_id,
                 "hash": row.hash,
             }
-        return True
 
     async def select(
         self,
         ids=[],
         hashes=[],
         dataset_id=None,
         user_id=None,
@@ -109,15 +108,14 @@
                 and (
                     dataset_id is None
                     or self.storage[doc_id]["dataset_id"] == dataset_id
                 )
                 and (user_id is None or self.storage[doc_id]["user_id"] == user_id)
             ):
                 del self.storage[doc_id]
-        return None
 
     async def get_datasets(self, user_id=None):
         datasets = {}
         for doc in self.storage.values():
             if user_id is None or doc["user_id"] == user_id:
                 dataset_id = doc["dataset_id"]
                 if dataset_id not in datasets:
@@ -131,8 +129,7 @@
             doc_id
             for doc_id, doc in self.storage.items()
             if doc["dataset_id"] == dataset_id
             and (user_id is None or doc["user_id"] == user_id)
         ]
         for doc_id in doc_ids_to_remove:
             del self.storage[doc_id]
-        return None
```

### Comparing `embedbase-1.0.9/embedbase/database/postgres_db.py` & `embedbase-1.1.0/embedbase/database/postgres_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         self,
         ids: List[str] = [],
         hashes: List[str] = [],
         dataset_id: Optional[str] = None,
         user_id: Optional[str] = None,
         # todo: distinct is not implemented
         distinct: bool = True,
-    ) -> List[dict]:
+    ):
         # either ids or hashes must be provided
         assert ids or hashes, "ids or hashes must be provided"
         from psycopg import sql
 
         query = """
 select id, data, embedding, hash, metadata
 from documents
@@ -196,30 +196,30 @@
             cur.execute(q, flat_values)
 
     async def delete(
         self,
         ids: List[str],
         dataset_id: str,
         user_id: Optional[str] = None,
-    ) -> None:
+    ):
         req = "delete from documents where id in %s and dataset_id = %s", (
             tuple(ids),
             dataset_id,
         )
         if user_id:
             req += f" and user_id = {user_id}"
-        return [dict(row) for row in self.conn.execute(req)]
+        [dict(row) for row in self.conn.execute(req)]
 
     async def search(
         self,
         vector: List[float],
         top_k: Optional[int],
         dataset_ids: List[str],
         user_id: Optional[str] = None,
-    ) -> List[dict]:
+    ):
         d = {
             "query_embedding": str(vector),
             "similarity_threshold": 0,  # TODO: make this configurable
             "match_count": top_k,
             "query_dataset_ids": dataset_ids,
             "query_user_id": user_id,
         }
@@ -238,23 +238,23 @@
                     "hash": row[3],
                     "embedding": row[4].tolist(),
                     "metadata": row[5],
                 }
             )
         return data
 
-    async def clear(self, dataset_id: str, user_id: Optional[str] = None) -> None:
+    async def clear(self, dataset_id: str, user_id: Optional[str] = None):
         req = f"delete from documents where dataset_id = '{dataset_id}'"
         if user_id:
             req += f" and user_id = {user_id}"
         from psycopg import sql
 
         self.conn.execute(req)
 
-    async def get_datasets(self, user_id: Optional[str] = None) -> List[dict]:
+    async def get_datasets(self, user_id: Optional[str] = None):
         req = "select * from distinct_datasets"
         if user_id:
             req += f" where user_id = '{user_id}'"
         results = self.conn.execute(req)
         if results.rowcount == 0:
             return []
         data = []
```

### Comparing `embedbase-1.0.9/embedbase/database/supabase_db.py` & `embedbase-1.1.0/embedbase/database/supabase_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from typing import Coroutine, List, Optional
+from typing import List, Optional
 from pandas import DataFrame, Series
 from embedbase.database import VectorDatabase
 from embedbase.utils import BatchGenerator
 
 
 class Supabase(VectorDatabase):
     def __init__(self, url: str, key: str, **kwargs):
@@ -24,15 +24,15 @@
     async def select(
         self,
         ids: List[str] = [],
         hashes: List[str] = [],
         dataset_id: Optional[str] = None,
         user_id: Optional[str] = None,
         distinct: bool = True,
-    ) -> List[dict]:
+    ):
         # either ids or hashes must be provided
         assert ids or hashes, "ids or hashes must be provided"
 
         req = self.supabase.table("documents").select("*")
         if ids:
             req = req.in_("id", ids)
             if distinct:
@@ -45,25 +45,25 @@
                 # hack: supabase does not support distinct
                 req = req.order("hash", desc=True)
                 req = req.limit(len(hashes))
         if dataset_id:
             req = req.eq("dataset_id", dataset_id)
         if user_id:
             req = req.eq("user_id", user_id)
-        
+
         return req.execute().data
 
     async def update(
         self,
         df: DataFrame,
         dataset_id: str,
         user_id: Optional[str] = None,
         batch_size: Optional[int] = 100,
         store_data: bool = True,
-    ) -> Coroutine:
+    ):
         df_batcher = BatchGenerator(batch_size)
         batches = [batch_df for batch_df in df_batcher(df)]
 
         async def _insert(batch_df: DataFrame):
             def _d(row: Series):
                 data = {
                     "id": row.id,
@@ -89,27 +89,27 @@
         return results
 
     async def delete(
         self,
         ids: List[str],
         dataset_id: str,
         user_id: Optional[str] = None,
-    ) -> None:
+    ):
         req = self.supabase.table("documents").delete().eq("dataset_id", dataset_id)
         if user_id:
             req = req.eq("user_id", user_id)
-        return req.in_("id", ids).execute()
+        req.in_("id", ids).execute()
 
     async def search(
         self,
         vector: List[float],
         top_k: Optional[int],
         dataset_ids: List[str],
         user_id: Optional[str] = None,
-    ) -> List[dict]:
+    ):
         d = {
             "query_embedding": vector,
             "similarity_threshold": 0.1,  # TODO: make this configurable
             "match_count": top_k,
             "query_dataset_ids": dataset_ids,
         }
         if user_id:
@@ -119,21 +119,21 @@
                 "match_documents",
                 d,
             )
             .execute()
             .data
         )
 
-    async def clear(self, dataset_id: str, user_id: Optional[str] = None) -> None:
+    async def clear(self, dataset_id: str, user_id: Optional[str] = None):
         req = self.supabase.table("documents").delete().eq("dataset_id", dataset_id)
         if user_id:
             req = req.eq("user_id", user_id)
-        return req.execute()
+        req.execute()
 
-    async def get_datasets(self, user_id: Optional[str] = None) -> List[dict]:
+    async def get_datasets(self, user_id: Optional[str] = None):
         req = self.supabase.table("distinct_datasets").select(
             "dataset_id", "documents_count"
         )
         if user_id:
             req = req.eq("user_id", user_id)
         data = req.execute().data
         return data
```

### Comparing `embedbase-1.0.9/embedbase/embedding/base.py` & `embedbase-1.1.0/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.9/embedbase/embedding/cohere.py` & `embedbase-1.1.0/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.9/embedbase/embedding/openai.py` & `embedbase-1.1.0/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.9/embedbase/firebase_auth.py` & `embedbase-1.1.0/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.9/embedbase/logging_utils.py` & `embedbase-1.1.0/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.9/embedbase/models.py` & `embedbase-1.1.0/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.9/embedbase/settings.py` & `embedbase-1.1.0/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.9/embedbase/strings.py` & `embedbase-1.1.0/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.9/embedbase/utils.py` & `embedbase-1.1.0/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.9/pyproject.toml` & `embedbase-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.0.9"
+version = "1.1.0"
 description = "API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence"]
@@ -32,15 +32,14 @@
 python = "^3.8"
 
 fastapi = "^0.95.1"
 uvicorn = {extras = ["standard"], version = "^0.15.0"}
 pandas = "^1.3.4"
 openai = "^0.27.0"
 tenacity = "^8.0.1"
-gunicorn = "^20.1.0"
 pydantic_yaml = {extras = ["pyyaml"], version = "^0.4.0"}
 tiktoken = "^0.3.3"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.1"
 black = {version = "^21.10b0", allow-prereleases = true}
 darglint = "^1.8.1"
@@ -53,24 +52,24 @@
 pytest = "^7.3.1"
 pyupgrade = "^2.29.1"
 safety = "^1.10.3"
 coverage = "^6.1.2"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.1.1"
 pytest-cov = "^4.0.0"
-httpx = "^0.24.0"
+httpx = "^0.23.0"
 pytest-asyncio = "^0.21.0"
+requests-mock = "^1.10.0"
 
-[project.optional-dependencies]
-minimal = []
-firebase = ["firebase_admin"]
-observability = ["sentry-sdk[fastapi]"]
-pinecone = ["pinecone-client"]
-supabase = ["supabase"]
-postgres = ["psycopg[binary,pool]", "pgvector"]
+# TODO: following integrations might be moved outside this repo - loose coupling
+firebase-admin = "^6.1.0"
+sentry-sdk = {extras = ["fastapi"], version = "^1.21.1"}
+supabase = "^1.0.3"
+psycopg = {extras = ["binary", "pool"], version = "^3.1.8"}
+pgvector = "^0.1.6"
 
 [tool.black]
 target-version = ["py38"]
 line-length = 88
 color = true
 
 exclude = '''
```

### Comparing `embedbase-1.0.9/PKG-INFO` & `embedbase-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.0.9
+Version: 1.1.0
 Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
@@ -18,15 +18,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
-Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: openai (>=0.27.0,<0.28.0)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: pydantic_yaml[pyyaml] (>=0.4.0,<0.5.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Requires-Dist: uvicorn[standard] (>=0.15.0,<0.16.0)
 Project-URL: Repository, https://github.com/different-ai/embedbase
@@ -47,14 +46,18 @@
     <a href="https://discord.gg/pMNeuGrDky"><img alt="Discord" src="https://img.shields.io/discord/1066022656845025310?color=black&style=for-the-badge"></a>
     <a href="https://badge.fury.io/py/embedbase"><img alt="PyPI" src="https://img.shields.io/pypi/v/embedbase?color=black&style=for-the-badge"></a>
     <br />
     <a href="https://render.com/deploy?repo=https://github.com/different-ai/embedbase-render">
       <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
     </a>
     <br />
+    <a href="https://replit.com/@benjaminshafii/Embedbase-Quickstart-JS?v=1">
+      <img src="https://replit.com/badge?caption=Try%20with%20Replit" alt="Try with Replit Badge">
+    </a>
+    <br />
     <a target="_blank" href="https://colab.research.google.com/github/different-ai/embedbase/blob/main/notebooks/Embedbase_Getting_started.ipynb">
       <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     </a>
     <p align="center">Open-source API & SDK to sync your data and easily hook them up to LLMs</p>
     <p align="center">Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
     <div align="center">
       <a href="https://app.embedbase.xyz/signup">Try Embedbase Cloud now</a>
```

