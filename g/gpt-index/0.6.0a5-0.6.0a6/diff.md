# Comparing `tmp/gpt_index-0.6.0a5.tar.gz` & `tmp/gpt_index-0.6.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_index-0.6.0a5.tar", last modified: Mon May  1 06:30:54 2023, max compression
+gzip compressed data, was "gpt_index-0.6.0a6.tar", last modified: Tue May  2 07:45:04 2023, max compression
```

## Comparing `gpt_index-0.6.0a5.tar` & `gpt_index-0.6.0a6.tar`

### file list

```diff
@@ -1,435 +1,444 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.323142 gpt_index-0.6.0a5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-01 06:30:54.323142 gpt_index-0.6.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.275142 gpt_index-0.6.0a5/gpt_index/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/async_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.279142 gpt_index-0.6.0a5/gpt_index/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/composability/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/composability/joint_qa_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.279142 gpt_index-0.6.0a5/gpt_index/data_structs/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/data_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/data_structs/data_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/data_structs/data_structs_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/data_structs/node_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/data_structs/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/data_structs/struct_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/data_structs/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/data_structs/table_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.279142 gpt_index-0.6.0a5/gpt_index/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/embeddings/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/embeddings/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/embeddings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.279142 gpt_index-0.6.0a5/gpt_index/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/evaluation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/evaluation/dataset_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/img_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.279142 gpt_index-0.6.0a5/gpt_index/indices/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/base_retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.279142 gpt_index-0.6.0a5/gpt_index/indices/common/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.279142 gpt_index-0.6.0a5/gpt_index/indices/common/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/common/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/common/struct_store/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.279142 gpt_index-0.6.0a5/gpt_index/indices/common_tree/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/common_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/common_tree/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.279142 gpt_index-0.6.0a5/gpt_index/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/composability/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.287142 gpt_index-0.6.0a5/gpt_index/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/empty/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/empty/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.287142 gpt_index-0.6.0a5/gpt_index/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/keyword_table/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.287142 gpt_index-0.6.0a5/gpt_index/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/knowledge_graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/knowledge_graph/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.291142 gpt_index-0.6.0a5/gpt_index/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/list/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/list/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.291142 gpt_index-0.6.0a5/gpt_index/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/postprocessor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/postprocessor/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/postprocessor/pii.py
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/prompt_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.291142 gpt_index-0.6.0a5/gpt_index/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/query/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.291142 gpt_index-0.6.0a5/gpt_index/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/query/query_transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/query/response_synthesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.295142 gpt_index-0.6.0a5/gpt_index/indices/response/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21967 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/response/response_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/response/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/service_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.295142 gpt_index-0.6.0a5/gpt_index/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/struct_store/container_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/struct_store/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/struct_store/pandas_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/struct_store/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.299142 gpt_index-0.6.0a5/gpt_index/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/tree/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/tree/inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.299142 gpt_index-0.6.0a5/gpt_index/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/vector_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/indices/vector_store/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.299142 gpt_index-0.6.0a5/gpt_index/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.299142 gpt_index-0.6.0a5/gpt_index/langchain_helpers/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/langchain_helpers/chain_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18168 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.299142 gpt_index-0.6.0a5/gpt_index/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/llm_predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/llm_predictor/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/llm_predictor/stable_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/llm_predictor/structured.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.299142 gpt_index-0.6.0a5/gpt_index/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/logger/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.299142 gpt_index-0.6.0a5/gpt_index/node_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/node_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/node_parser/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/node_parser/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/node_parser/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.299142 gpt_index-0.6.0a5/gpt_index/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/optimization/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.299142 gpt_index-0.6.0a5/gpt_index/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/output_parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/output_parsers/guardrails.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/output_parsers/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/output_parsers/selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.299142 gpt_index-0.6.0a5/gpt_index/playground/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/playground/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.303142 gpt_index-0.6.0a5/gpt_index/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/prompts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/prompts/chat_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/prompts/default_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/prompts/prompt_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.303142 gpt_index-0.6.0a5/gpt_index/query_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/query_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/query_engine/graph_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/query_engine/router_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.303142 gpt_index-0.6.0a5/gpt_index/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.303142 gpt_index-0.6.0a5/gpt_index/readers/chatgpt_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/discord_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/faiss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.307142 gpt_index-0.6.0a5/gpt_index/readers/file/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/file/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/file/docs_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/file/epub_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/file/image_caption_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/file/image_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/file/image_vision_llm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/file/ipynb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/file/markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/file/mbox_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/file/slides_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/file/tabular_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/file/video_audio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.307142 gpt_index-0.6.0a5/gpt_index/readers/github_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/github_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/github_readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.307142 gpt_index-0.6.0a5/gpt_index/readers/google_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/google_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/google_readers/gdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/google_readers/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.307142 gpt_index-0.6.0a5/gpt_index/readers/make_com/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/make_com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/make_com/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/mbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/obsidian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.307142 gpt_index-0.6.0a5/gpt_index/readers/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.307142 gpt_index-0.6.0a5/gpt_index/readers/steamship/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/steamship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/steamship/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/string_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/twitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.307142 gpt_index-0.6.0a5/gpt_index/readers/weaviate/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/weaviate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/weaviate/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/weaviate/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/web.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/readers/youtube_transcript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.307142 gpt_index-0.6.0a5/gpt_index/response/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/response/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/response/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/response/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.307142 gpt_index-0.6.0a5/gpt_index/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/retrievers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/retrievers/transform_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.311142 gpt_index-0.6.0a5/gpt_index/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/selectors/llm_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/selectors/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/selectors/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.311142 gpt_index-0.6.0a5/gpt_index/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.311142 gpt_index-0.6.0a5/gpt_index/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/docstore/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/docstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/docstore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.311142 gpt_index-0.6.0a5/gpt_index/storage/index_store/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/index_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/index_store/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/index_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.311142 gpt_index-0.6.0a5/gpt_index/storage/kvstore/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/kvstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/kvstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/storage/storage_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.311142 gpt_index-0.6.0a5/gpt_index/token_counter/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/token_counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/token_counter/mock_chain_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/token_counter/mock_embed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/token_counter/token_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/token_counter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.311142 gpt_index-0.6.0a5/gpt_index/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/tools/query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/tools/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.311142 gpt_index-0.6.0a5/gpt_index/tts/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/tts/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/tts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/tts/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.315142 gpt_index-0.6.0a5/gpt_index/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/vector_stores/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/vector_stores/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/vector_stores/faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/vector_stores/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/vector_stores/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/vector_stores/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/vector_stores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/vector_stores/qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/vector_stores/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/vector_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/vector_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/gpt_index/vector_stores/weaviate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.279142 gpt_index-0.6.0a5/gpt_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-01 06:30:54.000000 gpt_index-0.6.0a5/gpt_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-05-01 06:30:54.000000 gpt_index-0.6.0a5/gpt_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 06:30:54.000000 gpt_index-0.6.0a5/gpt_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 06:30:54.000000 gpt_index-0.6.0a5/gpt_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 06:30:54.000000 gpt_index-0.6.0a5/gpt_index.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 06:30:54.323142 gpt_index-0.6.0a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.315142 gpt_index-0.6.0a5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.315142 gpt_index-0.6.0a5/tests/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/embeddings/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.315142 gpt_index-0.6.0a5/tests/indices/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.315142 gpt_index-0.6.0a5/tests/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/composability/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.315142 gpt_index-0.6.0a5/tests/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/empty/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.315142 gpt_index-0.6.0a5/tests/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/keyword_table/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/keyword_table/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/keyword_table/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.315142 gpt_index-0.6.0a5/tests/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/knowledge_graph/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/knowledge_graph/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/knowledge_graph/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.315142 gpt_index-0.6.0a5/tests/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/list/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/list/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.319142 gpt_index-0.6.0a5/tests/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/postprocessor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.319142 gpt_index-0.6.0a5/tests/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.319142 gpt_index-0.6.0a5/tests/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/query/query_transform/mock_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/query/query_transform/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/query/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/query/test_compose_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/query/test_query_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.319142 gpt_index-0.6.0a5/tests/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/struct_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/struct_store/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/struct_store/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/struct_store/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/test_loading_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/test_node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/test_prompt_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.319142 gpt_index-0.6.0a5/tests/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/tree/test_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/tree/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/tree/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.319142 gpt_index-0.6.0a5/tests/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/vector_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/vector_store/mock_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/vector_store/mock_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/vector_store/test_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/vector_store/test_milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/vector_store/test_myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/vector_store/test_pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/vector_store/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/vector_store/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/vector_store/test_weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/indices/vector_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.319142 gpt_index-0.6.0a5/tests/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/langchain_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/langchain_helpers/test_text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.319142 gpt_index-0.6.0a5/tests/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/llm_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.319142 gpt_index-0.6.0a5/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/logger/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.323142 gpt_index-0.6.0a5/tests/mock_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/mock_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/mock_utils/mock_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/mock_utils/mock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/mock_utils/mock_text_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/mock_utils/mock_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.323142 gpt_index-0.6.0a5/tests/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/optimization/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.323142 gpt_index-0.6.0a5/tests/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/output_parsers/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/output_parsers/test_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.323142 gpt_index-0.6.0a5/tests/playground/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/playground/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.323142 gpt_index-0.6.0a5/tests/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/prompts/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.323142 gpt_index-0.6.0a5/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/readers/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/readers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/readers/test_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/readers/test_string_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.323142 gpt_index-0.6.0a5/tests/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/selectors/test_llm_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.323142 gpt_index-0.6.0a5/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/storage/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.323142 gpt_index-0.6.0a5/tests/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/storage/docstore/test_mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/storage/docstore/test_simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.323142 gpt_index-0.6.0a5/tests/token_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/token_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/token_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:54.323142 gpt_index-0.6.0a5/tests/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-01 06:30:39.000000 gpt_index-0.6.0a5/tests/vector_stores/test_qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.031935 gpt_index-0.6.0a6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-02 07:44:43.000000 gpt_index-0.6.0a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 07:44:43.000000 gpt_index-0.6.0a6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-02 07:45:04.031935 gpt_index-0.6.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-02 07:44:43.000000 gpt_index-0.6.0a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.995935 gpt_index-0.6.0a6/gpt_index/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.995935 gpt_index-0.6.0a6/gpt_index/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/callbacks/llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/callbacks/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.995935 gpt_index-0.6.0a6/gpt_index/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/composability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/composability/joint_qa_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.995935 gpt_index-0.6.0a6/gpt_index/data_structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/data_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/data_structs/data_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/data_structs/data_structs_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/data_structs/node_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/data_structs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/data_structs/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/data_structs/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/data_structs/table_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.995935 gpt_index-0.6.0a6/gpt_index/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/embeddings/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/embeddings/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/embeddings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.999935 gpt_index-0.6.0a6/gpt_index/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/evaluation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/evaluation/dataset_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/img_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.999935 gpt_index-0.6.0a6/gpt_index/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/base_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.999935 gpt_index-0.6.0a6/gpt_index/indices/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.999935 gpt_index-0.6.0a6/gpt_index/indices/common/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/common/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.999935 gpt_index-0.6.0a6/gpt_index/indices/common_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/common_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/common_tree/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.999935 gpt_index-0.6.0a6/gpt_index/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/composability/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.999935 gpt_index-0.6.0a6/gpt_index/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/empty/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/empty/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.999935 gpt_index-0.6.0a6/gpt_index/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/keyword_table/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.999935 gpt_index-0.6.0a6/gpt_index/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/knowledge_graph/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.003935 gpt_index-0.6.0a6/gpt_index/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/list/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.003935 gpt_index-0.6.0a6/gpt_index/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/postprocessor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/postprocessor/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/postprocessor/pii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/prompt_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.003935 gpt_index-0.6.0a6/gpt_index/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.003935 gpt_index-0.6.0a6/gpt_index/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/query/query_transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/query/response_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.003935 gpt_index-0.6.0a6/gpt_index/indices/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24744 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/response/response_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/response/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/service_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.003935 gpt_index-0.6.0a6/gpt_index/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/struct_store/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/struct_store/pandas_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/struct_store/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.003935 gpt_index-0.6.0a6/gpt_index/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/tree/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/tree/inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.003935 gpt_index-0.6.0a6/gpt_index/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/vector_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/indices/vector_store/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.007935 gpt_index-0.6.0a6/gpt_index/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.007935 gpt_index-0.6.0a6/gpt_index/langchain_helpers/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/langchain_helpers/chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18168 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.007935 gpt_index-0.6.0a6/gpt_index/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/llm_predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/llm_predictor/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/llm_predictor/stable_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/llm_predictor/structured.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.007935 gpt_index-0.6.0a6/gpt_index/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/logger/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.007935 gpt_index-0.6.0a6/gpt_index/node_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/node_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/node_parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/node_parser/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/node_parser/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.007935 gpt_index-0.6.0a6/gpt_index/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/optimization/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.007935 gpt_index-0.6.0a6/gpt_index/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/output_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/output_parsers/guardrails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/output_parsers/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/output_parsers/selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.007935 gpt_index-0.6.0a6/gpt_index/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/playground/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.011935 gpt_index-0.6.0a6/gpt_index/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/prompts/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/prompts/default_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/prompts/prompt_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.011935 gpt_index-0.6.0a6/gpt_index/query_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/query_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/query_engine/router_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.011935 gpt_index-0.6.0a6/gpt_index/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.011935 gpt_index-0.6.0a6/gpt_index/readers/chatgpt_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/discord_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/faiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.015935 gpt_index-0.6.0a6/gpt_index/readers/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/file/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/file/docs_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/file/epub_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/file/image_caption_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/file/image_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/file/image_vision_llm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/file/ipynb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/file/markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/file/mbox_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/file/slides_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/file/tabular_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/file/video_audio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.015935 gpt_index-0.6.0a6/gpt_index/readers/github_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/github_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15915 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/github_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.015935 gpt_index-0.6.0a6/gpt_index/readers/google_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/google_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.015935 gpt_index-0.6.0a6/gpt_index/readers/make_com/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/make_com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/make_com/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/mbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.015935 gpt_index-0.6.0a6/gpt_index/readers/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.015935 gpt_index-0.6.0a6/gpt_index/readers/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/steamship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/steamship/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/string_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/twitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.015935 gpt_index-0.6.0a6/gpt_index/readers/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/weaviate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/weaviate/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/weaviate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/readers/youtube_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.015935 gpt_index-0.6.0a6/gpt_index/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/response/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/response/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.015935 gpt_index-0.6.0a6/gpt_index/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/retrievers/transform_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.015935 gpt_index-0.6.0a6/gpt_index/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/selectors/llm_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/selectors/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/selectors/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.019935 gpt_index-0.6.0a6/gpt_index/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.019935 gpt_index-0.6.0a6/gpt_index/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/docstore/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/docstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/docstore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.019935 gpt_index-0.6.0a6/gpt_index/storage/index_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/index_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/index_store/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/index_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.019935 gpt_index-0.6.0a6/gpt_index/storage/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/kvstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/kvstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/storage/storage_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.019935 gpt_index-0.6.0a6/gpt_index/token_counter/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/token_counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/token_counter/mock_chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/token_counter/token_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/token_counter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.019935 gpt_index-0.6.0a6/gpt_index/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/tools/query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/tools/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.019935 gpt_index-0.6.0a6/gpt_index/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/tts/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/tts/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.023935 gpt_index-0.6.0a6/gpt_index/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/vector_stores/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/vector_stores/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/vector_stores/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/vector_stores/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/vector_stores/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/vector_stores/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/vector_stores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/vector_stores/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/vector_stores/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/vector_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/vector_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/gpt_index/vector_stores/weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:03.995935 gpt_index-0.6.0a6/gpt_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-02 07:45:03.000000 gpt_index-0.6.0a6/gpt_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-05-02 07:45:03.000000 gpt_index-0.6.0a6/gpt_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:45:03.000000 gpt_index-0.6.0a6/gpt_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 07:45:03.000000 gpt_index-0.6.0a6/gpt_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 07:45:03.000000 gpt_index-0.6.0a6/gpt_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 07:45:04.031935 gpt_index-0.6.0a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.023935 gpt_index-0.6.0a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.023935 gpt_index-0.6.0a6/tests/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/callbacks/test_llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.023935 gpt_index-0.6.0a6/tests/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/embeddings/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.023935 gpt_index-0.6.0a6/tests/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.023935 gpt_index-0.6.0a6/tests/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/composability/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.023935 gpt_index-0.6.0a6/tests/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/empty/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.023935 gpt_index-0.6.0a6/tests/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/keyword_table/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/keyword_table/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/keyword_table/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.023935 gpt_index-0.6.0a6/tests/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/knowledge_graph/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/knowledge_graph/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/knowledge_graph/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.023935 gpt_index-0.6.0a6/tests/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/list/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/list/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.023935 gpt_index-0.6.0a6/tests/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/postprocessor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.023935 gpt_index-0.6.0a6/tests/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.027935 gpt_index-0.6.0a6/tests/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/query/query_transform/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/query/query_transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/query/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/query/test_compose_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/query/test_query_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.027935 gpt_index-0.6.0a6/tests/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/struct_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/struct_store/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/struct_store/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/struct_store/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/test_loading_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/test_node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/test_prompt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.027935 gpt_index-0.6.0a6/tests/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/tree/test_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/tree/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/tree/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.027935 gpt_index-0.6.0a6/tests/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/vector_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/vector_store/mock_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/vector_store/mock_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/vector_store/test_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/vector_store/test_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/vector_store/test_myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/vector_store/test_pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/vector_store/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/vector_store/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/vector_store/test_weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/indices/vector_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.027935 gpt_index-0.6.0a6/tests/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/langchain_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/langchain_helpers/test_text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.027935 gpt_index-0.6.0a6/tests/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/llm_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.027935 gpt_index-0.6.0a6/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/logger/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.027935 gpt_index-0.6.0a6/tests/mock_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/mock_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/mock_utils/mock_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/mock_utils/mock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/mock_utils/mock_text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/mock_utils/mock_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.031935 gpt_index-0.6.0a6/tests/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/optimization/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.031935 gpt_index-0.6.0a6/tests/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/output_parsers/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/output_parsers/test_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.031935 gpt_index-0.6.0a6/tests/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/playground/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.031935 gpt_index-0.6.0a6/tests/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/prompts/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.031935 gpt_index-0.6.0a6/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/readers/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/readers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/readers/test_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/readers/test_string_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.031935 gpt_index-0.6.0a6/tests/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/selectors/test_llm_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.031935 gpt_index-0.6.0a6/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/storage/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.031935 gpt_index-0.6.0a6/tests/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/storage/docstore/test_mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/storage/docstore/test_simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.031935 gpt_index-0.6.0a6/tests/token_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/token_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/token_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:45:04.031935 gpt_index-0.6.0a6/tests/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/vector_stores/test_qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-02 07:44:44.000000 gpt_index-0.6.0a6/tests/vector_stores/test_weaviate.py
```

### Comparing `gpt_index-0.6.0a5/LICENSE` & `gpt_index-0.6.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/PKG-INFO` & `gpt_index-0.6.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_index
-Version: 0.6.0a5
+Version: 0.6.0a6
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/gpt_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `gpt_index-0.6.0a5/README.md` & `gpt_index-0.6.0a6/README.md`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/__init__.py` & `gpt_index-0.6.0a6/gpt_index/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/composability/joint_qa_summary.py` & `gpt_index-0.6.0a6/gpt_index/composability/joint_qa_summary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Joint QA Summary graph."""
 
 
 from typing import Sequence, Optional
 from gpt_index.storage.docstore.registry import get_default_docstore
 
+from gpt_index.callbacks.schema import CBEventType
 from gpt_index.indices.service_context import ServiceContext
 from gpt_index.composability import ComposableGraph
 from gpt_index.indices.list.base import GPTListIndex
 from gpt_index.indices.tree.base import GPTTreeIndex
 from gpt_index.indices.vector_store import GPTVectorStoreIndex
 from gpt_index.readers.schema.base import Document
 from gpt_index.storage.docstore import BaseDocumentStore
@@ -51,16 +52,21 @@
         self._qa_text = qa_text
 
     def build_graph_from_documents(
         self,
         documents: Sequence[Document],
     ) -> "ComposableGraph":
         """Build graph from index."""
-
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.CHUNKING, payload={"documents": documents}
+        )
         nodes = self._service_context.node_parser.get_nodes_from_documents(documents)
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.CHUNKING, payload={"nodes": nodes}, event_id=event_id
+        )
         self._docstore.add_documents(nodes, allow_update=True)
 
         # used for QA
         vector_index = GPTVectorStoreIndex(
             nodes,
             service_context=self._service_context,
         )
```

### Comparing `gpt_index-0.6.0a5/gpt_index/data_structs/data_structs.py` & `gpt_index-0.6.0a6/gpt_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/data_structs/data_structs_v2.py` & `gpt_index-0.6.0a6/gpt_index/data_structs/data_structs_v2.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/data_structs/node_v2.py` & `gpt_index-0.6.0a6/gpt_index/data_structs/node_v2.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/data_structs/registry.py` & `gpt_index-0.6.0a6/gpt_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/data_structs/struct_type.py` & `gpt_index-0.6.0a6/gpt_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/data_structs/table.py` & `gpt_index-0.6.0a6/gpt_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/data_structs/table_v2.py` & `gpt_index-0.6.0a6/gpt_index/data_structs/table_v2.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/embeddings/base.py` & `gpt_index-0.6.0a6/gpt_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/embeddings/langchain.py` & `gpt_index-0.6.0a6/gpt_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/embeddings/openai.py` & `gpt_index-0.6.0a6/gpt_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/embeddings/utils.py` & `gpt_index-0.6.0a6/gpt_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/evaluation/base.py` & `gpt_index-0.6.0a6/gpt_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/evaluation/dataset_generation.py` & `gpt_index-0.6.0a6/gpt_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/img_utils.py` & `gpt_index-0.6.0a6/gpt_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/__init__.py` & `gpt_index-0.6.0a6/gpt_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/base.py` & `gpt_index-0.6.0a6/gpt_index/indices/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Base index classes."""
 import logging
 from abc import ABC, abstractmethod
 from typing import Any, Generic, List, Optional, Sequence, Type, TypeVar
 
