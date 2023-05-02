# Comparing `tmp/hnsqlite-0.2.0.tar.gz` & `tmp/hnsqlite-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnsqlite-0.2.0.tar", last modified: Mon Apr  3 17:29:12 2023, max compression
+gzip compressed data, was "hnsqlite-0.2.1.tar", last modified: Tue May  2 16:31:40 2023, max compression
```

## Comparing `hnsqlite-0.2.0.tar` & `hnsqlite-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-03 17:29:12.282012 hnsqlite-0.2.0/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-03-20 17:17:48.000000 hnsqlite-0.2.0/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     6300 2023-04-03 17:29:12.281729 hnsqlite-0.2.0/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     5696 2023-04-03 17:17:09.000000 hnsqlite-0.2.0/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-03 17:29:12.279268 hnsqlite-0.2.0/hnsqlite/
--rw-r--r--   0 wsk        (501) staff       (20)      116 2023-03-26 23:42:40.000000 hnsqlite-0.2.0/hnsqlite/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)    27786 2023-04-03 17:02:56.000000 hnsqlite-0.2.0/hnsqlite/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)     4758 2023-03-27 02:41:29.000000 hnsqlite-0.2.0/hnsqlite/filter.py
--rw-r--r--   0 wsk        (501) staff       (20)     1238 2023-03-19 01:38:08.000000 hnsqlite-0.2.0/hnsqlite/util.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-03 17:29:12.280556 hnsqlite-0.2.0/hnsqlite.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     6300 2023-04-03 17:29:12.000000 hnsqlite-0.2.0/hnsqlite.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      346 2023-04-03 17:29:12.000000 hnsqlite-0.2.0/hnsqlite.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-03 17:29:12.000000 hnsqlite-0.2.0/hnsqlite.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       37 2023-04-03 17:29:12.000000 hnsqlite-0.2.0/hnsqlite.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)        9 2023-04-03 17:29:12.000000 hnsqlite-0.2.0/hnsqlite.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      747 2023-04-03 15:54:02.000000 hnsqlite-0.2.0/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-03 17:29:12.282112 hnsqlite-0.2.0/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-03 17:29:12.281391 hnsqlite-0.2.0/test/
--rw-r--r--   0 wsk        (501) staff       (20)    12583 2023-04-03 17:13:06.000000 hnsqlite-0.2.0/test/test_collection.py
--rw-r--r--   0 wsk        (501) staff       (20)     2832 2023-04-03 17:16:06.000000 hnsqlite-0.2.0/test/test_collection_filter.py
--rw-r--r--   0 wsk        (501) staff       (20)    12321 2023-03-20 05:54:20.000000 hnsqlite-0.2.0/test/test_filter.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-02 16:31:40.368013 hnsqlite-0.2.1/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-03-20 17:17:48.000000 hnsqlite-0.2.1/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     7584 2023-05-02 16:31:40.367688 hnsqlite-0.2.1/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     6980 2023-05-01 19:05:01.000000 hnsqlite-0.2.1/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-02 16:31:40.365159 hnsqlite-0.2.1/hnsqlite/
+-rw-r--r--   0 wsk        (501) staff       (20)      116 2023-03-26 23:42:40.000000 hnsqlite-0.2.1/hnsqlite/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)    27458 2023-05-02 16:29:21.000000 hnsqlite-0.2.1/hnsqlite/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4758 2023-03-27 02:41:29.000000 hnsqlite-0.2.1/hnsqlite/filter.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1238 2023-03-19 01:38:08.000000 hnsqlite-0.2.1/hnsqlite/util.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-02 16:31:40.366473 hnsqlite-0.2.1/hnsqlite.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     7584 2023-05-02 16:31:40.000000 hnsqlite-0.2.1/hnsqlite.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      346 2023-05-02 16:31:40.000000 hnsqlite-0.2.1/hnsqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-02 16:31:40.000000 hnsqlite-0.2.1/hnsqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       37 2023-05-02 16:31:40.000000 hnsqlite-0.2.1/hnsqlite.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        9 2023-05-02 16:31:40.000000 hnsqlite-0.2.1/hnsqlite.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      747 2023-05-02 16:21:03.000000 hnsqlite-0.2.1/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-02 16:31:40.368111 hnsqlite-0.2.1/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-02 16:31:40.367292 hnsqlite-0.2.1/test/
+-rw-r--r--   0 wsk        (501) staff       (20)    12583 2023-05-01 19:05:01.000000 hnsqlite-0.2.1/test/test_collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2832 2023-05-01 19:05:01.000000 hnsqlite-0.2.1/test/test_collection_filter.py
+-rw-r--r--   0 wsk        (501) staff       (20)    12321 2023-03-20 05:54:20.000000 hnsqlite-0.2.1/test/test_filter.py
```

### Comparing `hnsqlite-0.2.0/LICENSE` & `hnsqlite-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.0/PKG-INFO` & `hnsqlite-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,62 @@
-Metadata-Version: 2.1
-Name: hnsqlite
-Version: 0.2.0
-Summary: A minimalist integration of sqlite and hnswlib focused on providing simple embedding persistence and search for text applications.
-Author-email: Bill Kish <bk@jiggy.ai>
-Project-URL: Homepage, https://github.com/jiggy-ai/hnsqlite
-Project-URL: Bug Tracker, https://github.com/jiggy-ai/hnsqlite/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # hnsqlite
 
