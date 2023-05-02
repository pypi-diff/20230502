# Comparing `tmp/llama_index-0.6.0a5.tar.gz` & `tmp/llama_index-0.6.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index-0.6.0a5.tar", last modified: Mon May  1 06:33:46 2023, max compression
+gzip compressed data, was "llama_index-0.6.0a6.tar", last modified: Tue May  2 07:46:53 2023, max compression
```

## Comparing `llama_index-0.6.0a5.tar` & `llama_index-0.6.0a6.tar`

### file list

```diff
@@ -1,312 +1,319 @@
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.759964 llama_index-0.6.0a5/
--rw-r--r--   0 jerryliu   (501) staff       (20)     1064 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/LICENSE
--rw-r--r--   0 jerryliu   (501) staff       (20)       73 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/MANIFEST.in
--rw-r--r--   0 jerryliu   (501) staff       (20)     4354 2023-05-01 06:33:46.759859 llama_index-0.6.0a5/PKG-INFO
--rw-r--r--   0 jerryliu   (501) staff       (20)     4124 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/README.md
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.735778 llama_index-0.6.0a5/llama_index/
--rw-r--r--   0 jerryliu   (501) staff       (20)       13 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/VERSION
--rw-r--r--   0 jerryliu   (501) staff       (20)     4719 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      322 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/async_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.736499 llama_index-0.6.0a5/llama_index/composability/
--rw-r--r--   0 jerryliu   (501) staff       (20)      220 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/composability/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      171 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/composability/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2739 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      219 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/constants.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.737321 llama_index-0.6.0a5/llama_index/data_structs/
--rw-r--r--   0 jerryliu   (501) staff       (20)      409 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    12377 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/data_structs.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     9476 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/data_structs_v2.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      264 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/node_mapping.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6221 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/node_v2.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      779 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/registry.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3256 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/struct_type.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      908 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/table.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1032 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/data_structs/table_v2.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.737770 llama_index-0.6.0a5/llama_index/embeddings/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/embeddings/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7721 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/embeddings/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1109 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/embeddings/langchain.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    10103 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/embeddings/openai.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      559 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/embeddings/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.738038 llama_index-0.6.0a5/llama_index/evaluation/
--rw-r--r--   0 jerryliu   (501) staff       (20)      259 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/evaluation/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11972 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/evaluation/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5344 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      544 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/img_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.738744 llama_index-0.6.0a5/llama_index/indices/
--rw-r--r--   0 jerryliu   (501) staff       (20)      542 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     9112 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      859 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/base_retriever.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.738830 llama_index-0.6.0a5/llama_index/indices/common/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.739191 llama_index-0.6.0a5/llama_index/indices/common/struct_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8114 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      776 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2676 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.739371 llama_index-0.6.0a5/llama_index/indices/common_tree/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7244 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.739552 llama_index-0.6.0a5/llama_index/indices/composability/
--rw-r--r--   0 jerryliu   (501) staff       (20)      180 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/composability/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3962 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/composability/graph.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.739819 llama_index-0.6.0a5/llama_index/indices/empty/
--rw-r--r--   0 jerryliu   (501) staff       (20)      198 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/empty/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2151 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/empty/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1176 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/empty/retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.740370 llama_index-0.6.0a5/llama_index/indices/keyword_table/
--rw-r--r--   0 jerryliu   (501) staff       (20)      656 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7652 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      650 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5891 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      844 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2264 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.740638 llama_index-0.6.0a5/llama_index/indices/knowledge_graph/
--rw-r--r--   0 jerryliu   (501) staff       (20)      254 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7816 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     9543 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/knowledge_graph/retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.740906 llama_index-0.6.0a5/llama_index/indices/list/
--rw-r--r--   0 jerryliu   (501) staff       (20)      295 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/list/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3305 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/list/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3455 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/list/retrievers.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3608 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/loading.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.741353 llama_index-0.6.0a5/llama_index/indices/postprocessor/
--rw-r--r--   0 jerryliu   (501) staff       (20)      888 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)       83 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/postprocessor/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11695 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8778 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4896 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/postprocessor/pii.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8492 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.741801 llama_index-0.6.0a5/llama_index/indices/query/
--rw-r--r--   0 jerryliu   (501) staff       (20)      137 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1937 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3386 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.742080 llama_index-0.6.0a5/llama_index/indices/query/query_transform/
--rw-r--r--   0 jerryliu   (501) staff       (20)      281 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8904 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5920 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8098 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/response_synthesis.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1248 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/query/schema.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1811 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/registry.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.742383 llama_index-0.6.0a5/llama_index/indices/response/
--rw-r--r--   0 jerryliu   (501) staff       (20)      419 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/response/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    21995 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/response/response_builder.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      262 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/response/type.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3296 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/service_context.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.743013 llama_index-0.6.0a5/llama_index/indices/struct_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)      622 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2115 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/struct_store/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5765 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2214 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4688 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/struct_store/pandas_query.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6139 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5887 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.743641 llama_index-0.6.0a5/llama_index/indices/tree/
--rw-r--r--   0 jerryliu   (501) staff       (20)      616 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/tree/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1612 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5834 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/tree/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7181 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/tree/inserter.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4663 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    15299 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1402 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2005 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.743907 llama_index-0.6.0a5/llama_index/indices/vector_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)      260 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8183 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/vector_store/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3987 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/indices/vector_store/retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.744466 llama_index-0.6.0a5/llama_index/langchain_helpers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       39 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.744858 llama_index-0.6.0a5/llama_index/langchain_helpers/agents/
--rw-r--r--   0 jerryliu   (501) staff       (20)      514 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2994 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      837 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2211 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      252 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/chain_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7675 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3287 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    18172 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.745310 llama_index-0.6.0a5/llama_index/llm_predictor/
--rw-r--r--   0 jerryliu   (501) staff       (20)      330 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    10838 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/llm_predictor/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4282 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/llm_predictor/chatgpt.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4732 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/llm_predictor/stable_lm.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2274 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/llm_predictor/structured.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.745503 llama_index-0.6.0a5/llama_index/logger/
--rw-r--r--   0 jerryliu   (501) staff       (20)       95 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/logger/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      995 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/logger/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.745882 llama_index-0.6.0a5/llama_index/node_parser/
--rw-r--r--   0 jerryliu   (501) staff       (20)      184 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/node_parser/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      530 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/node_parser/interface.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3585 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/node_parser/node_utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1821 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/node_parser/simple.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.746079 llama_index-0.6.0a5/llama_index/optimization/
--rw-r--r--   0 jerryliu   (501) staff       (20)      144 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/optimization/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4301 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/optimization/optimizer.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.746603 llama_index-0.6.0a5/llama_index/output_parsers/
--rw-r--r--   0 jerryliu   (501) staff       (20)      230 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/output_parsers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      611 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/output_parsers/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2742 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1828 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/output_parsers/langchain.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1345 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/output_parsers/selection.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.746817 llama_index-0.6.0a5/llama_index/playground/
--rw-r--r--   0 jerryliu   (501) staff       (20)      202 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/playground/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6471 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/playground/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.747555 llama_index-0.6.0a5/llama_index/prompts/
--rw-r--r--   0 jerryliu   (501) staff       (20)       87 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/prompts/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6633 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/prompts/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1969 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1134 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    10843 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/prompts/default_prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1120 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/prompts/prompt_type.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7685 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/prompts/prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/py.typed
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.748194 llama_index-0.6.0a5/llama_index/query_engine/
--rw-r--r--   0 jerryliu   (501) staff       (20)      560 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/query_engine/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3572 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5814 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5322 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2449 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/query_engine/router_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2967 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.750991 llama_index-0.6.0a5/llama_index/readers/
--rw-r--r--   0 jerryliu   (501) staff       (20)     2974 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      659 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.751232 llama_index-0.6.0a5/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 jerryliu   (501) staff       (20)      145 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2111 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3755 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/chroma.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3308 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/database.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3457 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/deeplake.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4981 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/discord_reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7775 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/download.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2392 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/elasticsearch.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2510 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/faiss.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.752745 llama_index-0.6.0a5/llama_index/readers/file/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8535 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1342 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/base_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1629 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/docs_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1318 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/epub_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3180 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/image_caption_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4106 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/image_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3222 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/image_vision_llm_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1027 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/ipynb_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3616 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/markdown_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3162 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/mbox_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3945 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/slides_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3357 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/tabular_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1770 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/file/video_audio.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.753140 llama_index-0.6.0a5/llama_index/readers/github_readers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11730 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    15928 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5473 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.753402 llama_index-0.6.0a5/llama_index/readers/google_readers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5659 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4989 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3708 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/json.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.753626 llama_index-0.6.0a5/llama_index/readers/make_com/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1696 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1261 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/mbox.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4588 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/milvus.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2608 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/mongo.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5541 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/myscale.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5679 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/notion.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1601 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/obsidian.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2766 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/pinecone.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3909 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/qdrant.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.753847 llama_index-0.6.0a5/llama_index/readers/schema/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/schema/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1214 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/schema/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7892 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/slack.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.754066 llama_index-0.6.0a5/llama_index/readers/steamship/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3498 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1042 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/string_iterable.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1918 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/twitter.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.754507 llama_index-0.6.0a5/llama_index/readers/weaviate/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7766 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/weaviate/client.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3986 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1867 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/weaviate/utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7987 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/web.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      981 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/wikipedia.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1255 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.754942 llama_index-0.6.0a5/llama_index/response/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/response/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2039 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/response/notebook_utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3071 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/response/schema.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      262 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/response/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.755177 llama_index-0.6.0a5/llama_index/retrievers/
--rw-r--r--   0 jerryliu   (501) staff       (20)     1258 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/retrievers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1066 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2768 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/schema.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.755576 llama_index-0.6.0a5/llama_index/selectors/
--rw-r--r--   0 jerryliu   (501) staff       (20)      259 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/selectors/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7055 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/selectors/llm_selectors.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2438 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/selectors/prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2006 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/selectors/types.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.755752 llama_index-0.6.0a5/llama_index/storage/
--rw-r--r--   0 jerryliu   (501) staff       (20)      124 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.756385 llama_index-0.6.0a5/llama_index/storage/docstore/
--rw-r--r--   0 jerryliu   (501) staff       (20)      536 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/docstore/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4825 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1408 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      762 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/docstore/registry.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2294 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2532 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/docstore/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      918 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/docstore/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.756931 llama_index-0.6.0a5/llama_index/storage/index_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)      301 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/index_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2224 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1341 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1508 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      884 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/index_store/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      644 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/index_store/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.757287 llama_index-0.6.0a5/llama_index/storage/kvstore/
--rw-r--r--   0 jerryliu   (501) staff       (20)      187 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4061 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2330 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      973 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/kvstore/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3114 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/storage/storage_context.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.757727 llama_index-0.6.0a5/llama_index/token_counter/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/token_counter/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4664 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/token_counter/mock_chain_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      722 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2874 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/token_counter/token_counter.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      908 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/token_counter/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.758015 llama_index-0.6.0a5/llama_index/tools/
--rw-r--r--   0 jerryliu   (501) staff       (20)      162 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/tools/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1557 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/tools/query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      366 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/tools/types.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.758403 llama_index-0.6.0a5/llama_index/tts/
--rw-r--r--   0 jerryliu   (501) staff       (20)      154 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/tts/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2589 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/tts/bark.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      631 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/tts/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1282 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/tts/elevenlabs.py
--rw-r--r--   0 jerryliu   (501) staff       (20)       81 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5847 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.759711 llama_index-0.6.0a5/llama_index/vector_stores/
--rw-r--r--   0 jerryliu   (501) staff       (20)     1132 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5240 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3947 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/chroma.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8631 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/deeplake.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4365 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/faiss.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    15768 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/milvus.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8344 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/myscale.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7186 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11419 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6505 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1973 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/registry.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5084 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/simple.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2210 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3385 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index/vector_stores/weaviate.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-01 06:33:46.736230 llama_index-0.6.0a5/llama_index.egg-info/
--rw-r--r--   0 jerryliu   (501) staff       (20)     4354 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index.egg-info/PKG-INFO
--rw-r--r--   0 jerryliu   (501) staff       (20)     9915 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index.egg-info/SOURCES.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)        1 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index.egg-info/dependency_links.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)       96 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index.egg-info/requires.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)       12 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/llama_index.egg-info/top_level.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)       38 2023-05-01 06:33:46.759993 llama_index-0.6.0a5/setup.cfg
--rw-r--r--   0 jerryliu   (501) staff       (20)     1130 2023-05-01 06:33:46.000000 llama_index-0.6.0a5/setup.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.818520 llama_index-0.6.0a6/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1064 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/LICENSE
+-rw-r--r--   0 jerryliu   (501) staff       (20)       73 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/MANIFEST.in
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4354 2023-05-02 07:46:53.818386 llama_index-0.6.0a6/PKG-INFO
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4124 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/README.md
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.792635 llama_index-0.6.0a6/llama_index/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       13 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/VERSION
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4719 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      322 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/async_utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.793628 llama_index-0.6.0a6/llama_index/callbacks/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      196 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/callbacks/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3068 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/callbacks/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5526 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/callbacks/llama_debug.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1073 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/callbacks/schema.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.794024 llama_index-0.6.0a6/llama_index/composability/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      220 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/composability/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      171 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/composability/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3091 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      219 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/constants.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.795142 llama_index-0.6.0a6/llama_index/data_structs/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      409 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    12377 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     9476 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/data_structs_v2.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      264 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/node_mapping.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6221 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/node_v2.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      779 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/registry.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3256 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      908 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/table.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1032 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/table_v2.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.795707 llama_index-0.6.0a6/llama_index/embeddings/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/embeddings/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7721 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/embeddings/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1109 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/embeddings/langchain.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    10103 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/embeddings/openai.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      559 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/embeddings/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.796046 llama_index-0.6.0a6/llama_index/evaluation/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      259 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/evaluation/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    11972 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/evaluation/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5344 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      544 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/img_utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.797020 llama_index-0.6.0a6/llama_index/indices/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      542 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     9752 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      859 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.797130 llama_index-0.6.0a6/llama_index/indices/common/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.797579 llama_index-0.6.0a6/llama_index/indices/common/struct_store/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8474 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      776 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2676 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.797829 llama_index-0.6.0a6/llama_index/indices/common_tree/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7977 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.798049 llama_index-0.6.0a6/llama_index/indices/composability/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      180 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3962 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.798365 llama_index-0.6.0a6/llama_index/indices/empty/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      198 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2151 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/empty/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1176 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.798967 llama_index-0.6.0a6/llama_index/indices/keyword_table/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      656 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8545 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      650 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6487 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      844 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2264 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.799238 llama_index-0.6.0a6/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      254 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     9049 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    10431 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/knowledge_graph/retrievers.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.799512 llama_index-0.6.0a6/llama_index/indices/list/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      295 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/list/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3305 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/list/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4198 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3608 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/loading.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.799958 llama_index-0.6.0a6/llama_index/indices/postprocessor/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      888 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)       83 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/postprocessor/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    11695 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8778 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4896 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8492 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.800416 llama_index-0.6.0a6/llama_index/indices/query/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      137 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1937 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3386 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.800680 llama_index-0.6.0a6/llama_index/indices/query/query_transform/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      281 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8904 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5920 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8098 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/response_synthesis.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1248 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/schema.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1811 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/registry.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.800975 llama_index-0.6.0a6/llama_index/indices/response/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      419 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/response/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    24774 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/response/response_builder.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      262 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/response/type.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3643 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/service_context.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.801598 llama_index-0.6.0a6/llama_index/indices/struct_store/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      622 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2115 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5765 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2214 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5409 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/struct_store/pandas_query.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6139 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7149 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.802219 llama_index-0.6.0a6/llama_index/indices/tree/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      616 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1612 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5834 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/tree/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7181 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4663 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    15299 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1402 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2005 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.802481 llama_index-0.6.0a6/llama_index/indices/vector_store/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      260 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8914 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/vector_store/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4355 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/vector_store/retrievers.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.802916 llama_index-0.6.0a6/llama_index/langchain_helpers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       39 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.803288 llama_index-0.6.0a6/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      514 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2994 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      837 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2211 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      252 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/chain_wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7675 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3287 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    18172 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.803718 llama_index-0.6.0a6/llama_index/llm_predictor/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      330 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    10838 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/llm_predictor/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4282 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/llm_predictor/chatgpt.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4732 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/llm_predictor/stable_lm.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2274 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/llm_predictor/structured.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.803890 llama_index-0.6.0a6/llama_index/logger/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       95 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/logger/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      995 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/logger/base.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.804242 llama_index-0.6.0a6/llama_index/node_parser/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      184 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/node_parser/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      530 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/node_parser/interface.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3585 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1821 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/node_parser/simple.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.804417 llama_index-0.6.0a6/llama_index/optimization/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      144 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/optimization/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4301 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/optimization/optimizer.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.804852 llama_index-0.6.0a6/llama_index/output_parsers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      230 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      611 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/output_parsers/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2742 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1828 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/output_parsers/langchain.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1345 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/output_parsers/selection.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.805019 llama_index-0.6.0a6/llama_index/playground/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      202 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/playground/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6471 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/playground/base.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.805630 llama_index-0.6.0a6/llama_index/prompts/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       87 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/prompts/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6633 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/prompts/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1969 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1134 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    10843 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1120 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7685 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/prompts/prompts.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/py.typed
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.806167 llama_index-0.6.0a6/llama_index/query_engine/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      560 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/query_engine/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3572 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5814 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6999 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2449 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/query_engine/router_query_engine.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2967 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.808870 llama_index-0.6.0a6/llama_index/readers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2974 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      659 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/base.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.809124 llama_index-0.6.0a6/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      145 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2111 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3755 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/chroma.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3308 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/database.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3456 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/deeplake.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4981 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/discord_reader.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7775 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/download.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2392 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2510 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/faiss.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.810894 llama_index-0.6.0a6/llama_index/readers/file/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8535 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1342 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/base_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1629 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/docs_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1318 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/epub_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3180 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/image_caption_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4106 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/image_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3222 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/image_vision_llm_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1027 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/ipynb_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3616 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/markdown_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3162 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/mbox_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3945 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/slides_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3357 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/tabular_parser.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1770 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/video_audio.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.811387 llama_index-0.6.0a6/llama_index/readers/github_readers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    11730 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    15929 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5473 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.811742 llama_index-0.6.0a6/llama_index/readers/google_readers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5659 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4989 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3708 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/json.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.811884 llama_index-0.6.0a6/llama_index/readers/llamahub_modules/
+-rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/llamahub_modules/__init__.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.812086 llama_index-0.6.0a6/llama_index/readers/make_com/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1696 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1261 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/mbox.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4588 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/milvus.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2608 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/mongo.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5541 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/myscale.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5679 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/notion.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1601 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/obsidian.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2766 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/pinecone.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3909 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/qdrant.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.812317 llama_index-0.6.0a6/llama_index/readers/schema/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1214 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/schema/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7892 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/slack.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.812543 llama_index-0.6.0a6/llama_index/readers/steamship/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3498 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1042 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/string_iterable.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1918 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/twitter.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.812898 llama_index-0.6.0a6/llama_index/readers/weaviate/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7766 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/weaviate/client.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3986 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1867 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/weaviate/utils.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7987 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/web.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      981 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/wikipedia.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1255 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.813256 llama_index-0.6.0a6/llama_index/response/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/response/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2039 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/response/notebook_utils.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3071 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/response/schema.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      262 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/response/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.813444 llama_index-0.6.0a6/llama_index/retrievers/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1258 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/retrievers/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1066 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2768 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/schema.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.813814 llama_index-0.6.0a6/llama_index/selectors/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      259 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/selectors/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7055 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/selectors/llm_selectors.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2438 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/selectors/prompts.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2006 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/selectors/types.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.813996 llama_index-0.6.0a6/llama_index/storage/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      124 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/__init__.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.814669 llama_index-0.6.0a6/llama_index/storage/docstore/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      536 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4825 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1408 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      762 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2294 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2532 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/docstore/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      918 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.815234 llama_index-0.6.0a6/llama_index/storage/index_store/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      301 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2224 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1341 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1508 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      884 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/index_store/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      644 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.815650 llama_index-0.6.0a6/llama_index/storage/kvstore/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      187 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4061 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2330 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      973 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3114 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/storage_context.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.816139 llama_index-0.6.0a6/llama_index/token_counter/
+-rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/token_counter/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4664 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/token_counter/mock_chain_wrapper.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      722 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2874 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/token_counter/token_counter.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      908 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/token_counter/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.816457 llama_index-0.6.0a6/llama_index/tools/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      162 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/tools/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1557 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/tools/query_engine.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      366 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/tools/types.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.816875 llama_index-0.6.0a6/llama_index/tts/
+-rw-r--r--   0 jerryliu   (501) staff       (20)      154 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/tts/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2589 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/tts/bark.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)      631 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/tts/base.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1282 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/tts/elevenlabs.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)       81 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5847 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/utils.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.818227 llama_index-0.6.0a6/llama_index/vector_stores/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1132 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5240 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3947 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8631 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/deeplake.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4365 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    15768 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     8344 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     7186 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)    11419 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     6505 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1973 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/registry.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     5084 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/simple.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     2210 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/types.py
+-rw-r--r--   0 jerryliu   (501) staff       (20)     3385 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/weaviate.py
+drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.793183 llama_index-0.6.0a6/llama_index.egg-info/
+-rw-r--r--   0 jerryliu   (501) staff       (20)     4354 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index.egg-info/PKG-INFO
+-rw-r--r--   0 jerryliu   (501) staff       (20)    10097 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index.egg-info/SOURCES.txt
+-rw-r--r--   0 jerryliu   (501) staff       (20)        1 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index.egg-info/dependency_links.txt
+-rw-r--r--   0 jerryliu   (501) staff       (20)       96 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index.egg-info/requires.txt
+-rw-r--r--   0 jerryliu   (501) staff       (20)       12 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index.egg-info/top_level.txt
+-rw-r--r--   0 jerryliu   (501) staff       (20)       38 2023-05-02 07:46:53.818557 llama_index-0.6.0a6/setup.cfg
+-rw-r--r--   0 jerryliu   (501) staff       (20)     1130 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/setup.py
```

### Comparing `llama_index-0.6.0a5/LICENSE` & `llama_index-0.6.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/PKG-INFO` & `llama_index-0.6.0a6/llama_index.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: llama_index
-Version: 0.6.0a5
+Name: llama-index
+Version: 0.6.0a6
 Summary: Interface between LLMs and your data.
 Home-page: https://github.com/jerryjliu/gpt_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `llama_index-0.6.0a5/README.md` & `llama_index-0.6.0a6/README.md`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/__init__.py` & `llama_index-0.6.0a6/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/composability/joint_qa_summary.py` & `llama_index-0.6.0a6/llama_index/composability/joint_qa_summary.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Joint QA Summary graph."""
 
 
 from typing import Sequence, Optional
 from llama_index.storage.docstore.registry import get_default_docstore
 
