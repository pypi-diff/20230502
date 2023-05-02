# Comparing `tmp/benchling_sdk-1.7.0a8.tar.gz` & `tmp/benchling_sdk-1.7.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchling_sdk-1.7.0a8.tar", max compression
+gzip compressed data, was "benchling_sdk-1.7.0a9.tar", max compression
```

## Comparing `benchling_sdk-1.7.0a8.tar` & `benchling_sdk-1.7.0a9.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0    11357 2023-03-30 07:06:36.261979 benchling_sdk-1.7.0a8/LICENSE
--rw-r--r--   0        0        0      826 2023-03-30 07:21:24.290477 benchling_sdk-1.7.0a8/README.md
--rw-r--r--   0        0        0        0 2023-03-30 07:21:13.620375 benchling_sdk-1.7.0a8/benchling_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 07:21:13.620375 benchling_sdk-1.7.0a8/benchling_sdk/apps/__init__.py
--rw-r--r--   0        0        0      132 2023-03-30 07:06:36.261979 benchling_sdk-1.7.0a8/benchling_sdk/apps/config/__init__.py
--rw-r--r--   0        0        0     2185 2023-03-30 07:06:36.261979 benchling_sdk-1.7.0a8/benchling_sdk/apps/config/decryption_provider.py
--rw-r--r--   0        0        0    36607 2023-03-30 07:06:36.261979 benchling_sdk-1.7.0a8/benchling_sdk/apps/config/dependencies.py
--rw-r--r--   0        0        0    25203 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/apps/config/mock_dependencies.py
--rw-r--r--   0        0        0     6872 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/apps/config/scalars.py
--rw-r--r--   0        0        0    13205 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/apps/framework.py
--rw-r--r--   0        0        0        0 2023-03-30 07:21:13.620375 benchling_sdk-1.7.0a8/benchling_sdk/apps/helpers/__init__.py
--rw-r--r--   0        0        0    17317 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/apps/helpers/canvas_helpers.py
--rw-r--r--   0        0        0    15358 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/apps/helpers/config_helpers.py
--rw-r--r--   0        0        0     1789 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/apps/helpers/cryptography_helpers.py
--rw-r--r--   0        0        0      945 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/apps/helpers/manifest_helpers.py
--rw-r--r--   0        0        0    26922 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/apps/helpers/session_helpers.py
--rw-r--r--   0        0        0     6918 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/apps/helpers/webhook_helpers.py
--rw-r--r--   0        0        0      120 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/auth/__init__.py
--rw-r--r--   0        0        0      643 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/auth/api_key_auth.py
--rw-r--r--   0        0        0     5271 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/auth/client_credentials_oauth2.py
--rw-r--r--   0        0        0    24967 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/benchling.py
--rw-r--r--   0        0        0       38 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/docs/__init__.py
--rw-r--r--   0        0        0      244 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/docs/__main__.py
--rw-r--r--   0        0        0     7859 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/errors.py
--rw-r--r--   0        0        0        0 2023-03-30 07:21:13.620375 benchling_sdk-1.7.0a8/benchling_sdk/helpers/__init__.py
--rw-r--r--   0        0        0      833 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/helpers/client_helpers.py
--rw-r--r--   0        0        0     1094 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/helpers/constants.py
--rw-r--r--   0        0        0     1466 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/helpers/decorators.py
--rw-r--r--   0        0        0      338 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/helpers/file_helpers.py
--rw-r--r--   0        0        0     2500 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/helpers/logging_helpers.py
--rw-r--r--   0        0        0     1998 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/helpers/package_helpers.py
--rw-r--r--   0        0        0     7774 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/helpers/pagination_helpers.py
--rw-r--r--   0        0        0      613 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/helpers/response_helpers.py
--rw-r--r--   0        0        0     2677 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/helpers/retry_helpers.py
--rw-r--r--   0        0        0     3662 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/helpers/serialization_helpers.py
--rw-r--r--   0        0        0     3693 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/helpers/transaction_manager.py
--rw-r--r--   0        0        0   295288 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/models/__init__.py
--rw-r--r--   0        0        0       25 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/py.typed
--rw-r--r--   0        0        0       85 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 07:21:13.620375 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 07:21:13.620375 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/alpha/__init__.py
--rw-r--r--   0        0        0     1443 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/alpha/v2_alpha_app_service.py
--rw-r--r--   0        0        0     1347 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/alpha/v2_alpha_dna_sequence_service.py
--rw-r--r--   0        0        0      951 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/base_service.py
--rw-r--r--   0        0        0        0 2023-03-30 07:21:13.620375 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/__init__.py
--rw-r--r--   0        0        0     2551 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_aa_sequence_service.py
--rw-r--r--   0        0        0    11210 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_app_service.py
--rw-r--r--   0        0        0     1840 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_custom_entity_service.py
--rw-r--r--   0        0        0     1704 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_dna_oligo_service.py
--rw-r--r--   0        0        0     1843 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_dna_sequence_service.py
--rw-r--r--   0        0        0     1970 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_entity_service.py
--rw-r--r--   0        0        0     1053 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_entry_service.py
--rw-r--r--   0        0        0     1704 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_rna_oligo_service.py
--rw-r--r--   0        0        0     5544 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_worklist_service.py
--rw-r--r--   0        0        0        0 2023-03-30 07:21:13.620375 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/__init__.py
--rw-r--r--   0        0        0    11204 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/aa_sequence_service.py
--rw-r--r--   0        0        0    12371 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/api_service.py
--rw-r--r--   0        0        0    12448 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/app_service.py
--rw-r--r--   0        0        0    12317 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/assay_result_service.py
--rw-r--r--   0        0        0     9023 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/assay_run_service.py
--rw-r--r--   0        0        0    16738 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/blob_service.py
--rw-r--r--   0        0        0    12144 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/box_service.py
--rw-r--r--   0        0        0    18055 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/container_service.py
--rw-r--r--   0        0        0    10828 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/custom_entity_service.py
--rw-r--r--   0        0        0     7445 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/dna_alignments_service.py
--rw-r--r--   0        0        0     9456 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/dna_oligo_service.py
--rw-r--r--   0        0        0    12238 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/dna_sequence_service.py
--rw-r--r--   0        0        0     4919 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/dropdown_service.py
--rw-r--r--   0        0        0    11770 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/entry_service.py
--rw-r--r--   0        0        0     2538 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/event_service.py
--rw-r--r--   0        0        0     1080 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/export_service.py
--rw-r--r--   0        0        0     8988 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/feature_library_service.py
--rw-r--r--   0        0        0     5219 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/folder_service.py
--rw-r--r--   0        0        0     1761 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/inventory_service.py
--rw-r--r--   0        0        0     9869 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/lab_automation_service.py
--rw-r--r--   0        0        0     1300 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/label_template_service.py
--rw-r--r--   0        0        0     8026 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/location_service.py
--rw-r--r--   0        0        0     9952 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/mixture_service.py
--rw-r--r--   0        0        0    10149 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/molecule_service.py
--rw-r--r--   0        0        0     6100 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/nucleotide_alignments_service.py
--rw-r--r--   0        0        0    11598 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/oligo_service.py
--rw-r--r--   0        0        0     4927 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/organization_service.py
--rw-r--r--   0        0        0    11006 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/plate_service.py
--rw-r--r--   0        0        0     1181 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/printer_service.py
--rw-r--r--   0        0        0     4140 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/project_service.py
--rw-r--r--   0        0        0     4627 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/registry_service.py
--rw-r--r--   0        0        0     8917 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/request_service.py
--rw-r--r--   0        0        0     9459 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/rna_oligo_service.py
--rw-r--r--   0        0        0    11980 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/rna_sequence_service.py
--rw-r--r--   0        0        0    23509 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/schema_service.py
--rw-r--r--   0        0        0     4982 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/task_service.py
--rw-r--r--   0        0        0     4723 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/team_service.py
--rw-r--r--   0        0        0     6803 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/user_service.py
--rw-r--r--   0        0        0     1286 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/warehouse_service.py
--rw-r--r--   0        0        0     9993 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/workflow_output_service.py
--rw-r--r--   0        0        0     8848 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/workflow_task_group_service.py
--rw-r--r--   0        0        0    12819 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/workflow_task_service.py
--rw-r--r--   0        0        0     2015 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/v2_alpha_service.py
--rw-r--r--   0        0        0     6483 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/v2_beta_service.py
--rw-r--r--   0        0        0    25286 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2/v2_stable_service.py
--rw-r--r--   0        0        0     2179 2023-03-30 07:06:36.271979 benchling_sdk-1.7.0a8/benchling_sdk/services/v2_service.py
--rw-r--r--   0        0        0     3431 2023-03-30 07:21:24.260477 benchling_sdk-1.7.0a8/pyproject.toml
--rw-r--r--   0        0        0     2389 1970-01-01 00:00:00.000000 benchling_sdk-1.7.0a8/setup.py
--rw-r--r--   0        0        0     2220 1970-01-01 00:00:00.000000 benchling_sdk-1.7.0a8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/LICENSE
+-rw-r--r--   0        0        0      826 2023-03-31 07:21:09.263610 benchling_sdk-1.7.0a9/README.md
+-rw-r--r--   0        0        0        0 2023-03-31 07:20:56.663565 benchling_sdk-1.7.0a9/benchling_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-31 07:20:56.663565 benchling_sdk-1.7.0a9/benchling_sdk/apps/__init__.py
+-rw-r--r--   0        0        0      132 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/apps/config/__init__.py
+-rw-r--r--   0        0        0     2185 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/apps/config/decryption_provider.py
+-rw-r--r--   0        0        0    36607 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/apps/config/dependencies.py
+-rw-r--r--   0        0        0    26640 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/apps/config/mock_dependencies.py
+-rw-r--r--   0        0        0     6872 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/apps/config/scalars.py
+-rw-r--r--   0        0        0    13205 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/apps/framework.py
+-rw-r--r--   0        0        0        0 2023-03-31 07:20:56.663565 benchling_sdk-1.7.0a9/benchling_sdk/apps/helpers/__init__.py
+-rw-r--r--   0        0        0    17317 2023-03-31 07:06:54.371337 benchling_sdk-1.7.0a9/benchling_sdk/apps/helpers/canvas_helpers.py
+-rw-r--r--   0        0        0    16163 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/apps/helpers/config_helpers.py
+-rw-r--r--   0        0        0     1789 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/apps/helpers/cryptography_helpers.py
+-rw-r--r--   0        0        0      945 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/apps/helpers/manifest_helpers.py
+-rw-r--r--   0        0        0    26922 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/apps/helpers/session_helpers.py
+-rw-r--r--   0        0        0     6918 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/apps/helpers/webhook_helpers.py
+-rw-r--r--   0        0        0      120 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/auth/__init__.py
+-rw-r--r--   0        0        0      643 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/auth/api_key_auth.py
+-rw-r--r--   0        0        0     5271 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/auth/client_credentials_oauth2.py
+-rw-r--r--   0        0        0    24967 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/benchling.py
+-rw-r--r--   0        0        0       38 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/docs/__init__.py
+-rw-r--r--   0        0        0      244 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/docs/__main__.py
+-rw-r--r--   0        0        0     7859 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/errors.py
+-rw-r--r--   0        0        0        0 2023-03-31 07:20:56.663565 benchling_sdk-1.7.0a9/benchling_sdk/helpers/__init__.py
+-rw-r--r--   0        0        0      833 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/helpers/client_helpers.py
+-rw-r--r--   0        0        0     1094 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/helpers/constants.py
+-rw-r--r--   0        0        0     1466 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/helpers/decorators.py
+-rw-r--r--   0        0        0      338 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/helpers/file_helpers.py
+-rw-r--r--   0        0        0     2500 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/helpers/logging_helpers.py
+-rw-r--r--   0        0        0     1998 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/helpers/package_helpers.py
+-rw-r--r--   0        0        0     7774 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/helpers/pagination_helpers.py
+-rw-r--r--   0        0        0      613 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/helpers/response_helpers.py
+-rw-r--r--   0        0        0     2677 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/helpers/retry_helpers.py
+-rw-r--r--   0        0        0     3662 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/helpers/serialization_helpers.py
+-rw-r--r--   0        0        0     3693 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/helpers/transaction_manager.py
+-rw-r--r--   0        0        0   295633 2023-03-31 07:06:54.371337 benchling_sdk-1.7.0a9/benchling_sdk/models/__init__.py
+-rw-r--r--   0        0        0       25 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/py.typed
+-rw-r--r--   0        0        0       85 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-31 07:20:56.663565 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-31 07:20:56.663565 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/alpha/__init__.py
+-rw-r--r--   0        0        0     1443 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/alpha/v2_alpha_app_service.py
+-rw-r--r--   0        0        0     1347 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/alpha/v2_alpha_dna_sequence_service.py
+-rw-r--r--   0        0        0      951 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/base_service.py
+-rw-r--r--   0        0        0        0 2023-03-31 07:20:56.663565 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/__init__.py
+-rw-r--r--   0        0        0     2551 2023-03-30 18:21:13.461007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_aa_sequence_service.py
+-rw-r--r--   0        0        0    11210 2023-03-31 07:06:54.371337 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_app_service.py
+-rw-r--r--   0        0        0     1840 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_custom_entity_service.py
+-rw-r--r--   0        0        0     1704 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_dna_oligo_service.py
+-rw-r--r--   0        0        0     1843 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_dna_sequence_service.py
+-rw-r--r--   0        0        0     1970 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_entity_service.py
+-rw-r--r--   0        0        0     1053 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_entry_service.py
+-rw-r--r--   0        0        0     1704 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_rna_oligo_service.py
+-rw-r--r--   0        0        0     5544 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_worklist_service.py
+-rw-r--r--   0        0        0        0 2023-03-31 07:20:56.663565 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/__init__.py
+-rw-r--r--   0        0        0    11204 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/aa_sequence_service.py
+-rw-r--r--   0        0        0    12371 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/api_service.py
+-rw-r--r--   0        0        0    12448 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/app_service.py
+-rw-r--r--   0        0        0    12317 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/assay_result_service.py
+-rw-r--r--   0        0        0     9023 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/assay_run_service.py
+-rw-r--r--   0        0        0    16738 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/blob_service.py
+-rw-r--r--   0        0        0    12144 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/box_service.py
+-rw-r--r--   0        0        0    18055 2023-03-31 07:06:54.371337 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/container_service.py
+-rw-r--r--   0        0        0    10828 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/custom_entity_service.py
+-rw-r--r--   0        0        0     7445 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/dna_alignments_service.py
+-rw-r--r--   0        0        0     9456 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/dna_oligo_service.py
+-rw-r--r--   0        0        0    12238 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/dna_sequence_service.py
+-rw-r--r--   0        0        0     4919 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/dropdown_service.py
+-rw-r--r--   0        0        0    11770 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/entry_service.py
+-rw-r--r--   0        0        0     2538 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/event_service.py
+-rw-r--r--   0        0        0     1080 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/export_service.py
+-rw-r--r--   0        0        0     8988 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/feature_library_service.py
+-rw-r--r--   0        0        0     5219 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/folder_service.py
+-rw-r--r--   0        0        0     1761 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/inventory_service.py
+-rw-r--r--   0        0        0     9869 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/lab_automation_service.py
+-rw-r--r--   0        0        0     1300 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/label_template_service.py
+-rw-r--r--   0        0        0     8026 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/location_service.py
+-rw-r--r--   0        0        0     9952 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/mixture_service.py
+-rw-r--r--   0        0        0    10149 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/molecule_service.py
+-rw-r--r--   0        0        0     6100 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/nucleotide_alignments_service.py
+-rw-r--r--   0        0        0    11598 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/oligo_service.py
+-rw-r--r--   0        0        0     4927 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/organization_service.py
+-rw-r--r--   0        0        0    11006 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/plate_service.py
+-rw-r--r--   0        0        0     1181 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/printer_service.py
+-rw-r--r--   0        0        0     4140 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/project_service.py
+-rw-r--r--   0        0        0     4627 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/registry_service.py
+-rw-r--r--   0        0        0     8917 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/request_service.py
+-rw-r--r--   0        0        0     9459 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/rna_oligo_service.py
+-rw-r--r--   0        0        0    11980 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/rna_sequence_service.py
+-rw-r--r--   0        0        0    23509 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/schema_service.py
+-rw-r--r--   0        0        0     4982 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/task_service.py
+-rw-r--r--   0        0        0     4723 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/team_service.py
+-rw-r--r--   0        0        0     6803 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/user_service.py
+-rw-r--r--   0        0        0     1286 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/warehouse_service.py
+-rw-r--r--   0        0        0     9993 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/workflow_output_service.py
+-rw-r--r--   0        0        0     8848 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/workflow_task_group_service.py
+-rw-r--r--   0        0        0    12819 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/workflow_task_service.py
+-rw-r--r--   0        0        0     2015 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/v2_alpha_service.py
+-rw-r--r--   0        0        0     6483 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/v2_beta_service.py
+-rw-r--r--   0        0        0    25286 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2/v2_stable_service.py
+-rw-r--r--   0        0        0     2179 2023-03-30 18:21:13.471007 benchling_sdk-1.7.0a9/benchling_sdk/services/v2_service.py
+-rw-r--r--   0        0        0     3431 2023-03-31 07:21:09.213609 benchling_sdk-1.7.0a9/pyproject.toml
+-rw-r--r--   0        0        0     2389 1970-01-01 00:00:00.000000 benchling_sdk-1.7.0a9/setup.py
+-rw-r--r--   0        0        0     2220 1970-01-01 00:00:00.000000 benchling_sdk-1.7.0a9/PKG-INFO
```

### Comparing `benchling_sdk-1.7.0a8/LICENSE` & `benchling_sdk-1.7.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/README.md` & `benchling_sdk-1.7.0a9/README.md`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/apps/config/decryption_provider.py` & `benchling_sdk-1.7.0a9/benchling_sdk/apps/config/decryption_provider.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/apps/config/dependencies.py` & `benchling_sdk-1.7.0a9/benchling_sdk/apps/config/dependencies.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/apps/config/mock_dependencies.py` & `benchling_sdk-1.7.0a9/benchling_sdk/apps/config/mock_dependencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,34 @@
 
 from benchling_api_client.v2.beta.models.base_manifest_config import BaseManifestConfig
 from benchling_api_client.v2.beta.models.benchling_app_manifest import BenchlingAppManifest
 from benchling_api_client.v2.beta.models.dropdown_dependency import DropdownDependency
 from benchling_api_client.v2.beta.models.entity_schema_dependency import EntitySchemaDependency
 from benchling_api_client.v2.beta.models.field_definitions_manifest import FieldDefinitionsManifest
 from benchling_api_client.v2.beta.models.manifest_array_config import ManifestArrayConfig
+from benchling_api_client.v2.beta.models.manifest_boolean_scalar_config import ManifestBooleanScalarConfig
+from benchling_api_client.v2.beta.models.manifest_date_scalar_config import ManifestDateScalarConfig
+from benchling_api_client.v2.beta.models.manifest_datetime_scalar_config import ManifestDatetimeScalarConfig
+from benchling_api_client.v2.beta.models.manifest_float_scalar_config import ManifestFloatScalarConfig
+from benchling_api_client.v2.beta.models.manifest_integer_scalar_config import ManifestIntegerScalarConfig
+from benchling_api_client.v2.beta.models.manifest_json_scalar_config import ManifestJsonScalarConfig
 from benchling_api_client.v2.beta.models.manifest_scalar_config import ManifestScalarConfig
+from benchling_api_client.v2.beta.models.manifest_secure_text_scalar_config import (
+    ManifestSecureTextScalarConfig,
+)
 from benchling_api_client.v2.beta.models.resource_dependency import ResourceDependency
 from benchling_api_client.v2.beta.models.scalar_config_types import ScalarConfigTypes
 from benchling_api_client.v2.beta.models.schema_dependency import SchemaDependency
 from benchling_api_client.v2.beta.models.schema_dependency_subtypes import (
     SchemaDependencySubtypes as SchemaDependencySubtypesBeta,
 )
 from benchling_api_client.v2.beta.models.workflow_task_schema_dependency import WorkflowTaskSchemaDependency
 from benchling_api_client.v2.extensions import UnknownType
 from benchling_api_client.v2.stable.types import UNSET, Unset
+import typing_extensions
 from typing_extensions import Protocol
 
 from benchling_sdk.apps.config.decryption_provider import BaseDecryptionProvider
 from benchling_sdk.apps.config.dependencies import (
     _supported_config_item,
     BaseDependencies,
     ConfigurationReference,
@@ -436,16 +446,19 @@
             output_fields = field_definitions_from_dependency(workflow_task_output)
             output_items = [
                 _mock_workflow_output_subdependency(subdependency, dependency, parent_path=parent_path)
                 for subdependency in output_fields
             ]
             sub_items += output_items
         return [*[config_item], *sub_items]
-    elif isinstance(dependency, ManifestScalarConfig):
-        return [_mock_scalar_dependency(dependency, parent_path=parent_path)]
+    # Python can't compare isinstance for Union types until Python 3.10 so just do this for now
+    # from: https://github.com/python/typing/discussions/1132#discussioncomment-2560441
+    elif isinstance(dependency, typing_extensions.get_args(ManifestScalarConfig)):
+        # Ignore type since MyPy definitely can't tell from above
+        return [_mock_scalar_dependency(dependency, parent_path=parent_path)]  # type: ignore
     elif isinstance(dependency, ManifestArrayConfig):
         return _mock_array_dependency(dependency, parent_path=parent_path)
     elif isinstance(dependency, UnknownType):
         return [UnknownType(value="Unknown")]
     else:
         linked_resource_id = _random_string("val_")
         return [
@@ -464,43 +477,44 @@
     source_value: str = manifest_subtype.value
     return SchemaDependencySubtypes(source_value)
 
 
 def _mock_scalar_dependency(
     dependency: ManifestScalarConfig, parent_path: List[str] = list()
 ) -> AppConfigItem:
-    if dependency.type == ScalarConfigTypes.BOOLEAN:
+    if isinstance(dependency, ManifestBooleanScalarConfig):
         bool_value = _mock_scalar_value_with_conversion(dependency, BoolScalar)
         bool_config = mock_bool_app_config_item([dependency.name], bool_value)
         return _append_config_item_path(bool_config, parent_path)
-    elif dependency.type == ScalarConfigTypes.DATE:
+    elif isinstance(dependency, ManifestDateScalarConfig):
         date_value = _mock_scalar_value_with_conversion(dependency, DateScalar)
         date_config = mock_date_app_config_item([dependency.name], date_value)
         return _append_config_item_path(date_config, parent_path)
-    elif dependency.type == ScalarConfigTypes.DATETIME:
+    elif isinstance(dependency, ManifestDatetimeScalarConfig):
         datetime_value = _mock_scalar_value_with_conversion(dependency, DateTimeScalar)
         datetime_config = mock_datetime_app_config_item([dependency.name], datetime_value)
         return _append_config_item_path(datetime_config, parent_path)
-    elif dependency.type == ScalarConfigTypes.FLOAT:
+    elif isinstance(dependency, ManifestFloatScalarConfig):
         float_value = _mock_scalar_value_with_conversion(dependency, FloatScalar)
         float_config = mock_float_app_config_item([dependency.name], float_value)
         return _append_config_item_path(float_config, parent_path)
-    elif dependency.type == ScalarConfigTypes.INTEGER:
+    elif isinstance(dependency, ManifestIntegerScalarConfig):
         int_value = _mock_scalar_value_with_conversion(dependency, IntScalar)
         int_config = mock_int_app_config_item([dependency.name], int_value)
         return _append_config_item_path(int_config, parent_path)
-    elif dependency.type == ScalarConfigTypes.JSON:
+    elif isinstance(dependency, ManifestJsonScalarConfig):
         json_value = _mock_scalar_value_with_conversion(dependency, JsonScalar)
         json_config = mock_json_app_config_item([dependency.name], json_value)
         return _append_config_item_path(json_config, parent_path)
-    elif dependency.type == ScalarConfigTypes.SECURE_TEXT:
+    elif isinstance(dependency, ManifestSecureTextScalarConfig):
         secure_text_value = _mock_scalar_value_with_conversion(dependency, SecureTextScalar)
         secure_text_config = mock_secure_text_app_config_item([dependency.name], secure_text_value)
         return _append_config_item_path(secure_text_config, parent_path)
     else:
+        assert not isinstance(dependency, UnknownType), f"Unable to mock unknown type {dependency}"
         text_value = _mock_scalar_value_with_conversion(dependency, TextScalar)
         text_config = mock_text_app_config_item([dependency.name], text_value)
         return _append_config_item_path(text_config, parent_path)
 
 
 def _append_config_item_path(config_item: AppConfigItem, parent_path: List[str]) -> AppConfigItem:
     if isinstance(config_item, UnknownType):
@@ -532,15 +546,18 @@
         value=row_name,
     )
 
 
 def _mock_scalar_value_with_conversion(
     dependency: ManifestScalarConfig, scalar_definition_type: Type[ScalarDefinition[ScalarType]]
 ) -> Optional[ScalarType]:
-    mocked_value_str = _mock_scalar_value(dependency.type)
+    assert not isinstance(dependency, UnknownType), f"Unable to mock unknown type {dependency}"
+    # These types should be equivalent and this appeases MyPy
+    mocked_value_type = ScalarConfigTypes(dependency.type)
+    mocked_value_str = _mock_scalar_value(mocked_value_type)
     return scalar_definition_type.from_str(mocked_value_str)
 
 
 def _mock_subdependency(
     subdependency: Union[BaseManifestConfig, FieldDefinitionsManifest],
     parent_config,
     parent_path: List[str] = list(),
```

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/apps/config/scalars.py` & `benchling_sdk-1.7.0a9/benchling_sdk/apps/config/scalars.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/apps/framework.py` & `benchling_sdk-1.7.0a9/benchling_sdk/apps/framework.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/apps/helpers/canvas_helpers.py` & `benchling_sdk-1.7.0a9/benchling_sdk/apps/helpers/canvas_helpers.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/apps/helpers/config_helpers.py` & `benchling_sdk-1.7.0a9/benchling_sdk/apps/helpers/config_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,25 @@
 from benchling_api_client.v2.beta.models.base_manifest_config import BaseManifestConfig
 from benchling_api_client.v2.beta.models.dropdown_dependency import DropdownDependency
 from benchling_api_client.v2.beta.models.dropdown_dependency_types import DropdownDependencyTypes
 from benchling_api_client.v2.beta.models.entity_schema_dependency import EntitySchemaDependency
 from benchling_api_client.v2.beta.models.entity_schema_dependency_type import EntitySchemaDependencyType
 from benchling_api_client.v2.beta.models.field_definitions_manifest import FieldDefinitionsManifest
 from benchling_api_client.v2.beta.models.manifest_array_config import ManifestArrayConfig