-`hnsqlite` is a text-centric integration of SQLite and [HNSWLIB](https://github.com/nmslib/hnswlib) to provide a persistent collection of embeddings (strings, vectors, and metadata) and search time filtering based on the metadata.
+`hnsqlite` is a text-centric integration of SQLite and [Hnswlib](https://github.com/nmslib/hnswlib) to provide a persistent collection of embeddings (strings, vectors, and metadata) and search time filtering based on the metadata.
 
 ## Classes
 
 ### Collection
 
 The `Collection` class represents a combination of a SQLite database and an HNSWLIB index. The purpose of this class is to provide a persistent collection of embeddings (strings, vectors, and metadata) and search time filtering based on the metadata.
 
-#### Methods
+### Embedding
 
-- `Collection()`:- Initializes a new Collection as a SQLite database file and associated HNSWLIB index. If the specified collection name is found in the database, the collection will be initialized from database. Otherwise, a new collection of the specified name will be created in the database.
-- `save_index`: Saves the current index after updates.
-- `make_index`: Creates an HNSW index that includes all embeddings in the collection database and uses this new index for the collection going forward.
-- `load_index`: Loads the latest HNSW index from disk and uses it for the collection.
-- `add_items`: Adds new items to the collection.
-- `add_embedding`: Adds a single Embedding object to the collection.
-- `add_embeddings`: Adds a list of Embedding objects to the collection.
-- `get_embeddings`: return a list of embeddings from an offset
-- `get_embeddings_doc_ids`: return a list of embeddings associated with specified doc_ids
-- `search`: Queries the HNSW index for the nearest neighbors of the given vector. Supply a k parameter (defaults to 12) and an optional filter dictionary.
-- `delete`: Deletes items from the collection based on a filter, a specific list of document_ids, or everything.
+`Embedding` is a class that represents an embedding sent to or received from the Collection API.
 
-### dbHnswIndexConfig
+**Attributes:**
 
-The `dbHnswIndexConfig` class represents the configuration associated with an HNSWLIB index as stored in the database.
+- `vector`: A list of float values representing the user-supplied vector element. The vector can be sent as a numpy array and will be converted to a list of floats.
+- `text`: The text that was input to the model to generate this embedding.
+- `doc_id`: An optional document_id associated with the embedding.
+- `metadata`: An optional dictionary of metadata associated with the text.
+- `created_at`: The epoch timestamp when the embedding was created (in seconds).
 
-### dbCollectionConfig
+### SearchResponse
 
-The `dbCollectionConfig` class represents the configuration associated with a collection of strings and embeddings as persisted in the database.
+`SearchResponse` is a class derived from the `Embedding` class, specifically designed for returning search results. A `SearchResponse` object consists of an embedding along with its distance to the query vector.
 
-### dbEmbedding
+**Attributes:**
 
-The `dbEmbedding` class represents an embedding as stored in the database.
+- `vector`: A list of float values representing the user-supplied vector element. The vector can be sent as a numpy array and will be converted to a list of floats.
+- `text`: The text that was input to the model to generate this embedding.
+- `doc_id`: An optional document_id associated with the embedding.
+- `metadata`: An optional dictionary of metadata associated with the text.
+- `created_at`: The epoch timestamp when the embedding was created (in seconds).
+- `distance`: A float value representing the cosine similarity distance between the search result and the query vector.  Lower distances represent closer matches.
 
-### Embedding
 
-The `Embedding` class represents an Embedding as sent to/from the Collection API.
+#### Collection Methods
 
-### SearchResponse
+- `Collection()`:- Initializes a new Collection as a SQLite database file and associated HNSWLIB index. If the specified collection name is found in the database, the collection will be initialized from database. Otherwise, a new collection of the specified name will be created in the database.
+- `add_items`: Adds new items to the collection as lists of individual components.  An alternative interface to add_embeddings().
+- `add_embedding`: Adds a single Embedding object to the collection.  A convenience alternative to add_embeddings().
+- `add_embeddings`: Adds a list of Embedding objects to the collection.  An alternative interface to add_items().
+- `get_embeddings`: return a list of embeddings from an offset
+- `get_embeddings_doc_ids`: return a list of embeddings associated with specified doc_ids
+- `search`: Queries the HNSW index for the nearest neighbors of the given vector. Supply a k parameter (defaults to 12) and an optional filter dictionary.
+- `delete`: Deletes items from the collection based on a filter, a specific list of document_ids, or everything.
+
+
+### Database classes
+
+The following classes are the internal SqlModel data classes used to persist the embeddings and configuration in sqlite. They are not directly accessed by the user, but will be created as tables in the sqlite database:
+ - The `dbHnswIndexConfig` class represents the configuration associated with an HNSWLIB index as stored in the database.  
+ - The `dbCollectionConfig` class represents the configuration associated with a collection of strings and embeddings as persisted in the database.
+ - The `dbEmbedding` class represents an embedding as stored in the database.
 
-The `SearchResponse` class represents the response of a search operation, containing the item (embedding) and its distance from the query vector.
 
 
 ## Usage
 
 To use `hnsqlite`, you can create a new collection, add items to it, and perform search operations. Here's an example:
```

### Comparing `hnsqlite-0.2.0/README.md` & `hnsqlite-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,76 @@
+Metadata-Version: 2.1
+Name: hnsqlite
+Version: 0.2.1
+Summary: A minimalist integration of sqlite and hnswlib focused on providing simple embedding persistence and search for text applications.
+Author-email: Bill Kish <bk@jiggy.ai>
+Project-URL: Homepage, https://github.com/jiggy-ai/hnsqlite
+Project-URL: Bug Tracker, https://github.com/jiggy-ai/hnsqlite/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # hnsqlite
 
-`hnsqlite` is a text-centric integration of SQLite and [HNSWLIB](https://github.com/nmslib/hnswlib) to provide a persistent collection of embeddings (strings, vectors, and metadata) and search time filtering based on the metadata.
+`hnsqlite` is a text-centric integration of SQLite and [Hnswlib](https://github.com/nmslib/hnswlib) to provide a persistent collection of embeddings (strings, vectors, and metadata) and search time filtering based on the metadata.
 
 ## Classes
 
 ### Collection
 
 The `Collection` class represents a combination of a SQLite database and an HNSWLIB index. The purpose of this class is to provide a persistent collection of embeddings (strings, vectors, and metadata) and search time filtering based on the metadata.
 
-#### Methods
+### Embedding
 
-- `Collection()`:- Initializes a new Collection as a SQLite database file and associated HNSWLIB index. If the specified collection name is found in the database, the collection will be initialized from database. Otherwise, a new collection of the specified name will be created in the database.
-- `save_index`: Saves the current index after updates.
-- `make_index`: Creates an HNSW index that includes all embeddings in the collection database and uses this new index for the collection going forward.
-- `load_index`: Loads the latest HNSW index from disk and uses it for the collection.
-- `add_items`: Adds new items to the collection.
-- `add_embedding`: Adds a single Embedding object to the collection.
-- `add_embeddings`: Adds a list of Embedding objects to the collection.
-- `get_embeddings`: return a list of embeddings from an offset
-- `get_embeddings_doc_ids`: return a list of embeddings associated with specified doc_ids
-- `search`: Queries the HNSW index for the nearest neighbors of the given vector. Supply a k parameter (defaults to 12) and an optional filter dictionary.
-- `delete`: Deletes items from the collection based on a filter, a specific list of document_ids, or everything.
+`Embedding` is a class that represents an embedding sent to or received from the Collection API.
 
-### dbHnswIndexConfig
+**Attributes:**
 
-The `dbHnswIndexConfig` class represents the configuration associated with an HNSWLIB index as stored in the database.
+- `vector`: A list of float values representing the user-supplied vector element. The vector can be sent as a numpy array and will be converted to a list of floats.
+- `text`: The text that was input to the model to generate this embedding.
+- `doc_id`: An optional document_id associated with the embedding.
+- `metadata`: An optional dictionary of metadata associated with the text.
+- `created_at`: The epoch timestamp when the embedding was created (in seconds).
 
-### dbCollectionConfig
+### SearchResponse
 
-The `dbCollectionConfig` class represents the configuration associated with a collection of strings and embeddings as persisted in the database.
+`SearchResponse` is a class derived from the `Embedding` class, specifically designed for returning search results. A `SearchResponse` object consists of an embedding along with its distance to the query vector.
 
-### dbEmbedding
+**Attributes:**
 
-The `dbEmbedding` class represents an embedding as stored in the database.
+- `vector`: A list of float values representing the user-supplied vector element. The vector can be sent as a numpy array and will be converted to a list of floats.
+- `text`: The text that was input to the model to generate this embedding.
+- `doc_id`: An optional document_id associated with the embedding.
+- `metadata`: An optional dictionary of metadata associated with the text.
+- `created_at`: The epoch timestamp when the embedding was created (in seconds).
+- `distance`: A float value representing the cosine similarity distance between the search result and the query vector.  Lower distances represent closer matches.
 
-### Embedding
 
-The `Embedding` class represents an Embedding as sent to/from the Collection API.
+#### Collection Methods
 
-### SearchResponse
+- `Collection()`:- Initializes a new Collection as a SQLite database file and associated HNSWLIB index. If the specified collection name is found in the database, the collection will be initialized from database. Otherwise, a new collection of the specified name will be created in the database.
+- `add_items`: Adds new items to the collection as lists of individual components.  An alternative interface to add_embeddings().
+- `add_embedding`: Adds a single Embedding object to the collection.  A convenience alternative to add_embeddings().
+- `add_embeddings`: Adds a list of Embedding objects to the collection.  An alternative interface to add_items().
+- `get_embeddings`: return a list of embeddings from an offset
+- `get_embeddings_doc_ids`: return a list of embeddings associated with specified doc_ids
+- `search`: Queries the HNSW index for the nearest neighbors of the given vector. Supply a k parameter (defaults to 12) and an optional filter dictionary.
+- `delete`: Deletes items from the collection based on a filter, a specific list of document_ids, or everything.
+
+
+### Database classes
+
+The following classes are the internal SqlModel data classes used to persist the embeddings and configuration in sqlite. They are not directly accessed by the user, but will be created as tables in the sqlite database:
+ - The `dbHnswIndexConfig` class represents the configuration associated with an HNSWLIB index as stored in the database.  
+ - The `dbCollectionConfig` class represents the configuration associated with a collection of strings and embeddings as persisted in the database.
+ - The `dbEmbedding` class represents an embedding as stored in the database.
 
-The `SearchResponse` class represents the response of a search operation, containing the item (embedding) and its distance from the query vector.
 
 
 ## Usage
 
 To use `hnsqlite`, you can create a new collection, add items to it, and perform search operations. Here's an example:
```

### Comparing `hnsqlite-0.2.0/hnsqlite/collection.py` & `hnsqlite-0.2.1/hnsqlite/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,39 +231,36 @@
 
     @classmethod
     def _save_index_to_disk(cls, name: str, hnsw_ix : dbHnswIndexConfig) -> Tuple[str, str, int]:
         """
         Save the current index to disk and return the filename, md5sum, and count of items in the index
         """
         count = len(hnsw_ix.get_ids_list())
-        filename = f"index_{name}_{count}_{int(1000 * time())}.hnsw"
+        filename = f"index_{name}.hnsw"
+        try:
+            os.unlink(filename)
+        except:
+            pass
         hnsw_ix.save_index(filename)
         md5sum = md5_file(filename)
         logger.info(f"saved index to {filename} with md5sum {md5sum} and {count} items")
         return filename, md5sum, count
 
     def _save_index_to_db(self, index: dbHnswIndexConfig, delete_previous_index=True):
         """
         Save the current index config to the database
         """
         with Session(self.db_engine) as session:
-            # delete old index from database and filesystem
-            old_filenames = []
+            # delete old index from database
             if delete_previous_index:
                 for old_index in session.query(dbHnswIndexConfig).filter(dbHnswIndexConfig.collection_id == self.config.id).all():
-                    old_filenames.append(old_index.filename)
                     session.delete(old_index)
             session.add(index)
             session.commit()   # commit the new index record and deletion of the old index records
             session.refresh(index)
-            for fn in old_filenames:
-                try:
-                    os.remove(fn) # finally remove the old index files from the filesystem after the commit
-                except:
-                    logger.debug(f"exception removing old index file {fn}")
             logger.info(f"saved index to database with id {index.id}")
 
         
     def save_index(self, delete_previous_index=True) -> str:
         """
         Save the current hnsw index
         Used to persist the dbHnswIndexConfig after calling add_items or delete_items
@@ -349,15 +346,16 @@
             if not index_config:
                 self.make_index()   # intialize and load the index
                 return
         logger.info(f"loading index {index_config}")
         md5sum = md5_file(index_config.filename)
         if md5sum != index_config.md5sum:
             logger.error(f"md5sum {md5sum} does not match config.md5sum {index_config.md5sum}")
-            raise Exception(f"md5sum {md5sum} does not match config.md5sum {index_config.md5sum}")
+            self.make_index()   # intialize and load the index from scratch
+            return
         else:
             logger.info(f"md5sum matches index.md5sum")
         hnsw_ix = hnswlib.Index(space='cosine', dim=self.config.dim)
         hnsw_ix.load_index(index_config.filename, max_elements=index_config.count, allow_replace_deleted=True)
         hnsw_ix.set_ef(index_config.ef)
         hnsw_ix.set_num_threads(1)   # filtering requires 1 thread only
         logger.info(f"load hnswlib index {index_config} complete")
```

### Comparing `hnsqlite-0.2.0/hnsqlite/filter.py` & `hnsqlite-0.2.1/hnsqlite/filter.py`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.0/hnsqlite/util.py` & `hnsqlite-0.2.1/hnsqlite/util.py`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.0/hnsqlite.egg-info/PKG-INFO` & `hnsqlite-0.2.1/hnsqlite.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,76 @@
 Metadata-Version: 2.1
 Name: hnsqlite
-Version: 0.2.0
+Version: 0.2.1
 Summary: A minimalist integration of sqlite and hnswlib focused on providing simple embedding persistence and search for text applications.
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/hnsqlite
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/hnsqlite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hnsqlite
 
-`hnsqlite` is a text-centric integration of SQLite and [HNSWLIB](https://github.com/nmslib/hnswlib) to provide a persistent collection of embeddings (strings, vectors, and metadata) and search time filtering based on the metadata.
+`hnsqlite` is a text-centric integration of SQLite and [Hnswlib](https://github.com/nmslib/hnswlib) to provide a persistent collection of embeddings (strings, vectors, and metadata) and search time filtering based on the metadata.
 
 ## Classes
 
 ### Collection
 
 The `Collection` class represents a combination of a SQLite database and an HNSWLIB index. The purpose of this class is to provide a persistent collection of embeddings (strings, vectors, and metadata) and search time filtering based on the metadata.
 
-#### Methods
+### Embedding
 
-- `Collection()`:- Initializes a new Collection as a SQLite database file and associated HNSWLIB index. If the specified collection name is found in the database, the collection will be initialized from database. Otherwise, a new collection of the specified name will be created in the database.
-- `save_index`: Saves the current index after updates.
-- `make_index`: Creates an HNSW index that includes all embeddings in the collection database and uses this new index for the collection going forward.
-- `load_index`: Loads the latest HNSW index from disk and uses it for the collection.
-- `add_items`: Adds new items to the collection.
-- `add_embedding`: Adds a single Embedding object to the collection.
-- `add_embeddings`: Adds a list of Embedding objects to the collection.
-- `get_embeddings`: return a list of embeddings from an offset
-- `get_embeddings_doc_ids`: return a list of embeddings associated with specified doc_ids
-- `search`: Queries the HNSW index for the nearest neighbors of the given vector. Supply a k parameter (defaults to 12) and an optional filter dictionary.
-- `delete`: Deletes items from the collection based on a filter, a specific list of document_ids, or everything.
+`Embedding` is a class that represents an embedding sent to or received from the Collection API.
 
-### dbHnswIndexConfig
+**Attributes:**
 
-The `dbHnswIndexConfig` class represents the configuration associated with an HNSWLIB index as stored in the database.
+- `vector`: A list of float values representing the user-supplied vector element. The vector can be sent as a numpy array and will be converted to a list of floats.
+- `text`: The text that was input to the model to generate this embedding.
+- `doc_id`: An optional document_id associated with the embedding.
+- `metadata`: An optional dictionary of metadata associated with the text.
+- `created_at`: The epoch timestamp when the embedding was created (in seconds).
 
-### dbCollectionConfig
+### SearchResponse
 
-The `dbCollectionConfig` class represents the configuration associated with a collection of strings and embeddings as persisted in the database.
+`SearchResponse` is a class derived from the `Embedding` class, specifically designed for returning search results. A `SearchResponse` object consists of an embedding along with its distance to the query vector.
 
-### dbEmbedding
+**Attributes:**
 
-The `dbEmbedding` class represents an embedding as stored in the database.
+- `vector`: A list of float values representing the user-supplied vector element. The vector can be sent as a numpy array and will be converted to a list of floats.
+- `text`: The text that was input to the model to generate this embedding.
+- `doc_id`: An optional document_id associated with the embedding.
+- `metadata`: An optional dictionary of metadata associated with the text.
+- `created_at`: The epoch timestamp when the embedding was created (in seconds).
+- `distance`: A float value representing the cosine similarity distance between the search result and the query vector.  Lower distances represent closer matches.
 
-### Embedding
 
-The `Embedding` class represents an Embedding as sent to/from the Collection API.
+#### Collection Methods
 
-### SearchResponse
+- `Collection()`:- Initializes a new Collection as a SQLite database file and associated HNSWLIB index. If the specified collection name is found in the database, the collection will be initialized from database. Otherwise, a new collection of the specified name will be created in the database.
+- `add_items`: Adds new items to the collection as lists of individual components.  An alternative interface to add_embeddings().
+- `add_embedding`: Adds a single Embedding object to the collection.  A convenience alternative to add_embeddings().
+- `add_embeddings`: Adds a list of Embedding objects to the collection.  An alternative interface to add_items().
+- `get_embeddings`: return a list of embeddings from an offset
+- `get_embeddings_doc_ids`: return a list of embeddings associated with specified doc_ids
+- `search`: Queries the HNSW index for the nearest neighbors of the given vector. Supply a k parameter (defaults to 12) and an optional filter dictionary.
+- `delete`: Deletes items from the collection based on a filter, a specific list of document_ids, or everything.
+
+
+### Database classes
+
+The following classes are the internal SqlModel data classes used to persist the embeddings and configuration in sqlite. They are not directly accessed by the user, but will be created as tables in the sqlite database:
+ - The `dbHnswIndexConfig` class represents the configuration associated with an HNSWLIB index as stored in the database.  
+ - The `dbCollectionConfig` class represents the configuration associated with a collection of strings and embeddings as persisted in the database.
+ - The `dbEmbedding` class represents an embedding as stored in the database.
 
-The `SearchResponse` class represents the response of a search operation, containing the item (embedding) and its distance from the query vector.
 
 
 ## Usage
 
 To use `hnsqlite`, you can create a new collection, add items to it, and perform search operations. Here's an example:
```

### Comparing `hnsqlite-0.2.0/pyproject.toml` & `hnsqlite-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hnsqlite"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['sqlmodel', 'hnswlib', 'psutil', 'numpy', 'loguru']
 description = "A minimalist integration of sqlite and hnswlib focused on providing simple embedding persistence and search for text applications."
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `hnsqlite-0.2.0/test/test_collection.py` & `hnsqlite-0.2.1/test/test_collection.py`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.0/test/test_collection_filter.py` & `hnsqlite-0.2.1/test/test_collection_filter.py`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.0/test/test_filter.py` & `hnsqlite-0.2.1/test/test_filter.py`

 * *Files identical despite different names*

