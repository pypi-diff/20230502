# Comparing `tmp/sphinx-embeddings-builder-0.0.2.tar.gz` & `tmp/sphinx-embeddings-builder-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-embeddings-builder-0.0.2.tar", last modified: Tue May  2 18:56:06 2023, max compression
+gzip compressed data, was "sphinx-embeddings-builder-0.0.3.tar", last modified: Tue May  2 20:01:01 2023, max compression
```

## Comparing `sphinx-embeddings-builder-0.0.2.tar` & `sphinx-embeddings-builder-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 18:56:06.318376 sphinx-embeddings-builder-0.0.2/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       69 2023-05-02 18:56:06.318376 sphinx-embeddings-builder-0.0.2/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)     3540 2023-05-02 18:46:37.000000 sphinx-embeddings-builder-0.0.2/README.md
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-05-02 18:56:06.318376 sphinx-embeddings-builder-0.0.2/setup.cfg
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      330 2023-05-02 18:56:03.000000 sphinx-embeddings-builder-0.0.2/setup.py
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 18:56:06.318376 sphinx-embeddings-builder-0.0.2/sphinx-embeddings-builder/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)     2856 2023-05-02 17:45:26.000000 sphinx-embeddings-builder-0.0.2/sphinx-embeddings-builder/__init__.py
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 18:56:06.318376 sphinx-embeddings-builder-0.0.2/sphinx_embeddings_builder.egg-info/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       69 2023-05-02 18:56:06.000000 sphinx-embeddings-builder-0.0.2/sphinx_embeddings_builder.egg-info/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      300 2023-05-02 18:56:06.000000 sphinx-embeddings-builder-0.0.2/sphinx_embeddings_builder.egg-info/SOURCES.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-05-02 18:56:06.000000 sphinx-embeddings-builder-0.0.2/sphinx_embeddings_builder.egg-info/dependency_links.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)     1364 2023-05-02 18:56:06.000000 sphinx-embeddings-builder-0.0.2/sphinx_embeddings_builder.egg-info/requires.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       26 2023-05-02 18:56:06.000000 sphinx-embeddings-builder-0.0.2/sphinx_embeddings_builder.egg-info/top_level.txt
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:01:01.167222 sphinx-embeddings-builder-0.0.3/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       69 2023-05-02 20:01:01.167222 sphinx-embeddings-builder-0.0.3/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)     3540 2023-05-02 18:46:37.000000 sphinx-embeddings-builder-0.0.3/README.md
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-05-02 20:01:01.167222 sphinx-embeddings-builder-0.0.3/setup.cfg
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      330 2023-05-02 19:59:04.000000 sphinx-embeddings-builder-0.0.3/setup.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:01:01.167222 sphinx-embeddings-builder-0.0.3/sphinx-embeddings-builder/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)     3470 2023-05-02 20:00:41.000000 sphinx-embeddings-builder-0.0.3/sphinx-embeddings-builder/__init__.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:01:01.167222 sphinx-embeddings-builder-0.0.3/sphinx_embeddings_builder.egg-info/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       69 2023-05-02 20:01:01.000000 sphinx-embeddings-builder-0.0.3/sphinx_embeddings_builder.egg-info/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      300 2023-05-02 20:01:01.000000 sphinx-embeddings-builder-0.0.3/sphinx_embeddings_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-05-02 20:01:01.000000 sphinx-embeddings-builder-0.0.3/sphinx_embeddings_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)     1364 2023-05-02 20:01:01.000000 sphinx-embeddings-builder-0.0.3/sphinx_embeddings_builder.egg-info/requires.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       26 2023-05-02 20:01:01.000000 sphinx-embeddings-builder-0.0.3/sphinx_embeddings_builder.egg-info/top_level.txt
```

### Comparing `sphinx-embeddings-builder-0.0.2/README.md` & `sphinx-embeddings-builder-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sphinx-embeddings-builder-0.0.2/sphinx-embeddings-builder/__init__.py` & `sphinx-embeddings-builder-0.0.3/sphinx-embeddings-builder/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,23 +3,35 @@
 from hashlib import md5
 from tiktoken import get_encoding
 from sphinx.util.osutil import ensuredir
 from os import path
 from json import dump
 from docutils.nodes import section as section_node
 import openai
+from sphinx.util import logging
 
 __version__ = '0.0.1'
 
 class EmbeddingsBuilder(Builder):
     name = 'embeddings'
     format = 'json'
 
     def init(self):
         self.data = {}
+        config = dir(self.config)
+        logger = logging.getLogger(__name__)
+        required_config_vars = [
+            'sphinx_embeddings_builder_max_tokens',
+            'sphinx_embeddings_builder_count_tokens',
+            'sphinx_embeddings_builder_generate_embedding'
+        ]
+        for required_config_var in required_config_vars:
+            if config[required_config_var] is None:
+                logger.error('Missing required configuration variable: {}'.format(required_config_var))
+                raise RuntimeError(required_config_var)
         self.count = self.config.sphinx_embeddings_builder_count_tokens
         # self.count = lambda text: 5
         self.generate = self.config.sphinx_embeddings_builder_generate_embedding
         self.max_tokens = self.config.sphinx_embeddings_builder_max_tokens
         # openai.api_key = 'TODO'
         # def gen(text):
         #     model = 'text-embedding-ada-002'
@@ -53,14 +65,15 @@
 
     def finish(self):
         data_path = path.join(self.outdir, 'embeddings.json')
         with open(data_path, 'w') as f:
             dump(self.data, f, indent=2)
 
 def setup(app):
+    logging.stderr = True
     app.add_builder(EmbeddingsBuilder)
     # Defaults to max token size for text-embedding-ada-002
     # https://platform.openai.com/docs/guides/embeddings/embedding-models
     # max_tokens = 8191
     # app.add_config_value('sphinx_embeddings_builder_max_tokens', max_tokens, 'env')
     # count_tokens = lambda text: len(get_encoding('cl100k_base').encode(text))
     app.add_config_value('sphinx_embeddings_builder_count_tokens', None, 'env')
```

### Comparing `sphinx-embeddings-builder-0.0.2/sphinx_embeddings_builder.egg-info/requires.txt` & `sphinx-embeddings-builder-0.0.3/sphinx_embeddings_builder.egg-info/requires.txt`

 * *Files identical despite different names*