+from gpt_index.callbacks.schema import CBEventType
 from gpt_index.data_structs.data_structs_v2 import V2IndexStruct
 from gpt_index.data_structs.node_v2 import Node
 from gpt_index.indices.base_retriever import BaseRetriever
 from gpt_index.indices.query.base import BaseQueryEngine
 from gpt_index.indices.service_context import ServiceContext
 from gpt_index.readers.schema.base import Document
 from gpt_index.storage.docstore.types import BaseDocumentStore
@@ -84,15 +85,21 @@
         storage_context = storage_context or StorageContext.from_defaults()
         service_context = service_context or ServiceContext.from_defaults()
         docstore = storage_context.docstore
 
         for doc in documents:
             docstore.set_document_hash(doc.get_doc_id(), doc.get_doc_hash())
 
+        event_id = service_context.callback_manager.on_event_start(
+            CBEventType.CHUNKING, payload={"documents": documents}
+        )
         nodes = service_context.node_parser.get_nodes_from_documents(documents)
+        service_context.callback_manager.on_event_end(
+            CBEventType.CHUNKING, payload={"nodes": nodes}, event_id=event_id
+        )
 
         return cls(
             nodes=nodes,
             storage_context=storage_context,
             service_context=service_context,
             **kwargs,
         )
@@ -161,15 +168,21 @@
         """Insert nodes."""
         self.docstore.add_documents(nodes, allow_update=True)
         self._insert(nodes, **insert_kwargs)
         self._storage_context.index_store.add_index_struct(self._index_struct)
 
     def insert(self, document: Document, **insert_kwargs: Any) -> None:
         """Insert a document."""
