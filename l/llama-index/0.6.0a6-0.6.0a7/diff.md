# Comparing `tmp/llama_index-0.6.0a6.tar.gz` & `tmp/llama_index-0.6.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index-0.6.0a6.tar", last modified: Tue May  2 07:46:53 2023, max compression
+gzip compressed data, was "llama_index-0.6.0a7.tar", last modified: Tue May  2 20:09:00 2023, max compression
```

## Comparing `llama_index-0.6.0a6.tar` & `llama_index-0.6.0a7.tar`

### file list

```diff
@@ -1,319 +1,445 @@
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.818520 llama_index-0.6.0a6/
--rw-r--r--   0 jerryliu   (501) staff       (20)     1064 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/LICENSE
--rw-r--r--   0 jerryliu   (501) staff       (20)       73 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/MANIFEST.in
--rw-r--r--   0 jerryliu   (501) staff       (20)     4354 2023-05-02 07:46:53.818386 llama_index-0.6.0a6/PKG-INFO
--rw-r--r--   0 jerryliu   (501) staff       (20)     4124 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/README.md
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.792635 llama_index-0.6.0a6/llama_index/
--rw-r--r--   0 jerryliu   (501) staff       (20)       13 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/VERSION
--rw-r--r--   0 jerryliu   (501) staff       (20)     4719 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      322 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/async_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.793628 llama_index-0.6.0a6/llama_index/callbacks/
--rw-r--r--   0 jerryliu   (501) staff       (20)      196 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/callbacks/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3068 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/callbacks/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5526 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/callbacks/llama_debug.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1073 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/callbacks/schema.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.794024 llama_index-0.6.0a6/llama_index/composability/
--rw-r--r--   0 jerryliu   (501) staff       (20)      220 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/composability/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      171 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/composability/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3091 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      219 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/constants.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.795142 llama_index-0.6.0a6/llama_index/data_structs/
--rw-r--r--   0 jerryliu   (501) staff       (20)      409 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    12377 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/data_structs.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     9476 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/data_structs_v2.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      264 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/node_mapping.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6221 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/node_v2.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      779 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/registry.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3256 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/struct_type.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      908 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/table.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1032 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/data_structs/table_v2.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.795707 llama_index-0.6.0a6/llama_index/embeddings/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/embeddings/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7721 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/embeddings/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1109 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/embeddings/langchain.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    10103 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/embeddings/openai.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      559 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/embeddings/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.796046 llama_index-0.6.0a6/llama_index/evaluation/
--rw-r--r--   0 jerryliu   (501) staff       (20)      259 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/evaluation/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11972 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/evaluation/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5344 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      544 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/img_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.797020 llama_index-0.6.0a6/llama_index/indices/
--rw-r--r--   0 jerryliu   (501) staff       (20)      542 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     9752 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      859 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/base_retriever.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.797130 llama_index-0.6.0a6/llama_index/indices/common/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.797579 llama_index-0.6.0a6/llama_index/indices/common/struct_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8474 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      776 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2676 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.797829 llama_index-0.6.0a6/llama_index/indices/common_tree/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7977 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.798049 llama_index-0.6.0a6/llama_index/indices/composability/
--rw-r--r--   0 jerryliu   (501) staff       (20)      180 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/composability/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3962 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/composability/graph.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.798365 llama_index-0.6.0a6/llama_index/indices/empty/
--rw-r--r--   0 jerryliu   (501) staff       (20)      198 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/empty/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2151 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/empty/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1176 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/empty/retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.798967 llama_index-0.6.0a6/llama_index/indices/keyword_table/
--rw-r--r--   0 jerryliu   (501) staff       (20)      656 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8545 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      650 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6487 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      844 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2264 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.799238 llama_index-0.6.0a6/llama_index/indices/knowledge_graph/
--rw-r--r--   0 jerryliu   (501) staff       (20)      254 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     9049 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    10431 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/knowledge_graph/retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.799512 llama_index-0.6.0a6/llama_index/indices/list/
--rw-r--r--   0 jerryliu   (501) staff       (20)      295 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/list/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3305 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/list/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4198 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/list/retrievers.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3608 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/loading.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.799958 llama_index-0.6.0a6/llama_index/indices/postprocessor/
--rw-r--r--   0 jerryliu   (501) staff       (20)      888 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)       83 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/postprocessor/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11695 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8778 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4896 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/postprocessor/pii.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8492 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.800416 llama_index-0.6.0a6/llama_index/indices/query/
--rw-r--r--   0 jerryliu   (501) staff       (20)      137 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1937 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3386 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.800680 llama_index-0.6.0a6/llama_index/indices/query/query_transform/
--rw-r--r--   0 jerryliu   (501) staff       (20)      281 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8904 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5920 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8098 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/response_synthesis.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1248 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/query/schema.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1811 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/registry.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.800975 llama_index-0.6.0a6/llama_index/indices/response/
--rw-r--r--   0 jerryliu   (501) staff       (20)      419 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/response/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    24774 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/response/response_builder.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      262 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/response/type.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3643 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/service_context.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.801598 llama_index-0.6.0a6/llama_index/indices/struct_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)      622 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2115 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/struct_store/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5765 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2214 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5409 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/struct_store/pandas_query.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6139 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7149 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.802219 llama_index-0.6.0a6/llama_index/indices/tree/
--rw-r--r--   0 jerryliu   (501) staff       (20)      616 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/tree/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1612 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5834 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/tree/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7181 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/tree/inserter.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4663 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    15299 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1402 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2005 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.802481 llama_index-0.6.0a6/llama_index/indices/vector_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)      260 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8914 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/vector_store/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4355 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/indices/vector_store/retrievers.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.802916 llama_index-0.6.0a6/llama_index/langchain_helpers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       39 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.803288 llama_index-0.6.0a6/llama_index/langchain_helpers/agents/
--rw-r--r--   0 jerryliu   (501) staff       (20)      514 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2994 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      837 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2211 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      252 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/chain_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7675 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3287 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    18172 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.803718 llama_index-0.6.0a6/llama_index/llm_predictor/
--rw-r--r--   0 jerryliu   (501) staff       (20)      330 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    10838 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/llm_predictor/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4282 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/llm_predictor/chatgpt.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4732 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/llm_predictor/stable_lm.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2274 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/llm_predictor/structured.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.803890 llama_index-0.6.0a6/llama_index/logger/
--rw-r--r--   0 jerryliu   (501) staff       (20)       95 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/logger/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      995 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/logger/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.804242 llama_index-0.6.0a6/llama_index/node_parser/
--rw-r--r--   0 jerryliu   (501) staff       (20)      184 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/node_parser/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      530 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/node_parser/interface.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3585 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/node_parser/node_utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1821 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/node_parser/simple.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.804417 llama_index-0.6.0a6/llama_index/optimization/
--rw-r--r--   0 jerryliu   (501) staff       (20)      144 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/optimization/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4301 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/optimization/optimizer.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.804852 llama_index-0.6.0a6/llama_index/output_parsers/
--rw-r--r--   0 jerryliu   (501) staff       (20)      230 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/output_parsers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      611 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/output_parsers/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2742 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1828 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/output_parsers/langchain.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1345 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/output_parsers/selection.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.805019 llama_index-0.6.0a6/llama_index/playground/
--rw-r--r--   0 jerryliu   (501) staff       (20)      202 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/playground/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6471 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/playground/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.805630 llama_index-0.6.0a6/llama_index/prompts/
--rw-r--r--   0 jerryliu   (501) staff       (20)       87 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/prompts/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6633 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/prompts/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1969 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1134 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    10843 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/prompts/default_prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1120 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/prompts/prompt_type.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7685 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/prompts/prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/py.typed
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.806167 llama_index-0.6.0a6/llama_index/query_engine/
--rw-r--r--   0 jerryliu   (501) staff       (20)      560 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/query_engine/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3572 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5814 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6999 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2449 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/query_engine/router_query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2967 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.808870 llama_index-0.6.0a6/llama_index/readers/
--rw-r--r--   0 jerryliu   (501) staff       (20)     2974 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      659 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/base.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.809124 llama_index-0.6.0a6/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 jerryliu   (501) staff       (20)      145 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2111 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3755 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/chroma.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3308 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/database.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3456 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/deeplake.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4981 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/discord_reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7775 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/download.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2392 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/elasticsearch.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2510 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/faiss.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.810894 llama_index-0.6.0a6/llama_index/readers/file/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8535 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1342 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/base_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1629 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/docs_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1318 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/epub_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3180 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/image_caption_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4106 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/image_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3222 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/image_vision_llm_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1027 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/ipynb_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3616 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/markdown_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3162 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/mbox_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3945 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/slides_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3357 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/tabular_parser.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1770 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/file/video_audio.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.811387 llama_index-0.6.0a6/llama_index/readers/github_readers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11730 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    15929 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5473 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.811742 llama_index-0.6.0a6/llama_index/readers/google_readers/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5659 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4989 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3708 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/json.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.811884 llama_index-0.6.0a6/llama_index/readers/llamahub_modules/
--rw-r--r--   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/llamahub_modules/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.812086 llama_index-0.6.0a6/llama_index/readers/make_com/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1696 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1261 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/mbox.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4588 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/milvus.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2608 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/mongo.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5541 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/myscale.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5679 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/notion.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1601 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/obsidian.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2766 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/pinecone.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3909 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/qdrant.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.812317 llama_index-0.6.0a6/llama_index/readers/schema/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/schema/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1214 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/schema/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7892 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/slack.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.812543 llama_index-0.6.0a6/llama_index/readers/steamship/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3498 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1042 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/string_iterable.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1918 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/twitter.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.812898 llama_index-0.6.0a6/llama_index/readers/weaviate/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7766 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/weaviate/client.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3986 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1867 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/weaviate/utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7987 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/web.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      981 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/wikipedia.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1255 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.813256 llama_index-0.6.0a6/llama_index/response/
--rw-r--r--   0 jerryliu   (501) staff       (20)       19 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/response/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2039 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/response/notebook_utils.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3071 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/response/schema.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      262 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/response/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.813444 llama_index-0.6.0a6/llama_index/retrievers/
--rw-r--r--   0 jerryliu   (501) staff       (20)     1258 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/retrievers/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1066 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2768 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/schema.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.813814 llama_index-0.6.0a6/llama_index/selectors/
--rw-r--r--   0 jerryliu   (501) staff       (20)      259 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/selectors/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7055 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/selectors/llm_selectors.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2438 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/selectors/prompts.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2006 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/selectors/types.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.813996 llama_index-0.6.0a6/llama_index/storage/
--rw-r--r--   0 jerryliu   (501) staff       (20)      124 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/__init__.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.814669 llama_index-0.6.0a6/llama_index/storage/docstore/
--rw-r--r--   0 jerryliu   (501) staff       (20)      536 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/docstore/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4825 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1408 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      762 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/docstore/registry.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2294 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2532 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/docstore/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      918 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/docstore/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.815234 llama_index-0.6.0a6/llama_index/storage/index_store/
--rw-r--r--   0 jerryliu   (501) staff       (20)      301 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/index_store/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2224 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1341 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1508 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      884 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/index_store/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      644 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/index_store/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.815650 llama_index-0.6.0a6/llama_index/storage/kvstore/
--rw-r--r--   0 jerryliu   (501) staff       (20)      187 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4061 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2330 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      973 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/kvstore/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3114 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/storage/storage_context.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.816139 llama_index-0.6.0a6/llama_index/token_counter/
--rw-r--r--   0 jerryliu   (501) staff       (20)       17 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/token_counter/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4664 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/token_counter/mock_chain_wrapper.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      722 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2874 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/token_counter/token_counter.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      908 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/token_counter/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.816457 llama_index-0.6.0a6/llama_index/tools/
--rw-r--r--   0 jerryliu   (501) staff       (20)      162 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/tools/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1557 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/tools/query_engine.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      366 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/tools/types.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.816875 llama_index-0.6.0a6/llama_index/tts/
--rw-r--r--   0 jerryliu   (501) staff       (20)      154 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/tts/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2589 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/tts/bark.py
--rw-r--r--   0 jerryliu   (501) staff       (20)      631 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/tts/base.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1282 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/tts/elevenlabs.py
--rw-r--r--   0 jerryliu   (501) staff       (20)       81 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5847 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/utils.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.818227 llama_index-0.6.0a6/llama_index/vector_stores/
--rw-r--r--   0 jerryliu   (501) staff       (20)     1132 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/__init__.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5240 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3947 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/chroma.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8631 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/deeplake.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     4365 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/faiss.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    15768 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/milvus.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     8344 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/myscale.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     7186 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 jerryliu   (501) staff       (20)    11419 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     6505 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     1973 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/registry.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     5084 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/simple.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     2210 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/types.py
--rw-r--r--   0 jerryliu   (501) staff       (20)     3385 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index/vector_stores/weaviate.py
-drwxr-xr-x   0 jerryliu   (501) staff       (20)        0 2023-05-02 07:46:53.793183 llama_index-0.6.0a6/llama_index.egg-info/
--rw-r--r--   0 jerryliu   (501) staff       (20)     4354 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index.egg-info/PKG-INFO
--rw-r--r--   0 jerryliu   (501) staff       (20)    10097 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index.egg-info/SOURCES.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)        1 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index.egg-info/dependency_links.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)       96 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index.egg-info/requires.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)       12 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/llama_index.egg-info/top_level.txt
--rw-r--r--   0 jerryliu   (501) staff       (20)       38 2023-05-02 07:46:53.818557 llama_index-0.6.0a6/setup.cfg
--rw-r--r--   0 jerryliu   (501) staff       (20)     1130 2023-05-02 07:46:53.000000 llama_index-0.6.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-02 20:08:43.000000 llama_index-0.6.0a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 20:08:43.000000 llama_index-0.6.0a7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-02 20:08:43.000000 llama_index-0.6.0a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.609001 llama_index-0.6.0a7/llama_index/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.609001 llama_index-0.6.0a7/llama_index/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/callbacks/llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/callbacks/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.609001 llama_index-0.6.0a7/llama_index/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/composability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.609001 llama_index-0.6.0a7/llama_index/data_structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/data_structs_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/node_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/table_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/embeddings/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/embeddings/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/embeddings/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/embeddings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/evaluation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/img_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/indices/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/indices/common/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/indices/common_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/empty/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.617001 llama_index-0.6.0a7/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/knowledge_graph/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.617001 llama_index-0.6.0a7/llama_index/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.617001 llama_index-0.6.0a7/llama_index/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/postprocessor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.617001 llama_index-0.6.0a7/llama_index/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.617001 llama_index-0.6.0a7/llama_index/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/response_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.617001 llama_index-0.6.0a7/llama_index/indices/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24774 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/response/response_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/response/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/service_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.617001 llama_index-0.6.0a7/llama_index/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/struct_store/pandas_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/tree/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/vector_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/vector_store/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/llm_predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/llm_predictor/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/llm_predictor/stable_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/llm_predictor/structured.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/logger/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/node_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/node_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/node_parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/node_parser/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/optimization/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/output_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/output_parsers/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/output_parsers/selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/playground/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.625001 llama_index-0.6.0a7/llama_index/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.625001 llama_index-0.6.0a7/llama_index/query_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/query_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/query_engine/router_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.625001 llama_index-0.6.0a7/llama_index/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/discord_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/faiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/docs_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/epub_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/image_caption_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/image_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/image_vision_llm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/ipynb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/mbox_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/slides_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/tabular_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/video_audio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/github_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/google_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/make_com/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/mbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/string_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/twitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/weaviate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/weaviate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/response/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/response/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/selectors/llm_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/selectors/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/selectors/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/docstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/storage/index_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/index_store/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/storage/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/storage_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/token_counter/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/token_counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/token_counter/mock_chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/token_counter/token_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/token_counter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/tools/query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/tools/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.637001 llama_index-0.6.0a7/llama_index/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/tts/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/tts/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.637001 llama_index-0.6.0a7/llama_index/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15768 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.609001 llama_index-0.6.0a7/llama_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-02 20:09:00.000000 llama_index-0.6.0a7/llama_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-05-02 20:09:00.000000 llama_index-0.6.0a7/llama_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:09:00.000000 llama_index-0.6.0a7/llama_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 20:09:00.000000 llama_index-0.6.0a7/llama_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 20:09:00.000000 llama_index-0.6.0a7/llama_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.637001 llama_index-0.6.0a7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.637001 llama_index-0.6.0a7/tests/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/callbacks/test_llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.637001 llama_index-0.6.0a7/tests/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/embeddings/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.637001 llama_index-0.6.0a7/tests/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.637001 llama_index-0.6.0a7/tests/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/composability/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/empty/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/keyword_table/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/keyword_table/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/keyword_table/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/knowledge_graph/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/knowledge_graph/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/knowledge_graph/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/list/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/list/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13923 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/postprocessor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/query_transform/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/query_transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/test_compose_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/test_query_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/struct_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/struct_store/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/struct_store/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/struct_store/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/test_loading_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/test_node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/test_prompt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/tree/test_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/tree/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/tree/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/mock_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/mock_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/test_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/test_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/test_myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/test_pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/test_weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/langchain_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/langchain_helpers/test_text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/llm_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/logger/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/mock_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/mock_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/mock_utils/mock_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/mock_utils/mock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/mock_utils/mock_text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/mock_utils/mock_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/optimization/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/output_parsers/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/output_parsers/test_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/playground/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/prompts/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/readers/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/readers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/readers/test_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/readers/test_string_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/tests/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/selectors/test_llm_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/storage/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/tests/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/storage/docstore/test_mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/storage/docstore/test_simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/tests/token_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/token_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/token_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/tests/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/vector_stores/test_qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/vector_stores/test_weaviate.py
```

### Comparing `llama_index-0.6.0a6/LICENSE` & `llama_index-0.6.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/PKG-INFO` & `llama_index-0.6.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: llama_index
-Version: 0.6.0a6
-Summary: Interface between LLMs and your data.
-Home-page: https://github.com/jerryjliu/gpt_index
+Version: 0.6.0a7
+Summary: Interface between LLMs and your data
+Home-page: https://github.com/jerryjliu/llama_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
 
 LlamaIndex (GPT Index) is a project that provides a central interface to connect your LLM's with external data.
