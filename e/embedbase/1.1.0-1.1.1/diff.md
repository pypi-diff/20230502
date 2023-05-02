# Comparing `tmp/embedbase-1.1.0.tar.gz` & `tmp/embedbase-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.1.0.tar", max compression
+gzip compressed data, was "embedbase-1.1.1.tar", max compression
```

## Comparing `embedbase-1.1.0.tar` & `embedbase-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-05-02 14:23:45.366326 embedbase-1.1.0/LICENSE
--rw-r--r--   0        0        0     6149 2023-05-02 14:23:45.366326 embedbase-1.1.0/README.md
--rw-r--r--   0        0        0      121 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/__init__.py
--rw-r--r--   0        0        0     1658 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/api.py
--rw-r--r--   0        0        0    16796 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/database/__init__.py
--rw-r--r--   0        0        0     2848 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/database/base.py
--rw-r--r--   0        0        0     1903 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/database/db_utils.py
--rw-r--r--   0        0        0     4763 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/database/memory_db.py
--rw-r--r--   0        0        0     7946 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     4375 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/logging_utils.py
--rw-r--r--   0        0        0      743 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-02 14:23:45.430330 embedbase-1.1.0/embedbase/utils.py
--rw-r--r--   0        0        0     3636 2023-05-02 14:23:45.434331 embedbase-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     7587 1970-01-01 00:00:00.000000 embedbase-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-02 15:22:23.509918 embedbase-1.1.1/LICENSE
+-rw-r--r--   0        0        0     6149 2023-05-02 15:22:23.509918 embedbase-1.1.1/README.md
+-rw-r--r--   0        0        0      121 2023-05-02 15:22:23.577919 embedbase-1.1.1/embedbase/__init__.py
+-rw-r--r--   0        0        0     1658 2023-05-02 15:22:23.577919 embedbase-1.1.1/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-05-02 15:22:23.577919 embedbase-1.1.1/embedbase/api.py
+-rw-r--r--   0        0        0    16662 2023-05-02 15:22:23.577919 embedbase-1.1.1/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-02 15:22:23.577919 embedbase-1.1.1/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     2848 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/database/base.py
+-rw-r--r--   0        0        0     1903 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/database/db_utils.py
+-rw-r--r--   0        0        0     4763 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0     7946 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     4375 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      743 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-02 15:22:23.581919 embedbase-1.1.1/embedbase/utils.py
+-rw-r--r--   0        0        0     3636 2023-05-02 15:22:23.581919 embedbase-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7587 1970-01-01 00:00:00.000000 embedbase-1.1.1/PKG-INFO
```

### Comparing `embedbase-1.1.0/LICENSE` & `embedbase-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/README.md` & `embedbase-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/__main__.py` & `embedbase-1.1.1/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/api.py` & `embedbase-1.1.1/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/app.py` & `embedbase-1.1.1/embedbase/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,19 +176,17 @@
                 if row["hash"] == doc["hash"]:
                     return doc["embedding"]
             return row["embedding"]
 
         # add existing embeddings to the dataframe
         df["embedding"] = df.apply(update_embedding, args=(existing_documents,), axis=1)
 
-        # generate ids using hash of uuid + time to avoid collisions
+        # generate ids
         df.id = df.apply(
-            lambda x: hashlib.sha256(
-                (str(uuid.uuid4()) + str(time.time())).encode()
-            ).hexdigest(),
+            lambda _: str(uuid.uuid4()),
             axis=1,
         )
 
         # count rows without embeddings
         rows_without_embeddings = df[df.embedding.isna()].shape[0]
 
         self.logger.info(
@@ -291,17 +289,15 @@
                 status_code=400,
                 content={
                     "error": "You need to provide at least one data or metadata to update a document"
                 },
             )
 
         # hash the data
-        df.hash = df.data.apply(
-            lambda x: hashlib.sha256(x.encode()).hexdigest()
-        )
+        df.hash = df.data.apply(lambda x: hashlib.sha256(x.encode()).hexdigest())
 
         df_length = len(df)
 
         self.logger.info(
             f"Checking embeddings computing necessity for {df_length} documents"
         )
         # get existing embeddings from database
@@ -316,15 +312,17 @@
         def update_embedding(row, docs):
             for doc in docs:
                 if row["hash"] == doc["hash"]:
                     return doc["embedding"]
             return row["embedding"]
 
         # add existing embeddings to the dataframe
-        df["embedding"] = df.apply(update_embedding, args=(existing_embeddings,), axis=1)
+        df["embedding"] = df.apply(
+            update_embedding, args=(existing_embeddings,), axis=1
+        )
 
         # compute embeddings for documents without embeddings using embed
         if not df[df.embedding.isna()].empty:
             df[df.embedding.isna()] = df[df.embedding.isna()].assign(
                 embedding=await self.embedder.embed(
                     df[df.embedding.isna()].data.tolist()
                 )
```

### Comparing `embedbase-1.1.0/embedbase/database/base.py` & `embedbase-1.1.1/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/database/db_utils.py` & `embedbase-1.1.1/embedbase/database/db_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/database/memory_db.py` & `embedbase-1.1.1/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/database/postgres_db.py` & `embedbase-1.1.1/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/database/supabase_db.py` & `embedbase-1.1.1/embedbase/database/supabase_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/embedding/base.py` & `embedbase-1.1.1/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/embedding/cohere.py` & `embedbase-1.1.1/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/embedding/openai.py` & `embedbase-1.1.1/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/firebase_auth.py` & `embedbase-1.1.1/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/logging_utils.py` & `embedbase-1.1.1/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/models.py` & `embedbase-1.1.1/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/settings.py` & `embedbase-1.1.1/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/strings.py` & `embedbase-1.1.1/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/embedbase/utils.py` & `embedbase-1.1.1/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.1.0/pyproject.toml` & `embedbase-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.1.0"
+version = "1.1.1"
 description = "API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence"]
```

### Comparing `embedbase-1.1.0/PKG-INFO` & `embedbase-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.1.0
+Version: 1.1.1
 Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