+        event_id = self.service_context.callback_manager.on_event_start(
+            CBEventType.CHUNKING, payload={"documents": [document]}
+        )
         nodes = self.service_context.node_parser.get_nodes_from_documents([document])
+        self.service_context.callback_manager.on_event_end(
+            CBEventType.CHUNKING, payload={"nodes": nodes}, event_id=event_id
+        )
         self.insert_nodes(nodes, **insert_kwargs)
         self.docstore.set_document_hash(document.get_doc_id(), document.get_doc_hash())
 
     @abstractmethod
     def _delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete a document."""
```

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/base_retriever.py` & `gpt_index-0.6.0a6/gpt_index/indices/base_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/common/struct_store/base.py` & `gpt_index-0.6.0a6/gpt_index/indices/common/struct_store/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Common classes for structured operations."""
 
 import logging
 from abc import abstractmethod
 from typing import Any, Callable, Dict, List, Optional, Sequence, cast
 
+from gpt_index.callbacks.schema import CBEventType
 from gpt_index.data_structs.node_v2 import Node
 from gpt_index.data_structs.table import StructDatapoint
 from gpt_index.indices.response.response_builder import get_response_builder
 from gpt_index.indices.service_context import ServiceContext
 from gpt_index.langchain_helpers.chain_wrapper import LLMPredictor
 from gpt_index.langchain_helpers.sql_wrapper import SQLDatabase
 from gpt_index.langchain_helpers.text_splitter import TextSplitter
@@ -105,18 +106,24 @@
         )
         # we use the ResponseBuilder to iteratively go through all texts
         response_builder = get_response_builder(
             self._service_context,
             prompt_with_schema,
             refine_prompt_with_schema,
         )
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.CHUNKING, payload={"documents": documents}
+        )
         text_chunks = []
         for doc in documents:
             chunks = text_splitter.split_text(doc.get_text())
             text_chunks.extend(chunks)
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.CHUNKING, payload={"chunks": text_chunks}, event_id=event_id
+        )
 
         # feed in the "query_str" or the task
         table_context = response_builder.get_response(
             text_chunks=text_chunks, query_str=self._table_context_task
         )
         return cast(str, table_context)
```

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/common/struct_store/schema.py` & `gpt_index-0.6.0a6/gpt_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/common/struct_store/sql.py` & `gpt_index-0.6.0a6/gpt_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/common_tree/base.py` & `gpt_index-0.6.0a6/gpt_index/indices/common_tree/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 import asyncio
 import logging
 from typing import Dict, List, Optional, Sequence, Tuple
 
 from gpt_index.async_utils import run_async_tasks
+from gpt_index.callbacks.schema import CBEventType
 from gpt_index.data_structs.data_structs_v2 import IndexGraph
 from gpt_index.data_structs.node_v2 import Node
 from gpt_index.storage.docstore import BaseDocumentStore
 from gpt_index.storage.docstore.registry import get_default_docstore
 from gpt_index.indices.service_context import ServiceContext
 from gpt_index.indices.utils import get_sorted_node_list, truncate_text
 from gpt_index.prompts.prompts import SummaryPrompt
@@ -132,14 +133,17 @@
         if len(cur_node_ids) <= self.num_children:
             index_graph.root_nodes = cur_node_ids
             return index_graph
 
         indices, cur_nodes_chunks, text_chunks = self._prepare_node_and_text_chunks(
             cur_node_ids
         )
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.TREE, payload={"chunks": text_chunks}
+        )
 
         if self._use_async:
             tasks = [
                 self._service_context.llm_predictor.apredict(
                     self.summary_prompt, context_str=text_chunk
                 )
                 for text_chunk in text_chunks
@@ -152,14 +156,19 @@
                     self.summary_prompt, context_str=text_chunk
                 )[0]
                 for text_chunk in text_chunks
             ]
         self._service_context.llama_logger.add_log(
             {"summaries": summaries, "level": level}
         )
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.TREE,
+            payload={"summaries": summaries, "level": level},
+            event_id=event_id,
+        )
 
         new_node_dict = self._construct_parent_nodes(
             index_graph, indices, cur_nodes_chunks, summaries
         )
         all_node_ids.update(new_node_dict)
 
         index_graph.root_nodes = new_node_dict
@@ -182,26 +191,34 @@
         if len(cur_node_ids) <= self.num_children:
             index_graph.root_nodes = cur_node_ids
             return index_graph
 
         indices, cur_nodes_chunks, text_chunks = self._prepare_node_and_text_chunks(
             cur_node_ids
         )
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.TREE, payload={"chunks": text_chunks}
+        )
 
         tasks = [
             self._service_context.llm_predictor.apredict(
                 self.summary_prompt, context_str=text_chunk
             )
             for text_chunk in text_chunks
         ]
         outputs: List[Tuple[str, str]] = await asyncio.gather(*tasks)
         summaries = [output[0] for output in outputs]
         self._service_context.llama_logger.add_log(
             {"summaries": summaries, "level": level}
         )
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.TREE,
+            payload={"summaries": summaries, "level": level},
+            event_id=event_id,
+        )
 
         new_node_dict = self._construct_parent_nodes(
             index_graph, indices, cur_nodes_chunks, summaries
         )
         all_node_ids.update(new_node_dict)
 
         index_graph.root_nodes = new_node_dict
```

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/composability/graph.py` & `gpt_index-0.6.0a6/gpt_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/empty/base.py` & `gpt_index-0.6.0a6/gpt_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/empty/retrievers.py` & `gpt_index-0.6.0a6/gpt_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/keyword_table/__init__.py` & `gpt_index-0.6.0a6/gpt_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/keyword_table/base.py` & `gpt_index-0.6.0a6/gpt_index/indices/keyword_table/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 from abc import abstractmethod
 from enum import Enum
 from typing import Any, Optional, Sequence, Set, Union
 
 from gpt_index.async_utils import run_async_tasks