```

### Comparing `llama_index-0.6.0a6/README.md` & `llama_index-0.6.0a7/README.md`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/__init__.py` & `llama_index-0.6.0a7/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/callbacks/base.py` & `llama_index-0.6.0a7/llama_index/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/callbacks/llama_debug.py` & `llama_index-0.6.0a7/llama_index/callbacks/llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/callbacks/schema.py` & `llama_index-0.6.0a7/llama_index/callbacks/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/composability/joint_qa_summary.py` & `llama_index-0.6.0a7/llama_index/composability/joint_qa_summary.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """Joint QA Summary graph."""
 
 
 from typing import Sequence, Optional
-from llama_index.storage.docstore.registry import get_default_docstore
 
 from llama_index.callbacks.schema import CBEventType
 from llama_index.indices.service_context import ServiceContext
-from llama_index.composability import ComposableGraph
 from llama_index.indices.list.base import GPTListIndex
-from llama_index.indices.tree.base import GPTTreeIndex
 from llama_index.indices.vector_store import GPTVectorStoreIndex
 from llama_index.readers.schema.base import Document
-from llama_index.storage.docstore import BaseDocumentStore
+from llama_index.selectors.llm_selectors import LLMSingleSelector
+from llama_index.storage.storage_context import StorageContext
+
+from llama_index.query_engine.router_query_engine import RouterQueryEngine
+from llama_index.tools.query_engine import QueryEngineTool
 
 DEFAULT_SUMMARY_TEXT = "Use this index for summarization queries"
 DEFAULT_QA_TEXT = (
     "Use this index for queries that require retrieval of specific "
     "context from documents."
 )
 
 
-class QASummaryGraphBuilder:
+class QASummaryQueryEngineBuilder:
     """Joint QA Summary graph builder.
 
     Can build a graph that provides a unified query interface
     for both QA and summarization tasks.
 
     NOTE: this is a beta feature. The API may change in the future.
 
@@ -36,50 +37,69 @@
         qa_text (str): Text to use for the QA index.
         node_parser (NodeParser): A NodeParser to use for parsing.
 
     """
 
     def __init__(
         self,
-        docstore: Optional[BaseDocumentStore] = None,
+        storage_context: Optional[StorageContext] = None,
         service_context: Optional[ServiceContext] = None,
         summary_text: str = DEFAULT_SUMMARY_TEXT,
         qa_text: str = DEFAULT_QA_TEXT,
     ) -> None:
         """Init params."""
-        self._docstore = docstore or get_default_docstore()
+        self._storage_context = storage_context or StorageContext.from_defaults()
         self._service_context = service_context or ServiceContext.from_defaults()
         self._summary_text = summary_text
         self._qa_text = qa_text
 
-    def build_graph_from_documents(
+    def build_from_documents(
         self,
         documents: Sequence[Document],
-    ) -> "ComposableGraph":
-        """Build graph from index."""
+    ) -> RouterQueryEngine:
+        """Build query engine."""
+
+        # parse nodes
         event_id = self._service_context.callback_manager.on_event_start(
             CBEventType.CHUNKING, payload={"documents": documents}
         )
         nodes = self._service_context.node_parser.get_nodes_from_documents(documents)
         self._service_context.callback_manager.on_event_end(
             CBEventType.CHUNKING, payload={"nodes": nodes}, event_id=event_id
         )
-        self._docstore.add_documents(nodes, allow_update=True)
 
-        # used for QA
+        # ingest nodes
+        self._storage_context.docstore.add_documents(nodes, allow_update=True)
+
+        # build indices
         vector_index = GPTVectorStoreIndex(
             nodes,
             service_context=self._service_context,
+            storage_context=self._storage_context,
+        )
+        list_index = GPTListIndex(
+            nodes,
+            service_context=self._service_context,
+            storage_context=self._storage_context,
         )
-        # used for summarization
-        list_index = GPTListIndex(nodes, service_context=self._service_context)
-
-        vector_index.index_struct.summary = self._qa_text
-        list_index.index_struct.summary = self._summary_text
 
-        graph = ComposableGraph.from_indices(
-            GPTTreeIndex,
-            [vector_index, list_index],
+        vector_query_engine = vector_index.as_query_engine(
+            service_context=self._service_context
+        )
+        list_query_engine = list_index.as_query_engine(
             service_context=self._service_context,
+            response_mode="tree_summarize",
         )
 
-        return graph
+        # build query engine
+        query_engine = RouterQueryEngine(
+            selector=LLMSingleSelector.from_defaults(self._service_context),
+            query_engine_tools=[
+                QueryEngineTool.from_defaults(
+                    vector_query_engine, description=self._qa_text
+                ),
+                QueryEngineTool.from_defaults(
+                    list_query_engine, description=self._summary_text
+                ),
+            ],
+        )
+        return query_engine
```