+from benchling_api_client.v2.beta.models.manifest_boolean_scalar_config import ManifestBooleanScalarConfig
+from benchling_api_client.v2.beta.models.manifest_date_scalar_config import ManifestDateScalarConfig
+from benchling_api_client.v2.beta.models.manifest_datetime_scalar_config import ManifestDatetimeScalarConfig
+from benchling_api_client.v2.beta.models.manifest_float_scalar_config import ManifestFloatScalarConfig
+from benchling_api_client.v2.beta.models.manifest_integer_scalar_config import ManifestIntegerScalarConfig
+from benchling_api_client.v2.beta.models.manifest_json_scalar_config import ManifestJsonScalarConfig
 from benchling_api_client.v2.beta.models.manifest_scalar_config import ManifestScalarConfig
+from benchling_api_client.v2.beta.models.manifest_secure_text_scalar_config import (
+    ManifestSecureTextScalarConfig,
+)
+from benchling_api_client.v2.beta.models.manifest_text_scalar_config import ManifestTextScalarConfig
 from benchling_api_client.v2.beta.models.resource_dependency import ResourceDependency
 from benchling_api_client.v2.beta.models.resource_dependency_types import ResourceDependencyTypes
 from benchling_api_client.v2.beta.models.scalar_config import ScalarConfig
 from benchling_api_client.v2.beta.models.scalar_config_types import ScalarConfigTypes
 from benchling_api_client.v2.beta.models.schema_dependency import SchemaDependency
 from benchling_api_client.v2.beta.models.schema_dependency_subtypes import SchemaDependencySubtypes
 from benchling_api_client.v2.beta.models.schema_dependency_types import SchemaDependencyTypes