+from gpt_index.callbacks.schema import CBEventType
 from gpt_index.data_structs.data_structs_v2 import KeywordTable
 from gpt_index.data_structs.node_v2 import Node
 from gpt_index.indices.base import BaseGPTIndex
 from gpt_index.indices.base_retriever import BaseRetriever
 from gpt_index.indices.keyword_table.utils import extract_keywords_given_response
 from gpt_index.indices.service_context import ServiceContext
 from gpt_index.prompts.default_prompts import (
@@ -182,22 +183,40 @@
 
     This index uses a GPT model to extract keywords from the text.
 
     """
 
     def _extract_keywords(self, text: str) -> Set[str]:
         """Extract keywords from text."""
-        response, _ = self._service_context.llm_predictor.predict(
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.LLM,
+            payload={"template": self.keyword_extract_template, "text": text},
+        )
+        response, formatted_prompt = self._service_context.llm_predictor.predict(
             self.keyword_extract_template,
             text=text,
         )
         keywords = extract_keywords_given_response(response, start_token="KEYWORDS:")
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.LLM,
+            payload={"keywords": keywords, "formatted_prompt": formatted_prompt},
+            event_id=event_id,
+        )
         return keywords
 
     async def _async_extract_keywords(self, text: str) -> Set[str]:
         """Extract keywords from text."""
-        response, _ = await self._service_context.llm_predictor.apredict(
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.LLM,
+            payload={"template": self.keyword_extract_template, "text": text},
+        )
+        response, formatted_prompt = await self._service_context.llm_predictor.apredict(
             self.keyword_extract_template,
             text=text,
         )
         keywords = extract_keywords_given_response(response, start_token="KEYWORDS:")
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.LLM,
+            payload={"keywords": keywords, "formatted_prompt": formatted_prompt},
+            event_id=event_id,
+        )
         return keywords
```

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/keyword_table/rake_base.py` & `gpt_index-0.6.0a6/gpt_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/keyword_table/retrievers.py` & `gpt_index-0.6.0a6/gpt_index/indices/keyword_table/retrievers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Query for GPTKeywordTableIndex."""
 import logging
 from abc import abstractmethod
 from collections import defaultdict
 from typing import Any, Dict, List, Optional
 
+from gpt_index.callbacks.schema import CBEventType
 from gpt_index.data_structs.node_v2 import NodeWithScore
 from gpt_index.indices.base_retriever import BaseRetriever
 from gpt_index.indices.keyword_table.base import (
     BaseGPTKeywordTableIndex,
 )
 from gpt_index.indices.keyword_table.utils import (
     extract_keywords_given_response,
@@ -116,20 +117,33 @@
 
     See BaseGPTKeywordTableQuery for arguments.
 
     """
 
     def _get_keywords(self, query_str: str) -> List[str]:
         """Extract keywords."""
-        response, _ = self._service_context.llm_predictor.predict(
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.LLM,
+            payload={
+                "template": self.query_keyword_extract_template,
+                "question": query_str,
+                "max_keywords": self.max_keywords_per_query,
+            },
+        )
+        response, formatted_prompt = self._service_context.llm_predictor.predict(
             self.query_keyword_extract_template,
             max_keywords=self.max_keywords_per_query,
             question=query_str,
         )
         keywords = extract_keywords_given_response(response, start_token="KEYWORDS:")
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.LLM,
+            payload={"keywords": keywords, "formatted_prompt": formatted_prompt},
+            event_id=event_id,
+        )
         return list(keywords)
 
 
 class KeywordTableSimpleRetriever(BaseKeywordTableRetriever):
     """Keyword Table Index Simple Retriever.
 
     Extracts keywords using simple regex-based keyword extractor.
```

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/keyword_table/simple_base.py` & `gpt_index-0.6.0a6/gpt_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/keyword_table/utils.py` & `gpt_index-0.6.0a6/gpt_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/knowledge_graph/base.py` & `gpt_index-0.6.0a6/gpt_index/indices/knowledge_graph/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 existing keywords in the table.
 
 """
 
 import logging
 from typing import Any, List, Optional, Sequence, Tuple
 
+from gpt_index.callbacks.schema import CBEventType
 from gpt_index.data_structs.data_structs_v2 import KG
 from gpt_index.data_structs.node_v2 import Node
 from gpt_index.indices.base import BaseGPTIndex
 from gpt_index.indices.base_retriever import BaseRetriever
 from gpt_index.prompts.default_prompts import (
     DEFAULT_KG_TRIPLET_EXTRACT_PROMPT,
     DEFAULT_QUERY_KEYWORD_EXTRACT_TEMPLATE,
@@ -78,18 +79,27 @@
         if len(self.index_struct.embedding_dict) > 0 and "retriever_mode" not in kwargs:
             kwargs["retriever_mode"] = KGRetrieverMode.HYBRID
 
         return KGTableRetriever(self, **kwargs)
 
     def _extract_triplets(self, text: str) -> List[Tuple[str, str, str]]:
         """Extract keywords from text."""
-        response, _ = self._service_context.llm_predictor.predict(
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.LLM,
+            payload={"template": self.kg_triple_extract_template, "text": text},
+        )
+        response, formatted_prompt = self._service_context.llm_predictor.predict(
             self.kg_triple_extract_template,
             text=text,
         )
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.LLM,
+            payload={"response": response, "formatted_prompt": formatted_prompt},
+            event_id=event_id,
+        )
         return self._parse_triplet_response(response)
 
     @staticmethod
     def _parse_triplet_response(response: str) -> List[Tuple[str, str, str]]:
         knowledge_strs = response.strip().split("\n")
         results = []
         for text in knowledge_strs:
@@ -109,22 +119,30 @@
             logger.debug(f"> Extracted triplets: {triplets}")
             for triplet in triplets:
                 subj, _, obj = triplet
                 index_struct.upsert_triplet(triplet)
                 index_struct.add_node([subj, obj], n)
 
             if self.include_embeddings:
+                event_id = self._service_context.callback_manager.on_event_start(
+                    CBEventType.EMBEDDING
+                )
                 for i, triplet in enumerate(triplets):
                     self._service_context.embed_model.queue_text_for_embedding(
                         str(triplet), str(triplet)
                     )
 
                 embed_outputs = (
                     self._service_context.embed_model.get_queued_text_embeddings()
                 )
+                self._service_context.callback_manager.on_event_end(
+                    CBEventType.EMBEDDING,
+                    payload={"num_nodes": len(triplets)},
+                    event_id=event_id,
+                )
                 for rel_text, rel_embed in zip(*embed_outputs):
                     index_struct.add_to_embedding_dict(rel_text, rel_embed)
 
         return index_struct
 
     def _insert(self, nodes: Sequence[Node], **insert_kwargs: Any) -> None:
         """Insert a document."""
@@ -136,19 +154,27 @@
                 triplet_str = str(triplet)
                 self._index_struct.upsert_triplet(triplet)
                 self._index_struct.add_node([subj, obj], n)
                 if (
                     self.include_embeddings
                     and triplet_str not in self._index_struct.embedding_dict
                 ):
+                    event_id = self._service_context.callback_manager.on_event_start(
+                        CBEventType.EMBEDDING
+                    )
                     rel_embedding = (
                         self._service_context.embed_model.get_text_embedding(
                             triplet_str
                         )
                     )
+                    self._service_context.callback_manager.on_event_end(
+                        CBEventType.EMBEDDING,
+                        payload={"num_nodes": 1},
+                        event_id=event_id,
+                    )
                     self.index_struct.add_to_embedding_dict(triplet_str, rel_embedding)
 
     def upsert_triplet(self, triplet: Tuple[str, str, str]) -> None:
         """Insert triplets.
 
         Used for manual insertion of KG triplets (in the form
         of (subject, relationship, object)).
```

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/knowledge_graph/retrievers.py` & `gpt_index-0.6.0a6/gpt_index/indices/knowledge_graph/retrievers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Query for GPTKGTableIndex."""
 import logging
 from collections import defaultdict
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
+from gpt_index.callbacks.schema import CBEventType
 from gpt_index.data_structs.node_v2 import Node, NodeWithScore
 from gpt_index.indices.base_retriever import BaseRetriever
 from gpt_index.indices.keyword_table.utils import extract_keywords_given_response
 from gpt_index.indices.knowledge_graph.base import GPTKnowledgeGraphIndex
 from gpt_index.indices.query.embedding_utils import (
     get_top_k_embeddings,
 )
@@ -89,22 +90,35 @@
         self.query_keyword_extract_template = query_keyword_extract_template or DQKET
         self.similarity_top_k = similarity_top_k
         self._include_text = include_text
         self._retriever_mode = KGRetrieverMode(retriever_mode)
 
     def _get_keywords(self, query_str: str) -> List[str]:
         """Extract keywords."""
-        response, _ = self._service_context.llm_predictor.predict(
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.LLM,
+            payload={
+                "template": self.query_keyword_extract_template,
+                "question": query_str,
+                "max_keywords": self.max_keywords_per_query,
+            },
+        )
+        response, formatted_prompt = self._service_context.llm_predictor.predict(
             self.query_keyword_extract_template,
             max_keywords=self.max_keywords_per_query,
             question=query_str,
         )
         keywords = extract_keywords_given_response(
             response, start_token="KEYWORDS:", lowercase=False
         )
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.LLM,
+            payload={"keywords": keywords, "formatted_prompt": formatted_prompt},
+            event_id=event_id,
+        )
         return list(keywords)
 
     def _extract_rel_text_keywords(self, rel_texts: List[str]) -> List[str]:
         """Find the keywords for given rel text triplets."""
         keywords = []
         for rel_text in rel_texts:
             keyword = rel_text.split(",")[0]
@@ -133,17 +147,23 @@
                     for node_id in self._index_struct.get_node_ids(keyword):
                         chunk_indices_count[node_id] += 1
 
         if (
             self._retriever_mode != KGRetrieverMode.KEYWORD
             and len(self._index_struct.embedding_dict) > 0
         ):
+            event_id = self._service_context.callback_manager.on_event_start(
+                CBEventType.EMBEDDING
+            )
             query_embedding = self._service_context.embed_model.get_text_embedding(
                 query_bundle.query_str
             )
+            self._service_context.callback_manager.on_event_end(
+                CBEventType.EMBEDDING, payload={"num_nodes": 1}, event_id=event_id
+            )
             all_rel_texts = list(self._index_struct.embedding_dict.keys())
 
             rel_text_embeddings = [
                 self._index_struct.embedding_dict[_id] for _id in all_rel_texts
             ]
             similarities, top_rel_texts = get_top_k_embeddings(
                 query_embedding,
```

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/list/base.py` & `gpt_index-0.6.0a6/gpt_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/list/retrievers.py` & `gpt_index-0.6.0a6/gpt_index/indices/list/retrievers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Default query for GPTListIndex."""
 import logging
 from typing import Any, List, Optional, Tuple
 
+from gpt_index.callbacks.schema import CBEventType
 from gpt_index.data_structs.node_v2 import Node, NodeWithScore
 from gpt_index.indices.base_retriever import BaseRetriever
 from gpt_index.indices.query.embedding_utils import (
     get_top_k_embeddings,
 )
 from gpt_index.indices.query.schema import QueryBundle
 from gpt_index.indices.list.base import GPTListIndex
@@ -86,23 +87,40 @@
         return node_with_scores
 
     def _get_embeddings(
         self, query_bundle: QueryBundle, nodes: List[Node]
     ) -> Tuple[List[float], List[List[float]]]:
         """Get top nodes by similarity to the query."""
         if query_bundle.embedding is None:
+            event_id = self._index._service_context.callback_manager.on_event_start(
+                CBEventType.EMBEDDING
+            )
             query_bundle.embedding = (
                 self._index._service_context.embed_model.get_agg_embedding_from_queries(
                     query_bundle.embedding_strs
                 )
             )
+            self._index._service_context.callback_manager.on_event_end(
+                CBEventType.EMBEDDING, payload={"num_nodes": 1}, event_id=event_id
+            )
         node_embeddings: List[List[float]] = []
+
+        event_id = self._index._service_context.callback_manager.on_event_start(
+            CBEventType.EMBEDDING
+        )
+        nodes_embedded = 0
         for node in nodes:
             if node.embedding is None:
+                nodes_embedded += 1
                 node.embedding = (
                     self._index.service_context.embed_model.get_text_embedding(
                         node.get_text()
                     )
                 )
 
             node_embeddings.append(node.embedding)
+        self._index._service_context.callback_manager.on_event_end(
+            CBEventType.EMBEDDING,
+            payload={"num_nodes": nodes_embedded},
+            event_id=event_id,
+        )
         return query_bundle.embedding, node_embeddings
```

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/loading.py` & `gpt_index-0.6.0a6/gpt_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/postprocessor/__init__.py` & `gpt_index-0.6.0a6/gpt_index/indices/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/postprocessor/node.py` & `gpt_index-0.6.0a6/gpt_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/postprocessor/node_recency.py` & `gpt_index-0.6.0a6/gpt_index/indices/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/postprocessor/pii.py` & `gpt_index-0.6.0a6/gpt_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/prompt_helper.py` & `gpt_index-0.6.0a6/gpt_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/query/base.py` & `gpt_index-0.6.0a6/gpt_index/indices/query/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/query/embedding_utils.py` & `gpt_index-0.6.0a6/gpt_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/query/query_transform/base.py` & `gpt_index-0.6.0a6/gpt_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/query/query_transform/prompts.py` & `gpt_index-0.6.0a6/gpt_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/query/response_synthesis.py` & `gpt_index-0.6.0a6/gpt_index/indices/query/response_synthesis.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/query/schema.py` & `gpt_index-0.6.0a6/gpt_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/registry.py` & `gpt_index-0.6.0a6/gpt_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/response/response_builder.py` & `gpt_index-0.6.0a6/gpt_index/indices/response/response_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 2) create and refine separately over each chunk, 3) tree summarization.
 
 """
 from abc import ABC, abstractmethod
 import logging
 from typing import Any, Dict, Generator, List, Optional, Sequence, Tuple, cast
 
+from gpt_index.callbacks.schema import CBEventType
 from gpt_index.data_structs.data_structs_v2 import IndexGraph
 from gpt_index.data_structs.node_v2 import Node
 from gpt_index.storage.docstore.registry import get_default_docstore
 from gpt_index.indices.common_tree.base import GPTTreeIndexBuilder
 from gpt_index.indices.response.type import ResponseMode
 from gpt_index.indices.service_context import ServiceContext
 from gpt_index.indices.utils import get_sorted_node_list, truncate_text
@@ -65,14 +66,51 @@
             {"formatted_prompt_template": formatted_prompt}
         )
         logger.debug(f"> {log_prefix} response: {response}")
         self._service_context.llama_logger.add_log(
             {f"{log_prefix.lower()}_response": response or "Empty Response"}
         )
 
+    def _callback_llm_on_start(self) -> str:
+        """Call the callback manager on_start and return event id."""
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.LLM
+        )
+        return event_id
+
+    def _callback_llm_on_end(
+        self,
+        formatted_prompt: str,
+        response: RESPONSE_TEXT_TYPE,
+        event_id: str,
+        stage: Optional[str] = "",
+    ) -> None:
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.LLM,
+            payload={
+                "stage": stage,
+                "response": response,
+                "formatted_prompt": formatted_prompt,
+            },
+            event_id=event_id,
+        )
+
+    def _callback_chunking_on_start(self, text: str) -> str:
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.CHUNKING, payload={"node": text}
+        )
+        return event_id
+
+    def _callback_chunking_on_end(
+        self, text_chunks: Sequence[str], event_id: str
+    ) -> None:
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.CHUNKING, payload={"chunks": text_chunks}, event_id=event_id
+        )
+
     @abstractmethod
     @llm_token_counter("get_response")
     def get_response(
         self,
         query_str: str,
         text_chunks: Sequence[str],
         prev_response: Optional[str] = None,
@@ -155,37 +193,48 @@
         """Give response given a query and a corresponding text chunk."""
         text_qa_template = self.text_qa_template.partial_format(query_str=query_str)
         qa_text_splitter = (
             self._service_context.prompt_helper.get_text_splitter_given_prompt(
                 text_qa_template, 1
             )
         )
+        event_id = self._callback_chunking_on_start(text_chunk)
         text_chunks = qa_text_splitter.split_text(text_chunk)
+        self._callback_chunking_on_end(text_chunk, event_id)
+
         response: Optional[RESPONSE_TEXT_TYPE] = None
         # TODO: consolidate with loop in get_response_default
         for cur_text_chunk in text_chunks:
             if response is None and not self._streaming:
+                event_id = self._callback_llm_on_start()
                 (
                     response,
                     formatted_prompt,
                 ) = self._service_context.llm_predictor.predict(
                     text_qa_template,
                     context_str=cur_text_chunk,
                 )
                 self._log_prompt_and_response(
                     formatted_prompt, response, log_prefix="Initial"
                 )
+                self._callback_llm_on_end(
+                    formatted_prompt, response, event_id, stage="Initial"
+                )
             elif response is None and self._streaming:
+                event_id = self._callback_llm_on_start()
                 response, formatted_prompt = self._service_context.llm_predictor.stream(
                     text_qa_template,
                     context_str=cur_text_chunk,
                 )
                 self._log_prompt_and_response(
                     formatted_prompt, response, log_prefix="Initial"
                 )
+                self._callback_llm_on_end(
+                    formatted_prompt, response, event_id, stage="Initial"
+                )
             else:
                 response = self._refine_response_single(
                     cast(RESPONSE_TEXT_TYPE, response),
                     query_str,
                     cur_text_chunk,
                 )
         if isinstance(response, str):
@@ -213,16 +262,21 @@
             query_str=query_str, existing_answer=response
         )
         refine_text_splitter = (
             self._service_context.prompt_helper.get_text_splitter_given_prompt(
                 refine_template, 1
             )
         )
+
+        event_id = self._callback_chunking_on_start(text_chunk)
         text_chunks = refine_text_splitter.split_text(text_chunk)
+        self._callback_chunking_on_end(text_chunks, event_id)
+
         for cur_text_chunk in text_chunks:
+            event_id = self._callback_llm_on_start()
             if not self._streaming:
                 (
                     response,
                     formatted_prompt,
                 ) = self._service_context.llm_predictor.predict(
                     refine_template,
                     context_msg=cur_text_chunk,
@@ -235,14 +289,17 @@
             refine_template = self._refine_template.partial_format(
                 query_str=query_str, existing_answer=response
             )
 
             self._log_prompt_and_response(
                 formatted_prompt, response, log_prefix="Refined"
             )
+            self._callback_llm_on_end(
+                formatted_prompt, response, event_id, stage="Refined"
+            )
         return response
 
 
 class CompactAndRefine(Refine):
     def __init__(
         self,
         service_context: ServiceContext,
@@ -387,15 +444,18 @@
 
         # then get text splitter
         text_splitter = (
             self._service_context.prompt_helper.get_text_splitter_given_prompt(
                 summary_template, num_children
             )
         )
+        event_id = self._callback_chunking_on_start(all_text)
         text_chunks = text_splitter.split_text(all_text)
+        self._callback_chunking_on_end(text_chunks, event_id)
+
         new_nodes = [Node(text=t) for t in text_chunks]
 
         docstore = get_default_docstore()
         docstore.add_documents(new_nodes, allow_update=False)
         index_builder = GPTTreeIndexBuilder(
             num_children,
             summary_template,
@@ -448,29 +508,33 @@
     ) -> RESPONSE_TEXT_TYPE:
         text_qa_template = self._text_qa_template.partial_format(query_str=query_str)
         node_text = self._service_context.prompt_helper.get_text_from_nodes(
             [Node(text=text) for text in text_chunks], prompt=text_qa_template
         )
 
         response: RESPONSE_TEXT_TYPE
+        event_id = self._callback_llm_on_start()
         if not self._streaming:
             (
                 response,
                 formatted_prompt,
             ) = await self._service_context.llm_predictor.apredict(
                 text_qa_template,
                 context_str=node_text,
             )
-            self._log_prompt_and_response(formatted_prompt, response)
         else:
+            event_id = self._callback_llm_on_start()
             response, formatted_prompt = self._service_context.llm_predictor.stream(
                 text_qa_template,
                 context_str=node_text,
             )
-            self._log_prompt_and_response(formatted_prompt, response)
+        self._log_prompt_and_response(formatted_prompt, response)
+        self._callback_llm_on_end(
+            formatted_prompt, response, event_id, stage="summarize"
+        )
         if isinstance(response, str):
             response = response or "Empty Response"
         else:
             response = cast(Generator, response)
 
         return response
 
@@ -484,26 +548,29 @@
     ) -> RESPONSE_TEXT_TYPE:
         text_qa_template = self._text_qa_template.partial_format(query_str=query_str)
         node_text = self._service_context.prompt_helper.get_text_from_nodes(
             [Node(text=text) for text in text_chunks], prompt=text_qa_template
         )
 
         response: RESPONSE_TEXT_TYPE
+        event_id = self._callback_llm_on_start()
         if not self._streaming:
             (response, formatted_prompt,) = self._service_context.llm_predictor.predict(
                 text_qa_template,
                 context_str=node_text,
             )
-            self._log_prompt_and_response(formatted_prompt, response)
         else:
             response, formatted_prompt = self._service_context.llm_predictor.stream(
                 text_qa_template,
                 context_str=node_text,
             )
-            self._log_prompt_and_response(formatted_prompt, response)
+        self._log_prompt_and_response(formatted_prompt, response)
+        self._callback_llm_on_end(
+            formatted_prompt, response, event_id, stage="summarize"
+        )
         if isinstance(response, str):
             response = response or "Empty Response"
         else:
             response = cast(Generator, response)
 
         return response
 
@@ -527,18 +594,23 @@
         **response_kwargs: Any,
     ) -> RESPONSE_TEXT_TYPE:
         # NOTE: ignore text chunks and previous response
         del text_chunks
         del prev_response
 
         if not self._streaming:
-            response, _ = await self._service_context.llm_predictor.apredict(
+            event_id = self._callback_llm_on_start()
+            (
+                response,
+                formatted_prompt,
+            ) = await self._service_context.llm_predictor.apredict(
                 self._input_prompt,
                 query_str=query_str,
             )
+            self._callback_llm_on_end(formatted_prompt, response, event_id)
             return response
         else:
             stream_response, _ = self._service_context.llm_predictor.stream(
                 self._input_prompt,
                 query_str=query_str,
             )
             return stream_response
@@ -552,18 +624,20 @@
         **response_kwargs: Any,
     ) -> RESPONSE_TEXT_TYPE:
         # NOTE: ignore text chunks and previous response
         del text_chunks
         del prev_response
 
         if not self._streaming:
-            response, _ = self._service_context.llm_predictor.predict(
+            event_id = self._callback_llm_on_start()
+            response, formatted_prompt = self._service_context.llm_predictor.predict(
                 self._input_prompt,
                 query_str=query_str,
             )
+            self._callback_llm_on_end(formatted_prompt, response, event_id)
             return response
         else:
             stream_response, _ = self._service_context.llm_predictor.stream(
                 self._input_prompt,
                 query_str=query_str,
             )
             return stream_response
```

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/service_context.py` & `gpt_index-0.6.0a6/gpt_index/indices/service_context.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from typing import Optional
 
+from gpt_index.callbacks.base import CallbackManager
 from gpt_index.embeddings.base import BaseEmbedding
 from gpt_index.embeddings.openai import OpenAIEmbedding
 from gpt_index.indices.prompt_helper import PromptHelper
 from gpt_index.langchain_helpers.chain_wrapper import LLMPredictor
 from gpt_index.langchain_helpers.text_splitter import TokenTextSplitter
 from gpt_index.logger import LlamaLogger
 from gpt_index.node_parser.interface import NodeParser
@@ -26,49 +27,53 @@
 
     The service context container is a utility container for LlamaIndex
     index and query classes. It contains the following:
     - llm_predictor: LLMPredictor
     - prompt_helper: PromptHelper
     - embed_model: BaseEmbedding
     - node_parser: NodeParser
-    - llama_logger: LlamaLogger
+    - llama_logger: LlamaLogger (deprecated)
+    - callback_manager: CallbackManager
     - chunk_size_limit: chunk size limit
 
     """
 
     llm_predictor: LLMPredictor
     prompt_helper: PromptHelper
     embed_model: BaseEmbedding
     node_parser: NodeParser
     llama_logger: LlamaLogger
+    callback_manager: CallbackManager
     chunk_size_limit: Optional[int] = None
 
     @classmethod
     def from_defaults(
         cls,
         llm_predictor: Optional[LLMPredictor] = None,
         prompt_helper: Optional[PromptHelper] = None,
         embed_model: Optional[BaseEmbedding] = None,
         node_parser: Optional[NodeParser] = None,
         llama_logger: Optional[LlamaLogger] = None,
+        callback_manager: Optional[CallbackManager] = None,
         chunk_size_limit: Optional[int] = None,
     ) -> "ServiceContext":
         """Create a ServiceContext from defaults.
         If an argument is specified, then use the argument value provided for that
         parameter. If an argument is not specified, then use the default value.
 
         Args:
             llm_predictor (Optional[LLMPredictor]): LLMPredictor
             prompt_helper (Optional[PromptHelper]): PromptHelper
             embed_model (Optional[BaseEmbedding]): BaseEmbedding
             node_parser (Optional[NodeParser]): NodeParser
-            llama_logger (Optional[LlamaLogger]): LlamaLogger
+            llama_logger (Optional[LlamaLogger]): LlamaLogger (deprecated)
             chunk_size_limit (Optional[int]): chunk_size_limit
 
         """
+        callback_manager = callback_manager or CallbackManager([])
         llm_predictor = llm_predictor or LLMPredictor()
         # NOTE: the embed_model isn't used in all indices
         embed_model = embed_model or OpenAIEmbedding()
         prompt_helper = prompt_helper or PromptHelper.from_llm_predictor(
             llm_predictor, chunk_size_limit=chunk_size_limit
         )
         node_parser = node_parser or _get_default_node_parser(
@@ -77,10 +82,11 @@
         llama_logger = llama_logger or LlamaLogger()
 
         return cls(
             llm_predictor=llm_predictor,
             embed_model=embed_model,
             prompt_helper=prompt_helper,
             node_parser=node_parser,
-            llama_logger=llama_logger,
+            llama_logger=llama_logger,  # deprecated
+            callback_manager=callback_manager,
             chunk_size_limit=chunk_size_limit,
         )
```

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/struct_store/__init__.py` & `gpt_index-0.6.0a6/gpt_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/struct_store/base.py` & `gpt_index-0.6.0a6/gpt_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/struct_store/container_builder.py` & `gpt_index-0.6.0a6/gpt_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/struct_store/pandas.py` & `gpt_index-0.6.0a6/gpt_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/struct_store/pandas_query.py` & `gpt_index-0.6.0a6/gpt_index/indices/struct_store/pandas_query.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 from typing import Any, Callable, Optional
 
 import pandas as pd
 from langchain.input import print_text
 
+from gpt_index.callbacks.schema import CBEventType
 from gpt_index.indices.query.base import BaseQueryEngine
 from gpt_index.indices.query.schema import QueryBundle
 from gpt_index.indices.struct_store.pandas import GPTPandasIndex
 from gpt_index.prompts.default_prompts import DEFAULT_PANDAS_PROMPT
 from gpt_index.prompts.prompts import PandasPrompt
 from gpt_index.response.schema import Response
 
@@ -106,20 +107,40 @@
         """Get table context."""
         return str(self.df.head(self._head))
 
     def _query(self, query_bundle: QueryBundle) -> Response:
         """Answer a query."""
         context = self._get_table_context()
 
-        pandas_response_str, _ = self._service_context.llm_predictor.predict(
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.LLM,
+            payload={
+                "template": self._pandas_prompt,
+                "df_str": context,
+                "query_str": query_bundle.query_str,
+                "instruction_str": self._instruction_str,
+            },
+        )
+        (
+            pandas_response_str,
+            formatted_prompt,
+        ) = self._service_context.llm_predictor.predict(
             self._pandas_prompt,
             df_str=context,
             query_str=query_bundle.query_str,
             instruction_str=self._instruction_str,
         )
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.LLM,
+            payload={
+                "response": pandas_response_str,
+                "formatted_prompt": formatted_prompt,
+            },
+            event_id=event_id,
+        )
         if self._verbose:
             print_text(f"> Pandas Instructions:\n" f"```\n{pandas_response_str}\n```\n")
         pandas_output = self._output_processor(
             pandas_response_str,
             self.df,
             **self._output_kwargs,
         )
```

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/struct_store/sql.py` & `gpt_index-0.6.0a6/gpt_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/struct_store/sql_query.py` & `gpt_index-0.6.0a6/gpt_index/indices/struct_store/sql_query.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Default query for GPTSQLStructStoreIndex."""
 import logging
 from typing import Any, Optional
 
+from gpt_index.callbacks.schema import CBEventType
 from gpt_index.indices.query.base import BaseQueryEngine
 from gpt_index.indices.query.schema import QueryBundle
 from gpt_index.indices.struct_store.container_builder import SQLContextContainerBuilder
 from gpt_index.indices.struct_store.sql import GPTSQLStructStoreIndex
 from gpt_index.prompts.default_prompts import DEFAULT_TEXT_TO_SQL_PROMPT
 from gpt_index.prompts.prompts import TextToSQLPrompt
 from gpt_index.response.schema import Response
@@ -103,20 +104,34 @@
         return tables_desc_str
 
     @llm_token_counter("query")
     def _query(self, query_bundle: QueryBundle) -> Response:
         """Answer a query."""
         table_desc_str = self._get_table_context(query_bundle)
         logger.info(f"> Table desc str: {table_desc_str}")
-        response_str, _ = self._service_context.llm_predictor.predict(
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.LLM,
+            payload={
+                "template": self._text_to_sql_prompt,
+                "query_str": query_bundle.query_str,
+                "schema": table_desc_str,
+                "dialect": self._sql_database.dialect,
+            },
+        )
+        response_str, formatted_prompt = self._service_context.llm_predictor.predict(
             self._text_to_sql_prompt,
             query_str=query_bundle.query_str,
             schema=table_desc_str,
             dialect=self._sql_database.dialect,
         )
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.LLM,
+            payload={"response": response_str, "formatted_prompt": formatted_prompt},
+            event_id=event_id,
+        )
 
         sql_query_str = self._parse_response_to_sql(response_str)
         # assume that it's a valid SQL query
         logger.debug(f"> Predicted SQL query: {sql_query_str}")
 
         response_str, extra_info = self._sql_database.run_sql(sql_query_str)
         extra_info["sql_query"] = sql_query_str
@@ -124,20 +139,37 @@
         return response
 
     @llm_token_counter("aquery")
     async def _aquery(self, query_bundle: QueryBundle) -> Response:
         """Answer a query."""
         table_desc_str = self._get_table_context(query_bundle)
         logger.info(f"> Table desc str: {table_desc_str}")
-        response_str, _ = await self._service_context.llm_predictor.apredict(
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.LLM,
+            payload={
+                "template": self._text_to_sql_prompt,
+                "query_str": query_bundle.query_str,
+                "schema": table_desc_str,
+                "dialect": self._sql_database.dialect,
+            },
+        )
+        (
+            response_str,
+            formatted_prompt,
+        ) = await self._service_context.llm_predictor.apredict(
             self._text_to_sql_prompt,
             query_str=query_bundle.query_str,
             schema=table_desc_str,
             dialect=self._sql_database.dialect,
         )
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.LLM,
+            payload={"response": response_str, "formatted_prompt": formatted_prompt},
+            event_id=event_id,
+        )
 
         sql_query_str = self._parse_response_to_sql(response_str)
         # assume that it's a valid SQL query
         logger.debug(f"> Predicted SQL query: {sql_query_str}")
 
         response_str, extra_info = self._sql_database.run_sql(sql_query_str)
         extra_info["sql_query"] = sql_query_str