### Comparing `llama_index-0.6.0a6/llama_index/data_structs/data_structs.py` & `llama_index-0.6.0a7/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/data_structs/data_structs_v2.py` & `llama_index-0.6.0a7/llama_index/data_structs/data_structs_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/data_structs/node_v2.py` & `llama_index-0.6.0a7/llama_index/data_structs/node_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/data_structs/registry.py` & `llama_index-0.6.0a7/llama_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/data_structs/struct_type.py` & `llama_index-0.6.0a7/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/data_structs/table.py` & `llama_index-0.6.0a7/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/data_structs/table_v2.py` & `llama_index-0.6.0a7/llama_index/data_structs/table_v2.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/embeddings/base.py` & `llama_index-0.6.0a7/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/embeddings/langchain.py` & `llama_index-0.6.0a7/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/embeddings/openai.py` & `llama_index-0.6.0a7/llama_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/embeddings/utils.py` & `llama_index-0.6.0a7/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/evaluation/base.py` & `llama_index-0.6.0a7/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/evaluation/dataset_generation.py` & `llama_index-0.6.0a7/llama_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/img_utils.py` & `llama_index-0.6.0a7/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/__init__.py` & `llama_index-0.6.0a7/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/base.py` & `llama_index-0.6.0a7/llama_index/indices/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/base_retriever.py` & `llama_index-0.6.0a7/llama_index/indices/base_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/common/struct_store/base.py` & `llama_index-0.6.0a7/llama_index/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/common/struct_store/schema.py` & `llama_index-0.6.0a7/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/common/struct_store/sql.py` & `llama_index-0.6.0a7/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/common_tree/base.py` & `llama_index-0.6.0a7/llama_index/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/composability/graph.py` & `llama_index-0.6.0a7/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/empty/base.py` & `llama_index-0.6.0a7/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/empty/retrievers.py` & `llama_index-0.6.0a7/llama_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/keyword_table/__init__.py` & `llama_index-0.6.0a7/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/keyword_table/base.py` & `llama_index-0.6.0a7/llama_index/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/keyword_table/rake_base.py` & `llama_index-0.6.0a7/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/keyword_table/retrievers.py` & `llama_index-0.6.0a7/llama_index/indices/keyword_table/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/keyword_table/simple_base.py` & `llama_index-0.6.0a7/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/keyword_table/utils.py` & `llama_index-0.6.0a7/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/knowledge_graph/base.py` & `llama_index-0.6.0a7/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/knowledge_graph/retrievers.py` & `llama_index-0.6.0a7/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/list/base.py` & `llama_index-0.6.0a7/llama_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/list/retrievers.py` & `llama_index-0.6.0a7/llama_index/indices/list/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/loading.py` & `llama_index-0.6.0a7/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/postprocessor/__init__.py` & `llama_index-0.6.0a7/llama_index/indices/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/postprocessor/node.py` & `llama_index-0.6.0a7/llama_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/postprocessor/node_recency.py` & `llama_index-0.6.0a7/llama_index/indices/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/postprocessor/pii.py` & `llama_index-0.6.0a7/llama_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/prompt_helper.py` & `llama_index-0.6.0a7/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/query/base.py` & `llama_index-0.6.0a7/llama_index/indices/query/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/query/embedding_utils.py` & `llama_index-0.6.0a7/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/query/query_transform/base.py` & `llama_index-0.6.0a7/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/query/query_transform/prompts.py` & `llama_index-0.6.0a7/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/query/response_synthesis.py` & `llama_index-0.6.0a7/llama_index/indices/query/response_synthesis.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/query/schema.py` & `llama_index-0.6.0a7/llama_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/registry.py` & `llama_index-0.6.0a7/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/response/response_builder.py` & `llama_index-0.6.0a7/llama_index/indices/response/response_builder.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/service_context.py` & `llama_index-0.6.0a7/llama_index/indices/service_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/struct_store/__init__.py` & `llama_index-0.6.0a7/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/struct_store/base.py` & `llama_index-0.6.0a7/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/struct_store/container_builder.py` & `llama_index-0.6.0a7/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/struct_store/pandas.py` & `llama_index-0.6.0a7/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/struct_store/pandas_query.py` & `llama_index-0.6.0a7/llama_index/indices/struct_store/pandas_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/struct_store/sql.py` & `llama_index-0.6.0a7/llama_index/indices/struct_store/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from llama_index.data_structs.table_v2 import SQLStructTable
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.common.struct_store.schema import SQLContextContainer
 from llama_index.indices.common.struct_store.sql import SQLStructDatapointExtractor
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.struct_store.base import BaseGPTStructStoreIndex
-from llama_index.indices.struct_store.container_builder import SQLContextContainerBuilder
+from llama_index.indices.struct_store.container_builder import (
+    SQLContextContainerBuilder,
+)
 from llama_index.langchain_helpers.sql_wrapper import SQLDatabase
 from sqlalchemy import Table
 
 
 class SQLQueryMode(str, Enum):
     SQL = "sql"
     NL = "nl"
