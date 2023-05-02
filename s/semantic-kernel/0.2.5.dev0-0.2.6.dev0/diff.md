# Comparing `tmp/semantic_kernel-0.2.5.dev0.tar.gz` & `tmp/semantic_kernel-0.2.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.2.5.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.2.6.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.2.5.dev0.tar` & `semantic_kernel-0.2.6.dev0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     4573 2023-04-30 18:57:02.979916 semantic_kernel-0.2.5.dev0/README.md
--rw-r--r--   0        0        0      719 2023-05-01 18:50:34.098615 semantic_kernel-0.2.5.dev0/pyproject.toml
--rw-r--r--   0        0        0     1302 2023-04-18 17:46:11.883057 semantic_kernel-0.2.5.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.983569 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/ai_exception.py
--rw-r--r--   0        0        0      506 2023-04-30 18:57:02.983999 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1129 2023-04-30 18:57:02.985239 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1332 2023-04-30 18:57:02.985587 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-30 18:57:02.986074 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      352 2023-04-30 18:57:02.986678 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     3463 2023-04-30 18:57:02.987541 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2093 2023-04-30 18:57:02.988126 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      892 2023-04-30 18:57:02.988571 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2782 2023-04-30 18:57:02.989002 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2774 2023-04-30 18:57:02.989380 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2769 2023-04-30 18:57:02.990041 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     5227 2023-04-30 18:57:02.990444 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     4471 2023-04-30 18:57:02.990953 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2449 2023-04-30 18:57:02.991301 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0      497 2023-04-30 18:57:02.991644 semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      457 2023-04-22 04:06:40.780007 semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2072 2023-04-13 23:12:46.166679 semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.780276 semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/http_skill.py
--rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.194344 semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2403 2023-04-13 23:12:46.167467 semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     5849 2023-04-30 18:57:02.992220 semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0    12503 2023-04-30 18:57:02.992677 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     2240 2023-04-22 04:06:40.781294 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_base.py
--rw-r--r--   0        0        0     9401 2023-04-30 18:57:02.993097 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_config.py
--rw-r--r--   0        0        0     1626 2023-04-30 18:57:02.993735 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      710 2023-04-14 00:51:57.196637 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/__init__.py
--rw-r--r--   0        0        0      210 2023-04-13 23:12:46.171776 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
--rw-r--r--   0        0        0     3822 2023-04-30 18:57:02.994407 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/import_skills.py
--rw-r--r--   0        0        0     2323 2023-04-13 23:12:46.172614 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/inline_definition.py
--rw-r--r--   0        0        0     1481 2023-04-30 18:57:02.995123 semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
--rw-r--r--   0        0        0      160 2023-04-13 23:12:46.173418 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2345 2023-04-30 18:57:02.996159 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     3089 2023-04-30 18:57:02.996701 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     2012 2023-04-30 18:57:02.997202 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1137 2023-04-13 23:12:46.175270 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6036 2023-04-30 18:57:02.997638 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1196 2023-04-30 18:57:02.998063 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12032 2023-04-30 18:57:02.998486 semantic_kernel-0.2.5.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.782347 semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.199808 semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     8966 2023-04-14 00:51:57.200548 semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-13 23:12:46.179530 semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.160748 semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    15917 2023-04-30 18:57:02.998992 semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.999492 semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      919 2023-04-13 23:12:46.181682 semantic_kernel-0.2.5.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      673 2023-04-13 23:12:46.182155 semantic_kernel-0.2.5.dev0/semantic_kernel/reliability/retry_mechanism.py
--rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.182583 semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.203325 semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-13 23:12:46.183441 semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4269 2023-04-30 18:57:02.999997 semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-14 00:51:57.204455 semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-14 00:51:57.205241 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.205757 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     1717 2023-04-13 23:12:46.186028 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.206300 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.206885 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.207475 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-13 23:12:46.187552 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-14 00:51:57.208334 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.208951 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-13 23:12:46.188719 semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.189034 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      830 2023-04-14 00:51:57.209567 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-14 00:51:57.210164 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000489 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.192355 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-13 23:12:46.192840 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.211524 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.193631 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.212261 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.194683 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.212967 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-13 23:12:46.195769 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.196165 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-13 23:12:46.196572 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.196999 semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      473 2023-04-30 18:57:03.001133 semantic_kernel-0.2.5.dev0/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      667 2023-04-30 18:57:03.001562 semantic_kernel-0.2.5.dev0/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     6466 2023-05-01 18:36:22.039798 semantic_kernel-0.2.5.dev0/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      403 2023-04-13 23:12:46.197533 semantic_kernel-0.2.5.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2436 2023-04-14 00:51:57.213683 semantic_kernel-0.2.5.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-13 23:12:46.198404 semantic_kernel-0.2.5.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.198764 semantic_kernel-0.2.5.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     5285 1970-01-01 00:00:00.000000 semantic_kernel-0.2.5.dev0/PKG-INFO
+-rw-r--r--   0        0        0     4595 2023-05-02 00:16:15.432235 semantic_kernel-0.2.6.dev0/README.md
+-rw-r--r--   0        0        0      719 2023-05-02 00:16:15.432829 semantic_kernel-0.2.6.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1302 2023-04-18 17:46:11.883057 semantic_kernel-0.2.6.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.983569 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/ai_exception.py
+-rw-r--r--   0        0        0      506 2023-04-30 18:57:02.983999 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1129 2023-04-30 18:57:02.985239 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1332 2023-04-30 18:57:02.985587 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-30 18:57:02.986074 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      352 2023-04-30 18:57:02.986678 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     3569 2023-05-01 23:42:05.935410 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2093 2023-04-30 18:57:02.988126 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      892 2023-04-30 18:57:02.988571 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2782 2023-04-30 18:57:02.989002 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2774 2023-04-30 18:57:02.989380 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2769 2023-04-30 18:57:02.990041 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     5227 2023-04-30 18:57:02.990444 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     4471 2023-04-30 18:57:02.990953 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2572 2023-05-01 23:42:05.936356 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0      497 2023-04-30 18:57:02.991644 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      457 2023-04-22 04:06:40.780007 semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2072 2023-04-13 23:12:46.166679 semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.780276 semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/http_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.194344 semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2403 2023-04-13 23:12:46.167467 semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     5849 2023-04-30 18:57:02.992220 semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0    12503 2023-04-30 18:57:02.992677 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     2240 2023-04-22 04:06:40.781294 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_base.py
+-rw-r--r--   0        0        0    10319 2023-05-02 00:16:15.433586 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_config.py
+-rw-r--r--   0        0        0     1626 2023-04-30 18:57:02.993735 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      710 2023-04-14 00:51:57.196637 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/__init__.py
+-rw-r--r--   0        0        0      210 2023-04-13 23:12:46.171776 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
+-rw-r--r--   0        0        0     3822 2023-04-30 18:57:02.994407 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/import_skills.py
+-rw-r--r--   0        0        0     2323 2023-04-13 23:12:46.172614 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/inline_definition.py
+-rw-r--r--   0        0        0     1497 2023-05-02 00:16:15.434300 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
+-rw-r--r--   0        0        0      160 2023-04-13 23:12:46.173418 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2345 2023-04-30 18:57:02.996159 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     3089 2023-04-30 18:57:02.996701 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     2012 2023-04-30 18:57:02.997202 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1137 2023-04-13 23:12:46.175270 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6045 2023-05-02 00:16:15.434951 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     1196 2023-04-30 18:57:02.998063 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12032 2023-04-30 18:57:02.998486 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.782347 semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.199808 semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     8966 2023-04-14 00:51:57.200548 semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-13 23:12:46.179530 semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.160748 semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    15917 2023-04-30 18:57:02.998992 semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.999492 semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      919 2023-04-13 23:12:46.181682 semantic_kernel-0.2.6.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      673 2023-04-13 23:12:46.182155 semantic_kernel-0.2.6.dev0/semantic_kernel/reliability/retry_mechanism.py
+-rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.182583 semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.203325 semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-13 23:12:46.183441 semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4269 2023-04-30 18:57:02.999997 semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-14 00:51:57.204455 semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-14 00:51:57.205241 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.205757 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     1717 2023-04-13 23:12:46.186028 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.206300 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.206885 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.207475 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-13 23:12:46.187552 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-14 00:51:57.208334 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.208951 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-13 23:12:46.188719 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.189034 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      830 2023-04-14 00:51:57.209567 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-14 00:51:57.210164 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000489 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.192355 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-13 23:12:46.192840 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.211524 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.193631 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.212261 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.194683 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.212967 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-13 23:12:46.195769 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.196165 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-13 23:12:46.196572 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.196999 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      473 2023-04-30 18:57:03.001133 semantic_kernel-0.2.6.dev0/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-30 18:57:03.001562 semantic_kernel-0.2.6.dev0/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     6466 2023-05-01 18:36:22.039798 semantic_kernel-0.2.6.dev0/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      403 2023-04-13 23:12:46.197533 semantic_kernel-0.2.6.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2436 2023-04-14 00:51:57.213683 semantic_kernel-0.2.6.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-13 23:12:46.198404 semantic_kernel-0.2.6.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.198764 semantic_kernel-0.2.6.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     5307 1970-01-01 00:00:00.000000 semantic_kernel-0.2.6.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.2.5.dev0/README.md` & `semantic_kernel-0.2.6.dev0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 import semantic_kernel as sk
 from semantic_kernel.connectors.ai.open_ai import OpenAITextCompletion, AzureTextCompletion
 
 kernel = sk.Kernel()
 
 # Prepare OpenAI service using credentials stored in the `.env` file
 api_key, org_id = sk.openai_settings_from_dot_env()