```

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/tree/__init__.py` & `gpt_index-0.6.0a6/gpt_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/tree/all_leaf_retriever.py` & `gpt_index-0.6.0a6/gpt_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/tree/base.py` & `gpt_index-0.6.0a6/gpt_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/tree/inserter.py` & `gpt_index-0.6.0a6/gpt_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/tree/select_leaf_embedding_retriever.py` & `gpt_index-0.6.0a6/gpt_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/tree/select_leaf_retriever.py` & `gpt_index-0.6.0a6/gpt_index/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/tree/tree_root_retriever.py` & `gpt_index-0.6.0a6/gpt_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/utils.py` & `gpt_index-0.6.0a6/gpt_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/vector_store/base.py` & `gpt_index-0.6.0a6/gpt_index/indices/vector_store/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 An index that that is built on top of an existing vector store.
 
 """
 
 from typing import Any, Dict, List, Optional, Sequence, Set, Tuple
 
+from gpt_index.callbacks.schema import CBEventType
 from gpt_index.async_utils import run_async_tasks
 from gpt_index.data_structs.data_structs_v2 import IndexDict
 from gpt_index.data_structs.node_v2 import ImageNode, IndexNode, Node
 from gpt_index.indices.base import BaseGPTIndex
 from gpt_index.indices.base_retriever import BaseRetriever
 from gpt_index.indices.service_context import ServiceContext
 from gpt_index.storage.storage_context import StorageContext
@@ -63,30 +64,40 @@
         Allows us to store these nodes in a vector store.
         Embeddings are called in batches.
 
         """
         id_to_node_map: Dict[str, Node] = {}
         id_to_embed_map: Dict[str, List[float]] = {}
 
+        nodes_embedded = 0
         for n in nodes:
             new_id = n.get_doc_id()
             if n.embedding is None:
+                nodes_embedded += 1
                 self._service_context.embed_model.queue_text_for_embedding(
                     new_id, n.get_text()
                 )
             else:
                 id_to_embed_map[new_id] = n.embedding
 
             id_to_node_map[new_id] = n
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.EMBEDDING
+        )
 
         # call embedding model to get embeddings
         (
             result_ids,
             result_embeddings,
         ) = self._service_context.embed_model.get_queued_text_embeddings()
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.EMBEDDING,
+            payload={"num_nodes": nodes_embedded},
+            event_id=event_id,
+        )
         for new_id, text_embedding in zip(result_ids, result_embeddings):
             id_to_embed_map[new_id] = text_embedding
 
         result_tups = []
         for id, embed in id_to_embed_map.items():
             doc_id = id_to_node_map[id].ref_doc_id
             if doc_id is None:
@@ -116,21 +127,31 @@
             if n.embedding is None:
                 text_queue.append((new_id, n.get_text()))
             else:
                 id_to_embed_map[new_id] = n.embedding
 
             id_to_node_map[new_id] = n
 
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.EMBEDDING
+        )
+
         # call embedding model to get embeddings
         (
             result_ids,
             result_embeddings,
         ) = await self._service_context.embed_model.aget_queued_text_embeddings(
             text_queue
         )
+
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.EMBEDDING,
+            payload={"num_nodes": len(text_queue)},
+            event_id=event_id,
+        )
         for new_id, text_embedding in zip(result_ids, result_embeddings):
             id_to_embed_map[new_id] = text_embedding
 
         result_tups = []
         for id, embed in id_to_embed_map.items():
             doc_id = id_to_node_map[id].ref_doc_id
             if doc_id is None:
```