```

### Comparing `llama_index-0.6.0a6/llama_index/indices/struct_store/sql_query.py` & `llama_index-0.6.0a7/llama_index/indices/struct_store/sql_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Default query for GPTSQLStructStoreIndex."""
 import logging
 from typing import Any, Optional
 
 from llama_index.callbacks.schema import CBEventType
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.query.schema import QueryBundle
-from llama_index.indices.struct_store.container_builder import SQLContextContainerBuilder
+from llama_index.indices.struct_store.container_builder import (
+    SQLContextContainerBuilder,
+)
 from llama_index.indices.struct_store.sql import GPTSQLStructStoreIndex
 from llama_index.prompts.default_prompts import DEFAULT_TEXT_TO_SQL_PROMPT
 from llama_index.prompts.prompts import TextToSQLPrompt
 from llama_index.response.schema import Response
 from llama_index.token_counter.token_counter import llm_token_counter
 
 logger = logging.getLogger(__name__)
```

### Comparing `llama_index-0.6.0a6/llama_index/indices/tree/__init__.py` & `llama_index-0.6.0a7/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/tree/all_leaf_retriever.py` & `llama_index-0.6.0a7/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/tree/base.py` & `llama_index-0.6.0a7/llama_index/indices/tree/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,17 @@
         retriever_mode: Union[str, TreeRetrieverMode] = TreeRetrieverMode.SELECT_LEAF,
         **kwargs: Any,
     ) -> BaseRetriever:
         # NOTE: lazy import
         from llama_index.indices.tree.select_leaf_embedding_retriever import (
             TreeSelectLeafEmbeddingRetriever,
         )
-        from llama_index.indices.tree.select_leaf_retriever import TreeSelectLeafRetriever
+        from llama_index.indices.tree.select_leaf_retriever import (
+            TreeSelectLeafRetriever,
+        )
         from llama_index.indices.tree.all_leaf_retriever import TreeAllLeafRetriever
         from llama_index.indices.tree.tree_root_retriever import TreeRootRetriever
 
         self._validate_build_tree_required(TreeRetrieverMode(retriever_mode))
 
         if retriever_mode == TreeRetrieverMode.SELECT_LEAF:
             return TreeSelectLeafRetriever(self, **kwargs)
```

### Comparing `llama_index-0.6.0a6/llama_index/indices/tree/inserter.py` & `llama_index-0.6.0a7/llama_index/indices/tree/inserter.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from typing import Optional, Sequence
 
 from llama_index.data_structs.data_structs_v2 import IndexGraph
 from llama_index.data_structs.node_v2 import Node
 from llama_index.storage.docstore import BaseDocumentStore
 from llama_index.storage.docstore.registry import get_default_docstore
 from llama_index.indices.service_context import ServiceContext
-from llama_index.indices.utils import extract_numbers_given_response, get_sorted_node_list
+from llama_index.indices.utils import (
+    extract_numbers_given_response,
+    get_sorted_node_list,
+)
 from llama_index.prompts.base import Prompt
 from llama_index.prompts.default_prompts import (
     DEFAULT_INSERT_PROMPT,
     DEFAULT_SUMMARY_PROMPT,
 )
```

### Comparing `llama_index-0.6.0a6/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `llama_index-0.6.0a7/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/tree/select_leaf_retriever.py` & `llama_index-0.6.0a7/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 from langchain.input import print_text
 
 from llama_index.data_structs.node_v2 import Node, NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.response.response_builder import get_response_builder
 from llama_index.indices.tree.base import GPTTreeIndex
-from llama_index.indices.utils import extract_numbers_given_response, get_sorted_node_list
+from llama_index.indices.utils import (
+    extract_numbers_given_response,
+    get_sorted_node_list,
+)
 from llama_index.prompts.default_prompt_selectors import DEFAULT_REFINE_PROMPT_SEL
 from llama_index.prompts.default_prompts import (
     DEFAULT_QUERY_PROMPT,
     DEFAULT_QUERY_PROMPT_MULTIPLE,
     DEFAULT_TEXT_QA_PROMPT,
 )
 from llama_index.prompts.prompts import (
```

### Comparing `llama_index-0.6.0a6/llama_index/indices/tree/tree_root_retriever.py` & `llama_index-0.6.0a7/llama_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/utils.py` & `llama_index-0.6.0a7/llama_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/vector_store/base.py` & `llama_index-0.6.0a7/llama_index/indices/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/indices/vector_store/retrievers.py` & `llama_index-0.6.0a7/llama_index/indices/vector_store/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/langchain_helpers/agents/__init__.py` & `llama_index-0.6.0a7/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/langchain_helpers/agents/agents.py` & `llama_index-0.6.0a7/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/langchain_helpers/agents/toolkits.py` & `llama_index-0.6.0a7/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/langchain_helpers/agents/tools.py` & `llama_index-0.6.0a7/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/langchain_helpers/memory_wrapper.py` & `llama_index-0.6.0a7/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/langchain_helpers/sql_wrapper.py` & `llama_index-0.6.0a7/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/langchain_helpers/text_splitter.py` & `llama_index-0.6.0a7/llama_index/langchain_helpers/text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/llm_predictor/base.py` & `llama_index-0.6.0a7/llama_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/llm_predictor/chatgpt.py` & `llama_index-0.6.0a7/llama_index/llm_predictor/chatgpt.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/llm_predictor/stable_lm.py` & `llama_index-0.6.0a7/llama_index/llm_predictor/stable_lm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/llm_predictor/structured.py` & `llama_index-0.6.0a7/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/logger/base.py` & `llama_index-0.6.0a7/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/node_parser/interface.py` & `llama_index-0.6.0a7/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/node_parser/node_utils.py` & `llama_index-0.6.0a7/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/node_parser/simple.py` & `llama_index-0.6.0a7/llama_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/optimization/optimizer.py` & `llama_index-0.6.0a7/llama_index/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/output_parsers/base.py` & `llama_index-0.6.0a7/llama_index/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/output_parsers/guardrails.py` & `llama_index-0.6.0a7/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/output_parsers/langchain.py` & `llama_index-0.6.0a7/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/output_parsers/selection.py` & `llama_index-0.6.0a7/llama_index/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/playground/base.py` & `llama_index-0.6.0a7/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/prompts/base.py` & `llama_index-0.6.0a7/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/prompts/chat_prompts.py` & `llama_index-0.6.0a7/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/prompts/default_prompt_selectors.py` & `llama_index-0.6.0a7/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/prompts/default_prompts.py` & `llama_index-0.6.0a7/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/prompts/prompt_type.py` & `llama_index-0.6.0a7/llama_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/prompts/prompts.py` & `llama_index-0.6.0a7/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/query_engine/__init__.py` & `llama_index-0.6.0a7/llama_index/query_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/query_engine/graph_query_engine.py` & `llama_index-0.6.0a7/llama_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/query_engine/multistep_query_engine.py` & `llama_index-0.6.0a7/llama_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/query_engine/retriever_query_engine.py` & `llama_index-0.6.0a7/llama_index/query_engine/retriever_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/query_engine/router_query_engine.py` & `llama_index-0.6.0a7/llama_index/query_engine/router_query_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,22 +42,22 @@
         selector = selector or LLMSingleSelector.from_defaults()
         return cls(selector, query_engine_tools)
 
     def _query(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
         result = self._selector.select(self._metadatas, query_bundle)
         try:
             selected_query_engine = self._query_engines[result.ind]
-            logger.info(f"Selecting query engine {result.ind}.")
+            logger.info(f"Selecting query engine {result.ind}: {result.reason}.")
         except ValueError as e:
             raise ValueError("Failed to select query engine") from e
 
         return selected_query_engine.query(query_bundle)
 
     async def _aquery(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
         result = await self._selector.aselect(self._metadatas, query_bundle)
         try:
             selected_query_engine = self._query_engines[result.ind]
-            logger.info(f"Selecting query engine {result.ind}.")
+            logger.info(f"Selecting query engine {result.ind}: {result.reason}.")
         except ValueError as e:
             raise ValueError("Failed to select query engine") from e
 
         return await selected_query_engine.aquery(query_bundle)
```

### Comparing `llama_index-0.6.0a6/llama_index/query_engine/transform_query_engine.py` & `llama_index-0.6.0a7/llama_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/__init__.py` & `llama_index-0.6.0a7/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/base.py` & `llama_index-0.6.0a7/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/chatgpt_plugin/base.py` & `llama_index-0.6.0a7/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/chroma.py` & `llama_index-0.6.0a7/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/database.py` & `llama_index-0.6.0a7/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/deeplake.py` & `llama_index-0.6.0a7/llama_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/discord_reader.py` & `llama_index-0.6.0a7/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/download.py` & `llama_index-0.6.0a7/llama_index/readers/download.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,25 +79,25 @@
         f.write(f"__all__ = {list(set(exports))}" + os.linesep)
 
 
 def download_loader(
     loader_class: str,
     loader_hub_url: str = LOADER_HUB_URL,
     refresh_cache: Optional[bool] = False,
-    use_llama_index_import: bool = False,
+    use_gpt_index_import: bool = False,
     custom_path: Optional[str] = None,
 ) -> Type[BaseReader]:
     """Download a single loader from the Loader Hub.
 
     Args:
         loader_class: The name of the loader class you want to download,
             such as `SimpleWebPageReader`.
         refresh_cache: If true, the local cache will be skipped and the
             loader will be fetched directly from the remote repo.