+from llama_index.callbacks.schema import CBEventType
 from llama_index.indices.service_context import ServiceContext
 from llama_index.composability import ComposableGraph
 from llama_index.indices.list.base import GPTListIndex
 from llama_index.indices.tree.base import GPTTreeIndex
 from llama_index.indices.vector_store import GPTVectorStoreIndex
 from llama_index.readers.schema.base import Document
 from llama_index.storage.docstore import BaseDocumentStore
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

### Comparing `llama_index-0.6.0a5/llama_index/data_structs/data_structs.py` & `llama_index-0.6.0a6/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/data_structs/data_structs_v2.py` & `llama_index-0.6.0a6/llama_index/data_structs/data_structs_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/data_structs/node_v2.py` & `llama_index-0.6.0a6/llama_index/data_structs/node_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/data_structs/registry.py` & `llama_index-0.6.0a6/llama_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/data_structs/struct_type.py` & `llama_index-0.6.0a6/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/data_structs/table.py` & `llama_index-0.6.0a6/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/data_structs/table_v2.py` & `llama_index-0.6.0a6/llama_index/data_structs/table_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/embeddings/base.py` & `llama_index-0.6.0a6/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/embeddings/langchain.py` & `llama_index-0.6.0a6/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/embeddings/openai.py` & `llama_index-0.6.0a6/llama_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/embeddings/utils.py` & `llama_index-0.6.0a6/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/evaluation/base.py` & `llama_index-0.6.0a6/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/evaluation/dataset_generation.py` & `llama_index-0.6.0a6/llama_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/img_utils.py` & `llama_index-0.6.0a6/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/__init__.py` & `llama_index-0.6.0a6/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/base.py` & `llama_index-0.6.0a6/llama_index/indices/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Base index classes."""
 import logging
 from abc import ABC, abstractmethod
 from typing import Any, Generic, List, Optional, Sequence, Type, TypeVar
 