### Comparing `gpt_index-0.6.0a5/gpt_index/indices/vector_store/retrievers.py` & `gpt_index-0.6.0a6/gpt_index/indices/vector_store/retrievers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Base vector store index query."""
 
 
 from typing import Any, List, Optional
 from gpt_index.constants import DEFAULT_SIMILARITY_TOP_K
 
+from gpt_index.callbacks.schema import CBEventType
 from gpt_index.data_structs.data_structs_v2 import IndexDict
-
 from gpt_index.data_structs.node_v2 import NodeWithScore
 from gpt_index.indices.base_retriever import BaseRetriever
 from gpt_index.indices.query.schema import QueryBundle
 from gpt_index.indices.utils import log_vector_store_query_result
 from gpt_index.indices.vector_store.base import GPTVectorStoreIndex
 from gpt_index.token_counter.token_counter import llm_token_counter
 from gpt_index.vector_stores.types import (
@@ -51,19 +51,25 @@
     @llm_token_counter("retrieve")
     def _retrieve(
         self,
         query_bundle: QueryBundle,
     ) -> List[NodeWithScore]:
         if self._vector_store.is_embedding_query:
             if query_bundle.embedding is None:
+                event_id = self._service_context.callback_manager.on_event_start(
+                    CBEventType.EMBEDDING
+                )
                 query_bundle.embedding = (
                     self._service_context.embed_model.get_agg_embedding_from_queries(
                         query_bundle.embedding_strs
                     )
                 )
+                self._service_context.callback_manager.on_event_end(
+                    CBEventType.EMBEDDING, payload={"num_nodes": 1}, event_id=event_id
+                )
 
         query = VectorStoreQuery(
             query_embedding=query_bundle.embedding,
             similarity_top_k=self._similarity_top_k,
             doc_ids=self._doc_ids,
             query_str=query_bundle.query_str,
             mode=self._vector_store_query_mode,
```

### Comparing `gpt_index-0.6.0a5/gpt_index/langchain_helpers/agents/agents.py` & `gpt_index-0.6.0a6/gpt_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/langchain_helpers/agents/toolkits.py` & `gpt_index-0.6.0a6/gpt_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/langchain_helpers/agents/tools.py` & `gpt_index-0.6.0a6/gpt_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/langchain_helpers/memory_wrapper.py` & `gpt_index-0.6.0a6/gpt_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/langchain_helpers/sql_wrapper.py` & `gpt_index-0.6.0a6/gpt_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/langchain_helpers/text_splitter.py` & `gpt_index-0.6.0a6/gpt_index/langchain_helpers/text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/llm_predictor/base.py` & `gpt_index-0.6.0a6/gpt_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/llm_predictor/chatgpt.py` & `gpt_index-0.6.0a6/gpt_index/llm_predictor/chatgpt.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/llm_predictor/stable_lm.py` & `gpt_index-0.6.0a6/gpt_index/llm_predictor/stable_lm.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/llm_predictor/structured.py` & `gpt_index-0.6.0a6/gpt_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/logger/base.py` & `gpt_index-0.6.0a6/gpt_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/node_parser/interface.py` & `gpt_index-0.6.0a6/gpt_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/node_parser/node_utils.py` & `gpt_index-0.6.0a6/gpt_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/node_parser/simple.py` & `gpt_index-0.6.0a6/gpt_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/optimization/optimizer.py` & `gpt_index-0.6.0a6/gpt_index/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/output_parsers/base.py` & `gpt_index-0.6.0a6/gpt_index/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/output_parsers/guardrails.py` & `gpt_index-0.6.0a6/gpt_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/output_parsers/langchain.py` & `gpt_index-0.6.0a6/gpt_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/output_parsers/selection.py` & `gpt_index-0.6.0a6/gpt_index/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/playground/base.py` & `gpt_index-0.6.0a6/gpt_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/prompts/base.py` & `gpt_index-0.6.0a6/gpt_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/prompts/chat_prompts.py` & `gpt_index-0.6.0a6/gpt_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/prompts/default_prompt_selectors.py` & `gpt_index-0.6.0a6/gpt_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/prompts/default_prompts.py` & `gpt_index-0.6.0a6/gpt_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/prompts/prompt_type.py` & `gpt_index-0.6.0a6/gpt_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/prompts/prompts.py` & `gpt_index-0.6.0a6/gpt_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/query_engine/__init__.py` & `gpt_index-0.6.0a6/gpt_index/query_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/query_engine/graph_query_engine.py` & `gpt_index-0.6.0a6/gpt_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/query_engine/multistep_query_engine.py` & `gpt_index-0.6.0a6/gpt_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/query_engine/router_query_engine.py` & `gpt_index-0.6.0a6/gpt_index/query_engine/router_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/query_engine/transform_query_engine.py` & `gpt_index-0.6.0a6/gpt_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/__init__.py` & `gpt_index-0.6.0a6/gpt_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/base.py` & `gpt_index-0.6.0a6/gpt_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/chatgpt_plugin/base.py` & `gpt_index-0.6.0a6/gpt_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/chroma.py` & `gpt_index-0.6.0a6/gpt_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/database.py` & `gpt_index-0.6.0a6/gpt_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/deeplake.py` & `gpt_index-0.6.0a6/gpt_index/readers/deeplake.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         dataset_name: Name of the deeplake dataset.
     """
 
     def __init__(
         self,
         token: Optional[str] = None,
     ):
-
         """initializing the deepLake reader"""
         import_err_msg = (
             "`deeplake` package not found, please run `pip install deeplake`"
         )
         try:
             import deeplake  # noqa: F401
         except ImportError:
```

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/discord_reader.py` & `gpt_index-0.6.0a6/gpt_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/download.py` & `gpt_index-0.6.0a6/gpt_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/elasticsearch.py` & `gpt_index-0.6.0a6/gpt_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/faiss.py` & `gpt_index-0.6.0a6/gpt_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/file/base.py` & `gpt_index-0.6.0a6/gpt_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/file/base_parser.py` & `gpt_index-0.6.0a6/gpt_index/readers/file/base_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/file/docs_parser.py` & `gpt_index-0.6.0a6/gpt_index/readers/file/docs_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/file/epub_parser.py` & `gpt_index-0.6.0a6/gpt_index/readers/file/epub_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/file/image_caption_parser.py` & `gpt_index-0.6.0a6/gpt_index/readers/file/image_caption_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/file/image_parser.py` & `gpt_index-0.6.0a6/gpt_index/readers/file/image_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/file/image_vision_llm_parser.py` & `gpt_index-0.6.0a6/gpt_index/readers/file/image_vision_llm_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/file/ipynb_parser.py` & `gpt_index-0.6.0a6/gpt_index/readers/file/ipynb_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/file/markdown_parser.py` & `gpt_index-0.6.0a6/gpt_index/readers/file/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/file/mbox_parser.py` & `gpt_index-0.6.0a6/gpt_index/readers/file/mbox_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/file/slides_parser.py` & `gpt_index-0.6.0a6/gpt_index/readers/file/slides_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/file/tabular_parser.py` & `gpt_index-0.6.0a6/gpt_index/readers/file/tabular_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/file/video_audio.py` & `gpt_index-0.6.0a6/gpt_index/readers/file/video_audio.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/github_readers/github_api_client.py` & `gpt_index-0.6.0a6/gpt_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/github_readers/github_repository_reader.py` & `gpt_index-0.6.0a6/gpt_index/readers/github_readers/github_repository_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         """
         super().__init__()
         if github_token is None:
             github_token = os.getenv("GITHUB_TOKEN")
             if github_token is None:
                 raise ValueError(
                     "Please provide a Github token. "
-                    "You can do so by passing it as an argument or"
+                    "You can do so by passing it as an argument or "
                     + "by setting the GITHUB_TOKEN environment variable."
                 )
 
         self._owner = owner
         self._repo = repo
         self._use_parser = use_parser
         self._verbose = verbose
```

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/github_readers/utils.py` & `gpt_index-0.6.0a6/gpt_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/google_readers/gdocs.py` & `gpt_index-0.6.0a6/gpt_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/google_readers/gsheets.py` & `gpt_index-0.6.0a6/gpt_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/json.py` & `gpt_index-0.6.0a6/gpt_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/make_com/wrapper.py` & `gpt_index-0.6.0a6/gpt_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/mbox.py` & `gpt_index-0.6.0a6/gpt_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/milvus.py` & `gpt_index-0.6.0a6/gpt_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/mongo.py` & `gpt_index-0.6.0a6/gpt_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/myscale.py` & `gpt_index-0.6.0a6/gpt_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/notion.py` & `gpt_index-0.6.0a6/gpt_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/obsidian.py` & `gpt_index-0.6.0a6/gpt_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/pinecone.py` & `gpt_index-0.6.0a6/gpt_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/qdrant.py` & `gpt_index-0.6.0a6/gpt_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/schema/base.py` & `gpt_index-0.6.0a6/gpt_index/readers/schema/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/slack.py` & `gpt_index-0.6.0a6/gpt_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/steamship/file_reader.py` & `gpt_index-0.6.0a6/gpt_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/string_iterable.py` & `gpt_index-0.6.0a6/gpt_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/twitter.py` & `gpt_index-0.6.0a6/gpt_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/weaviate/client.py` & `gpt_index-0.6.0a6/gpt_index/readers/weaviate/client.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/weaviate/reader.py` & `gpt_index-0.6.0a6/gpt_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/weaviate/utils.py` & `gpt_index-0.6.0a6/gpt_index/readers/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/web.py` & `gpt_index-0.6.0a6/gpt_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/wikipedia.py` & `gpt_index-0.6.0a6/gpt_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/readers/youtube_transcript.py` & `gpt_index-0.6.0a6/gpt_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/response/notebook_utils.py` & `gpt_index-0.6.0a6/gpt_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/response/schema.py` & `gpt_index-0.6.0a6/gpt_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/retrievers/__init__.py` & `gpt_index-0.6.0a6/gpt_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/retrievers/transform_retriever.py` & `gpt_index-0.6.0a6/gpt_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/schema.py` & `gpt_index-0.6.0a6/gpt_index/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/selectors/llm_selectors.py` & `gpt_index-0.6.0a6/gpt_index/selectors/llm_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/selectors/prompts.py` & `gpt_index-0.6.0a6/gpt_index/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/selectors/types.py` & `gpt_index-0.6.0a6/gpt_index/selectors/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/docstore/__init__.py` & `gpt_index-0.6.0a6/gpt_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/docstore/keyval_docstore.py` & `gpt_index-0.6.0a6/gpt_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/docstore/mongo_docstore.py` & `gpt_index-0.6.0a6/gpt_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/docstore/registry.py` & `gpt_index-0.6.0a6/gpt_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/docstore/simple_docstore.py` & `gpt_index-0.6.0a6/gpt_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/docstore/types.py` & `gpt_index-0.6.0a6/gpt_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/docstore/utils.py` & `gpt_index-0.6.0a6/gpt_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/index_store/keyval_index_store.py` & `gpt_index-0.6.0a6/gpt_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/index_store/mongo_index_store.py` & `gpt_index-0.6.0a6/gpt_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/index_store/simple_index_store.py` & `gpt_index-0.6.0a6/gpt_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/index_store/types.py` & `gpt_index-0.6.0a6/gpt_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/index_store/utils.py` & `gpt_index-0.6.0a6/gpt_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/kvstore/mongodb_kvstore.py` & `gpt_index-0.6.0a6/gpt_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/kvstore/simple_kvstore.py` & `gpt_index-0.6.0a6/gpt_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/kvstore/types.py` & `gpt_index-0.6.0a6/gpt_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/storage/storage_context.py` & `gpt_index-0.6.0a6/gpt_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/token_counter/mock_chain_wrapper.py` & `gpt_index-0.6.0a6/gpt_index/token_counter/mock_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/token_counter/mock_embed_model.py` & `gpt_index-0.6.0a6/gpt_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/token_counter/token_counter.py` & `gpt_index-0.6.0a6/gpt_index/token_counter/token_counter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/token_counter/utils.py` & `gpt_index-0.6.0a6/gpt_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/tools/query_engine.py` & `gpt_index-0.6.0a6/gpt_index/tools/query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/tts/bark.py` & `gpt_index-0.6.0a6/gpt_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/tts/base.py` & `gpt_index-0.6.0a6/gpt_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/tts/elevenlabs.py` & `gpt_index-0.6.0a6/gpt_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/utils.py` & `gpt_index-0.6.0a6/gpt_index/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/vector_stores/__init__.py` & `gpt_index-0.6.0a6/gpt_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/vector_stores/chatgpt_plugin.py` & `gpt_index-0.6.0a6/gpt_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/vector_stores/chroma.py` & `gpt_index-0.6.0a6/gpt_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/vector_stores/deeplake.py` & `gpt_index-0.6.0a6/gpt_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/vector_stores/faiss.py` & `gpt_index-0.6.0a6/gpt_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/vector_stores/milvus.py` & `gpt_index-0.6.0a6/gpt_index/vector_stores/milvus.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/vector_stores/myscale.py` & `gpt_index-0.6.0a6/gpt_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/vector_stores/opensearch.py` & `gpt_index-0.6.0a6/gpt_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/vector_stores/pinecone.py` & `gpt_index-0.6.0a6/gpt_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/vector_stores/qdrant.py` & `gpt_index-0.6.0a6/gpt_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/vector_stores/registry.py` & `gpt_index-0.6.0a6/gpt_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/vector_stores/simple.py` & `gpt_index-0.6.0a6/gpt_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/vector_stores/types.py` & `gpt_index-0.6.0a6/gpt_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index/vector_stores/weaviate.py` & `gpt_index-0.6.0a6/gpt_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/gpt_index.egg-info/PKG-INFO` & `gpt_index-0.6.0a6/gpt_index.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-index
-Version: 0.6.0a5
+Version: 0.6.0a6
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/gpt_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `gpt_index-0.6.0a5/gpt_index.egg-info/SOURCES.txt` & `gpt_index-0.6.0a6/gpt_index.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 gpt_index/types.py
 gpt_index/utils.py
 gpt_index.egg-info/PKG-INFO
 gpt_index.egg-info/SOURCES.txt
 gpt_index.egg-info/dependency_links.txt
 gpt_index.egg-info/requires.txt
 gpt_index.egg-info/top_level.txt
+gpt_index/callbacks/__init__.py
+gpt_index/callbacks/base.py
+gpt_index/callbacks/llama_debug.py
+gpt_index/callbacks/schema.py
 gpt_index/composability/__init__.py
 gpt_index/composability/base.py
 gpt_index/composability/joint_qa_summary.py
 gpt_index/data_structs/__init__.py
 gpt_index/data_structs/data_structs.py
 gpt_index/data_structs/data_structs_v2.py
 gpt_index/data_structs/node_v2.py
@@ -254,14 +258,16 @@
 gpt_index/vector_stores/registry.py
 gpt_index/vector_stores/simple.py
 gpt_index/vector_stores/types.py
 gpt_index/vector_stores/weaviate.py
 tests/__init__.py
 tests/conftest.py
 tests/test_utils.py
+tests/callbacks/__init__.py
+tests/callbacks/test_llama_debug.py
 tests/embeddings/__init__.py
 tests/embeddings/test_base.py
 tests/indices/__init__.py
 tests/indices/conftest.py
 tests/indices/test_loading.py
 tests/indices/test_loading_graph.py
 tests/indices/test_node_utils.py
@@ -345,8 +351,9 @@
 tests/storage/conftest.py
 tests/storage/docstore/__init__.py
 tests/storage/docstore/test_mongo_docstore.py
 tests/storage/docstore/test_simple_docstore.py
 tests/token_predictor/__init__.py
 tests/token_predictor/test_base.py
 tests/vector_stores/__init__.py
-tests/vector_stores/test_qdrant.py
+tests/vector_stores/test_qdrant.py
+tests/vector_stores/test_weaviate.py
```

### Comparing `gpt_index-0.6.0a5/setup.py` & `gpt_index-0.6.0a6/setup.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/conftest.py` & `gpt_index-0.6.0a6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/embeddings/test_base.py` & `gpt_index-0.6.0a6/tests/embeddings/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/composability/test_utils.py` & `gpt_index-0.6.0a6/tests/indices/composability/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/conftest.py` & `gpt_index-0.6.0a6/tests/indices/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/empty/test_base.py` & `gpt_index-0.6.0a6/tests/indices/empty/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/keyword_table/test_base.py` & `gpt_index-0.6.0a6/tests/indices/keyword_table/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/keyword_table/test_retrievers.py` & `gpt_index-0.6.0a6/tests/indices/keyword_table/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/keyword_table/test_utils.py` & `gpt_index-0.6.0a6/tests/indices/keyword_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/knowledge_graph/test_base.py` & `gpt_index-0.6.0a6/tests/indices/knowledge_graph/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/knowledge_graph/test_retrievers.py` & `gpt_index-0.6.0a6/tests/indices/knowledge_graph/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/list/test_index.py` & `gpt_index-0.6.0a6/tests/indices/list/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/list/test_retrievers.py` & `gpt_index-0.6.0a6/tests/indices/list/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/postprocessor/test_base.py` & `gpt_index-0.6.0a6/tests/indices/postprocessor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/query/conftest.py` & `gpt_index-0.6.0a6/tests/indices/query/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/query/query_transform/test_base.py` & `gpt_index-0.6.0a6/tests/indices/query/query_transform/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/query/test_compose.py` & `gpt_index-0.6.0a6/tests/indices/query/test_compose.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/query/test_compose_vector.py` & `gpt_index-0.6.0a6/tests/indices/query/test_compose_vector.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/query/test_query_bundle.py` & `gpt_index-0.6.0a6/tests/indices/query/test_query_bundle.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/struct_store/conftest.py` & `gpt_index-0.6.0a6/tests/indices/struct_store/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/struct_store/test_base.py` & `gpt_index-0.6.0a6/tests/indices/struct_store/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/struct_store/test_pandas.py` & `gpt_index-0.6.0a6/tests/indices/struct_store/test_pandas.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/struct_store/test_sql_query.py` & `gpt_index-0.6.0a6/tests/indices/struct_store/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/test_loading.py` & `gpt_index-0.6.0a6/tests/indices/test_loading.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/test_loading_graph.py` & `gpt_index-0.6.0a6/tests/indices/test_loading_graph.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/test_node_utils.py` & `gpt_index-0.6.0a6/tests/indices/test_node_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/test_prompt_helper.py` & `gpt_index-0.6.0a6/tests/indices/test_prompt_helper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/tree/conftest.py` & `gpt_index-0.6.0a6/tests/indices/tree/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/tree/test_embedding_retriever.py` & `gpt_index-0.6.0a6/tests/indices/tree/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/tree/test_index.py` & `gpt_index-0.6.0a6/tests/indices/tree/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/tree/test_retrievers.py` & `gpt_index-0.6.0a6/tests/indices/tree/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/vector_store/conftest.py` & `gpt_index-0.6.0a6/tests/indices/vector_store/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/vector_store/mock_faiss.py` & `gpt_index-0.6.0a6/tests/indices/vector_store/mock_faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/vector_store/mock_services.py` & `gpt_index-0.6.0a6/tests/indices/vector_store/mock_services.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/vector_store/test_faiss.py` & `gpt_index-0.6.0a6/tests/indices/vector_store/test_faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/vector_store/test_milvus.py` & `gpt_index-0.6.0a6/tests/indices/vector_store/test_milvus.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/vector_store/test_myscale.py` & `gpt_index-0.6.0a6/tests/indices/vector_store/test_myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/vector_store/test_pinecone.py` & `gpt_index-0.6.0a6/tests/indices/vector_store/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/vector_store/test_retrievers.py` & `gpt_index-0.6.0a6/tests/indices/vector_store/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/vector_store/test_simple.py` & `gpt_index-0.6.0a6/tests/indices/vector_store/test_simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/vector_store/test_weaviate.py` & `gpt_index-0.6.0a6/tests/indices/vector_store/test_weaviate.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/indices/vector_store/utils.py` & `gpt_index-0.6.0a6/tests/indices/vector_store/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/langchain_helpers/test_text_splitter.py` & `gpt_index-0.6.0a6/tests/langchain_helpers/test_text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/llm_predictor/test_base.py` & `gpt_index-0.6.0a6/tests/llm_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/logger/test_base.py` & `gpt_index-0.6.0a6/tests/logger/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/mock_utils/mock_predict.py` & `gpt_index-0.6.0a6/tests/mock_utils/mock_predict.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/mock_utils/mock_prompts.py` & `gpt_index-0.6.0a6/tests/mock_utils/mock_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/mock_utils/mock_text_splitter.py` & `gpt_index-0.6.0a6/tests/mock_utils/mock_text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/mock_utils/mock_utils.py` & `gpt_index-0.6.0a6/tests/mock_utils/mock_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/optimization/test_base.py` & `gpt_index-0.6.0a6/tests/optimization/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/output_parsers/test_base.py` & `gpt_index-0.6.0a6/tests/output_parsers/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/output_parsers/test_selection.py` & `gpt_index-0.6.0a6/tests/output_parsers/test_selection.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/playground/test_base.py` & `gpt_index-0.6.0a6/tests/playground/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/prompts/test_base.py` & `gpt_index-0.6.0a6/tests/prompts/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/readers/test_file.py` & `gpt_index-0.6.0a6/tests/readers/test_file.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/readers/test_json.py` & `gpt_index-0.6.0a6/tests/readers/test_json.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/readers/test_mongo.py` & `gpt_index-0.6.0a6/tests/readers/test_mongo.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/selectors/test_llm_selectors.py` & `gpt_index-0.6.0a6/tests/selectors/test_llm_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/storage/conftest.py` & `gpt_index-0.6.0a6/tests/storage/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/storage/docstore/test_mongo_docstore.py` & `gpt_index-0.6.0a6/tests/storage/docstore/test_mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/storage/docstore/test_simple_docstore.py` & `gpt_index-0.6.0a6/tests/storage/docstore/test_simple_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/test_utils.py` & `gpt_index-0.6.0a6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/token_predictor/test_base.py` & `gpt_index-0.6.0a6/tests/token_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.0a5/tests/vector_stores/test_qdrant.py` & `gpt_index-0.6.0a6/tests/vector_stores/test_qdrant.py`

 * *Files identical despite different names*