-        use_llama_index_import: If true, the loader files will use
+        use_gpt_index_import: If true, the loader files will use
             llama_index as the base dependency. By default (False),
             the loader files use llama_index as the base dependency.
             NOTE: this is a temporary workaround while we fully migrate all usages
             to llama_index.
         custom_path: Custom dirpath to download loader into.
 
     Returns:
@@ -147,15 +147,15 @@
     requirements_path = f"{loader_path}/requirements.txt"
 
     if refresh_cache or not os.path.exists(loader_path):
         os.makedirs(loader_path, exist_ok=True)
         basepy_raw_content, _ = _get_file_content(
             loader_hub_url, f"/{loader_id}/base.py"
         )
-        if use_llama_index_import:
+        if use_gpt_index_import:
             basepy_raw_content = basepy_raw_content.replace(
                 "import llama_index", "import llama_index"
             )
             basepy_raw_content = basepy_raw_content.replace(
                 "from llama_index", "from llama_index"
             )
```

### Comparing `llama_index-0.6.0a6/llama_index/readers/elasticsearch.py` & `llama_index-0.6.0a7/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/faiss.py` & `llama_index-0.6.0a7/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/file/base.py` & `llama_index-0.6.0a7/llama_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/file/base_parser.py` & `llama_index-0.6.0a7/llama_index/readers/file/base_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/file/docs_parser.py` & `llama_index-0.6.0a7/llama_index/readers/file/docs_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/file/epub_parser.py` & `llama_index-0.6.0a7/llama_index/readers/file/epub_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/file/image_caption_parser.py` & `llama_index-0.6.0a7/llama_index/readers/file/image_caption_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/file/image_parser.py` & `llama_index-0.6.0a7/llama_index/readers/file/image_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/file/image_vision_llm_parser.py` & `llama_index-0.6.0a7/llama_index/readers/file/image_vision_llm_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/file/ipynb_parser.py` & `llama_index-0.6.0a7/llama_index/readers/file/ipynb_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/file/markdown_parser.py` & `llama_index-0.6.0a7/llama_index/readers/file/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/file/mbox_parser.py` & `llama_index-0.6.0a7/llama_index/readers/file/mbox_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/file/slides_parser.py` & `llama_index-0.6.0a7/llama_index/readers/file/slides_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/file/tabular_parser.py` & `llama_index-0.6.0a7/llama_index/readers/file/tabular_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/file/video_audio.py` & `llama_index-0.6.0a7/llama_index/readers/file/video_audio.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/github_readers/github_api_client.py` & `llama_index-0.6.0a7/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/github_readers/github_repository_reader.py` & `llama_index-0.6.0a7/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/github_readers/utils.py` & `llama_index-0.6.0a7/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/google_readers/gdocs.py` & `llama_index-0.6.0a7/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/google_readers/gsheets.py` & `llama_index-0.6.0a7/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/json.py` & `llama_index-0.6.0a7/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/make_com/wrapper.py` & `llama_index-0.6.0a7/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/mbox.py` & `llama_index-0.6.0a7/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/milvus.py` & `llama_index-0.6.0a7/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/mongo.py` & `llama_index-0.6.0a7/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/myscale.py` & `llama_index-0.6.0a7/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/notion.py` & `llama_index-0.6.0a7/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/obsidian.py` & `llama_index-0.6.0a7/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/pinecone.py` & `llama_index-0.6.0a7/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/qdrant.py` & `llama_index-0.6.0a7/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/schema/base.py` & `llama_index-0.6.0a7/llama_index/readers/schema/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/slack.py` & `llama_index-0.6.0a7/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/steamship/file_reader.py` & `llama_index-0.6.0a7/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/string_iterable.py` & `llama_index-0.6.0a7/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/twitter.py` & `llama_index-0.6.0a7/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/weaviate/client.py` & `llama_index-0.6.0a7/llama_index/readers/weaviate/client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/weaviate/reader.py` & `llama_index-0.6.0a7/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/weaviate/utils.py` & `llama_index-0.6.0a7/llama_index/readers/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/web.py` & `llama_index-0.6.0a7/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/wikipedia.py` & `llama_index-0.6.0a7/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/readers/youtube_transcript.py` & `llama_index-0.6.0a7/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/response/notebook_utils.py` & `llama_index-0.6.0a7/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/response/schema.py` & `llama_index-0.6.0a7/llama_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/retrievers/__init__.py` & `llama_index-0.6.0a7/llama_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/retrievers/transform_retriever.py` & `llama_index-0.6.0a7/llama_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/schema.py` & `llama_index-0.6.0a7/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/selectors/llm_selectors.py` & `llama_index-0.6.0a7/llama_index/selectors/llm_selectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 def _build_choices_text(choices: Sequence[ToolMetadata]) -> str:
     """Convert sequence of metadata to enumeration text."""
     texts: List[str] = []
     for ind, choice in enumerate(choices):
         text = " ".join(choice.description.splitlines())
         text = f"({ind + 1}) {text}"  # to one indexing
