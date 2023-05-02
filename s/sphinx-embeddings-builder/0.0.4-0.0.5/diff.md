# Comparing `tmp/sphinx-embeddings-builder-0.0.4.tar.gz` & `tmp/sphinx-embeddings-builder-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-embeddings-builder-0.0.4.tar", last modified: Tue May  2 20:06:53 2023, max compression
+gzip compressed data, was "sphinx-embeddings-builder-0.0.5.tar", last modified: Tue May  2 20:10:15 2023, max compression
```

## Comparing `sphinx-embeddings-builder-0.0.4.tar` & `sphinx-embeddings-builder-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:06:53.906916 sphinx-embeddings-builder-0.0.4/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       69 2023-05-02 20:06:53.906916 sphinx-embeddings-builder-0.0.4/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)     3540 2023-05-02 18:46:37.000000 sphinx-embeddings-builder-0.0.4/README.md
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-05-02 20:06:53.906916 sphinx-embeddings-builder-0.0.4/setup.cfg
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      330 2023-05-02 20:06:21.000000 sphinx-embeddings-builder-0.0.4/setup.py
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:06:53.906916 sphinx-embeddings-builder-0.0.4/sphinx-embeddings-builder/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)     2053 2023-05-02 20:06:31.000000 sphinx-embeddings-builder-0.0.4/sphinx-embeddings-builder/__init__.py
-drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:06:53.906916 sphinx-embeddings-builder-0.0.4/sphinx_embeddings_builder.egg-info/
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       69 2023-05-02 20:06:53.000000 sphinx-embeddings-builder-0.0.4/sphinx_embeddings_builder.egg-info/PKG-INFO
--rw-r--r--   0 kayce    (319046) primarygroup (89939)      300 2023-05-02 20:06:53.000000 sphinx-embeddings-builder-0.0.4/sphinx_embeddings_builder.egg-info/SOURCES.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-05-02 20:06:53.000000 sphinx-embeddings-builder-0.0.4/sphinx_embeddings_builder.egg-info/dependency_links.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)     1364 2023-05-02 20:06:53.000000 sphinx-embeddings-builder-0.0.4/sphinx_embeddings_builder.egg-info/requires.txt
--rw-r--r--   0 kayce    (319046) primarygroup (89939)       26 2023-05-02 20:06:53.000000 sphinx-embeddings-builder-0.0.4/sphinx_embeddings_builder.egg-info/top_level.txt
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:10:15.734751 sphinx-embeddings-builder-0.0.5/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       69 2023-05-02 20:10:15.734751 sphinx-embeddings-builder-0.0.5/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)     3540 2023-05-02 18:46:37.000000 sphinx-embeddings-builder-0.0.5/README.md
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       38 2023-05-02 20:10:15.734751 sphinx-embeddings-builder-0.0.5/setup.cfg
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      330 2023-05-02 20:10:04.000000 sphinx-embeddings-builder-0.0.5/setup.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:10:15.734751 sphinx-embeddings-builder-0.0.5/sphinx-embeddings-builder/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)     1909 2023-05-02 20:09:58.000000 sphinx-embeddings-builder-0.0.5/sphinx-embeddings-builder/__init__.py
+drwxr-xr-x   0 kayce    (319046) primarygroup (89939)        0 2023-05-02 20:10:15.734751 sphinx-embeddings-builder-0.0.5/sphinx_embeddings_builder.egg-info/
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       69 2023-05-02 20:10:15.000000 sphinx-embeddings-builder-0.0.5/sphinx_embeddings_builder.egg-info/PKG-INFO
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)      300 2023-05-02 20:10:15.000000 sphinx-embeddings-builder-0.0.5/sphinx_embeddings_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)        1 2023-05-02 20:10:15.000000 sphinx-embeddings-builder-0.0.5/sphinx_embeddings_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)     1364 2023-05-02 20:10:15.000000 sphinx-embeddings-builder-0.0.5/sphinx_embeddings_builder.egg-info/requires.txt
+-rw-r--r--   0 kayce    (319046) primarygroup (89939)       26 2023-05-02 20:10:15.000000 sphinx-embeddings-builder-0.0.5/sphinx_embeddings_builder.egg-info/top_level.txt
```

### Comparing `sphinx-embeddings-builder-0.0.4/README.md` & `sphinx-embeddings-builder-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sphinx-embeddings-builder-0.0.4/sphinx-embeddings-builder/__init__.py` & `sphinx-embeddings-builder-0.0.5/sphinx-embeddings-builder/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from sphinx.builders import Builder
-from sphinx.locale import __
 from hashlib import md5
-from tiktoken import get_encoding
-from sphinx.util.osutil import ensuredir
 from os import path
 from json import dump
 from docutils.nodes import section as section_node
-import openai
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 
 class EmbeddingsBuilder(Builder):
     name = 'embeddings'
     format = 'json'
 
     def init(self):
         self.data = {}
@@ -46,15 +42,14 @@
 
     def finish(self):
         data_path = path.join(self.outdir, 'embeddings.json')
         with open(data_path, 'w') as f:
             dump(self.data, f, indent=2)
 
 def setup(app):
-    logging.stderr = True
     app.add_builder(EmbeddingsBuilder)
     app.add_config_value('sphinx_embeddings_builder_count_tokens', None, 'env')
     app.add_config_value('sphinx_embeddings_builder_max_tokens', None, 'env')
     app.add_config_value('sphinx_embeddings_builder_generate_embedding', None, 'env')
     return {
         'version': __version__,
         'parallel_read_safe': True,
```

### Comparing `sphinx-embeddings-builder-0.0.4/sphinx_embeddings_builder.egg-info/requires.txt` & `sphinx-embeddings-builder-0.0.5/sphinx_embeddings_builder.egg-info/requires.txt`

 * *Files identical despite different names*