@@ -217,15 +227,15 @@
             elif element_type in [member.value for member in SchemaDependencyTypes]:
                 return SchemaDependency.from_dict(element.value)
             elif element_type == DropdownDependencyTypes.DROPDOWN:
                 return DropdownDependency.from_dict(element.value)
             elif element_type in [member.value for member in ResourceDependencyTypes]:
                 return ResourceDependency.from_dict(element.value)
             elif element_type in [member.value for member in ScalarConfigTypes]:
-                return ManifestScalarConfig.from_dict(element.value)
+                return type(element_type).from_dict(element.value)
         raise NotImplementedError(f"No array deserialization fix for {element}")
     return element
 
 
 def workflow_task_schema_output_from_dependency(
     dependency: WorkflowTaskSchemaDependency,
 ) -> Optional[WorkflowTaskSchemaDependencyOutput]:
@@ -344,31 +354,31 @@
         return GenericApiIdentifiedAppConfigItem
     # Specially handled Schema types
     elif isinstance(dependency, FieldDefinitionsManifest):
         return FieldAppConfigItem
     elif isinstance(dependency, EntitySchemaDependency):
         return EntitySchemaAppConfigItem
     # Scalar types
-    elif isinstance(dependency, ManifestScalarConfig):
-        if dependency.type == ScalarConfigTypes.BOOLEAN:
-            return BooleanAppConfigItem
-        elif dependency.type == ScalarConfigTypes.DATE:
-            return DateAppConfigItem
-        elif dependency.type == ScalarConfigTypes.DATETIME:
-            return DatetimeAppConfigItem
-        elif dependency.type == ScalarConfigTypes.FLOAT:
-            return FloatAppConfigItem
-        elif dependency.type == ScalarConfigTypes.INTEGER:
-            return IntegerAppConfigItem
-        elif dependency.type == ScalarConfigTypes.JSON:
-            return JsonAppConfigItem
-        elif dependency.type == ScalarConfigTypes.SECURE_TEXT:
-            return SecureTextAppConfigItem
-        elif dependency.type == ScalarConfigTypes.TEXT:
-            return TextAppConfigItem
+    elif isinstance(dependency, ManifestBooleanScalarConfig):
+        return BooleanAppConfigItem
+    elif isinstance(dependency, ManifestDateScalarConfig):
+        return DateAppConfigItem
+    elif isinstance(dependency, ManifestDatetimeScalarConfig):
+        return DatetimeAppConfigItem
+    elif isinstance(dependency, ManifestFloatScalarConfig):
+        return FloatAppConfigItem
+    elif isinstance(dependency, ManifestIntegerScalarConfig):
+        return IntegerAppConfigItem
+    elif isinstance(dependency, ManifestJsonScalarConfig):
+        return JsonAppConfigItem
+    elif isinstance(dependency, ManifestSecureTextScalarConfig):
+        return SecureTextAppConfigItem
+    elif isinstance(dependency, ManifestTextScalarConfig):
+        return TextAppConfigItem
+    # Array type
     elif isinstance(dependency, ManifestArrayConfig):
         return ArrayElementAppConfigItem
     raise UnsupportedDependencyError(f"Unrecognized type for {dependency}]")
 
 
 def _subtype_instance_from_dependency(dependency: EntitySchemaDependency) -> Type[EntitySubtype]:
     if dependency.subtype in _INSTANCE_FROM_SCHEMA_SUBTYPE:
```

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/apps/helpers/cryptography_helpers.py` & `benchling_sdk-1.7.0a9/benchling_sdk/apps/helpers/cryptography_helpers.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/apps/helpers/manifest_helpers.py` & `benchling_sdk-1.7.0a9/benchling_sdk/apps/helpers/manifest_helpers.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/apps/helpers/session_helpers.py` & `benchling_sdk-1.7.0a9/benchling_sdk/apps/helpers/session_helpers.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/apps/helpers/webhook_helpers.py` & `benchling_sdk-1.7.0a9/benchling_sdk/apps/helpers/webhook_helpers.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/auth/api_key_auth.py` & `benchling_sdk-1.7.0a9/benchling_sdk/auth/api_key_auth.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/auth/client_credentials_oauth2.py` & `benchling_sdk-1.7.0a9/benchling_sdk/auth/client_credentials_oauth2.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/benchling.py` & `benchling_sdk-1.7.0a9/benchling_sdk/benchling.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/errors.py` & `benchling_sdk-1.7.0a9/benchling_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/helpers/client_helpers.py` & `benchling_sdk-1.7.0a9/benchling_sdk/helpers/client_helpers.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/helpers/constants.py` & `benchling_sdk-1.7.0a9/benchling_sdk/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/helpers/decorators.py` & `benchling_sdk-1.7.0a9/benchling_sdk/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/helpers/logging_helpers.py` & `benchling_sdk-1.7.0a9/benchling_sdk/helpers/logging_helpers.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/helpers/package_helpers.py` & `benchling_sdk-1.7.0a9/benchling_sdk/helpers/package_helpers.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/helpers/pagination_helpers.py` & `benchling_sdk-1.7.0a9/benchling_sdk/helpers/pagination_helpers.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/helpers/response_helpers.py` & `benchling_sdk-1.7.0a9/benchling_sdk/helpers/response_helpers.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/helpers/retry_helpers.py` & `benchling_sdk-1.7.0a9/benchling_sdk/helpers/retry_helpers.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/helpers/serialization_helpers.py` & `benchling_sdk-1.7.0a9/benchling_sdk/helpers/serialization_helpers.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/helpers/transaction_manager.py` & `benchling_sdk-1.7.0a9/benchling_sdk/helpers/transaction_manager.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/models/__init__.py` & `benchling_sdk-1.7.0a9/benchling_sdk/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,14 +412,15 @@
     "EntryCreatedEventEventType",
     "EntryDay",
     "EntryExternalFile",
     "EntryExternalFileById",
     "EntryLink",
     "EntryLinkType",
     "EntryReviewRecord",
+    "EntryReviewRecordStatus",
     "EntrySchema",
     "EntrySchemaDetailed",
     "EntrySchemaDetailedType",
     "EntrySchemasPaginatedList",
     "EntryTable",
     "EntryTableCell",
     "EntryTableRow",
@@ -1304,14 +1305,15 @@
     import benchling_api_client.v2.stable.models.entry_created_event_event_type
     import benchling_api_client.v2.stable.models.entry_day
     import benchling_api_client.v2.stable.models.entry_external_file
     import benchling_api_client.v2.stable.models.entry_external_file_by_id
     import benchling_api_client.v2.stable.models.entry_link
     import benchling_api_client.v2.stable.models.entry_link_type
     import benchling_api_client.v2.stable.models.entry_review_record
+    import benchling_api_client.v2.stable.models.entry_review_record_status
     import benchling_api_client.v2.stable.models.entry_schema
     import benchling_api_client.v2.stable.models.entry_schema_detailed
     import benchling_api_client.v2.stable.models.entry_schema_detailed_type
     import benchling_api_client.v2.stable.models.entry_schemas_paginated_list
     import benchling_api_client.v2.stable.models.entry_table
     import benchling_api_client.v2.stable.models.entry_table_cell
     import benchling_api_client.v2.stable.models.entry_table_row
@@ -2684,14 +2686,17 @@
     EntryExternalFile = benchling_api_client.v2.stable.models.entry_external_file.EntryExternalFile
     EntryExternalFileById = (
         benchling_api_client.v2.stable.models.entry_external_file_by_id.EntryExternalFileById
     )
     EntryLink = benchling_api_client.v2.stable.models.entry_link.EntryLink
     EntryLinkType = benchling_api_client.v2.stable.models.entry_link_type.EntryLinkType
     EntryReviewRecord = benchling_api_client.v2.stable.models.entry_review_record.EntryReviewRecord
+    EntryReviewRecordStatus = (
+        benchling_api_client.v2.stable.models.entry_review_record_status.EntryReviewRecordStatus
+    )
     EntrySchema = benchling_api_client.v2.stable.models.entry_schema.EntrySchema
     EntrySchemaDetailed = benchling_api_client.v2.stable.models.entry_schema_detailed.EntrySchemaDetailed
     EntrySchemaDetailedType = (
         benchling_api_client.v2.stable.models.entry_schema_detailed_type.EntrySchemaDetailedType
     )
     EntrySchemasPaginatedList = (
         benchling_api_client.v2.stable.models.entry_schemas_paginated_list.EntrySchemasPaginatedList
@@ -4072,14 +4077,15 @@
         "EntryCreatedEventEventType": "benchling_api_client.v2.stable.models.entry_created_event_event_type",
         "EntryDay": "benchling_api_client.v2.stable.models.entry_day",
         "EntryExternalFile": "benchling_api_client.v2.stable.models.entry_external_file",
         "EntryExternalFileById": "benchling_api_client.v2.stable.models.entry_external_file_by_id",
         "EntryLink": "benchling_api_client.v2.stable.models.entry_link",
         "EntryLinkType": "benchling_api_client.v2.stable.models.entry_link_type",
         "EntryReviewRecord": "benchling_api_client.v2.stable.models.entry_review_record",
+        "EntryReviewRecordStatus": "benchling_api_client.v2.stable.models.entry_review_record_status",
         "EntrySchema": "benchling_api_client.v2.stable.models.entry_schema",
         "EntrySchemaDetailed": "benchling_api_client.v2.stable.models.entry_schema_detailed",
         "EntrySchemaDetailedType": "benchling_api_client.v2.stable.models.entry_schema_detailed_type",
         "EntrySchemasPaginatedList": "benchling_api_client.v2.stable.models.entry_schemas_paginated_list",
         "EntryTable": "benchling_api_client.v2.stable.models.entry_table",
         "EntryTableCell": "benchling_api_client.v2.stable.models.entry_table_cell",
         "EntryTableRow": "benchling_api_client.v2.stable.models.entry_table_row",
```

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/alpha/v2_alpha_app_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/alpha/v2_alpha_app_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/alpha/v2_alpha_dna_sequence_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/alpha/v2_alpha_dna_sequence_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/base_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/base_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_aa_sequence_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_aa_sequence_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_app_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_app_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_custom_entity_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_custom_entity_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_dna_oligo_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_dna_oligo_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_dna_sequence_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_dna_sequence_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_entity_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_entity_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_entry_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_entry_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_rna_oligo_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_rna_oligo_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/beta/v2_beta_worklist_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/beta/v2_beta_worklist_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/aa_sequence_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/aa_sequence_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/api_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/api_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/app_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/app_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/assay_result_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/assay_result_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/assay_run_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/assay_run_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/blob_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/blob_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/box_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/box_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/container_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/container_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/custom_entity_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/custom_entity_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/dna_alignments_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/dna_alignments_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/dna_oligo_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/dna_oligo_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/dna_sequence_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/dna_sequence_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/dropdown_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/dropdown_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/entry_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/entry_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/event_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/event_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/export_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/export_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/feature_library_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/feature_library_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/folder_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/folder_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/inventory_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/inventory_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/lab_automation_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/lab_automation_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/label_template_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/label_template_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/location_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/location_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/mixture_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/mixture_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/molecule_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/molecule_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/nucleotide_alignments_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/nucleotide_alignments_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/oligo_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/oligo_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/organization_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/organization_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/plate_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/plate_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/printer_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/printer_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/project_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/project_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/registry_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/registry_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/request_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/request_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/rna_oligo_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/rna_oligo_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/rna_sequence_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/rna_sequence_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/schema_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/schema_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/task_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/task_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/team_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/team_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/user_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/user_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/warehouse_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/warehouse_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/workflow_output_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/workflow_output_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/workflow_task_group_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/workflow_task_group_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/stable/workflow_task_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/stable/workflow_task_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/v2_alpha_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/v2_alpha_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/v2_beta_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/v2_beta_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2/v2_stable_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2/v2_stable_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/benchling_sdk/services/v2_service.py` & `benchling_sdk-1.7.0a9/benchling_sdk/services/v2_service.py`

 * *Files identical despite different names*

### Comparing `benchling_sdk-1.7.0a8/pyproject.toml` & `benchling_sdk-1.7.0a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "benchling-sdk"
-version = "1.7.0-alpha.8"   # NOTE: This version number is ignored and does not correspond to releases (see README)
+version = "1.7.0-alpha.9"   # NOTE: This version number is ignored and does not correspond to releases (see README)
 description = "SDK for interacting with the Benchling Platform."
 authors = ["Benchling Support <support@benchling.com>"]
 packages = [{include = "benchling_sdk"}]
 include = [
     "LICENSE", "benchling_sdk/py.typed", "docs"
 ]
 license = "Apache-2.0"