+        texts.append(text)
     return "\n\n".join(texts)
 
 
 def _structured_output_to_selector_result(output: Any) -> SelectorResult:
     """Convert structured output to selector result."""
     structured_output = cast(StructuredOutput, output)
     answers = cast(List[Answer], structured_output.parsed_output)
```

### Comparing `llama_index-0.6.0a6/llama_index/selectors/prompts.py` & `llama_index-0.6.0a7/llama_index/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/selectors/types.py` & `llama_index-0.6.0a7/llama_index/selectors/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,26 @@
     inds: List[int]
     reasons: List[str]
 
     @property
     def ind(self) -> int:
         if len(self.inds) != 1:
             raise ValueError(
-                f"There are {len(self.inds)} selections, " "please use .selection_inds."
+                f"There are {len(self.inds)} selections, " "please use .inds."
             )
         return self.inds[0]
 
+    @property
+    def reason(self) -> str:
+        if len(self.reasons) != 1:
+            raise ValueError(
+                f"There are {len(self.reasons)} selections, " "please use .reasons."
+            )
+        return self.reasons[0]
+
 
 def _wrap_choice(choice: MetadataType) -> ToolMetadata:
     if isinstance(choice, ToolMetadata):
         return choice
     elif isinstance(choice, str):
         return ToolMetadata(description=choice)
     else:
```

### Comparing `llama_index-0.6.0a6/llama_index/storage/docstore/__init__.py` & `llama_index-0.6.0a7/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/docstore/keyval_docstore.py` & `llama_index-0.6.0a7/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/docstore/mongo_docstore.py` & `llama_index-0.6.0a7/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/docstore/registry.py` & `llama_index-0.6.0a7/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/docstore/simple_docstore.py` & `llama_index-0.6.0a7/llama_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/docstore/types.py` & `llama_index-0.6.0a7/llama_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/docstore/utils.py` & `llama_index-0.6.0a7/llama_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/index_store/keyval_index_store.py` & `llama_index-0.6.0a7/llama_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/index_store/mongo_index_store.py` & `llama_index-0.6.0a7/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/index_store/simple_index_store.py` & `llama_index-0.6.0a7/llama_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/index_store/types.py` & `llama_index-0.6.0a7/llama_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/index_store/utils.py` & `llama_index-0.6.0a7/llama_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/kvstore/mongodb_kvstore.py` & `llama_index-0.6.0a7/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/kvstore/simple_kvstore.py` & `llama_index-0.6.0a7/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/kvstore/types.py` & `llama_index-0.6.0a7/llama_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/storage/storage_context.py` & `llama_index-0.6.0a7/llama_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/token_counter/mock_chain_wrapper.py` & `llama_index-0.6.0a7/llama_index/token_counter/mock_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/token_counter/mock_embed_model.py` & `llama_index-0.6.0a7/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/token_counter/token_counter.py` & `llama_index-0.6.0a7/llama_index/token_counter/token_counter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/token_counter/utils.py` & `llama_index-0.6.0a7/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/tools/query_engine.py` & `llama_index-0.6.0a7/llama_index/tools/query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/tts/bark.py` & `llama_index-0.6.0a7/llama_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/tts/base.py` & `llama_index-0.6.0a7/llama_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/tts/elevenlabs.py` & `llama_index-0.6.0a7/llama_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/utils.py` & `llama_index-0.6.0a7/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/vector_stores/__init__.py` & `llama_index-0.6.0a7/llama_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/vector_stores/chatgpt_plugin.py` & `llama_index-0.6.0a7/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/vector_stores/chroma.py` & `llama_index-0.6.0a7/llama_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/vector_stores/deeplake.py` & `llama_index-0.6.0a7/llama_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/vector_stores/faiss.py` & `llama_index-0.6.0a7/llama_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/vector_stores/milvus.py` & `llama_index-0.6.0a7/llama_index/vector_stores/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/vector_stores/myscale.py` & `llama_index-0.6.0a7/llama_index/vector_stores/myscale.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 """
 import json
 import logging
 from typing import Any, Dict, List, Optional, cast
 
 from llama_index.data_structs.node_v2 import DocumentRelationship, Node
 from llama_index.indices.service_context import ServiceContext
-from llama_index.readers.myscale import MyScaleSettings, escape_str, format_list_to_string
+from llama_index.readers.myscale import (
+    MyScaleSettings,
+    escape_str,
+    format_list_to_string,
+)
 from llama_index.utils import iter_batch
 from llama_index.vector_stores.types import (
     NodeEmbeddingResult,
     VectorStore,
     VectorStoreQuery,
     VectorStoreQueryResult,
 )
```

### Comparing `llama_index-0.6.0a6/llama_index/vector_stores/opensearch.py` & `llama_index-0.6.0a7/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/vector_stores/pinecone.py` & `llama_index-0.6.0a7/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/vector_stores/qdrant.py` & `llama_index-0.6.0a7/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/vector_stores/registry.py` & `llama_index-0.6.0a7/llama_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/vector_stores/simple.py` & `llama_index-0.6.0a7/llama_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/vector_stores/types.py` & `llama_index-0.6.0a7/llama_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index/vector_stores/weaviate.py` & `llama_index-0.6.0a7/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a6/llama_index.egg-info/PKG-INFO` & `llama_index-0.6.0a7/llama_index.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: llama-index
-Version: 0.6.0a6
-Summary: Interface between LLMs and your data.
-Home-page: https://github.com/jerryjliu/gpt_index
+Version: 0.6.0a7
+Summary: Interface between LLMs and your data
+Home-page: https://github.com/jerryjliu/llama_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
 
 LlamaIndex (GPT Index) is a project that provides a central interface to connect your LLM's with external data.
```

### Comparing `llama_index-0.6.0a6/llama_index.egg-info/SOURCES.txt` & `llama_index-0.6.0a7/llama_index.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 llama_index/VERSION
 llama_index/__init__.py
 llama_index/async_utils.py
 llama_index/constants.py
 llama_index/img_utils.py
 llama_index/py.typed
@@ -22,22 +23,22 @@
 llama_index/callbacks/schema.py
 llama_index/composability/__init__.py
 llama_index/composability/base.py
 llama_index/composability/joint_qa_summary.py
 llama_index/data_structs/__init__.py
 llama_index/data_structs/data_structs.py
 llama_index/data_structs/data_structs_v2.py
-llama_index/data_structs/node_mapping.py
 llama_index/data_structs/node_v2.py
 llama_index/data_structs/registry.py
 llama_index/data_structs/struct_type.py
 llama_index/data_structs/table.py
 llama_index/data_structs/table_v2.py
 llama_index/embeddings/__init__.py
 llama_index/embeddings/base.py
+llama_index/embeddings/google.py
 llama_index/embeddings/langchain.py
 llama_index/embeddings/openai.py
 llama_index/embeddings/utils.py
 llama_index/evaluation/__init__.py
 llama_index/evaluation/base.py
 llama_index/evaluation/dataset_generation.py
 llama_index/indices/__init__.py
@@ -190,15 +191,14 @@
 llama_index/readers/github_readers/__init__.py
 llama_index/readers/github_readers/github_api_client.py
 llama_index/readers/github_readers/github_repository_reader.py
 llama_index/readers/github_readers/utils.py
 llama_index/readers/google_readers/__init__.py
 llama_index/readers/google_readers/gdocs.py
 llama_index/readers/google_readers/gsheets.py
-llama_index/readers/llamahub_modules/__init__.py
 llama_index/readers/make_com/__init__.py
 llama_index/readers/make_com/wrapper.py
 llama_index/readers/schema/__init__.py
 llama_index/readers/schema/base.py
 llama_index/readers/steamship/__init__.py
 llama_index/readers/steamship/file_reader.py
 llama_index/readers/weaviate/__init__.py
@@ -255,8 +255,106 @@
 llama_index/vector_stores/myscale.py
 llama_index/vector_stores/opensearch.py
 llama_index/vector_stores/pinecone.py
 llama_index/vector_stores/qdrant.py
 llama_index/vector_stores/registry.py
 llama_index/vector_stores/simple.py
 llama_index/vector_stores/types.py
-llama_index/vector_stores/weaviate.py
+llama_index/vector_stores/weaviate.py
+tests/__init__.py
+tests/conftest.py
+tests/test_utils.py
+tests/callbacks/__init__.py
+tests/callbacks/test_llama_debug.py
+tests/embeddings/__init__.py
+tests/embeddings/test_base.py
+tests/indices/__init__.py
+tests/indices/conftest.py
+tests/indices/test_loading.py
+tests/indices/test_loading_graph.py
+tests/indices/test_node_utils.py
+tests/indices/test_prompt_helper.py
+tests/indices/test_utils.py
+tests/indices/composability/__init__.py
+tests/indices/composability/test_utils.py
+tests/indices/empty/__init__.py
+tests/indices/empty/test_base.py
+tests/indices/keyword_table/__init__.py
+tests/indices/keyword_table/test_base.py
+tests/indices/keyword_table/test_retrievers.py
+tests/indices/keyword_table/test_utils.py
+tests/indices/knowledge_graph/__init__.py
+tests/indices/knowledge_graph/conftest.py
+tests/indices/knowledge_graph/test_base.py
+tests/indices/knowledge_graph/test_retrievers.py
+tests/indices/list/__init__.py
+tests/indices/list/test_index.py
+tests/indices/list/test_retrievers.py
+tests/indices/postprocessor/__init__.py
+tests/indices/postprocessor/test_base.py
+tests/indices/query/__init__.py
+tests/indices/query/conftest.py
+tests/indices/query/test_compose.py
+tests/indices/query/test_compose_vector.py
+tests/indices/query/test_query_bundle.py
+tests/indices/query/query_transform/__init__.py
+tests/indices/query/query_transform/mock_utils.py
+tests/indices/query/query_transform/test_base.py
+tests/indices/struct_store/__init__.py
+tests/indices/struct_store/conftest.py
+tests/indices/struct_store/test_base.py
+tests/indices/struct_store/test_pandas.py
+tests/indices/struct_store/test_sql_query.py
+tests/indices/tree/__init__.py
+tests/indices/tree/conftest.py
+tests/indices/tree/test_embedding_retriever.py
+tests/indices/tree/test_index.py
+tests/indices/tree/test_retrievers.py
+tests/indices/vector_store/__init__.py
+tests/indices/vector_store/conftest.py
+tests/indices/vector_store/mock_faiss.py
+tests/indices/vector_store/mock_services.py
+tests/indices/vector_store/test_faiss.py
+tests/indices/vector_store/test_milvus.py
+tests/indices/vector_store/test_myscale.py
+tests/indices/vector_store/test_pinecone.py
+tests/indices/vector_store/test_retrievers.py
+tests/indices/vector_store/test_simple.py
+tests/indices/vector_store/test_weaviate.py
+tests/indices/vector_store/utils.py
+tests/langchain_helpers/__init__.py
+tests/langchain_helpers/test_text_splitter.py
+tests/llm_predictor/__init__.py
+tests/llm_predictor/test_base.py
+tests/logger/__init__.py
+tests/logger/test_base.py
+tests/mock_utils/__init__.py
+tests/mock_utils/mock_predict.py
+tests/mock_utils/mock_prompts.py
+tests/mock_utils/mock_text_splitter.py
+tests/mock_utils/mock_utils.py
+tests/optimization/__init__.py
+tests/optimization/test_base.py
+tests/output_parsers/__init__.py
+tests/output_parsers/test_base.py
+tests/output_parsers/test_selection.py
+tests/playground/__init__.py
+tests/playground/test_base.py
+tests/prompts/__init__.py
+tests/prompts/test_base.py
+tests/readers/__init__.py
+tests/readers/test_file.py
+tests/readers/test_json.py
+tests/readers/test_mongo.py
+tests/readers/test_string_iterable.py
+tests/selectors/__init__.py
+tests/selectors/test_llm_selectors.py
+tests/storage/__init__.py
+tests/storage/conftest.py
+tests/storage/docstore/__init__.py
+tests/storage/docstore/test_mongo_docstore.py
+tests/storage/docstore/test_simple_docstore.py
+tests/token_predictor/__init__.py
+tests/token_predictor/test_base.py
+tests/vector_stores/__init__.py
+tests/vector_stores/test_qdrant.py
+tests/vector_stores/test_weaviate.py
```

### Comparing `llama_index-0.6.0a6/setup.py` & `llama_index-0.6.0a7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Set up the package."""
 import sys
 from pathlib import Path