+from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.data_structs_v2 import V2IndexStruct
 from llama_index.data_structs.node_v2 import Node
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.service_context import ServiceContext
 from llama_index.readers.schema.base import Document
 from llama_index.storage.docstore.types import BaseDocumentStore
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

### Comparing `llama_index-0.6.0a5/llama_index/indices/base_retriever.py` & `llama_index-0.6.0a6/llama_index/indices/base_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/common/struct_store/base.py` & `llama_index-0.6.0a6/llama_index/indices/common/struct_store/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Common classes for structured operations."""
 
 import logging
 from abc import abstractmethod
 from typing import Any, Callable, Dict, List, Optional, Sequence, cast
 
+from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.node_v2 import Node
 from llama_index.data_structs.table import StructDatapoint
 from llama_index.indices.response.response_builder import get_response_builder
 from llama_index.indices.service_context import ServiceContext
 from llama_index.langchain_helpers.chain_wrapper import LLMPredictor
 from llama_index.langchain_helpers.sql_wrapper import SQLDatabase
 from llama_index.langchain_helpers.text_splitter import TextSplitter
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

### Comparing `llama_index-0.6.0a5/llama_index/indices/common/struct_store/schema.py` & `llama_index-0.6.0a6/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/common/struct_store/sql.py` & `llama_index-0.6.0a6/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/common_tree/base.py` & `llama_index-0.6.0a6/llama_index/indices/common_tree/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 import asyncio
 import logging
 from typing import Dict, List, Optional, Sequence, Tuple
 
 from llama_index.async_utils import run_async_tasks