-kernel.config.add_text_service("dv", OpenAITextCompletion("text-davinci-003", api_key, org_id))
+kernel.config.add_text_completion_service("dv", OpenAITextCompletion("text-davinci-003", api_key, org_id))
 
 # Alternative using Azure:
 # deployment, api_key, endpoint = sk.azure_openai_settings_from_dot_env()
-# kernel.config.add_text_service("dv", AzureTextCompletion(deployment, endpoint, api_key))
+# kernel.config.add_text_completion_service("dv", AzureTextCompletion(deployment, endpoint, api_key))
 
 # Wrap your prompt in a function
 prompt = kernel.create_semantic_function("""
 1) A robot may not injure a human being or, through inaction,
 allow a human being to come to harm.
 
 2) A robot must obey orders given it by human beings except where
```

### Comparing `semantic_kernel-0.2.5.dev0/pyproject.toml` & `semantic_kernel-0.2.6.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.2.5.dev"
+version = "0.2.6.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/ai_exception.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/chat_request_settings.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/complete_request_settings.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
 from typing import Optional
 
 import torch
-from transformers import pipeline
+from transformers import GenerationConfig, pipeline
 
 from semantic_kernel.connectors.ai.ai_exception import AIException
 from semantic_kernel.connectors.ai.complete_request_settings import (
     CompleteRequestSettings,
 )
 from semantic_kernel.connectors.ai.text_completion_client_base import (
     TextCompletionClientBase,
@@ -65,22 +65,23 @@
             prompt {str} -- Prompt to complete.
             request_settings {CompleteRequestSettings} -- Request settings.
 
         Returns:
             str -- Completion result.
         """
         try:
-            result = self.generator(
-                prompt,
-                num_return_sequences=1,
+            generation_config = GenerationConfig(
                 temperature=request_settings.temperature,
                 top_p=request_settings.top_p,
-                max_length=request_settings.max_tokens,
+                max_new_tokens=request_settings.max_tokens,
                 pad_token_id=50256,  # EOS token
             )
+            result = self.generator(
+                prompt, num_return_sequences=1, generation_config=generation_config
+            )
 
             if self._task == "text-generation" or self._task == "text2text-generation":
                 return result[0]["generated_text"]
 
             elif self._task == "summarization":
                 return result[0]["summary_text"]
```

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 
         self.open_ai_instance = self._setup_open_ai()
 
     def _setup_open_ai(self) -> Any:
         import openai
 
         openai.api_key = self._api_key
+        openai.api_base = "https://api.openai.com/v1"
+        openai.api_type = "openai"
+        openai.api_version = None
         if self._org_id is not None:
             openai.organization = self._org_id
 
         return openai
 
     async def generate_embeddings_async(self, texts: List[str]) -> ndarray:
         model_args = {}
```

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/http_skill.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/http_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_base.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_config.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,82 +21,82 @@
 
 
 T = TypeVar("T")
 
 
 class KernelConfig:
     def __init__(self) -> None:
-        self._text_services: Dict[
+        self._text_completion_services: Dict[
             str, Callable[["KernelBase"], TextCompletionClientBase]
         ] = {}
         self._chat_services: Dict[
             str, Callable[["KernelBase"], ChatCompletionClientBase]
         ] = {}
-        self._embedding_services: Dict[
+        self._text_embedding_generation_services: Dict[
             str, Callable[["KernelBase"], EmbeddingGeneratorBase]
         ] = {}
 
-        self._default_text_service: Optional[str] = None
+        self._default_text_completion_service: Optional[str] = None
         self._default_chat_service: Optional[str] = None
-        self._default_embedding_service: Optional[str] = None
+        self._default_text_embedding_generation_service: Optional[str] = None
 
         self._retry_mechanism: RetryMechanism = PassThroughWithoutRetry()
 
     def get_ai_service(
         self, type: Type[T], service_id: Optional[str] = None
     ) -> Callable[["KernelBase"], T]:
         matching_type = {}
         if type == TextCompletionClientBase:
-            service_id = service_id or self._default_text_service
-            matching_type = self._text_services
+            service_id = service_id or self._default_text_completion_service
+            matching_type = self._text_completion_services
         elif type == ChatCompletionClientBase:
             service_id = service_id or self._default_chat_service
             matching_type = self._chat_services
         elif type == EmbeddingGeneratorBase:
-            service_id = service_id or self._default_embedding_service
-            matching_type = self._embedding_services
+            service_id = service_id or self._default_text_embedding_generation_service
+            matching_type = self._text_embedding_generation_services
         else:
             raise ValueError(f"Unknown AI service type: {type.__name__}")
 
         if service_id not in matching_type:
             raise ValueError(
                 f"{type.__name__} service with service_id '{service_id}' not found"
             )
 
         return matching_type[service_id]
 
-    def all_text_services(self) -> List[str]:
-        return list(self._text_services.keys())
+    def all_text_completion_services(self) -> List[str]:
+        return list(self._text_completion_services.keys())
 
     def all_chat_services(self) -> List[str]:
         return list(self._chat_services.keys())
 
-    def all_embedding_services(self) -> List[str]:
-        return list(self._embedding_services.keys())
+    def all_text_embedding_generation_services(self) -> List[str]:
+        return list(self._text_embedding_generation_services.keys())
 
-    def add_text_service(
+    def add_text_completion_service(
         self,
         service_id: str,
         service: Union[
             TextCompletionClientBase, Callable[["KernelBase"], TextCompletionClientBase]
         ],
         overwrite: bool = True,
     ) -> "KernelConfig":
         if not service_id:
             raise ValueError("service_id must be a non-empty string")
-        if not overwrite and service_id in self._text_services:
+        if not overwrite and service_id in self._text_completion_services:
             raise ValueError(
                 f"Text service with service_id '{service_id}' already exists"
             )
 
-        self._text_services[service_id] = (
+        self._text_completion_services[service_id] = (
             service if isinstance(service, Callable) else lambda _: service
         )
-        if self._default_text_service is None:
-            self._default_text_service = service_id
+        if self._default_text_completion_service is None:
+            self._default_text_completion_service = service_id
 
         return self
 
     def add_chat_service(
         self,
         service_id: str,
         service: Union[
@@ -114,147 +114,157 @@
         self._chat_services[service_id] = (
             service if isinstance(service, Callable) else lambda _: service
         )
         if self._default_chat_service is None:
             self._default_chat_service = service_id
 
         if isinstance(service, TextCompletionClientBase):
-            self.add_text_service(service_id, service)
-            if self._default_text_service is None:
-                self._default_text_service = service_id
+            self.add_text_completion_service(service_id, service)
+            if self._default_text_completion_service is None:
+                self._default_text_completion_service = service_id
 
         return self
 
-    def add_embedding_service(
+    def add_text_embedding_generation_service(
         self,
         service_id: str,
         service: Union[
             EmbeddingGeneratorBase, Callable[["KernelBase"], EmbeddingGeneratorBase]
         ],
         overwrite: bool = False,
     ) -> "KernelConfig":
         if not service_id:
             raise ValueError("service_id must be a non-empty string")
-        if not overwrite and service_id in self._embedding_services:
+        if not overwrite and service_id in self._text_embedding_generation_services:
             raise ValueError(
                 f"Embedding service with service_id '{service_id}' already exists"
             )
 
-        self._embedding_services[service_id] = (
+        self._text_embedding_generation_services[service_id] = (
             service if isinstance(service, Callable) else lambda _: service
         )
-        if self._default_embedding_service is None:
-            self._default_embedding_service = service_id
+        if self._default_text_embedding_generation_service is None:
+            self._default_text_embedding_generation_service = service_id
 
         return self
 
     # TODO: look harder at retry stuff
 
-    def set_default_text_service(self, service_id: str) -> "KernelConfig":
-        if service_id not in self._text_services:
+    def set_default_text_completion_service(self, service_id: str) -> "KernelConfig":
+        if service_id not in self._text_completion_services:
             raise ValueError(
                 f"AI service with service_id '{service_id}' does not exist"
             )
 
-        self._default_text_service = service_id
+        self._default_text_completion_service = service_id
         return self
 
     def set_default_chat_service(self, service_id: str) -> "KernelConfig":
         if service_id not in self._chat_services:
             raise ValueError(
                 f"AI service with service_id '{service_id}' does not exist"
             )
 
         self._default_chat_service = service_id
         return self
 
-    def set_default_embedding_service(self, service_id: str) -> "KernelConfig":
-        if service_id not in self._embedding_services:
+    def set_default_text_embedding_generation_service(
+        self, service_id: str
+    ) -> "KernelConfig":
+        if service_id not in self._text_embedding_generation_services:
             raise ValueError(
                 f"AI service with service_id '{service_id}' does not exist"
             )
 
-        self._default_embedding_service = service_id
+        self._default_text_embedding_generation_service = service_id
         return self
 
-    def get_text_service_service_id(self, service_id: Optional[str] = None) -> str:
-        if service_id is None or service_id not in self._text_services:
-            if self._default_text_service is None:
+    def get_text_completion_service_service_id(
+        self, service_id: Optional[str] = None
+    ) -> str:
+        if service_id is None or service_id not in self._text_completion_services:
+            if self._default_text_completion_service is None:
                 raise ValueError("No default text service is set")
-            return self._default_text_service
+            return self._default_text_completion_service
 
         return service_id
 
     def get_chat_service_service_id(self, service_id: Optional[str] = None) -> str:
         if service_id is None or service_id not in self._chat_services:
             if self._default_chat_service is None:
                 raise ValueError("No default chat service is set")
             return self._default_chat_service
 
         return service_id
 
-    def get_embedding_service_id(self, service_id: Optional[str] = None) -> str:
-        if service_id is None or service_id not in self._embedding_services:
-            if self._default_embedding_service is None:
+    def get_text_embedding_generation_service_id(
+        self, service_id: Optional[str] = None
+    ) -> str:
+        if service_id is None or service_id not in self._text_embedding_generation_services:
+            if self._default_text_embedding_generation_service is None:
                 raise ValueError("No default embedding service is set")
-            return self._default_embedding_service
+            return self._default_text_embedding_generation_service
 
         return service_id
 
-    def remove_text_service(self, service_id: str) -> "KernelConfig":
-        if service_id not in self._text_services:
+    def remove_text_completion_service(self, service_id: str) -> "KernelConfig":
+        if service_id not in self._text_completion_services:
             raise ValueError(
                 f"AI service with service_id '{service_id}' does not exist"
             )
 
-        del self._text_services[service_id]
-        if self._default_text_service == service_id:
-            self._default_text_service = next(iter(self._text_services), None)
+        del self._text_completion_services[service_id]
+        if self._default_text_completion_service == service_id:
+            self._default_text_completion_service = next(
+                iter(self._text_completion_services), None
+            )
         return self
 
     def remove_chat_service(self, service_id: str) -> "KernelConfig":
         if service_id not in self._chat_services:
             raise ValueError(
                 f"AI service with service_id '{service_id}' does not exist"
             )
 
         del self._chat_services[service_id]
         if self._default_chat_service == service_id:
             self._default_chat_service = next(iter(self._chat_services), None)
         return self
 
-    def remove_embedding_service(self, service_id: str) -> "KernelConfig":
-        if service_id not in self._embedding_services:
+    def remove_text_embedding_generation_service(self, service_id: str) -> "KernelConfig":
+        if service_id not in self._text_embedding_generation_services:
             raise ValueError(
                 f"AI service with service_id '{service_id}' does not exist"
             )
 
-        del self._embedding_services[service_id]
-        if self._default_embedding_service == service_id:
-            self._default_embedding_service = next(iter(self._embedding_services), None)
+        del self._text_embedding_generation_services[service_id]
+        if self._default_text_embedding_generation_service == service_id:
+            self._default_text_embedding_generation_service = next(
+                iter(self._text_embedding_generation_services), None
+            )
         return self
 
-    def clear_all_text_services(self) -> "KernelConfig":
-        self._text_services = {}
-        self._default_text_service = None
+    def clear_all_text_completion_services(self) -> "KernelConfig":
+        self._text_completion_services = {}
+        self._default_text_completion_service = None
         return self
 
     def clear_all_chat_services(self) -> "KernelConfig":
         self._chat_services = {}
         self._default_chat_service = None
         return self
 
-    def clear_all_embedding_services(self) -> "KernelConfig":
-        self._embedding_services = {}
-        self._default_embedding_service = None
+    def clear_all_text_embedding_generation_services(self) -> "KernelConfig":
+        self._text_embedding_generation_services = {}
+        self._default_text_embedding_generation_service = None
         return self
 
     def clear_all_services(self) -> "KernelConfig":
-        self._text_services = {}
+        self._text_completion_services = {}
         self._chat_services = {}
-        self._embedding_services = {}
+        self._text_embedding_generation_services = {}
 
-        self._default_text_service = None
+        self._default_text_completion_service = None
         self._default_chat_service = None
-        self._default_embedding_service = None
+        self._default_text_embedding_generation_service = None
 
         return self
```

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/__init__.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/import_skills.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/import_skills.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/inline_definition.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/inline_definition.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/kernel_extensions/memory_configuration.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/memory_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self,
         storage: MemoryStoreBase,
         embeddings_generator: Optional[EmbeddingGeneratorBase] = None,
     ) -> None:
         kernel = self.kernel()
 
         if embeddings_generator is None:
-            service_id = kernel.config.get_embedding_service_id()
+            service_id = kernel.config.get_text_embedding_generation_service_id()
             if not service_id:
                 raise ValueError("The embedding service id cannot be `None` or empty")
 
             embeddings_service = kernel.config.get_ai_service(
                 EmbeddingGeneratorBase, service_id
             )
             if not embeddings_service:
```

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         if not await self._storage.does_collection_exist_async(
             collection_name=collection
         ):
             await self._storage.create_collection_async(collection_name=collection)
 
         embedding = await self._embeddings_generator.generate_embeddings_async([text])
         data = MemoryRecord.reference_record(
-            id=external_id,
+            external_id=external_id,
             source_name=external_source_name,
             description=description,
             embedding=embedding,
         )
 
         await self._storage.upsert_async(collection_name=collection, record=data)
```

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/reliability/retry_mechanism.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/reliability/retry_mechanism.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/utils/settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.2.6.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.5.dev0/PKG-INFO` & `semantic_kernel-0.2.6.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.2.5.dev0
+Version: 0.2.6.dev0
 Summary: 
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -49,19 +49,19 @@
 import semantic_kernel as sk
 from semantic_kernel.connectors.ai.open_ai import OpenAITextCompletion, AzureTextCompletion
 
 kernel = sk.Kernel()
 
 # Prepare OpenAI service using credentials stored in the `.env` file
 api_key, org_id = sk.openai_settings_from_dot_env()
-kernel.config.add_text_service("dv", OpenAITextCompletion("text-davinci-003", api_key, org_id))
+kernel.config.add_text_completion_service("dv", OpenAITextCompletion("text-davinci-003", api_key, org_id))
 
 # Alternative using Azure:
 # deployment, api_key, endpoint = sk.azure_openai_settings_from_dot_env()
-# kernel.config.add_text_service("dv", AzureTextCompletion(deployment, endpoint, api_key))
+# kernel.config.add_text_completion_service("dv", AzureTextCompletion(deployment, endpoint, api_key))
 
 # Wrap your prompt in a function
 prompt = kernel.create_semantic_function("""
 1) A robot may not injure a human being or, through inaction,
 allow a human being to come to harm.
 
 2) A robot must obey orders given it by human beings except where
```

