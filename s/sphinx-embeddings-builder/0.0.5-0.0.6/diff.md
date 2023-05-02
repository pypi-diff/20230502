# Comparing `tmp/sphinx-embeddings-builder-0.0.5.tar.gz` & `tmp/sphinx-embeddings-builder-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-embeddings-builder-0.0.5.tar", last modified: Tue May  2 20:10:15 2023, max compression
+gzip compressed data, was "sphinx-embeddings-builder-0.0.6.tar", last modified: Tue May  2 20:22:09 2023, max compression
```

## Comparing `sphinx-embeddings-builder-0.0.5.tar` & `sphinx-embeddings-builder-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:10:15.734751 sphinx-embeddings-builder-0.0.5/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       69 2023-05-02 20:10:15.734751 sphinx-embeddings-builder-0.0.5/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)     3540 2023-05-02 18:46:37.000000 sphinx-embeddings-builder-0.0.5/README.md
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-05-02 20:10:15.734751 sphinx-embeddings-builder-0.0.5/setup.cfg
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      330 2023-05-02 20:10:04.000000 sphinx-embeddings-builder-0.0.5/setup.py
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:10:15.734751 sphinx-embeddings-builder-0.0.5/sphinx-embeddings-builder/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)     1909 2023-05-02 20:09:58.000000 sphinx-embeddings-builder-0.0.5/sphinx-embeddings-builder/__init__.py
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:10:15.734751 sphinx-embeddings-builder-0.0.5/sphinx_embeddings_builder.egg-info/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       69 2023-05-02 20:10:15.000000 sphinx-embeddings-builder-0.0.5/sphinx_embeddings_builder.egg-info/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      300 2023-05-02 20:10:15.000000 sphinx-embeddings-builder-0.0.5/sphinx_embeddings_builder.egg-info/SOURCES.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-05-02 20:10:15.000000 sphinx-embeddings-builder-0.0.5/sphinx_embeddings_builder.egg-info/dependency_links.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)     1364 2023-05-02 20:10:15.000000 sphinx-embeddings-builder-0.0.5/sphinx_embeddings_builder.egg-info/requires.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       26 2023-05-02 20:10:15.000000 sphinx-embeddings-builder-0.0.5/sphinx_embeddings_builder.egg-info/top_level.txt
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:22:09.422198 sphinx-embeddings-builder-0.0.6/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       69 2023-05-02 20:22:09.422198 sphinx-embeddings-builder-0.0.6/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)     3681 2023-05-02 20:19:42.000000 sphinx-embeddings-builder-0.0.6/README.md
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-05-02 20:22:09.422198 sphinx-embeddings-builder-0.0.6/setup.cfg
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      330 2023-05-02 20:21:43.000000 sphinx-embeddings-builder-0.0.6/setup.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:22:09.422198 sphinx-embeddings-builder-0.0.6/sphinx-embeddings-builder/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)     1965 2023-05-02 20:21:49.000000 sphinx-embeddings-builder-0.0.6/sphinx-embeddings-builder/__init__.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:22:09.422198 sphinx-embeddings-builder-0.0.6/sphinx_embeddings_builder.egg-info/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       69 2023-05-02 20:22:09.000000 sphinx-embeddings-builder-0.0.6/sphinx_embeddings_builder.egg-info/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      300 2023-05-02 20:22:09.000000 sphinx-embeddings-builder-0.0.6/sphinx_embeddings_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-05-02 20:22:09.000000 sphinx-embeddings-builder-0.0.6/sphinx_embeddings_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)     1364 2023-05-02 20:22:09.000000 sphinx-embeddings-builder-0.0.6/sphinx_embeddings_builder.egg-info/requires.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       26 2023-05-02 20:22:09.000000 sphinx-embeddings-builder-0.0.6/sphinx_embeddings_builder.egg-info/top_level.txt
```

### Comparing `sphinx-embeddings-builder-0.0.5/README.md` & `sphinx-embeddings-builder-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ```
 pip install sphinx-embeddings-builder
 ```
 
 Update `conf.py` in your Sphinx project:
 
-```
+```py
 extensions = [
     # ...
     'sphinx-embeddings-builder
 ]
 
 sphinx_embeddings_builder_max_tokens = my_max_token_size
 sphinx_embeddings_builder_count_tokens = my_token_counting_function
@@ -26,15 +26,15 @@
 **All of the configuration variables are required.** See [Examples] to learn how
 to set them up with different generative AI services.
 
 <h2 id="examples">Examples</h2>
 
 ### Google
 
-```
+```py
 import google.generativeai as palm
 
 # ...
 
 extensions = [
     # ...
     'sphinx-embeddings-builder'
@@ -51,29 +51,35 @@
 }
 
 palm.configure(api_key=palm_api_key, client_options=palm_client_options)
 
 sphinx_embeddings_builder_max_tokens = 1024 # embedding-gecko-001's limit
 
 def count(text):
-    response = palm.count_message_tokens(text)
-    return response['token_count']
+    try:
+        response = palm.count_message_tokens(prompt=text)
+        return response['token_count']
+    except Exception as e:
+        return None
 sphinx_embeddings_builder_count_tokens = count
 
 def gen(text):
-    response = palm.generate_embeddings(model=palm_model, text=text)
-    return response['embedding']
+    try:
+        response = palm.generate_embeddings(model=palm_model, text=text)
+        return response['embedding']
+    except Exception as e:
+        return None
 sphinx_embeddings_builder_generate_embedding = gen
 
 # ...
 ```
 
 ### OpenAI
 
-```
+```py
 from tiktoken import get_encoding
 from openai import key as openai_key, Embedding
 
 # ...
 
 extensions = [
     # ...
```

### Comparing `sphinx-embeddings-builder-0.0.5/sphinx-embeddings-builder/__init__.py` & `sphinx-embeddings-builder-0.0.6/sphinx-embeddings-builder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from sphinx.builders import Builder
 from hashlib import md5
 from os import path
 from json import dump
 from docutils.nodes import section as section_node
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 
 class EmbeddingsBuilder(Builder):
     name = 'embeddings'
     format = 'json'
 
     def init(self):
         self.data = {}
@@ -28,14 +28,16 @@
     def write_doc(self, docname, doctree):
         self.data[docname] = {}
         for section in doctree.traverse(section_node):
             text = section.astext()
             # Checksum should be generated before any modifications are made to the section.
             checksum = md5(text.encode('utf-8')).hexdigest()
             tokens = self.count(text)
+            if tokens is None:
+                continue
             if tokens > self.max_tokens:
                 continue
             self.data[docname][checksum] = {
                 'tokens': tokens,
                 'text': text,
                 'embedding': self.generate(text)
             }
```

### Comparing `sphinx-embeddings-builder-0.0.5/sphinx_embeddings_builder.egg-info/requires.txt` & `sphinx-embeddings-builder-0.0.6/sphinx_embeddings_builder.egg-info/requires.txt`

 * *Files identical despite different names*