@@ -28,15 +28,15 @@
 httpx = ">=0.23.0"
 attrs = ">=20.1.0, <23"
 python-dateutil = "^2.8.0"
 PyYAML = "^6.0"
 # See issue: https://github.com/giampaolo/psutil/issues/2165
 psutil = {version = "^5.9.4", python = "^3.11" }
 jwcrypto = "^1.4.2"
-benchling-api-client = "2.0.117"
+benchling-api-client = "2.0.132"
 # Minimum version due to vulnerability in 2022.9.24
 certifi = ">=2022.12.7"
 # Cryptography extras - see ExtrasPackage.CRYPTOGRAPHY
 cryptography = { version = "^39.0.2", optional = true }
 # Python jose extras - see ExtrasPackage.PYTHON_JOSE
 python-jose = { version = "^3.3.0", extras=["cryptography"], optional = true }
 ordered-set = "^4.1.0"
```

### Comparing `benchling_sdk-1.7.0a8/setup.py` & `benchling_sdk-1.7.0a9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'attrs>=20.1.0,<23',
  'backoff>=1.10.0,<2.0.0',
- 'benchling-api-client==2.0.117',
+ 'benchling-api-client==2.0.132',
  'certifi>=2022.12.7',
  'dataclasses-json>=0.5.2,<0.6.0',
  'httpx>=0.23.0',
  'jwcrypto>=1.4.2,<2.0.0',
  'ordered-set>=4.1.0,<5.0.0',
  'python-dateutil>=2.8.0,<3.0.0',
  'typing-extensions>=3.7.4,<5.0']