+from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.data_structs_v2 import IndexGraph
 from llama_index.data_structs.node_v2 import Node
 from llama_index.storage.docstore import BaseDocumentStore
 from llama_index.storage.docstore.registry import get_default_docstore
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.utils import get_sorted_node_list, truncate_text
 from llama_index.prompts.prompts import SummaryPrompt
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

### Comparing `llama_index-0.6.0a5/llama_index/indices/composability/graph.py` & `llama_index-0.6.0a6/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/empty/base.py` & `llama_index-0.6.0a6/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/empty/retrievers.py` & `llama_index-0.6.0a6/llama_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/keyword_table/__init__.py` & `llama_index-0.6.0a6/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/keyword_table/base.py` & `llama_index-0.6.0a6/llama_index/indices/keyword_table/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 from abc import abstractmethod
 from enum import Enum
 from typing import Any, Optional, Sequence, Set, Union
 
 from llama_index.async_utils import run_async_tasks
+from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.data_structs_v2 import KeywordTable
 from llama_index.data_structs.node_v2 import Node
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.keyword_table.utils import extract_keywords_given_response
 from llama_index.indices.service_context import ServiceContext
 from llama_index.prompts.default_prompts import (
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

### Comparing `llama_index-0.6.0a5/llama_index/indices/keyword_table/rake_base.py` & `llama_index-0.6.0a6/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/keyword_table/retrievers.py` & `llama_index-0.6.0a6/llama_index/indices/keyword_table/retrievers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Query for GPTKeywordTableIndex."""
 import logging
 from abc import abstractmethod
 from collections import defaultdict
 from typing import Any, Dict, List, Optional
 
+from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.node_v2 import NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.keyword_table.base import (
     BaseGPTKeywordTableIndex,
 )
 from llama_index.indices.keyword_table.utils import (
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

### Comparing `llama_index-0.6.0a5/llama_index/indices/keyword_table/simple_base.py` & `llama_index-0.6.0a6/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/keyword_table/utils.py` & `llama_index-0.6.0a6/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/knowledge_graph/base.py` & `llama_index-0.6.0a6/llama_index/indices/knowledge_graph/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 existing keywords in the table.
 
 """
 
 import logging
 from typing import Any, List, Optional, Sequence, Tuple
 
+from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.data_structs_v2 import KG
 from llama_index.data_structs.node_v2 import Node
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.prompts.default_prompts import (
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

### Comparing `llama_index-0.6.0a5/llama_index/indices/knowledge_graph/retrievers.py` & `llama_index-0.6.0a6/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Query for GPTKGTableIndex."""
 import logging
 from collections import defaultdict
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
+from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.node_v2 import Node, NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.keyword_table.utils import extract_keywords_given_response
 from llama_index.indices.knowledge_graph.base import GPTKnowledgeGraphIndex
 from llama_index.indices.query.embedding_utils import (
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

### Comparing `llama_index-0.6.0a5/llama_index/indices/list/base.py` & `llama_index-0.6.0a6/llama_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/list/retrievers.py` & `llama_index-0.6.0a6/llama_index/indices/list/retrievers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Default query for GPTListIndex."""
 import logging
 from typing import Any, List, Optional, Tuple
 
+from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.node_v2 import Node, NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.embedding_utils import (
     get_top_k_embeddings,
 )
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.list.base import GPTListIndex
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

### Comparing `llama_index-0.6.0a5/llama_index/indices/loading.py` & `llama_index-0.6.0a6/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/postprocessor/__init__.py` & `llama_index-0.6.0a6/llama_index/indices/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/postprocessor/node.py` & `llama_index-0.6.0a6/llama_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/postprocessor/node_recency.py` & `llama_index-0.6.0a6/llama_index/indices/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/postprocessor/pii.py` & `llama_index-0.6.0a6/llama_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/prompt_helper.py` & `llama_index-0.6.0a6/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/query/base.py` & `llama_index-0.6.0a6/llama_index/indices/query/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/query/embedding_utils.py` & `llama_index-0.6.0a6/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/query/query_transform/base.py` & `llama_index-0.6.0a6/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/query/query_transform/prompts.py` & `llama_index-0.6.0a6/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/query/response_synthesis.py` & `llama_index-0.6.0a6/llama_index/indices/query/response_synthesis.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/query/schema.py` & `llama_index-0.6.0a6/llama_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/registry.py` & `llama_index-0.6.0a6/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/response/response_builder.py` & `llama_index-0.6.0a6/llama_index/indices/response/response_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 2) create and refine separately over each chunk, 3) tree summarization.
 
 """
 from abc import ABC, abstractmethod
 import logging
 from typing import Any, Dict, Generator, List, Optional, Sequence, Tuple, cast
 
+from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.data_structs_v2 import IndexGraph
 from llama_index.data_structs.node_v2 import Node
 from llama_index.storage.docstore.registry import get_default_docstore
 from llama_index.indices.common_tree.base import GPTTreeIndexBuilder
 from llama_index.indices.response.type import ResponseMode
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.utils import get_sorted_node_list, truncate_text
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

### Comparing `llama_index-0.6.0a5/llama_index/indices/service_context.py` & `llama_index-0.6.0a6/llama_index/indices/service_context.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from typing import Optional
 
+from llama_index.callbacks.base import CallbackManager
 from llama_index.embeddings.base import BaseEmbedding
 from llama_index.embeddings.openai import OpenAIEmbedding
 from llama_index.indices.prompt_helper import PromptHelper
 from llama_index.langchain_helpers.chain_wrapper import LLMPredictor
 from llama_index.langchain_helpers.text_splitter import TokenTextSplitter
 from llama_index.logger import LlamaLogger
 from llama_index.node_parser.interface import NodeParser
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

### Comparing `llama_index-0.6.0a5/llama_index/indices/struct_store/__init__.py` & `llama_index-0.6.0a6/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/struct_store/base.py` & `llama_index-0.6.0a6/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/struct_store/container_builder.py` & `llama_index-0.6.0a6/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/struct_store/pandas.py` & `llama_index-0.6.0a6/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/struct_store/pandas_query.py` & `llama_index-0.6.0a6/llama_index/indices/struct_store/pandas_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 from typing import Any, Callable, Optional
 
 import pandas as pd
 from langchain.input import print_text
 
+from llama_index.callbacks.schema import CBEventType
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.struct_store.pandas import GPTPandasIndex
 from llama_index.prompts.default_prompts import DEFAULT_PANDAS_PROMPT
 from llama_index.prompts.prompts import PandasPrompt
 from llama_index.response.schema import Response
 
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

### Comparing `llama_index-0.6.0a5/llama_index/indices/struct_store/sql.py` & `llama_index-0.6.0a6/llama_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/struct_store/sql_query.py` & `llama_index-0.6.0a6/llama_index/indices/struct_store/sql_query.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Default query for GPTSQLStructStoreIndex."""
 import logging
 from typing import Any, Optional
 
+from llama_index.callbacks.schema import CBEventType
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.struct_store.container_builder import SQLContextContainerBuilder
 from llama_index.indices.struct_store.sql import GPTSQLStructStoreIndex
 from llama_index.prompts.default_prompts import DEFAULT_TEXT_TO_SQL_PROMPT
 from llama_index.prompts.prompts import TextToSQLPrompt
 from llama_index.response.schema import Response
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

### Comparing `llama_index-0.6.0a5/llama_index/indices/tree/__init__.py` & `llama_index-0.6.0a6/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/tree/all_leaf_retriever.py` & `llama_index-0.6.0a6/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/tree/base.py` & `llama_index-0.6.0a6/llama_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/tree/inserter.py` & `llama_index-0.6.0a6/llama_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `llama_index-0.6.0a6/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/tree/select_leaf_retriever.py` & `llama_index-0.6.0a6/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/tree/tree_root_retriever.py` & `llama_index-0.6.0a6/llama_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/utils.py` & `llama_index-0.6.0a6/llama_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/indices/vector_store/base.py` & `llama_index-0.6.0a6/llama_index/indices/vector_store/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 An index that that is built on top of an existing vector store.
 
 """
 
 from typing import Any, Dict, List, Optional, Sequence, Set, Tuple
 
+from llama_index.callbacks.schema import CBEventType
 from llama_index.async_utils import run_async_tasks
 from llama_index.data_structs.data_structs_v2 import IndexDict
 from llama_index.data_structs.node_v2 import ImageNode, IndexNode, Node
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.service_context import ServiceContext
 from llama_index.storage.storage_context import StorageContext
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

### Comparing `llama_index-0.6.0a5/llama_index/indices/vector_store/retrievers.py` & `llama_index-0.6.0a6/llama_index/indices/vector_store/retrievers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Base vector store index query."""
 
 
 from typing import Any, List, Optional
 from llama_index.constants import DEFAULT_SIMILARITY_TOP_K
 
+from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.data_structs_v2 import IndexDict
-
 from llama_index.data_structs.node_v2 import NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.utils import log_vector_store_query_result
 from llama_index.indices.vector_store.base import GPTVectorStoreIndex
 from llama_index.token_counter.token_counter import llm_token_counter
 from llama_index.vector_stores.types import (
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

### Comparing `llama_index-0.6.0a5/llama_index/langchain_helpers/agents/__init__.py` & `llama_index-0.6.0a6/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/langchain_helpers/agents/agents.py` & `llama_index-0.6.0a6/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/langchain_helpers/agents/toolkits.py` & `llama_index-0.6.0a6/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/langchain_helpers/agents/tools.py` & `llama_index-0.6.0a6/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/langchain_helpers/memory_wrapper.py` & `llama_index-0.6.0a6/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/langchain_helpers/sql_wrapper.py` & `llama_index-0.6.0a6/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/langchain_helpers/text_splitter.py` & `llama_index-0.6.0a6/llama_index/langchain_helpers/text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/llm_predictor/base.py` & `llama_index-0.6.0a6/llama_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/llm_predictor/chatgpt.py` & `llama_index-0.6.0a6/llama_index/llm_predictor/chatgpt.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/llm_predictor/stable_lm.py` & `llama_index-0.6.0a6/llama_index/llm_predictor/stable_lm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/llm_predictor/structured.py` & `llama_index-0.6.0a6/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/logger/base.py` & `llama_index-0.6.0a6/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/node_parser/interface.py` & `llama_index-0.6.0a6/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/node_parser/node_utils.py` & `llama_index-0.6.0a6/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/node_parser/simple.py` & `llama_index-0.6.0a6/llama_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/optimization/optimizer.py` & `llama_index-0.6.0a6/llama_index/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/output_parsers/base.py` & `llama_index-0.6.0a6/llama_index/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/output_parsers/guardrails.py` & `llama_index-0.6.0a6/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/output_parsers/langchain.py` & `llama_index-0.6.0a6/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/output_parsers/selection.py` & `llama_index-0.6.0a6/llama_index/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/playground/base.py` & `llama_index-0.6.0a6/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/prompts/base.py` & `llama_index-0.6.0a6/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/prompts/chat_prompts.py` & `llama_index-0.6.0a6/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/prompts/default_prompt_selectors.py` & `llama_index-0.6.0a6/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/prompts/default_prompts.py` & `llama_index-0.6.0a6/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/prompts/prompt_type.py` & `llama_index-0.6.0a6/llama_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/prompts/prompts.py` & `llama_index-0.6.0a6/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/query_engine/__init__.py` & `llama_index-0.6.0a6/llama_index/query_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/query_engine/graph_query_engine.py` & `llama_index-0.6.0a6/llama_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/query_engine/multistep_query_engine.py` & `llama_index-0.6.0a6/llama_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/query_engine/retriever_query_engine.py` & `llama_index-0.6.0a6/llama_index/query_engine/retriever_query_engine.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from typing import Any, Dict, List, Optional, Sequence
+
+from llama_index.callbacks.base import CallbackManager
+from llama_index.callbacks.schema import CBEventType
 from llama_index.data_structs.node_v2 import NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.postprocessor.node import BaseNodePostprocessor
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.query.response_synthesis import ResponseSynthesizer
 from llama_index.indices.response.type import ResponseMode
@@ -26,19 +29,21 @@
 
     """
 
     def __init__(
         self,
         retriever: BaseRetriever,
         response_synthesizer: Optional[ResponseSynthesizer] = None,
+        callback_manager: Optional[CallbackManager] = None,
     ) -> None:
         self._retriever = retriever
         self._response_synthesizer = (
             response_synthesizer or ResponseSynthesizer.from_args()
         )
+        self._callback_manager = callback_manager or CallbackManager([])
 
     @classmethod
     def from_args(
         cls,
         retriever: BaseRetriever,
         service_context: Optional[ServiceContext] = None,
         node_postprocessors: Optional[List[BaseNodePostprocessor]] = None,
@@ -84,17 +89,23 @@
             response_kwargs=response_kwargs,
             use_async=use_async,
             streaming=streaming,
             optimizer=optimizer,
             node_postprocessors=node_postprocessors,
             verbose=verbose,
         )
+
+        callback_manager = (
+            service_context.callback_manager if service_context else CallbackManager([])
+        )
+
         return cls(
             retriever=retriever,
             response_synthesizer=response_synthesizer,
+            callback_manager=callback_manager,
         )
 
     def retrieve(self, query_bundle: QueryBundle) -> List[NodeWithScore]:
         return self._retriever.retrieve(query_bundle)
 
     def synthesize(
         self,
@@ -118,20 +129,48 @@
             query_bundle=query_bundle,
             nodes=nodes,
             additional_source_nodes=additional_source_nodes,
         )
 
     def _query(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
         """Answer a query."""
+        query_id = self._callback_manager.on_event_start(CBEventType.QUERY)
+
+        retrieve_id = self._callback_manager.on_event_start(CBEventType.RETRIEVE)
         nodes = self._retriever.retrieve(query_bundle)
-        return self._response_synthesizer.synthesize(
+        self._callback_manager.on_event_end(
+            CBEventType.RETRIEVE, payload={"nodes": nodes}, event_id=retrieve_id
+        )
+
+        synth_id = self._callback_manager.on_event_start(CBEventType.SYNTHESIZE)
+        response = self._response_synthesizer.synthesize(
             query_bundle=query_bundle,
             nodes=nodes,
         )
+        self._callback_manager.on_event_end(
+            CBEventType.SYNTHESIZE, payload={"response": response}, event_id=synth_id
+        )
+
+        self._callback_manager.on_event_end(CBEventType.QUERY, event_id=query_id)
+        return response
 
     async def _aquery(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
         """Answer a query."""
+        query_id = self._callback_manager.on_event_start(CBEventType.QUERY)
+
+        retrieve_id = self._callback_manager.on_event_start(CBEventType.RETRIEVE)
         nodes = self._retriever.retrieve(query_bundle)
-        return await self._response_synthesizer.asynthesize(
+        self._callback_manager.on_event_end(
+            CBEventType.RETRIEVE, payload={"nodes": nodes}, event_id=retrieve_id
+        )
+
+        synth_id = self._callback_manager.on_event_start(CBEventType.SYNTHESIZE)
+        response = await self._response_synthesizer.asynthesize(
             query_bundle=query_bundle,
             nodes=nodes,
         )
+        self._callback_manager.on_event_end(
+            CBEventType.SYNTHESIZE, payload={"response": response}, event_id=synth_id
+        )
+
+        self._callback_manager.on_event_end(CBEventType.QUERY, event_id=query_id)
+        return response
```

### Comparing `llama_index-0.6.0a5/llama_index/query_engine/router_query_engine.py` & `llama_index-0.6.0a6/llama_index/query_engine/router_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/query_engine/transform_query_engine.py` & `llama_index-0.6.0a6/llama_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/__init__.py` & `llama_index-0.6.0a6/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/base.py` & `llama_index-0.6.0a6/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/chatgpt_plugin/base.py` & `llama_index-0.6.0a6/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/chroma.py` & `llama_index-0.6.0a6/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/database.py` & `llama_index-0.6.0a6/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/deeplake.py` & `llama_index-0.6.0a6/llama_index/readers/deeplake.py`

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

### Comparing `llama_index-0.6.0a5/llama_index/readers/discord_reader.py` & `llama_index-0.6.0a6/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/download.py` & `llama_index-0.6.0a6/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/elasticsearch.py` & `llama_index-0.6.0a6/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/faiss.py` & `llama_index-0.6.0a6/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/file/base.py` & `llama_index-0.6.0a6/llama_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/file/base_parser.py` & `llama_index-0.6.0a6/llama_index/readers/file/base_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/file/docs_parser.py` & `llama_index-0.6.0a6/llama_index/readers/file/docs_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/file/epub_parser.py` & `llama_index-0.6.0a6/llama_index/readers/file/epub_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/file/image_caption_parser.py` & `llama_index-0.6.0a6/llama_index/readers/file/image_caption_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/file/image_parser.py` & `llama_index-0.6.0a6/llama_index/readers/file/image_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/file/image_vision_llm_parser.py` & `llama_index-0.6.0a6/llama_index/readers/file/image_vision_llm_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/file/ipynb_parser.py` & `llama_index-0.6.0a6/llama_index/readers/file/ipynb_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/file/markdown_parser.py` & `llama_index-0.6.0a6/llama_index/readers/file/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/file/mbox_parser.py` & `llama_index-0.6.0a6/llama_index/readers/file/mbox_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/file/slides_parser.py` & `llama_index-0.6.0a6/llama_index/readers/file/slides_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/file/tabular_parser.py` & `llama_index-0.6.0a6/llama_index/readers/file/tabular_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/file/video_audio.py` & `llama_index-0.6.0a6/llama_index/readers/file/video_audio.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/github_readers/github_api_client.py` & `llama_index-0.6.0a6/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/github_readers/github_repository_reader.py` & `llama_index-0.6.0a6/llama_index/readers/github_readers/github_repository_reader.py`

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

### Comparing `llama_index-0.6.0a5/llama_index/readers/github_readers/utils.py` & `llama_index-0.6.0a6/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/google_readers/gdocs.py` & `llama_index-0.6.0a6/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/google_readers/gsheets.py` & `llama_index-0.6.0a6/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/json.py` & `llama_index-0.6.0a6/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/make_com/wrapper.py` & `llama_index-0.6.0a6/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/mbox.py` & `llama_index-0.6.0a6/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/milvus.py` & `llama_index-0.6.0a6/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/mongo.py` & `llama_index-0.6.0a6/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/myscale.py` & `llama_index-0.6.0a6/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/notion.py` & `llama_index-0.6.0a6/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/obsidian.py` & `llama_index-0.6.0a6/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/pinecone.py` & `llama_index-0.6.0a6/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/qdrant.py` & `llama_index-0.6.0a6/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/schema/base.py` & `llama_index-0.6.0a6/llama_index/readers/schema/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/slack.py` & `llama_index-0.6.0a6/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/steamship/file_reader.py` & `llama_index-0.6.0a6/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/string_iterable.py` & `llama_index-0.6.0a6/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/twitter.py` & `llama_index-0.6.0a6/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/weaviate/client.py` & `llama_index-0.6.0a6/llama_index/readers/weaviate/client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/weaviate/reader.py` & `llama_index-0.6.0a6/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/weaviate/utils.py` & `llama_index-0.6.0a6/llama_index/readers/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/web.py` & `llama_index-0.6.0a6/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/wikipedia.py` & `llama_index-0.6.0a6/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/readers/youtube_transcript.py` & `llama_index-0.6.0a6/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/response/notebook_utils.py` & `llama_index-0.6.0a6/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/response/schema.py` & `llama_index-0.6.0a6/llama_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/retrievers/__init__.py` & `llama_index-0.6.0a6/llama_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/retrievers/transform_retriever.py` & `llama_index-0.6.0a6/llama_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/schema.py` & `llama_index-0.6.0a6/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/selectors/llm_selectors.py` & `llama_index-0.6.0a6/llama_index/selectors/llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/selectors/prompts.py` & `llama_index-0.6.0a6/llama_index/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/selectors/types.py` & `llama_index-0.6.0a6/llama_index/selectors/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/docstore/__init__.py` & `llama_index-0.6.0a6/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/docstore/keyval_docstore.py` & `llama_index-0.6.0a6/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/docstore/mongo_docstore.py` & `llama_index-0.6.0a6/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/docstore/registry.py` & `llama_index-0.6.0a6/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/docstore/simple_docstore.py` & `llama_index-0.6.0a6/llama_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/docstore/types.py` & `llama_index-0.6.0a6/llama_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/docstore/utils.py` & `llama_index-0.6.0a6/llama_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/index_store/keyval_index_store.py` & `llama_index-0.6.0a6/llama_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/index_store/mongo_index_store.py` & `llama_index-0.6.0a6/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/index_store/simple_index_store.py` & `llama_index-0.6.0a6/llama_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/index_store/types.py` & `llama_index-0.6.0a6/llama_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/index_store/utils.py` & `llama_index-0.6.0a6/llama_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/kvstore/mongodb_kvstore.py` & `llama_index-0.6.0a6/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/kvstore/simple_kvstore.py` & `llama_index-0.6.0a6/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/kvstore/types.py` & `llama_index-0.6.0a6/llama_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/storage/storage_context.py` & `llama_index-0.6.0a6/llama_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/token_counter/mock_chain_wrapper.py` & `llama_index-0.6.0a6/llama_index/token_counter/mock_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/token_counter/mock_embed_model.py` & `llama_index-0.6.0a6/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/token_counter/token_counter.py` & `llama_index-0.6.0a6/llama_index/token_counter/token_counter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/token_counter/utils.py` & `llama_index-0.6.0a6/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/tools/query_engine.py` & `llama_index-0.6.0a6/llama_index/tools/query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/tts/bark.py` & `llama_index-0.6.0a6/llama_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/tts/base.py` & `llama_index-0.6.0a6/llama_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/tts/elevenlabs.py` & `llama_index-0.6.0a6/llama_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/utils.py` & `llama_index-0.6.0a6/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/vector_stores/__init__.py` & `llama_index-0.6.0a6/llama_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/vector_stores/chatgpt_plugin.py` & `llama_index-0.6.0a6/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/vector_stores/chroma.py` & `llama_index-0.6.0a6/llama_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/vector_stores/deeplake.py` & `llama_index-0.6.0a6/llama_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/vector_stores/faiss.py` & `llama_index-0.6.0a6/llama_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/vector_stores/milvus.py` & `llama_index-0.6.0a6/llama_index/vector_stores/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/vector_stores/myscale.py` & `llama_index-0.6.0a6/llama_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/vector_stores/opensearch.py` & `llama_index-0.6.0a6/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/vector_stores/pinecone.py` & `llama_index-0.6.0a6/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/vector_stores/qdrant.py` & `llama_index-0.6.0a6/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/vector_stores/registry.py` & `llama_index-0.6.0a6/llama_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/vector_stores/simple.py` & `llama_index-0.6.0a6/llama_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/vector_stores/types.py` & `llama_index-0.6.0a6/llama_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index/vector_stores/weaviate.py` & `llama_index-0.6.0a6/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a5/llama_index.egg-info/PKG-INFO` & `llama_index-0.6.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: llama-index
-Version: 0.6.0a5
+Name: llama_index
+Version: 0.6.0a6
 Summary: Interface between LLMs and your data.
 Home-page: https://github.com/jerryjliu/gpt_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `llama_index-0.6.0a5/llama_index.egg-info/SOURCES.txt` & `llama_index-0.6.0a6/llama_index.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 llama_index/types.py
 llama_index/utils.py
 llama_index.egg-info/PKG-INFO
 llama_index.egg-info/SOURCES.txt
 llama_index.egg-info/dependency_links.txt
 llama_index.egg-info/requires.txt
 llama_index.egg-info/top_level.txt
+llama_index/callbacks/__init__.py
+llama_index/callbacks/base.py
+llama_index/callbacks/llama_debug.py
+llama_index/callbacks/schema.py
 llama_index/composability/__init__.py
 llama_index/composability/base.py
 llama_index/composability/joint_qa_summary.py
 llama_index/data_structs/__init__.py
 llama_index/data_structs/data_structs.py
 llama_index/data_structs/data_structs_v2.py
 llama_index/data_structs/node_mapping.py
@@ -186,14 +190,15 @@
 llama_index/readers/github_readers/__init__.py
 llama_index/readers/github_readers/github_api_client.py
 llama_index/readers/github_readers/github_repository_reader.py
 llama_index/readers/github_readers/utils.py
 llama_index/readers/google_readers/__init__.py
 llama_index/readers/google_readers/gdocs.py
 llama_index/readers/google_readers/gsheets.py
+llama_index/readers/llamahub_modules/__init__.py
 llama_index/readers/make_com/__init__.py
 llama_index/readers/make_com/wrapper.py
 llama_index/readers/schema/__init__.py
 llama_index/readers/schema/base.py
 llama_index/readers/steamship/__init__.py
 llama_index/readers/steamship/file_reader.py
 llama_index/readers/weaviate/__init__.py
```

### Comparing `llama_index-0.6.0a5/setup.py` & `llama_index-0.6.0a6/setup.py`

 * *Files identical despite different names*