-
+import os
 from setuptools import find_packages, setup
 
+DEFAULT_PACKAGE_NAME = "llama_index"
+PACKAGE_NAME = os.environ.get("PACKAGE_NAME_OVERRIDE", DEFAULT_PACKAGE_NAME)
+
 with open(Path(__file__).absolute().parents[0] / "llama_index" / "VERSION") as _f:
     __version__ = _f.read().strip()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 install_requires = [
@@ -22,21 +25,19 @@
 # NOTE: if python version >= 3.9, install tiktoken
 # else install transformers
 if sys.version_info >= (3, 9):
     install_requires.extend(["tiktoken"])
 else:
     install_requires.extend(["transformers"])
 
-# upload duplicate package to pypi
 setup(
-    name="llama_index",
+    name=PACKAGE_NAME,
     version=__version__,
-    # packages=find_packages(),
-    packages=find_packages(include=["llama*"]),
-    description="Interface between LLMs and your data.",
+    packages=find_packages(),
+    description="Interface between LLMs and your data",
     install_requires=install_requires,
     long_description=long_description,
     license="MIT",
-    url="https://github.com/jerryjliu/gpt_index",
+    url="https://github.com/jerryjliu/llama_index",
     include_package_data=True,
     long_description_content_type="text/markdown",
 )
```