@@ -35,15 +35,15 @@
 extras_require = \
 {':python_version >= "3.11" and python_version < "4.0"': ['psutil>=5.9.4,<6.0.0'],
  'cryptography': ['cryptography>=39.0.2,<40.0.0'],
  'python-jose': ['python-jose[cryptography]>=3.3.0,<4.0.0']}
 
 setup_kwargs = {
     'name': 'benchling-sdk',
-    'version': '1.7.0a8',
+    'version': '1.7.0a9',
     'description': 'SDK for interacting with the Benchling Platform.',
     'long_description': '# Benchling SDK\n\nA Python 3.7+ SDK for the [Benchling](https://www.benchling.com/) platform designed to provide typed, fluent\ninteractions with [Benchling APIs](https://docs.benchling.com/reference).\n\n## Installation\n\nInstall the dependency via [Poetry](https://python-poetry.org/) (if applicable):\n\n```bash\npoetry add benchling-sdk\n```\n \nOr [Pip](https://pypi.org/project/pip/):\n \n```bash\npip install benchling-sdk\n```\n\n## Documentation\n\nDocumentation for the SDK is kept up-to-date at [docs.benchling.com](https://docs.benchling.com), and you can get started with\nit using this guide:\n[https://docs.benchling.com/docs/getting-started-with-the-sdk](https://docs.benchling.com/docs/getting-started-with-the-sdk).\n\n## Support\n\nTo report issues with using the SDK, contact [support@benchling.com](mailto:support@benchling.com).\n',
     'author': 'Benchling Support',
     'author_email': 'support@benchling.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `benchling_sdk-1.7.0a8/PKG-INFO` & `benchling_sdk-1.7.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchling-sdk
-Version: 1.7.0a8
+Version: 1.7.0a9
 Summary: SDK for interacting with the Benchling Platform.
 License: Apache-2.0
 Author: Benchling Support
 Author-email: support@benchling.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cryptography
 Provides-Extra: python-jose
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: attrs (>=20.1.0,<23)
 Requires-Dist: backoff (>=1.10.0,<2.0.0)
-Requires-Dist: benchling-api-client (==2.0.117)
+Requires-Dist: benchling-api-client (==2.0.132)
 Requires-Dist: certifi (>=2022.12.7)
 Requires-Dist: cryptography (>=39.0.2,<40.0.0); extra == "cryptography"
 Requires-Dist: dataclasses-json (>=0.5.2,<0.6.0)
 Requires-Dist: httpx (>=0.23.0)
 Requires-Dist: jwcrypto (>=1.4.2,<2.0.0)
 Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0); python_version >= "3.11" and python_version < "4.0"
```

